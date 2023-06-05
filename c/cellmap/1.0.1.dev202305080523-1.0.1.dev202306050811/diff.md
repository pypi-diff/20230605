# Comparing `tmp/cellmap-1.0.1.dev202305080523-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202306050811-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19725 bytes, number of entries: 5
+Zip file size: 19797 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   112613 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/RECORD
-5 files, 115027 bytes uncompressed, 18971 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   112882 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1914 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202306050811.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202306050811.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202306050811.dist-info/RECORD
+5 files, 115341 bytes uncompressed, 19043 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305080523.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202306050811.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305080523.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202306050811.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305080523.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202306050811.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -9,14 +9,16 @@
 import matplotlib.cm
 import matplotlib.colors
 import matplotlib.animation as anm
 from matplotlib import patheffects as PathEffects
 import networkx as nx
 import scanpy
 import scipy
+import scipy.sparse
+import scipy.linalg
 import scvelo as scv
 import sklearn.preprocessing
 import sklearn.mixture
 import sklearn.neighbors
 import sklearn.linear_model
 # from sklearn.linear_model import LinearRegression
 # from sklearn.preprocessing import PolynomialFeatures
@@ -62,20 +64,21 @@
     else:
         judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
         judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)
     idx_mask_ = judge_vol_tri_ & judge_length_tri_
     tri_.set_mask(idx_mask_==False)
     edge_tri_ = np.vstack((np.vstack((tri_.triangles[idx_mask_][:,[0,1]],tri_.triangles[idx_mask_][:,[1,2]])),tri_.triangles[idx_mask_][:,[2,0]]))
     edge_tri_sort_ = np.array([np.sort(e) for e in edge_tri_])
-    np.sort(edge_tri_sort_,axis=0),np.unique(edge_tri_sort_,axis=0).shape
+    # np.sort(edge_tri_sort_,axis=0),np.unique(edge_tri_sort_,axis=0).shape
     edges_,count_ = np.unique(edge_tri_sort_,axis=0,return_counts=True)
     idx_bd_ = np.unique(edges_[count_==1].reshape(1,-1)[0])
     if return_type == 'edges': return edges_.T
     if return_type == 'edges_bd': return edges_[:,0],edges_[:,1],idx_bd_
     if return_type == 'triangles': return tri_,idx_mask_
+    if return_type == 'all': return tri_,idx_mask_,edges_[:,0],edges_[:,1],idx_bd_
 
 
 
 def check_arguments(
     adata,
     verbose = True,
     **kwargs
@@ -327,20 +330,20 @@
     
     ## Solve potential
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
-    lap = -np.dot(div_mat,grad_mat)
+    lap_ = -(scipy.sparse.csr_matrix(div_mat)).dot(scipy.sparse.csr_matrix(grad_mat)).toarray()
     edge_vel = (1-HD_rate)*edge_vel_LD+HD_rate*edge_vel_HD
-    source_term = np.dot(div_mat,edge_vel)
-    lap_inv_ = np.linalg.pinv(lap)
-    potential = np.dot(lap_inv_,source_term)
-    pot_flow_ = -np.dot(grad_mat,potential)
+    source_term = div_mat @ edge_vel
+    lap_inv_ = scipy.linalg.pinv(lap_)
+    potential = lap_inv_ @ source_term
+    pot_flow_ = -grad_mat @ potential
     rot_flow_ = edge_vel - pot_flow_
     adata.obs[potential_key] = potential - np.min(potential)
 
 
     # Compute potential & rotational flow
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
     vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
@@ -367,38 +370,38 @@
             ex_ = -(exp_LD[source[idx_]]-exp_LD[target[idx_]]).T/dis_
             vel_potential[i] = 4.*edge_vel_norm*np.mean(pot_flow_[idx_]*ex_,axis=1)
             vel_rotation[i]  = 4.*edge_vel_norm*np.mean(rot_flow_[idx_]*ex_,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
         adata.obsm[rot_vkey_] = vel_rotation
     
     
-    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
+    # vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False)
     div_ = np.linalg.norm(vel_LD,axis=1)
     div_[div_==0] = 1
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1]/div_,-vel_LD[:,0]/div_)).T,source,target,normalization=False))
+    vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((vel_LD[:,1]/div_,-vel_LD[:,0]/div_)).T,source,target,normalization=False)
     source_term_ = vorticity_
-    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    streamfunc_ = -lap_inv_ @ source_term_
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = streamfunc_-np.min(streamfunc_)
 
