# Comparing `tmp/gmm_mi-0.6.0.tar.gz` & `tmp/gmm_mi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmm_mi-0.6.0.tar", last modified: Mon May 15 22:09:15 2023, max compression
+gzip compressed data, was "gmm_mi-0.7.0.tar", last modified: Mon Jun  5 18:05:58 2023, max compression
```

## Comparing `gmm_mi-0.6.0.tar` & `gmm_mi-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.983382 gmm_mi-0.6.0/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.6.0/LICENSE.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.6.0/LICENSE_EXT.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-15 22:09:14.973382 gmm_mi-0.6.0/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-14 15:46:30.000000 gmm_mi-0.6.0/README.md
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.834382 gmm_mi-0.6.0/gmm_mi/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.6.0/gmm_mi/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.6.0/gmm_mi/cross_validation.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.868382 gmm_mi-0.6.0/gmm_mi/data/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.6.0/gmm_mi/data/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.6.0/gmm_mi/data/synthetic_data.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    24708 2023-05-14 14:04:14.000000 gmm_mi-0.6.0/gmm_mi/gmm.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.6.0/gmm_mi/initializations.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45340 2023-05-14 14:09:38.000000 gmm_mi-0.6.0/gmm_mi/mi.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.6.0/gmm_mi/param_holders.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.6.0/gmm_mi/single_fit.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.924382 gmm_mi-0.6.0/gmm_mi/utils/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.6.0/gmm_mi/utils/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.6.0/gmm_mi/utils/analytic_MI.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.6.0/gmm_mi/utils/plotting.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.6.0/gmm_mi/utils/transformations.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.859382 gmm_mi-0.6.0/gmm_mi.egg-info/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/requires.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/top_level.txt
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.955382 gmm_mi-0.6.0/notebooks/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.6.0/notebooks/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-05-15 22:09:14.985382 gmm_mi-0.6.0/setup.cfg
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-05-15 10:31:27.000000 gmm_mi-0.6.0/setup.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.167538 gmm_mi-0.7.0/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.7.0/LICENSE.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.7.0/LICENSE_EXT.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-05 18:05:58.165537 gmm_mi-0.7.0/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-30 14:51:38.000000 gmm_mi-0.7.0/README.md
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.061537 gmm_mi-0.7.0/gmm_mi/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.7.0/gmm_mi/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.7.0/gmm_mi/cross_validation.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.092537 gmm_mi-0.7.0/gmm_mi/data/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.7.0/gmm_mi/data/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.7.0/gmm_mi/data/synthetic_data.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    25656 2023-05-30 18:01:00.000000 gmm_mi-0.7.0/gmm_mi/gmm.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.7.0/gmm_mi/initializations.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45449 2023-05-30 15:21:34.000000 gmm_mi-0.7.0/gmm_mi/mi.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.7.0/gmm_mi/param_holders.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.7.0/gmm_mi/single_fit.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.150537 gmm_mi-0.7.0/gmm_mi/utils/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.7.0/gmm_mi/utils/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.7.0/gmm_mi/utils/analytic_MI.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.7.0/gmm_mi/utils/plotting.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.7.0/gmm_mi/utils/transformations.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.081537 gmm_mi-0.7.0/gmm_mi.egg-info/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/requires.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/top_level.txt
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.162537 gmm_mi-0.7.0/notebooks/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.7.0/notebooks/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-06-05 18:05:58.168537 gmm_mi-0.7.0/setup.cfg
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-06-04 15:25:40.000000 gmm_mi-0.7.0/setup.py
```

### Comparing `gmm_mi-0.6.0/LICENSE.txt` & `gmm_mi-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/LICENSE_EXT.txt` & `gmm_mi-0.7.0/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/PKG-INFO` & `gmm_mi-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm_mi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.6.0/README.md` & `gmm_mi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/cross_validation.py` & `gmm_mi-0.7.0/gmm_mi/cross_validation.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/data/synthetic_data.py` & `gmm_mi-0.7.0/gmm_mi/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/gmm.py` & `gmm_mi-0.7.0/gmm_mi/gmm.py`

 * *Files 6% similar despite different names*

```diff
@@ -322,52 +322,68 @@
         marginal_y = self.score_samples_marginal(points[:, 1:], index=1)
         MI = np.mean(joint - marginal_x - marginal_y)
         self.MI = MI
         return MI
     
     def estimate_cMI_MC(self, MC_samples=1e5):
         """Compute the conditional mutual information (cMI) associated with a particular GMM model, 
-        using MC integration. The order of variables matters: we compute MI(X, Y | Z), where Z is the
-        last variables among the three.
+        using MC integration. The order of variables matters: we compute MI(X, Y | Z_1, ..., z_n), 
+        where the Zs are the conditional variables.
         
         Parameters
         ----------
         MC_samples : integer, default=1e5
             Number of Monte Carlo (MC) samples to perform numerical integration of the MI integral.
         
         Returns
         -------
         MI : float
             The value of mutual information.
         """
         points, _ = self.sample(MC_samples)       
         # evaluate the log-likelihood for the joint probability
         joint = self.score_samples(points)
