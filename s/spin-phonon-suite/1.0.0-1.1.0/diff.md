# Comparing `tmp/spin_phonon_suite-1.0.0.tar.gz` & `tmp/spin_phonon_suite-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-1.0.0.tar", last modified: Thu Jun  1 13:19:24 2023, max compression
+gzip compressed data, was "spin_phonon_suite-1.1.0.tar", last modified: Mon Jun  5 14:15:09 2023, max compression
```

## Comparing `spin_phonon_suite-1.0.0.tar` & `spin_phonon_suite-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1660 2023-06-01 13:19:22.000000 spin_phonon_suite-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.961727 spin_phonon_suite-1.0.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-01 13:19:22.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10655 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    35667 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.962726 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.481142 spin_phonon_suite-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-05 14:15:09.480225 spin_phonon_suite-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 14:15:09.481142 spin_phonon_suite-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-05 14:15:06.000000 spin_phonon_suite-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.479309 spin_phonon_suite-1.1.0/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 14:15:06.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10740 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    36219 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.480225 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-1.0.0/LICENSE` & `spin_phonon_suite-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/PKG-INFO` & `spin_phonon_suite-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.0.0/README.md` & `spin_phonon_suite-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/setup.py` & `spin_phonon_suite-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
@@ -38,15 +38,16 @@
         'angmom_suite>=1.11.1',
         'hpc_suite>=1.8.0',
         'matplotlib',
         'gaussian_suite>=1.11.0',
         'phonopy',
         'molvis>=0.3.0',
         'molcas_suite>=1.21.0',
-        'ase'
+        'ase',
+        'pymatgen'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'spin_phonon_suite = spin_phonon_suite.cli:main'
             ]
         }
```

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/cells.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 from phonopy.interface.vasp import read_vasp
 import numpy as np
 import numpy.linalg as la
 import molvis.core as mvis
 import matplotlib.cm as cm
 
 
-def generate_molecular_graph(structure):
+def generate_molecular_graph(structure, equivalent_positions):
     strategy = IsayevNN(cutoff=3.0, allow_pathological=True)
     graph = StructureGraph.with_local_env_strategy(structure, strategy, weights=True)
 
     # build directed multi-graph
     twoway = nx.MultiDiGraph(graph.graph)
     # nodes are labelled by species
-    nx.set_node_attributes(twoway, {node: {'specie': str(structure[node].specie)} for node in twoway})
+    nx.set_node_attributes(twoway,
+        {node: {'symm_equiv': (structure[node].specie, equivalent_positions[node])} for node in twoway})
 
     def flip_edge(u, v, data):
         return v, u, {key: tuple(-i for i in val) if key == 'to_jimage'
                       else val for key, val in data.items()}
 
     # edges are labelled by periodic image crossing
     twoway.add_edges_from([flip_edge(*edge) for edge in twoway.edges(data=True)])
@@ -41,15 +42,15 @@
     connected = nx.connected_components(nx.Graph(graph))
 
     subgraphs = map(graph.subgraph, connected)
 
     def filter_unique_graphs(graphs):
 
         edge_match = iso.numerical_edge_match("weight", 1.0)
-        node_match = iso.categorical_node_match("specie", None)
+        node_match = iso.categorical_node_match("symm_equiv", None)
 
         unique_graphs = set()
 
         for graph in graphs:
 
             def graph_match(g):
                 return nx.is_isomorphic(
@@ -90,22 +91,22 @@
     molecule = Molecule(species, coords)
 
     return list(shifts.keys()), molecule
 
 
 def get_unique_entities(structure):
 
-    molecular_graph = generate_molecular_graph(structure)
-    connected_graphs = split_molecular_graph(molecular_graph, filter_unique=True)
-    indices, molecules = zip(*map(lambda x: extract_molecule(structure, x), connected_graphs))
-
     sym_structure = SpacegroupAnalyzer(structure).get_symmetrized_structure()
     structure_dict = sym_structure.as_dict()
     equivalent_positions = structure_dict['equivalent_positions']
 
+    molecular_graph = generate_molecular_graph(structure, equivalent_positions)
+    connected_graphs = split_molecular_graph(molecular_graph, filter_unique=True)
+    indices, molecules = zip(*map(lambda x: extract_molecule(structure, x), connected_graphs))
+
     elements = [site.specie.symbol for site in structure]
 
     mappings = [[equivalent_positions[idx] for idx in shift_dict]
                 for shift_dict in indices]
 
     return equivalent_positions, elements, mappings, molecules
```

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,26 @@
     elif args.parse:
         parse_charges_func(equivalent_positions, elements, mappings, entities)
     else:
         ValueError(f"{args.mode} mode not supported!")
 
 
 def format_formula(formula):
-    return formula.replace(" ", "")
+
+    def split_symbol_number(x):
+        elem = re.search('([a-zA-Z]+)', x).group(0)
+        num = int(re.search('(\d+)', x).group(0))
+        return (elem, num)
+
+    def format_constituent(x):
+        return x[0] + str("" if x[1] == 1 else x[1])
+
+    constituents = map(split_symbol_number, formula.split(" "))
+    ordered = map(format_constituent, sorted(constituents, key=lambda x: x[0]))
+    return ''.join(ordered)
 
 
 def gen_charges_func(entities):
     """
     Wrapper function for cli call to charges gen
     """
 
@@ -369,14 +380,19 @@
 def parse_charges_func(equivalent_positions, elements, mappings, entities):
     """
     Wrapper function for cli call to charges parse
     """
 
     def read_charges(mol, idx):
         file = f"gaussian/{format_formula(mol.formula)}_{idx}.log"
+        charges = gscd.get_chelpg_charges(file)
+
+        if not charges:
+            raise ValueError(f"{file} does not contain charges!")
+
         return np.array(gscd.get_chelpg_charges(file))
 
     def symmetrize(mapping, charges):
         for val in np.unique(mapping):
             for idc in np.flatnonzero(mapping == val):
                 yield val, np.mean(charges[idc])
 
@@ -402,28 +418,28 @@
 
 
 def cluster_func(args):
 
     structure = Structure.from_file(args.poscar)
     central_index = args.central_index
     central_index_unit = (central_index - 1) % structure.num_sites
+    central_site = structure.sites[central_index_unit]
 
     if args.from_central:
         molecular_graph = cells.generate_molecular_graph(structure)
         connected_graphs = cells.split_molecular_graph(molecular_graph, filter_unique=False)
         central_graph = next(filter(lambda nodes: central_index_unit in nodes, connected_graphs))
         _, qm_region = cells.extract_molecule(structure, central_graph, central_index=central_index_unit)
+        shift = np.array([central_site.x, central_site.y, central_site.z])
     elif args.qm_region is not None:
-        _, qm_region = Molecule.from_file(args.qm_region)
+        qm_region = Molecule.from_file(args.qm_region)
+        shift = np.zeros(3)
     else:
         raise NotImplementedError()
 
-    central_site = structure.sites[central_index_unit]
-    shift = np.array([central_site.x, central_site.y, central_site.z])
-
     cluster = cells.build_cluster(args.poscar, central_index=central_index,
                                   distortion_expansion=args.distortion_expansion,
                                   distortion_expansion_old=args.distortion_expansion_old,
                                   distortion_cutoff=args.distortion_cutoff)
 
     def format_label(args):
         idx, specie = args
```

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/coordinates.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/coordinates.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/lvc.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-1.1.0/spin_phonon_suite/vibrations.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/SOURCES.txt` & `spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