-    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
+    # vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False)
     div_ = np.linalg.norm(adata.obsm[pot_vkey_],axis=1)
     div_[div_==0] = 1
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1]/div_,-adata.obsm[pot_vkey_][:,0]/div_)).T,source,target,normalization=False))
+    vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1]/div_,-adata.obsm[pot_vkey_][:,0]/div_)).T,source,target,normalization=False)
     source_term_ = vorticity_
-    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    streamfunc_ = -lap_inv_ @ source_term_
     adata.obs[pot_vor_key_] = vorticity_
     adata.obs[pot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
-    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
+    # vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False)
     div_ = np.linalg.norm(adata.obsm[rot_vkey_],axis=1)
     div_[div_==0] = 1
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1]/div_,-adata.obsm[rot_vkey_][:,0]/div_)).T,source,target,normalization=False))
+    vorticity_ = div_mat @ edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1]/div_,-adata.obsm[rot_vkey_][:,0]/div_)).T,source,target,normalization=False)
     source_term_ = vorticity_
-    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    streamfunc_ = -lap_inv_ @ source_term_
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
     log_ = {}
@@ -482,24 +485,24 @@
         target = np.ravel(indices)
     
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
-    lap = -np.dot(div_mat,grad_mat)
+    lap = -div_mat @ grad_mat
     lap_inv = np.linalg.pinv(lap)
     
     for gene in genes:
         X1,X2 = exp_HD[:,adata.var.index == gene][source],exp_HD[:,adata.var.index == gene][target]
         V1,V2 = vel_HD[:,adata.var.index == gene][source],vel_HD[:,adata.var.index == gene][target]
         Dis = np.linalg.norm(exp_HD[target]-exp_HD[source],axis=1)
         edge_vel = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
-        source_term = np.dot(div_mat,edge_vel)
-        potential = np.dot(lap_inv,source_term)
+        source_term = div_mat @ edge_vel
+        potential = lap_inv @ source_term
         adata.obs[potential_key+'_Gene_%s' % gene] = potential - np.min(potential)
 
 def view(
     adata,
     basis = 'umap',
     color_key = 'potential',
     cluster_key = 'clusters',
@@ -860,14 +863,15 @@
     title = 'Landscape',
     bgcolor = "white",
     gridcolor = "gray",
     seed = None,
     n_points = 500,
     save = False,
     filename = 'CellMap_view_3D',
+    camera = dict(eye=dict(x=1.2, y=-1.2, z=1.0)),
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata, basis=basis, potential_key=potential_key)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
@@ -879,23 +883,22 @@
     c_list  = ['#0938BF','#50D9FB','#B7E5FA','#98D685','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09']
     c_level = [0,5,20,40,60,75,80,85,90,95,99,100]
     custom_cmap = [[0.01*c_level[i],c_list[i]] for i in range(len(c_list))]
 
     tri_,idx_tri = create_graph(adata.obsm[basis_key],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type = 'triangles')
     triangles = tri_.triangles[idx_tri]
 
-    camera = dict(eye=dict(x=1.2, y=-1.2, z=1.0))
     idx = np.zeros(adata.shape[0],dtype=bool)
     np.random.seed(seed)
     idx[np.random.choice(adata.shape[0],min(n_points,adata.shape[0]),replace=False)] = True
     shift = 0.01*(max(z)-min(z))
     shadow = go.Mesh3d(
         x=x,
         y=y,
-        z=np.zeros(adata.shape[0]),
+        z=np.zeros(adata.shape[0])-np.min(z),
         i=triangles[:, 0],
         j=triangles[:, 1],
         k=triangles[:, 2],
         opacity=shadow_alpha,
         color='black',
     )
 
@@ -1377,15 +1380,16 @@
         src_set_ = src_set_all_[idx_src_]
 
         pathes,edges,weights,dists  = [],[],[],[]
         for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
             # G.add_weighted_edges_from([(int(s),int(t),np.exp(-g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
             # G.add_weighted_edges_from([(int(t),int(s), np.exp(g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
             # weights_ = np.hstack((np.exp(-grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean),np.exp(grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean)))