-        # we need to compute the marginal z; index=2 corresponds to z
-        marginal_z = self.score_samples_marginal(points[:, 2:], index=2)
-        # and the marginals (x, z) and (y, z) too; 
-        # for this we create some custom 2-D GMMs
-        # for xz
-        xz_m_mask = [True, False, True]
-        xz_c_mask = [[True, False, True],
-                     [False, False, False],
-                     [True, False, True]]
+        # we need to compute the marginal zs; indices>=2 correspond to zs
+        # we work with masks, where each time we set to False the variables which are not part of the integral
+        n = points.shape[1] # this gives the total number of variables involved
+        zs_m_mask = [True]*n
+        zs_m_mask[0], zs_m_mask[1] = False, False
+        # similarly for the covariances
+        zs_c_mask = [[False]*n]*n # nxn matrix of False
+        zs_c_mask = np.array(zs_c_mask)
+        zs_c_mask[2:, 2:] = True    
+        gmm_zs = GMMWithMI(n_components=self.n_components, weights_init=self.weights_,
+                     means_init=self.means_[:, zs_m_mask], covariances_init=self.covariances_[:, zs_c_mask].reshape(-1, n-2, n-2))
+        marginal_zs = gmm_zs.score_samples(points[:, zs_m_mask])        
+        # and the marginals (x, zs) and (y, zs) too
+        xz_m_mask = [True]*n
+        xz_m_mask[1] = False
+        xz_c_mask = [[True]*n]*n # nxn matrix of True in this case
+        # for e.g. a 3D case, this should look like (all True except one row and column)
+        #[[True,  False, True ],
+        # [False, False, False],
+        # [True,  False, True ]]
+        xz_c_mask = np.array(xz_c_mask)
+        xz_c_mask[:, 1] = False        
+        xz_c_mask[1, :] = False        
         gmm_xz = GMMWithMI(n_components=self.n_components, weights_init=self.weights_,
-                     means_init=self.means_[:, xz_m_mask], covariances_init=self.covariances_[:, xz_c_mask].reshape(-1, 2, 2))
+                     means_init=self.means_[:, xz_m_mask], covariances_init=self.covariances_[:, xz_c_mask].reshape(-1, n-1, n-1))
         marginal_xz = gmm_xz.score_samples(points[:, xz_m_mask])
-        # and for yz
-        yz_m_mask = [False, True, True]
-        yz_c_mask = [[False, False, False],
-                     [False, True, True],
-                     [False, True, True]]
+        # and for yz        
+        yz_m_mask = [True]*n
+        yz_m_mask[0] = False
+        yz_c_mask = [[True]*n]*n # nxn matrix of True
+        yz_c_mask = np.array(yz_c_mask)
+        yz_c_mask[:, 0] = False        
+        yz_c_mask[0, :] = False  
         gmm_yz = GMMWithMI(n_components=self.n_components, weights_init=self.weights_,
-                     means_init=self.means_[:, yz_m_mask], covariances_init=self.covariances_[:, yz_c_mask].reshape(-1, 2, 2))
+                     means_init=self.means_[:, yz_m_mask], covariances_init=self.covariances_[:, yz_c_mask].reshape(-1, n-1, n-1))
         marginal_yz = gmm_yz.score_samples(points[:, yz_m_mask])
         # finally, we put everything together
-        MI = np.mean(marginal_z + joint - marginal_xz - marginal_yz)
+        MI = np.mean(marginal_zs + joint - marginal_xz - marginal_yz)
         self.MI = MI
         return MI
     
     def estimate_KL_MC(self, kl_order='forward', MC_samples=1e5):
         """Compute the KL-divergence (KL) associated with a particular GMM model,
         using MC integration. The KL is meant between the marginal distributions p(x) and p(y).
         In particular, if `kl_order` is 'forward', KL[p(x)||p(y)] is computed.
```

### Comparing `gmm_mi-0.6.0/gmm_mi/initializations.py` & `gmm_mi-0.7.0/gmm_mi/initializations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/mi.py` & `gmm_mi-0.7.0/gmm_mi/mi.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,32 +117,32 @@
     
     def _check_shapes(self, X, Y):
         """ Check that the shapes of the arrays given as input to GMM-MI are either 2D or 1D,
         and return the correct array to give as input.
 
         Parameters
         ----------  
-        X : array-like of shape (n_samples, 2), (n_samples, 1), (n_samples) or (n_samples, 3)
+        X : array-like of shape (n_samples, 2), (n_samples, 1), (n_samples) or (n_samples, 2+n_var)
             Samples from the joint distribution of the two variables whose MI or KL is calculated.
             If Y is None, must be of shape (n_samples, 2); otherwise, it must be either (n_samples, 1) or (n_samples).
