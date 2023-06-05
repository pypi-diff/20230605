# Comparing `tmp/GraphCASE-0.0.5.tar.gz` & `tmp/GraphCASE-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.5.tar", last modified: Fri Jun  2 14:11:57 2023, max compression
+gzip compressed data, was "GraphCASE-0.0.6.tar", last modified: Mon Jun  5 08:41:39 2023, max compression
```

## Comparing `GraphCASE-0.0.5.tar` & `GraphCASE-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.543315 GraphCASE-0.0.5/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.539535 GraphCASE-0.0.5/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.5/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.5/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.5/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.5/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.5/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7979 2023-06-02 13:29:34.000000 GraphCASE-0.0.5/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-02 08:41:20.000000 GraphCASE-0.0.5/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    12754 2023-06-02 11:23:19.000000 GraphCASE-0.0.5/GAE/position_manager.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.542421 GraphCASE-0.0.5/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-02 14:11:56.000000 GraphCASE-0.0.5/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-02 14:11:57.000000 GraphCASE-0.0.5/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-02 14:11:56.000000 GraphCASE-0.0.5/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-02 14:11:57.000000 GraphCASE-0.0.5/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.5/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-02 14:11:57.542882 GraphCASE-0.0.5/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.5/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-02 14:11:57.543450 GraphCASE-0.0.5/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-02 14:11:23.000000 GraphCASE-0.0.5/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.309867 GraphCASE-0.0.6/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.307182 GraphCASE-0.0.6/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.6/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.6/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.6/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.6/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.6/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8247 2023-06-05 08:32:48.000000 GraphCASE-0.0.6/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-02 08:41:20.000000 GraphCASE-0.0.6/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    12754 2023-06-02 11:23:19.000000 GraphCASE-0.0.6/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.6/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-05 08:41:39.309039 GraphCASE-0.0.6/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-05 08:41:38.000000 GraphCASE-0.0.6/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-05 08:41:39.000000 GraphCASE-0.0.6/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-05 08:41:38.000000 GraphCASE-0.0.6/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-05 08:41:39.000000 GraphCASE-0.0.6/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.6/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-05 08:41:39.309527 GraphCASE-0.0.6/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.6/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-05 08:41:39.309979 GraphCASE-0.0.6/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-05 08:39:26.000000 GraphCASE-0.0.6/setup.py
```

### Comparing `GraphCASE-0.0.5/GAE/dataFeeder.py` & `GraphCASE-0.0.6/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.6/GAE/data_feeder_graphframes.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/data_feeder_nx.py` & `GraphCASE-0.0.6/GAE/data_feeder_nx.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/graph_case_controller.py` & `GraphCASE-0.0.6/GAE/graph_case_controller.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/graph_case_tools.py` & `GraphCASE-0.0.6/GAE/graph_case_tools.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/graph_reconstructor.py` & `GraphCASE-0.0.6/GAE/graph_reconstructor.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,49 +80,53 @@
             if (current_switch % 2) == 0: 
                 # add new node    
                 child = self.__add_node_edge(graph, parent, block[:, 0:1, :], is_incoming)
                 self.node_dict[layer][current_switch] = child
             else:
                 #retrieve node id of child
                 child = self.node_dict[layer][current_switch-1]
-            self.__process_blocks(graph, layer+1, block[:, 1:, :], child, block_nr_ratio)
+            if child != 0:
+                # only process block if the parent is not a dummy node
+                self.__process_blocks(graph, layer+1, block[:, 1:, :], child, block_nr_ratio)
 
         else:
             for i in range(tf.shape(block)[1].numpy()):
                 self.__add_node_edge(graph, parent, block[:, i:i+1, :], is_incoming)
 
     def __get_switch_count(self, layer):
         return np.prod(self.support_size[:layer - 1]) * 2 ** layer
 
     def __add_node_edge(self, graph, parent, node_edge, is_incoming=True):
         pos_enc = node_edge[0, 0, 0:self.pos_encoding_size]
         node = node_edge[0, 0, -self.node_dim:]
         node = np.concatenate([node, pos_enc], axis=0)
         edge = node_edge[0, 0, self.pos_encoding_size:self.pos_encoding_size + self.node_dim]
         
-        node_id = self.__add_node(graph, node)
+        node_id = self.__add_node(graph, node, parent)
         if node_id != 0: #  node is not a dummy node
             edge_feat = dict([('edge_feat'+str(i), t) for i, t in enumerate(edge.numpy())])
             if is_incoming:
                 graph.add_edge(node_id, parent, **edge_feat)
             else:
                 graph.add_edge(parent, node_id, **edge_feat)
         return node_id
 
-    def __add_node(self, graph, node):
+    def __add_node(self, graph, node, parent):
         new_id = graph.number_of_nodes() + 1
 
         # check if node matches dummy node.
         equal_count = len([i for i, j in zip(node, self.dummy) if abs(i - j) < self.delta])
         if equal_count >= node.shape[0] * self.fraction_sim:
             return 0
 
-        # check if node is already part of the graph.
+        # check if node is already part of the graph. 
+        # exclude the parent node in this check otherwise we get self loops
+        non_parent_nodes = [u for u in graph.nodes(data=True) if u[0]!=parent]
         if self.deduplicate:
-            for u in graph.nodes(data=True):
+            for u in non_parent_nodes:
                 u_feat = [v for k, v in sorted(u[1].items(), key=lambda tup: int(tup[0][4:]))]
                 count = len([i for i, j in zip(node, u_feat) if abs(i - j) < self.delta])
                 if count >= node.shape[0] * self.fraction_sim:
                     return u[0]
 
         # add node to graph.
         node_feat = dict([('feat'+str(i), t) for i, t in enumerate(node.flatten())])
```

### Comparing `GraphCASE-0.0.5/GAE/input_layer_constructor.py` & `GraphCASE-0.0.6/GAE/input_layer_constructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/model.py` & `GraphCASE-0.0.6/GAE/model.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/position_manager.py` & `GraphCASE-0.0.6/GAE/position_manager.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/GAE/transformation_layer.py` & `GraphCASE-0.0.6/GAE/transformation_layer.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/LICENSE.txt` & `GraphCASE-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.5/README.md` & `GraphCASE-0.0.6/README.md`

 * *Files identical despite different names*