-            weights_i_ = np.exp(-weights_*(adata.obs[potential_key][edges_[:,0]].values - adata.obs[potential_key][edges_[:,1]].values)*register)*np.abs(streamfunc_[trg_]-streamfunc_[edges_[:,1]])*np.exp(np.linalg.norm(data_pos[edges_[:,0]]-data_pos[edges_[:,1]],axis=1)/dis_mean)
+            #weights_i_ = np.exp(-weights_*(adata.obs[potential_key][edges_[:,0]].values - adata.obs[potential_key][edges_[:,1]].values)*register)*np.abs(streamfunc_[trg_]-streamfunc_[edges_[:,1]])*np.exp(np.linalg.norm(data_pos[edges_[:,0]]-data_pos[edges_[:,1]],axis=1)/dis_mean)
+            weights_i_ = np.abs(streamfunc_[trg_] - streamfunc_[edges_[:, 1]]) * np.exp(np.linalg.norm(data_pos[edges_[:, 0]] - data_pos[edges_[:, 1]], axis=1) / dis_mean)
             nx.set_edge_attributes(G, values=dict(zip(G.edges(), weights_i_)), name='weight')
             path = nx.dijkstra_path(G, source=src_, target=trg_, weight='weight')
             pathes.append(path)
             edges.append(np.array([[path[i], path[i+1]] for i in range(len(path)-1)]))
             weights.append((sum([G[path[i]][path[i+1]]['weight'] for i in range(len(path)-1)]))/sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
             dists.append(sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
         path_all[source_cluster+'_'+target_clusters[i_trg_]] = pathes
@@ -2016,15 +2020,15 @@
     umap_ = umap.UMAP(n_components=n_components,random_state=seed,n_neighbors=n_neighbors,min_dist=min_dist)
     gene_dynamics_all_umap_ = umap_.fit_transform(gene_dynamics_all_)
 
     data_ = gene_dynamics_all_umap_
     gm = sklearn.mixture.GaussianMixture(n_components=n_clusters,random_state=0).fit(data_)
     clusters_tmp_ = gm.predict(data_)
     pc1_ = sklearn.decomposition.PCA(n_components=1).fit_transform(data_)[:,0]
-    pc1_ = np.sign(np.dot(pc1_,gene_dynamics_all_umap_[:,0]))*pc1_
+    pc1_ = np.sign(pc1_ @ gene_dynamics_all_umap_[:,0])*pc1_
     pc1_order_ = np.argsort([np.mean(pc1_[clusters_tmp_==i]) for i in range(n_clusters)])
     dict_sort_ = dict(zip(pc1_order_,np.unique(clusters_tmp_)))
     clusters_ = np.array([dict_sort_[c] for c in clusters_tmp_])
 
     texts_ = []
     index_ = []
     s_,e_ = 0,0
@@ -2353,20 +2357,20 @@
         for j in range(i+1,len(target_clusters)):
             columns_ = np.append(columns_,target_clusters[i]+'_vs_'+target_clusters[j])
 
     cmap_ = plt.get_cmap("tab10")
     vlines = [0,0.2,0.4,0.6,0.8,1]
     sign_dict_ = {'1':'+','-1':'-'}
     out_pd_ = pd.DataFrame(index=(np.arange(n_genes)+1),columns=pd.MultiIndex.from_product([list(columns_),[]]))
+    gene_dynamics_ = adata.uns[gene_dynamics_key]
     for i in range(len(target_clusters)):
         for j in range(i+1,len(target_clusters)):
             
             name_i_ = source_cluster + '_' + target_clusters[i]
             name_j_ = source_cluster + '_' + target_clusters[j]
-            gene_dynamics_ = adata.uns[gene_dynamics_key]
 
             max_i_,max_j_ = np.max(gene_dynamics_[name_i_],axis=0),np.max(gene_dynamics_[name_j_],axis=0)
             idx_max_ = (max_i_ > threshold_min) & (max_j_ > threshold_min)
 
             vol_p_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_p_]-gene_dynamics_[name_j_][idx_t_p_]),axis=0)
             vol_n_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_n_]-gene_dynamics_[name_j_][idx_t_n_]),axis=0)
             diff_ = vol_p_/(1e-5+vol_n_)
```

## Comparing `cellmap-1.0.1.dev202305080523.dist-info/METADATA` & `cellmap-1.0.1.dev202306050811.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202305080523
+Version: 1.0.1.dev202306050811
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: adjustText (>=0.8)
 Requires-Dist: anndata (>=0.8.0)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: plotly (>=5.14.1)
 Requires-Dist: scanpy (>=1.9.3)
 Requires-Dist: scikit-learn (>=0.24)
```