-            The (n_samples, 3) case is for the conditional MI(X, Y | Z).
+            The (n_samples, 2+n_var) case is for the conditional MI(X, Y | Z_1, ..., z_n), where conditional MI is computed.
         Y : array-like of shape (n_samples, 1) or (n_samples), default=None
             Samples from the marginal distribution of one of the two variables whose MI or KL is calculated.
             If None, X must be of shape (n_samples, 2); otherwise, X and Y must be (n_samples, 1) or (n_samples).
         
         Returns
         ----------
-        X : array-like of shape (n_samples, 2) or  (n_samples, 3)
-            The 2D array that is used to estimate MI or KL, with the expected shape.     
+        X : array-like of shape (n_samples, 2) or  (n_samples, 2+n_var)
+            The 2D (or higher-dimensional) array that is used to estimate MI or KL, with the expected shape.     
         """
         if len(X.shape) == 1:
             X = np.reshape(X, (X.shape[0], 1)) # add extra dimension       
         if Y is None:
-            if X.shape[1] != 2 and X.shape[1] != 3:
-                raise ValueError(f"Y is None, but the input array X is not 2- or 3-dimensional. "\
+            if X.shape[1] < 2:
+                raise ValueError(f"Y is None, but the input array X is not 2- (or higher-) dimensional. "\
                      f"In this case, both X and Y should be 1-dimensional.")
             else:
                 return X
         # if Y is not None, we can manipulate it    
         else:
             if len(Y.shape) == 1:
                 Y = np.reshape(Y, (Y.shape[0], 1)) # add extra dimension
@@ -419,19 +419,19 @@
 
         Parameters
         ----------  
         X : array-like of shape (n_samples, 2), (n_samples, 1), (n_samples) or (n_samples, 3)
             Samples from the joint distribution of the two variables whose MI or KL is calculated.
             If Y is None, must be of shape (n_samples, 2) or (n_samples, 3); 
             otherwise, it must be either (n_samples, 1) or (n_samples).
-            The case (n_samples, 3) is reserved for the conditional MI(X, Y | Z); 
+            The case (n_samples, 2+n_var) is reserved for the conditional MI(X, Y | Z_1, ..., Z_n); 
             the variables must be given in this order.
         Y : array-like of shape (n_samples, 1) or (n_samples), default=None
             Samples from the marginal distribution of one of the two variables whose MI or KL is calculated.
-            If None, X must be of shape (n_samples, 2) or (n_samples, 3); 
+            If None, X must be of shape (n_samples, 2) or (n_samples, 2+n_var); 
             otherwise, X and Y must be (n_samples, 1) or (n_samples).                   
         verbose : bool, default=False
             Whether to print useful procedural statements.
                 
         Returns
         ----------
         None
@@ -442,18 +442,18 @@
             if self.verbose:
                 print('Fit already done, not being repeated.')
             return
         
         # check shapes and proceed with fit
         X = self._check_shapes(X, Y)
         self.X = X
-        if X.shape[1] == 3:
+        if X.shape[1] >= 3:
             self.conditional = True
             if self.verbose:
-                print('Shape of input array is 3-D, so conditional mutual information '
+                print('Shape of input array is 3-D or higher, so conditional mutual information '
                       'will be computed.')
         
         if self.verbose:
             if not self.fixed_components:
                 print('Starting cross-validation procedure to select the number of GMM components...')
             else:
                 print(f'Using {self.fixed_components_number} GMM components, as specified in input.')
```

### Comparing `gmm_mi-0.6.0/gmm_mi/param_holders.py` & `gmm_mi-0.7.0/gmm_mi/param_holders.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/single_fit.py` & `gmm_mi-0.7.0/gmm_mi/single_fit.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/utils/analytic_MI.py` & `gmm_mi-0.7.0/gmm_mi/utils/analytic_MI.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/utils/plotting.py` & `gmm_mi-0.7.0/gmm_mi/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi/utils/transformations.py` & `gmm_mi-0.7.0/gmm_mi/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/gmm_mi.egg-info/PKG-INFO` & `gmm_mi-0.7.0/gmm_mi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm-mi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.6.0/gmm_mi.egg-info/SOURCES.txt` & `gmm_mi-0.7.0/gmm_mi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.6.0/setup.py` & `gmm_mi-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 PACKAGENAME = 'gmm_mi'
 
 setup(
     name='gmm_mi',
-    version="0.6.0",
+    version="0.7.0",
     author='Davide Piras',
     author_email='dr.davide.piras@gmail.com',
     description='Estimate mutual information distribution with Gaussian mixture models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dpiras/GMM-MI',
     license='GNU General Public License v3.0 (GPLv3)',
```

