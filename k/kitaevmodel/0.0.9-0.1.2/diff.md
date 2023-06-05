# Comparing `tmp/kitaevmodel-0.0.9.tar.gz` & `tmp/kitaevmodel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitaevmodel-0.0.9.tar", last modified: Sun Jul  3 12:03:33 2022, max compression
+gzip compressed data, was "kitaevmodel-0.1.2.tar", last modified: Mon Jun  5 19:50:31 2023, max compression
```

## Comparing `kitaevmodel-0.0.9.tar` & `kitaevmodel-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-07-03 12:03:33.791149 kitaevmodel-0.0.9/
--rw-rw-rw-   0        0        0     1089 2022-07-02 13:29:52.000000 kitaevmodel-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      652 2022-07-03 12:03:33.790153 kitaevmodel-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       21 2022-07-02 13:29:52.000000 kitaevmodel-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-07-03 12:03:33.784134 kitaevmodel-0.0.9/kitaevmodel/
--rw-rw-rw-   0        0        0        0 2022-07-02 12:40:31.000000 kitaevmodel-0.0.9/kitaevmodel/__init__.py
--rw-rw-rw-   0        0        0      686 2022-07-02 13:15:22.000000 kitaevmodel-0.0.9/kitaevmodel/eigenstates.py
--rw-rw-rw-   0        0        0     3060 2022-07-03 11:31:47.000000 kitaevmodel-0.0.9/kitaevmodel/examples.py
--rw-rw-rw-   0        0        0     9103 2022-07-03 11:22:35.000000 kitaevmodel-0.0.9/kitaevmodel/hamiltonian_creator.py
--rw-rw-rw-   0        0        0     3588 2022-07-03 11:27:48.000000 kitaevmodel-0.0.9/kitaevmodel/image_generator.py
--rw-rw-rw-   0        0        0     2570 2022-07-03 11:25:18.000000 kitaevmodel-0.0.9/kitaevmodel/time_evolution.py
-drwxrwxrwx   0        0        0        0 2022-07-03 12:03:33.789173 kitaevmodel-0.0.9/kitaevmodel.egg-info/
--rw-rw-rw-   0        0        0      652 2022-07-03 12:03:33.000000 kitaevmodel-0.0.9/kitaevmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2022-07-03 12:03:33.000000 kitaevmodel-0.0.9/kitaevmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-03 12:03:33.000000 kitaevmodel-0.0.9/kitaevmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-07-03 12:03:33.000000 kitaevmodel-0.0.9/kitaevmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-03 12:03:33.000000 kitaevmodel-0.0.9/kitaevmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-03 12:03:33.791149 kitaevmodel-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      979 2022-07-03 12:02:42.000000 kitaevmodel-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/kitaevmodel/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-02 20:16:55.000000 kitaevmodel-0.1.2/kitaevmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12973 2023-06-05 19:31:59.000000 kitaevmodel-0.1.2/kitaevmodel/basesample.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-29 10:08:17.000000 kitaevmodel-0.1.2/kitaevmodel/eigenstates.py
+-rw-r--r--   0 root         (0) root         (0)     8937 2023-05-29 10:05:50.000000 kitaevmodel-0.1.2/kitaevmodel/hamiltonian_creator.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-05-29 10:08:29.000000 kitaevmodel-0.1.2/kitaevmodel/image_generator.py
+-rw-r--r--   0 root         (0) root         (0)    19562 2023-06-05 17:39:48.000000 kitaevmodel-0.1.2/kitaevmodel/shapes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/kitaevmodel/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 10:03:46.000000 kitaevmodel-0.1.2/kitaevmodel/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6325 2023-06-05 19:45:46.000000 kitaevmodel-0.1.2/kitaevmodel/tests/kitaevmodel_tests.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-06-02 10:34:24.000000 kitaevmodel-0.1.2/kitaevmodel/time_evolution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/kitaevmodel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-05 19:50:31.000000 kitaevmodel-0.1.2/kitaevmodel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      446 2023-06-05 19:50:31.000000 kitaevmodel-0.1.2/kitaevmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:50:31.000000 kitaevmodel-0.1.2/kitaevmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-05 19:50:31.000000 kitaevmodel-0.1.2/kitaevmodel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-05 19:50:31.000000 kitaevmodel-0.1.2/kitaevmodel.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 19:50:31.827601 kitaevmodel-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      981 2023-06-05 19:32:41.000000 kitaevmodel-0.1.2/setup.py
```

### Comparing `kitaevmodel-0.0.9/kitaevmodel/eigenstates.py` & `kitaevmodel-0.1.2/kitaevmodel/eigenstates.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import tensorflow as tf
-import networkx as nx
-
-def eigenstates(graph):
-    hamiltonian = tf.linalg.band_part(tf.constant(nx.to_numpy_matrix(graph),
-                                                  dtype=tf.complex64), 0, -1)
-
-    hamiltonian = (hamiltonian -
-                   tf.transpose(hamiltonian))
-    
-    return tf.linalg.eigh(1j * hamiltonian) 
-
-def eigenvals(graph):
-    hamiltonian = tf.linalg.band_part(tf.constant(nx.to_numpy_matrix(graph),
-                                                  dtype=tf.complex64), 0, -1)
-
-    hamiltonian = (hamiltonian -
-                   tf.transpose(hamiltonian))
-    
-    return tf.linalg.eigh(1j * hamiltonian)[0]
+import tensorflow as tf
+import networkx as nx
+
+def eigenstates(graph):
+    hamiltonian = tf.linalg.band_part(tf.constant(nx.to_numpy_matrix(graph),
+                                                  dtype=tf.complex64), 0, -1)
+
+    hamiltonian = (hamiltonian -
+                   tf.transpose(hamiltonian))
+    
+    return tf.linalg.eigh(1j * hamiltonian) 
+
+def eigenvals(graph):
+    hamiltonian = tf.linalg.band_part(tf.constant(nx.to_numpy_matrix(graph),
+                                                  dtype=tf.complex64), 0, -1)
+
+    hamiltonian = (hamiltonian -
+                   tf.transpose(hamiltonian))
+    
+    return tf.linalg.eigh(1j * hamiltonian)[0]
```

### Comparing `kitaevmodel-0.0.9/kitaevmodel/hamiltonian_creator.py` & `kitaevmodel-0.1.2/kitaevmodel/hamiltonian_creator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,282 @@
-import networkx as nx
-import numpy as np
-
-def node_dist(x,y, cx, cy):
-    return abs(cx-x) + abs(cy-y)
-
-def remove_unwanted_nodes(G, m, k):
-    cx, cy = k-0.5, 2*m -(m%2) 
-    
-    unwanted = []
-    for n in G.nodes:    
-        x,y = n
-        if node_dist(x,y, cx, cy) > (m + k):
-            unwanted.append(n)
-
-    for n in unwanted:
-        G.remove_node(n)
-        
-    return G
-
-def add_kappa(graph, kappa):
-    results = {}
-    for node in graph.nodes:
-        dist = set()
-        for el in graph.neighbors(node):
-            data = set(graph.neighbors(el))
-            dist = set.union(dist, data)
-        dist.remove(node)
-        
-        results[node] = dist
-        
-    for node, dist in results.items():
-        for el in dist:
-            if (el[0] + el[1]) % 2 == 0:
-                if el[0] != node[0]:
-                    if el[1] > node[1]:
-                        graph.add_edge(node, el, weight=-kappa)
-                    else:
-                        graph.add_edge(node, el, weight=kappa)
-                else:
-                    if el[1] > node[1]:
-                        graph.add_edge(node, el, weight=kappa)
-                    else:
-                        graph.add_edge(node, el, weight=-kappa)
-            if (el[0] + el[1]) % 2 == 1:
-                if el[0] != node[0]:
-                    if el[1] > node[1]:
-                        graph.add_edge(node, el, weight=kappa)
-                    else:
-                        graph.add_edge(node, el, weight=-kappa)
-                else:
-                    if el[1] > node[1]:
-                        graph.add_edge(node, el, weight=-kappa)
-                    else:
-                        graph.add_edge(node, el, weight=kappa)
-                
-    return graph
-
-def find_edge(graph):
-    result = {}
-    for node in graph.nodes:
-        neighbors = list(graph.neighbors(node))
-        if len(neighbors) == 2:
-            result[node] = neighbors  
-    return result
-
-def add_edge_nodes(graph, edge_nodes, hz, hb):
-    if hb:
-        pos = nx.get_node_attributes(graph, 'pos')
-        for node, value in edge_nodes.items():
-            first, second = value
-            place = (pos[node][0] + 
-                     (2 * pos[node][0] - pos[first][0] - pos[second][0]) * 1, 
-                     pos[node][1] + 
-                     (2 * pos[node][1] - pos[first][1] - pos[second][1]) * 1)
-            name = (node[0] + 10000, node[1] + 10001)
-            graph.add_node(name, pos=place)
-
-            graph.add_edge(name, node, weight=hb)
-            signi = graph[first][second]['weight']
-            graph.remove_edge(first, second)
-            graph.add_edge(first, second, weight=(signi / hz * hb))
-    else:
-        for node, value in edge_nodes.items():
-            first, second = value
-            graph.remove_edge(first, second)
-        
-    return graph
-
-def rectangular_lattice(m, n, kappa, hz, hb):
-    graph = nx.hexagonal_lattice_graph(m, n, periodic=False, 
-                               with_positions=True, 
-                               create_using=None)
-    
-    edge_nodes = find_edge(graph)
-    
-    for edge in graph.edges(data=True):
-        edge[2]['weight'] = 1
-    for u, v, d in graph.edges(data=True):
-        if (u[0] + u[1]) % 2 == 0:
-            d['weight'] = -1
-            
-    pos = nx.get_node_attributes(graph, 'pos')
-    coord = np.array(list(pos.values()))
-            
-    graph = add_kappa(graph, kappa)
-    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
-    
-    pos = nx.get_node_attributes(graph, 'pos')
-    if hb:
-        max_x = np.max(coord[:, 0]) + 2
-        max_y = np.max(coord[:, 1]) + np.sqrt(3)
-    else:
-        max_x = np.max(coord[:, 0])
-        max_y = np.max(coord[:, 1])
-    
-    return graph, pos, max_x, max_y
-
-def hexagon_lattice_zigzag(m, kappa, hz, hb):
-    graph = nx.hexagonal_lattice_graph(2*m-1,2*m-1, periodic=False, 
-                               with_positions=True, 
-                               create_using=None)
-    
-    graph = remove_unwanted_nodes(graph, m, m)
-    
-    edge_nodes = find_edge(graph)
-    
-    for edge in graph.edges(data=True):
-        edge[2]['weight'] = 1
-    for u, v, d in graph.edges(data=True):
-        if (u[0] + u[1]) % 2 == 0:
-            d['weight'] = -1
-            
-    pos = nx.get_node_attributes(graph, 'pos')
-    coord = np.array(list(pos.values()))
-            
-    graph = add_kappa(graph, kappa)
-    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
-    
-    pos = nx.get_node_attributes(graph, 'pos')
-    if hb:
-        max_x = np.max(coord[:, 0]) + 2
-        max_y = np.max(coord[:, 1]) + np.sqrt(3)
-    else:
-        max_x = np.max(coord[:, 0])
-        max_y = np.max(coord[:, 1])
-    
-    return graph, pos, max_x, max_y
-
-def stripe_lattice_zigzag(m, n, kappa, hz, hb):
-    graph = nx.hexagonal_lattice_graph(2*m-1,2*n - 1, periodic=False, 
-                               with_positions=True, 
-                               create_using=None)
-    
-    graph = remove_unwanted_nodes(graph, m, n)
-    
-    edge_nodes = find_edge(graph)
-    
-    for edge in graph.edges(data=True):
-        edge[2]['weight'] = 1
-    for u, v, d in graph.edges(data=True):
-        if (u[0] + u[1]) % 2 == 0:
-            d['weight'] = -1
-            
-    pos = nx.get_node_attributes(graph, 'pos')
-    coord = np.array(list(pos.values()))
-            
-    graph = add_kappa(graph, kappa)
-    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
-    
-    pos = nx.get_node_attributes(graph, 'pos')
-    if hb:
-        max_x = np.max(coord[:, 0]) + 2
-        max_y = np.max(coord[:, 1]) + np.sqrt(3)
-    else:
-        max_x = np.max(coord[:, 0])
-        max_y = np.max(coord[:, 1])
-    
-    return graph, pos, max_x, max_y
-
-def hexagon_check(m, pos):
-        x, y = map(abs, pos)
-        return y - 0.015 > np.sqrt(3) * min(m - x, m / 2)
-
-def remove_unwanted_nodes_armchair(G, m, k):
-    cx, cy = m + 1.5, k * np.sqrt(3) + 0.01
-    pos = nx.get_node_attributes(G, 'pos')
-    unwanted = []
-    for n in G.nodes: 
-        x, y = pos[n]
-        if hexagon_check(m, (x - cx, y - cy)) or n[1] == 4 * k + 1:
-            unwanted.append(n)
-
-    for n in unwanted:
-        G.remove_node(n)
-        
-    return G
-
-def hexagon_lattice_armchair(m, kappa, hz, hb):
-    m = m / 2 * 3 - 1
-    graph = nx.hexagonal_lattice_graph(4 * int(m), 3 * int(m + 1),
-                               periodic=False, 
-                               with_positions=True, 
-                               create_using=None)
-    
-    graph = remove_unwanted_nodes_armchair(graph, 2 * m, 2 * m)
-    
-    edge_nodes = find_edge(graph)
-    
-    for edge in graph.edges(data=True):
-        edge[2]['weight'] = 1
-    for u, v, d in graph.edges(data=True):
-        if (u[0] + u[1]) % 2 == 0:
-            d['weight'] = -1
-            
-    pos = nx.get_node_attributes(graph, 'pos')
-    coord = np.array(list(pos.values()))
-            
-    graph = add_kappa(graph, kappa)
-    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
-    
-    pos = nx.get_node_attributes(graph, 'pos')
-    if hb:
-        max_x = np.max(coord[:, 0]) + 2
-        max_y = np.max(coord[:, 1]) + np.sqrt(3)
-    else:
-        max_x = np.max(coord[:, 0])
-        max_y = np.max(coord[:, 1])
-    
-    return graph, pos, max_x, max_y
-
-def stripe_lattice_armchair(m, n, kappa, hz, hb):
-    m = m / 2 * 3 - 1
-    n = n / 2 * 3 - 1
-    graph = nx.hexagonal_lattice_graph(2 * int(n), 3 * int(m + 1),
-                               periodic=False, 
-                               with_positions=True, 
-                               create_using=None)
-    
-    graph = remove_unwanted_nodes_armchair(graph, 2 * m, n)
-    
-    edge_nodes = find_edge(graph)
-    
-    for edge in graph.edges(data=True):
-        edge[2]['weight'] = 1
-    for u, v, d in graph.edges(data=True):
-        if (u[0] + u[1]) % 2 == 0:
-            d['weight'] = -1
-            
-    pos = nx.get_node_attributes(graph, 'pos')
-    coord = np.array(list(pos.values()))
-            
-    graph = add_kappa(graph, kappa)
-    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
-    
-    pos = nx.get_node_attributes(graph, 'pos')
-    if hb:
-        max_x = np.max(coord[:, 0]) + 2
-        max_y = np.max(coord[:, 1]) + np.sqrt(3)
-    else:
-        max_x = np.max(coord[:, 0])
-        max_y = np.max(coord[:, 1])
-    
-    return graph, pos, max_x, max_y
-
-def add_disorder(graph, disorder, kappa_disorder):
-    N = graph.number_of_edges()
-    disorder_params = np.random.normal(1, disorder, N)
-    i = 0
-    for node_1, node_2, data in graph.edges(data=True):
-        weight = data['weight']
-        if np.abs(weight) > 0.5:
-            graph[node_1][node_2]['weight'] *= disorder_params[i]
-        else:
-            graph[node_1][node_2]['weight'] *= (disorder_params[i] * 
-                               kappa_disorder)
-        i += 1
-    return graph
+import networkx as nx
+import numpy as np
+
+def node_dist(x,y, cx, cy):
+    return abs(cx-x) + abs(cy-y)
+
+def remove_unwanted_nodes(G, m, k):
+    cx, cy = k-0.5, 2*m -(m%2) 
+    
+    unwanted = []
+    for n in G.nodes:    
+        x,y = n
+        if node_dist(x,y, cx, cy) > (m + k):
+            unwanted.append(n)
+
+    for n in unwanted:
+        G.remove_node(n)
+        
+    return G
+
+def add_kappa(graph, kappa):
+    results = {}
+    for node in graph.nodes:
+        dist = set()
+        for el in graph.neighbors(node):
+            data = set(graph.neighbors(el))
+            dist = set.union(dist, data)
+        dist.remove(node)
+        
+        results[node] = dist
+        
+    for node, dist in results.items():
+        for el in dist:
+            if (el[0] + el[1]) % 2 == 0:
+                if el[0] != node[0]:
+                    if el[1] > node[1]:
+                        graph.add_edge(node, el, weight=-kappa)
+                    else:
+                        graph.add_edge(node, el, weight=kappa)
+                else:
+                    if el[1] > node[1]:
+                        graph.add_edge(node, el, weight=kappa)
+                    else:
+                        graph.add_edge(node, el, weight=-kappa)
+            if (el[0] + el[1]) % 2 == 1:
+                if el[0] != node[0]:
+                    if el[1] > node[1]:
+                        graph.add_edge(node, el, weight=kappa)
+                    else:
+                        graph.add_edge(node, el, weight=-kappa)
+                else:
+                    if el[1] > node[1]:
+                        graph.add_edge(node, el, weight=-kappa)
+                    else:
+                        graph.add_edge(node, el, weight=kappa)
+                
+    return graph
+
+def find_edge(graph):
+    result = {}
+    for node in graph.nodes:
+        neighbors = list(graph.neighbors(node))
+        if len(neighbors) == 2:
+            result[node] = neighbors  
+    return result
+
+def add_edge_nodes(graph, edge_nodes, hz, hb):
+    if hb:
+        pos = nx.get_node_attributes(graph, 'pos')
+        for node, value in edge_nodes.items():
+            first, second = value
+            place = (pos[node][0] + 
+                     (2 * pos[node][0] - pos[first][0] - pos[second][0]) * 1, 
+                     pos[node][1] + 
+                     (2 * pos[node][1] - pos[first][1] - pos[second][1]) * 1)
+            name = (node[0] + 10000, node[1] + 10001)
+            graph.add_node(name, pos=place)
+
+            graph.add_edge(name, node, weight=hb)
+            signi = graph[first][second]['weight']
+            graph.remove_edge(first, second)
+            graph.add_edge(first, second, weight=(signi / hz * hb))
+    else:
+        for node, value in edge_nodes.items():
+            first, second = value
+            graph.remove_edge(first, second)
+        
+    return graph
+
+def rectangular_lattice(m, n, kappa, hz, hb):
+    graph = nx.hexagonal_lattice_graph(m, n, periodic=False, 
+                               with_positions=True, 
+                               create_using=None)
+    
+    edge_nodes = find_edge(graph)
+    
+    for edge in graph.edges(data=True):
+        edge[2]['weight'] = 1
+    for u, v, d in graph.edges(data=True):
+        if (u[0] + u[1]) % 2 == 0:
+            d['weight'] = -1
+            
+    pos = nx.get_node_attributes(graph, 'pos')
+    coord = np.array(list(pos.values()))
+            
+    graph = add_kappa(graph, kappa)
+    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
+    
+    pos = nx.get_node_attributes(graph, 'pos')
+    if hb:
+        max_x = np.max(coord[:, 0]) + 2
+        max_y = np.max(coord[:, 1]) + np.sqrt(3)
+    else:
+        max_x = np.max(coord[:, 0])
+        max_y = np.max(coord[:, 1])
+    
+    return graph, pos, max_x, max_y
+
+def hexagon_lattice_zigzag(m, kappa, hz, hb):
+    graph = nx.hexagonal_lattice_graph(2*m-1,2*m-1, periodic=False, 
+                               with_positions=True, 
+                               create_using=None)
+    
+    graph = remove_unwanted_nodes(graph, m, m)
+    
+    edge_nodes = find_edge(graph)
+    
+    for edge in graph.edges(data=True):
+        edge[2]['weight'] = 1
+    for u, v, d in graph.edges(data=True):
+        if (u[0] + u[1]) % 2 == 0:
+            d['weight'] = -1
+            
+    pos = nx.get_node_attributes(graph, 'pos')
+    coord = np.array(list(pos.values()))
+            
+    graph = add_kappa(graph, kappa)
+    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
+    
+    pos = nx.get_node_attributes(graph, 'pos')
+    if hb:
+        max_x = np.max(coord[:, 0]) + 2
+        max_y = np.max(coord[:, 1]) + np.sqrt(3)
+    else:
+        max_x = np.max(coord[:, 0])
+        max_y = np.max(coord[:, 1])
+    
+    return graph, pos, max_x, max_y
+
+def stripe_lattice_zigzag(m, n, kappa, hz, hb):
+    graph = nx.hexagonal_lattice_graph(2*m-1,2*n - 1, periodic=False, 
+                               with_positions=True, 
+                               create_using=None)
+    
+    graph = remove_unwanted_nodes(graph, m, n)
+    
+    edge_nodes = find_edge(graph)
+    
+    for edge in graph.edges(data=True):
+        edge[2]['weight'] = 1
+    for u, v, d in graph.edges(data=True):
+        if (u[0] + u[1]) % 2 == 0:
+            d['weight'] = -1
+            
+    pos = nx.get_node_attributes(graph, 'pos')
+    coord = np.array(list(pos.values()))
+            
+    graph = add_kappa(graph, kappa)
+    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
+    
+    pos = nx.get_node_attributes(graph, 'pos')
+    if hb:
+        max_x = np.max(coord[:, 0]) + 2
+        max_y = np.max(coord[:, 1]) + np.sqrt(3)
+    else:
+        max_x = np.max(coord[:, 0])
+        max_y = np.max(coord[:, 1])
+    
+    return graph, pos, max_x, max_y
+
+def hexagon_check(m, pos):
+        x, y = map(abs, pos)
+        return y - 0.015 > np.sqrt(3) * min(m - x, m / 2)
+
+def remove_unwanted_nodes_armchair(G, m, k):
+    cx, cy = m + 1.5, k * np.sqrt(3) + 0.01
+    pos = nx.get_node_attributes(G, 'pos')
+    unwanted = []
+    for n in G.nodes: 
+        x, y = pos[n]
+        if hexagon_check(m, (x - cx, y - cy)) or n[1] == 4 * k + 1:
+            unwanted.append(n)
+
+    for n in unwanted:
+        G.remove_node(n)
+        
+    return G
+
+def hexagon_lattice_armchair(m, kappa, hz, hb):
+    m = m / 2 * 3 - 1
+    graph = nx.hexagonal_lattice_graph(4 * int(m), 3 * int(m + 1),
+                               periodic=False, 
+                               with_positions=True, 
+                               create_using=None)
+    
+    graph = remove_unwanted_nodes_armchair(graph, 2 * m, 2 * m)
+    
+    edge_nodes = find_edge(graph)
+    
+    for edge in graph.edges(data=True):
+        edge[2]['weight'] = 1
+    for u, v, d in graph.edges(data=True):
+        if (u[0] + u[1]) % 2 == 0:
+            d['weight'] = -1
+            
+    pos = nx.get_node_attributes(graph, 'pos')
+    coord = np.array(list(pos.values()))
+            
+    graph = add_kappa(graph, kappa)
+    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
+    
+    pos = nx.get_node_attributes(graph, 'pos')
+    if hb:
+        max_x = np.max(coord[:, 0]) + 2
+        max_y = np.max(coord[:, 1]) + np.sqrt(3)
+    else:
+        max_x = np.max(coord[:, 0])
+        max_y = np.max(coord[:, 1])
+    
+    return graph, pos, max_x, max_y
+
+def stripe_lattice_armchair(m, n, kappa, hz, hb):
+    m = m / 2 * 3 - 1
+    n = n / 2 * 3 - 1
+    graph = nx.hexagonal_lattice_graph(2 * int(n), 3 * int(m + 1),
+                               periodic=False, 
+                               with_positions=True, 
+                               create_using=None)
+    
+    graph = remove_unwanted_nodes_armchair(graph, 2 * m, n)
+    
+    edge_nodes = find_edge(graph)
+    
+    for edge in graph.edges(data=True):
+        edge[2]['weight'] = 1
+    for u, v, d in graph.edges(data=True):
+        if (u[0] + u[1]) % 2 == 0:
+            d['weight'] = -1
+            
+    pos = nx.get_node_attributes(graph, 'pos')
+    coord = np.array(list(pos.values()))
+            
+    graph = add_kappa(graph, kappa)
+    graph = add_edge_nodes(graph, edge_nodes, hz, hb)
+    
+    pos = nx.get_node_attributes(graph, 'pos')
+    if hb:
+        max_x = np.max(coord[:, 0]) + 2
+        max_y = np.max(coord[:, 1]) + np.sqrt(3)
+    else:
+        max_x = np.max(coord[:, 0])
+        max_y = np.max(coord[:, 1])
+    
+    return graph, pos, max_x, max_y
+
+def add_disorder(graph, disorder, kappa_disorder):
+    N = graph.number_of_edges()
+    disorder_params = np.random.normal(1, disorder, N)
+    i = 0
+    for node_1, node_2, data in graph.edges(data=True):
+        weight = data['weight']
+        if np.abs(weight) > 0.5:
+            graph[node_1][node_2]['weight'] *= disorder_params[i]
+        else:
+            graph[node_1][node_2]['weight'] *= (disorder_params[i] * 
+                               kappa_disorder)
+        i += 1
+    return graph
+
+if __name__ == '__main__':
+    graph, pos, max_x, max_y = hexagon_lattice_zigzag(2, 0.1, 0.4, 0)
+    print(pos)
```

### Comparing `kitaevmodel-0.0.9/setup.py` & `kitaevmodel-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from setuptools import setup, find_packages
-
-VERSION = '0.0.9' 
-DESCRIPTION = 'A tool for numerical simulation of Kitaev honeycomb model'
-LONG_DESCRIPTION = 'A tool for numerical simulation of Kitaev honeycomb model'
-
-setup(
-        name="kitaevmodel", 
-        version=VERSION,
-        author="Igor Timoshuk",
-        author_email="<iltimoshuk@gmail.com>",
-        description=DESCRIPTION,
-        long_description=LONG_DESCRIPTION,
-        packages=find_packages(),
-        install_requires=['numpy', 'tensorflow', 
-        'networkx', 'matplotlib', 'scipy'],
-        
-        keywords=['python', 'Kitaev model'],
-        classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
-        ]
+from setuptools import setup, find_packages
+
+VERSION = '0.1.2' 
+DESCRIPTION = 'A tool for numerical simulation of Kitaev honeycomb model'
+LONG_DESCRIPTION = 'A tool for numerical simulation of Kitaev honeycomb model'
+
+setup(
+        name="kitaevmodel", 
+        version=VERSION,
+        author="Igor Timoshuk",
+        author_email="<iltimoshuk@gmail.com>",
+        description=DESCRIPTION,
+        long_description=LONG_DESCRIPTION,
+        packages=find_packages(),
+        install_requires=['numpy', 'tensorflow', 
+        'networkx', 'matplotlib', 'scipy', 'sympy'],
+        
+        keywords=['python', 'Kitaev model'],
+        classifiers= [
+            "Development Status :: 3 - Alpha",
+            "Intended Audience :: Education",
+            "Programming Language :: Python :: 3",
+            "Operating System :: MacOS :: MacOS X",
+            "Operating System :: Microsoft :: Windows",
+        ], 
+        test_suite='nose.collector',
+        tests_require=['nose']
 )
```

