# Comparing `tmp/pyTigerGraph-1.4.tar.gz` & `tmp/pyTigerGraph-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTigerGraph-1.4.tar", last modified: Wed May 17 13:09:20 2023, max compression
+gzip compressed data, was "pyTigerGraph-1.4.1.tar", last modified: Mon Jun  5 19:06:10 2023, max compression
```

## Comparing `pyTigerGraph-1.4.tar` & `pyTigerGraph-1.4.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.166810 pyTigerGraph-1.4/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3651 2023-05-17 13:09:20.167033 pyTigerGraph-1.4/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2022-12-09 01:43:49.000000 pyTigerGraph-1.4/README.md
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.130884 pyTigerGraph-1.4/pyTigerGraph/
--rw-r--r--   0 parkererickson   (502) staff       (20)      106 2023-05-17 13:08:48.000000 pyTigerGraph-1.4/pyTigerGraph/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5291 2022-12-07 20:53:19.000000 pyTigerGraph-1.4/pyTigerGraph/datasets.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.136577 pyTigerGraph-1.4/pyTigerGraph/gds/
--rw-r--r--   0 parkererickson   (502) staff       (20)      211 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.140504 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-04-27 20:50:55.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    96874 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    19285 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9288 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     5470 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)   187415 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/dataloaders.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    34331 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    90195 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gds.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.122000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.142857 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/
--rw-r--r--   0 parkererickson   (502) staff       (20)     4147 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     6185 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5048 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     7804 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8697 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5929 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.144453 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/
--rw-r--r--   0 parkererickson   (502) staff       (20)     1546 2023-04-24 16:45:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2727 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)    22448 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/metrics.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.146770 pyTigerGraph-1.4/pyTigerGraph/gds/models/
--rw-r--r--   0 parkererickson   (502) staff       (20)    13081 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/GraphSAGE.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5949 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/NodePieceMLP.py
--rw-r--r--   0 parkererickson   (502) staff       (20)       50 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.148705 pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)     6025 2023-04-28 00:32:54.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     3741 2023-04-28 00:26:44.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)      230 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     1807 2023-04-28 00:26:42.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     1286 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/models/base_model.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/splitters.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17898 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/trainer.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.150567 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.153082 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-04-27 20:50:55.000000 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     8138 2023-04-27 20:50:55.000000 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     2158 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/nodepiece_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9955 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/gds/transforms/pyg_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9356 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/gds/utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2388 2022-11-23 18:58:50.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraph.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17679 2023-01-09 15:28:36.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    16032 2023-04-24 16:45:07.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphDataset.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    47508 2023-02-20 22:23:49.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphException.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    10551 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphLoading.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    26454 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9169 2023-02-20 22:23:49.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    12154 2023-05-17 13:08:36.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-24 16:45:07.000000 pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphVertex.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pyTigerGraph-1.4/pyTigerGraph/visualization.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.132274 pyTigerGraph-1.4/pyTigerGraph.egg-info/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3651 2023-05-17 13:09:20.000000 pyTigerGraph-1.4/pyTigerGraph.egg-info/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     3579 2023-05-17 13:09:20.000000 pyTigerGraph-1.4/pyTigerGraph.egg-info/SOURCES.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)        1 2023-05-17 13:09:20.000000 pyTigerGraph-1.4/pyTigerGraph.egg-info/dependency_links.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       72 2023-05-17 13:09:20.000000 pyTigerGraph-1.4/pyTigerGraph.egg-info/requires.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       19 2023-05-17 13:09:20.000000 pyTigerGraph-1.4/pyTigerGraph.egg-info/top_level.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pyTigerGraph-1.4/pyproject.toml
--rw-r--r--   0 parkererickson   (502) staff       (20)       78 2023-05-17 13:09:20.167615 pyTigerGraph-1.4/setup.cfg
--rw-r--r--   0 parkererickson   (502) staff       (20)     2573 2022-12-07 20:53:19.000000 pyTigerGraph-1.4/setup.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-05-17 13:09:20.166432 pyTigerGraph-1.4/tests/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pyTigerGraph-1.4/tests/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/pyTigerGraphUnitTest.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pyTigerGraph-1.4/tests/test_datasets.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    29857 2023-02-16 15:58:12.000000 pyTigerGraph-1.4/tests/test_gds_BaseLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    10546 2023-02-16 15:58:12.000000 pyTigerGraph-1.4/tests/test_gds_EdgeLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_gds_EdgeNeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7448 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_GDS.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pyTigerGraph-1.4/tests/test_gds_GraphLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4700 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/tests/test_gds_GraphSAGE.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pyTigerGraph-1.4/tests/test_gds_HGTLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    33875 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_NeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3443 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/tests/test_gds_NodePiece.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-04-21 18:31:54.000000 pyTigerGraph-1.4/tests/test_gds_NodePieceLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4190 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_Trainer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pyTigerGraph-1.4/tests/test_gds_VertexLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pyTigerGraph-1.4/tests/test_gds_featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7436 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_metrics.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pyTigerGraph-1.4/tests/test_gds_splitters.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5404 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_gds_utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2300 2023-05-17 13:08:33.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4156 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11799 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      706 2022-12-12 17:45:12.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2526 2023-05-03 19:52:07.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-24 16:45:07.000000 pyTigerGraph-1.4/tests/test_pyTigerGraphVertex.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.768610 pyTigerGraph-1.4.1/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-06-05 19:06:10.768750 pyTigerGraph-1.4.1/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2022-12-09 01:43:49.000000 pyTigerGraph-1.4.1/README.md
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.732236 pyTigerGraph-1.4.1/pyTigerGraph/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      108 2023-06-05 19:04:18.000000 pyTigerGraph-1.4.1/pyTigerGraph/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5291 2022-12-07 20:53:19.000000 pyTigerGraph-1.4.1/pyTigerGraph/datasets.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.738560 pyTigerGraph-1.4.1/pyTigerGraph/gds/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      211 2023-05-19 15:14:44.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.742696 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-04-27 20:50:55.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    96874 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    19285 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9288 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5470 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)   187784 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/dataloaders.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    34331 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    90195 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gds.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.721420 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.746371 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8717 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10445 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5048 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7804 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8697 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5929 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.747431 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1546 2023-04-24 16:45:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2727 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)    22448 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/metrics.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.748798 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/
+-rw-r--r--   0 parkererickson   (502) staff       (20)    13081 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/GraphSAGE.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5949 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/NodePieceMLP.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)       50 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.750602 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6025 2023-04-28 00:32:54.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3741 2023-04-28 00:26:44.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)      230 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1807 2023-04-28 00:26:42.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1286 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/models/base_model.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/splitters.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17904 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/trainer.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.751378 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.753064 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-04-27 20:50:55.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8138 2023-04-27 20:50:55.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2158 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/nodepiece_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9955 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/pyg_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9356 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/gds/utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2388 2022-11-23 18:58:50.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraph.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17679 2023-01-09 15:28:36.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    16042 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphDataset.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    47508 2023-02-20 22:23:49.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphException.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10551 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphLoading.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    26454 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9169 2023-02-20 22:23:49.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    12154 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-24 16:45:07.000000 pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphVertex.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pyTigerGraph-1.4.1/pyTigerGraph/visualization.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.733493 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-06-05 19:06:10.000000 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3579 2023-06-05 19:06:10.000000 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)        1 2023-06-05 19:06:10.000000 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       72 2023-06-05 19:06:10.000000 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/requires.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       19 2023-06-05 19:06:10.000000 pyTigerGraph-1.4.1/pyTigerGraph.egg-info/top_level.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pyTigerGraph-1.4.1/pyproject.toml
+-rw-r--r--   0 parkererickson   (502) staff       (20)       78 2023-06-05 19:06:10.769244 pyTigerGraph-1.4.1/setup.cfg
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2573 2022-12-07 20:53:19.000000 pyTigerGraph-1.4.1/setup.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-06-05 19:06:10.768293 pyTigerGraph-1.4.1/tests/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pyTigerGraph-1.4.1/tests/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/pyTigerGraphUnitTest.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pyTigerGraph-1.4.1/tests/test_datasets.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    29857 2023-02-16 15:58:12.000000 pyTigerGraph-1.4.1/tests/test_gds_BaseLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10639 2023-06-05 18:01:30.000000 pyTigerGraph-1.4.1/tests/test_gds_EdgeLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_gds_EdgeNeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7448 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_GDS.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pyTigerGraph-1.4.1/tests/test_gds_GraphLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4700 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/tests/test_gds_GraphSAGE.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pyTigerGraph-1.4.1/tests/test_gds_HGTLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    33875 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_NeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3443 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/tests/test_gds_NodePiece.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-04-21 18:31:54.000000 pyTigerGraph-1.4.1/tests/test_gds_NodePieceLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4190 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_Trainer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pyTigerGraph-1.4.1/tests/test_gds_VertexLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pyTigerGraph-1.4.1/tests/test_gds_featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7436 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_metrics.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pyTigerGraph-1.4.1/tests/test_gds_splitters.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5404 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_gds_utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2300 2023-05-19 19:02:11.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4156 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11799 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      706 2022-12-12 17:45:12.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2526 2023-05-03 19:52:07.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-24 16:45:07.000000 pyTigerGraph-1.4.1/tests/test_pyTigerGraphVertex.py
```

### Comparing `pyTigerGraph-1.4/PKG-INFO` & `pyTigerGraph-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.4
+Version: 1.4.1
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.4/README.md` & `pyTigerGraph-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/datasets.py` & `pyTigerGraph-1.4.1/pyTigerGraph/datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/dataloaders.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/dataloaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -855,15 +855,15 @@
                 v_file = (line.split(delimiter) for line in raw.split('\n') if line)
                 data = pd.DataFrame(v_file, columns=v_attributes)
                 for column in data.columns:
                     data[column] = pd.to_numeric(data[column], errors="ignore")
                 for v_attr in v_attributes:
                     if v_attr_types.get(v_attr, "") == "MAP":
                         # I am sorry that this is this ugly...
-                        data[v_attr] = data[v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                        data[v_attr] = data[v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
             else:
                 v_file = (line.split(delimiter) for line in raw.split('\n') if line)
                 v_file_dict = defaultdict(list)
                 for line in v_file:
                     v_file_dict[line[0]].append(line[1:])
                 vertices = {}
                 for vtype in v_file_dict:
@@ -871,30 +871,30 @@
                                    v_in_feats.get(vtype, []) + \
                                    v_out_labels.get(vtype, []) + \
                                    v_extra_feats.get(vtype, [])
                     vertices[vtype] = pd.DataFrame(v_file_dict[vtype], columns=v_attributes)
                     for v_attr in v_extra_feats.get(vtype, []):
                         if v_attr_types[vtype][v_attr] == "MAP":
                             # I am sorry that this is this ugly...
-                            vertices[vtype][v_attr] = vertices[vtype][v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                            vertices[vtype][v_attr] = vertices[vtype][v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
                 data = vertices
         elif in_format == "edge":
             # String of edges in format source_vid,target_vid
             if not is_hetero:
                 e_attributes = ["source", "target"] + e_in_feats + e_out_labels + e_extra_feats
                 #file = "\n".join(x for x in raw.split("\n") if x.strip())
                 #data = pd.read_table(io.StringIO(file), header=None, names=e_attributes, sep=delimiter)
                 e_file = (line.split(delimiter) for line in raw.split('\n') if line)
                 data = pd.DataFrame(e_file, columns=e_attributes)
                 for column in data.columns:
                     data[column] = pd.to_numeric(data[column], errors="ignore")
                 for e_attr in e_attributes:
                     if e_attr_types.get(e_attr, "") == "MAP":
                         # I am sorry that this is this ugly...
-                        data[e_attr] = data[e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                        data[e_attr] = data[e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
             else:
                 e_file = (line.split(delimiter) for line in raw.split('\n') if line)
                 e_file_dict = defaultdict(list)
                 for line in e_file:
                     e_file_dict[line[0]].append(line[1:])
                 edges = {}
                 for etype in e_file_dict:
@@ -902,15 +902,15 @@
                                    e_in_feats.get(etype, []) + \
                                    e_out_labels.get(etype, [])  + \
                                    e_extra_feats.get(etype, [])
                     edges[etype] = pd.DataFrame(e_file_dict[etype], columns=e_attributes)
                     for e_attr in e_extra_feats.get(etype, []):
                         if e_attr_types[etype][e_attr] == "MAP":
                             # I am sorry that this is this ugly...
-                            edges[etype][e_attr] = edges[etype][e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                            edges[etype][e_attr] = edges[etype][e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
                 del e_file_dict, e_file
                 data = edges
         elif in_format == "graph":
             # A pair of in-memory CSVs (vertex, edge)
             v_file, e_file = raw
             if not is_hetero:
                 v_attributes = ["vid"] + v_in_feats + v_out_labels + v_extra_feats
@@ -919,29 +919,29 @@
                 v_file = (line.split(delimiter) for line in v_file.split('\n') if line)
                 vertices = pd.DataFrame(v_file, columns=v_attributes)
                 for column in vertices.columns:
                     vertices[column] = pd.to_numeric(vertices[column], errors="ignore")
                 for v_attr in v_extra_feats:
                     if v_attr_types[v_attr] == "MAP":
                         # I am sorry that this is this ugly...
-                        vertices[v_attr] = vertices[v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                        vertices[v_attr] = vertices[v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
                 if primary_id:
                     id_map = pd.DataFrame({"vid": primary_id.keys(), "primary_id": primary_id.values()})
                     vertices = vertices.merge(id_map.astype({"vid": vertices["vid"].dtype}), on="vid")
                     v_extra_feats.append("primary_id")
                 #file = "\n".join(x for x in e_file.split("\n") if x.strip())
                 e_file = (line.split(delimiter) for line in e_file.split('\n') if line)
                 #edges = pd.read_table(io.StringIO(file), header=None, names=e_attributes, dtype="object", sep=delimiter)
                 edges = pd.DataFrame(e_file, columns=e_attributes)
                 for column in edges.columns:
                     edges[column] = pd.to_numeric(edges[column], errors="ignore")
                 for e_attr in e_attributes:
                     if e_attr_types.get(e_attr, "") == "MAP":
                         # I am sorry that this is this ugly...
-                        edges[e_attr] = edges[e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                        edges[e_attr] = edges[e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
             else:
                 v_file = (line.split(delimiter) for line in v_file.split('\n') if line)
                 v_file_dict = defaultdict(list)
                 for line in v_file:
                     v_file_dict[line[0]].append(line[1:])
                 vertices = {}
                 for vtype in v_file_dict:
@@ -949,15 +949,15 @@
                                    v_in_feats.get(vtype, []) + \
                                    v_out_labels.get(vtype, []) + \
                                    v_extra_feats.get(vtype, [])
                     vertices[vtype] = pd.DataFrame(v_file_dict[vtype], columns=v_attributes, dtype="object")
                     for v_attr in v_extra_feats.get(vtype, []):
                         if v_attr_types[vtype][v_attr] == "MAP":
                             # I am sorry that this is this ugly...
-                            vertices[vtype][v_attr] = vertices[vtype][v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                            vertices[vtype][v_attr] = vertices[vtype][v_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
                 if primary_id:
                     id_map = pd.DataFrame({"vid": primary_id.keys(), "primary_id": primary_id.values()},
                                           dtype="object")
                     for vtype in vertices:
                         vertices[vtype] = vertices[vtype].merge(id_map, on="vid")
                         v_extra_feats[vtype].append("primary_id")
                 del v_file_dict, v_file
@@ -971,15 +971,15 @@
                                    e_in_feats.get(etype, []) + \
                                    e_out_labels.get(etype, [])  + \
                                    e_extra_feats.get(etype, [])
                     edges[etype] = pd.DataFrame(e_file_dict[etype], columns=e_attributes, dtype="object")
                     for e_attr in e_extra_feats.get(etype, []):
                         if e_attr_types[etype][e_attr] == "MAP":
                             # I am sorry that this is this ugly...
-                            edges[etype][e_attr] = edges[etype][e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]})
+                            edges[etype][e_attr] = edges[etype][e_attr].apply(lambda x: {y.split(",")[0].strip("("): y.split(",")[1].strip(")") for y in x.strip("[").strip("]").split(" ")[:-1]} if x != "" else {})
                 del e_file_dict, e_file
             data = (vertices, edges)
         else:
             raise NotImplementedError
         # Convert dataframes into PyG or DGL graphs
         if out_format.lower() == "pyg" or out_format.lower() == "dgl":
             if vertices is None or edges is None:
@@ -2063,23 +2063,24 @@
         else:
             self._etypes = list(self._e_schema.keys())
         self._etypes = sorted(self._etypes)
         # Initialize parameters for the query
         if batch_size:
             # If batch_size is given, calculate the number of batches
             if filter_by:
-                # TODO: get edge count with filter
-                raise NotImplementedError
+                num_edges = sum(self._graph.getEdgeStats(e_type)[e_type][filter_by if isinstance(filter_by, str) else filter_by[e_type]]["TRUE"] for e_type in self._etypes)
             else:
                 num_edges = sum(self._graph.getEdgeCount(i) for i in self._etypes)
             self.num_batches = math.ceil(num_edges / batch_size)
         else:
             # Otherwise, take the number of batches as is.
             self.num_batches = num_batches
         # Initialize the exporter
+        if batch_size:
+            self._payload["batch_size"] = batch_size
         self._payload["num_batches"] = self.num_batches
         if filter_by:
             self._payload["filter_by"] = filter_by
         self._payload["shuffle"] = shuffle
         self._payload["e_types"] = self._etypes
         self._payload["delimiter"] = self.delimiter
         # Output
@@ -3016,23 +3017,24 @@
         self._etypes = sorted(self._etypes)
         # Resolve seeds
         self._seed_types = self._etypes if ((not filter_by) or isinstance(filter_by, str)) else list(filter_by.keys())
         # Resolve number of batches
         if batch_size:
             # If batch_size is given, calculate the number of batches
             if filter_by:
-                # TODO: get edge count with filter
-                raise NotImplementedError("Cannot specify batch_size and filter_by at the same time. Please use num_batches and filter_by.")
+                num_edges = sum(self._graph.getEdgeStats(e_type)[e_type][filter_by if isinstance(filter_by, str) else filter_by[e_type]]["TRUE"] for e_type in self._etypes)
             else:
-                num_edges = sum(self._graph.getEdgeCount(i) for i in self._etypes)
+                num_edges = sum(self._graph.getEdgeCount(i) for i in self._seed_types)
             self.num_batches = math.ceil(num_edges / batch_size)
         else:
             # Otherwise, take the number of batches as is.
             self.num_batches = num_batches
         # Initialize parameters for the query
+        if batch_size:
+            self._payload["batch_size"] = batch_size
         self._payload["num_batches"] = self.num_batches
         self._payload["num_neighbors"] = num_neighbors
         self._payload["num_hops"] = num_hops
         self._payload["delimiter"] = delimiter
         if filter_by:
             if isinstance(filter_by, str):
                 self._payload["filter_by"] = filter_by
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/featurizer.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gds.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gds.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-CREATE QUERY edge_loader_{QUERYSUFFIX}(
+CREATE QUERY graph_loader_{QUERYSUFFIX}(
     INT num_batches=1, 
     BOOL shuffle=FALSE,
     STRING filter_by,
+    SET<STRING> v_types,
     SET<STRING> e_types,
     STRING delimiter,
     STRING kafka_address="",
     STRING kafka_topic,
     INT kafka_topic_partitions=1,
     STRING kafka_max_size="104857600",
     INT kafka_timeout=300000,
@@ -19,30 +20,29 @@
     STRING ssl_key_password="",
     STRING ssl_endpoint_identification_algorithm="",
     STRING sasl_kerberos_service_name="",
     STRING sasl_kerberos_keytab="",
     STRING sasl_kerberos_principal=""
 ) SYNTAX V1 { 
     /*
-    This query generates batches of edges.
+    This query generates the batches of edges and vertices attached to those edges.
 
     Parameters :
-      num_batches    : Number of batches to divide the edges.
-      shuffle        : Whether to shuffle edges before collecting data.
+      num_batches    : Number of batches to divide all edges.
+      shuffle        : Whether to shuffle vertices before collecting data.
       filter_by      : A Boolean attribute to determine which edges are included.
+      v_types        : Vertex types to be included.
       e_types        : Edge types to be included.
       kafka_address  : Address of the Kafka cluster to send data to.
       kafka_topic    : The Kafka topic to send data to.
-      kafka_topic_partitions: Number of partitions for the given Kafka topic.
-      kafka_max_size : Maximum Kafka message size.
       security_protocol : Security prototol for Kafka.
       sasl_mechanism : Authentication mechanism for Kafka.
       sasl_username  : SASL username for Kafka. 
-      sasl_password  : SASL password for Kafka. 
-      ssl_ca_location: Path to CA certificate for verifying the Kafka broker key
+      sasl_password  : SASL password for Kafka.
+      ssl_ca_location: Path to CA certificate for verifying the Kafka broker key.
     */
     INT num_vertices;
     INT kafka_errcode;
     SumAccum<INT> @tmp_id;
     SumAccum<STRING> @@kafka_error;
     UINT producer;
 
@@ -53,58 +53,80 @@
             sasl_mechanism, sasl_username, sasl_password, ssl_ca_location,
             ssl_certificate_location, ssl_key_location, ssl_key_password,
             ssl_endpoint_identification_algorithm, sasl_kerberos_service_name,
             sasl_kerberos_keytab, sasl_kerberos_principal);
     END;
 
     # Shuffle vertex ID if needed
-    start = {ANY};
+    start = {v_types};
     IF shuffle THEN
+        IF filter_by IS NOT NULL THEN
+            start = SELECT s FROM start:s WHERE s.getAttr(filter_by, "BOOL");
+        END;
         num_vertices = start.size();
         res = SELECT s 
               FROM start:s
               POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
     ELSE
         res = SELECT s 
               FROM start:s
               POST-ACCUM s.@tmp_id = getvid(s);
     END;
 
     # Generate batches
     FOREACH batch_id IN RANGE[0, num_batches-1] DO
+        SetAccum<VERTEX> @@vertices;
         SumAccum<STRING> @@e_batch;
-        start = {ANY};
+        SumAccum<STRING> @@v_batch;
+       
+        start = {v_types};
         IF filter_by IS NOT NULL THEN
             res = 
                 SELECT s
-                FROM start:s -(e_types:e)- :t
+                FROM start:s -(e_types:e)- v_types:t
                 WHERE e.getAttr(filter_by, "BOOL") and ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_batches==batch_id
                 ACCUM 
-                    {EDGEATTRS}; 
+                    {EDGEATTRS},
+                    @@vertices += s,
+                    @@vertices += t;
         ELSE
             res = 
                 SELECT s
-                FROM start:s -(e_types:e)- :t
+                FROM start:s -(e_types:e)- v_types:t
                 WHERE ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_batches==batch_id
                 ACCUM 
-                    {EDGEATTRS};
+                    {EDGEATTRS},
+                    @@vertices += s,
+                    @@vertices += t;
         END;
-        # Export batch
+    
+        # Get vertex attributes
+        v_in_batch = @@vertices;
+        attr = 
+            SELECT s
+            FROM v_in_batch:s 
+            POST-ACCUM 
+                {VERTEXATTRS};
+
         IF kafka_address != "" THEN
             # Write to kafka
+            kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
+            IF kafka_errcode!=0 THEN 
+                @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
+            END;
             kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "edge_batch_" + stringify(batch_id), @@e_batch);
-            IF kafka_errcode != 0 THEN 
+            IF kafka_errcode!=0 THEN 
                 @@kafka_error += ("Error sending edge batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
             END;
         ELSE
             # Add to response
-            PRINT @@e_batch AS edge_batch;
+            PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch;   
         END;
-    END; 
+    END;
     IF kafka_address != "" THEN
         kafka_errcode = close_kafka_producer(producer, kafka_timeout);
-        IF kafka_errcode != 0 THEN 
+        IF kafka_errcode!=0 THEN 
             @@kafka_error += ("Error shutting down Kafka producer: " + stringify(kafka_errcode) + "\n");
         END;
         PRINT @@kafka_error as kafkaError;
     END;
 }
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-CREATE QUERY edge_nei_loader_{QUERYSUFFIX}(
+CREATE QUERY hgt_loader_{QUERYSUFFIX}(
+    SET<VERTEX> input_vertices,
+    INT batch_size,
     INT num_batches=1, 
-    INT num_neighbors=10, 
     INT num_hops=2, 
     BOOL shuffle=FALSE,
     STRING filter_by,
     SET<STRING> v_types,
     SET<STRING> e_types,
     SET<STRING> seed_types,
     STRING delimiter,
@@ -20,137 +21,170 @@
     STRING ssl_ca_location="",
     STRING ssl_certificate_location="",
     STRING ssl_key_location="",
     STRING ssl_key_password="",
     STRING ssl_endpoint_identification_algorithm="",
     STRING sasl_kerberos_service_name="",
     STRING sasl_kerberos_keytab="",
-    STRING sasl_kerberos_principal=""
+    STRING sasl_kerberos_principal="",
+    INT num_heap_inserts = 10
 ) SYNTAX V1 { 
     /*
-    This query generates the batches of edges and vertices attached to those edges.
+    This query generates the neighborhood subgraphs of given seed vertices (i.e., `input_vertices`).
+    If seed vertices are not given, then it will divide all vertices into `num_batches`, and use each 
+    batch as seeds.
 
     Parameters :
-      num_batches    : Number of batches to divide all edges.
-      num_neighbors  : Number of neighbors to expand from seeds.
+      input_vertices : Seed vertices to gather neighborhood subgraphs.
+      num_batches    : Number of batches to divide all vertices into.
       num_hops       : Number of hops to traverse to get neighbors.
       shuffle        : Whether to shuffle vertices before collecting data.
-      filter_by      : A Boolean attribute to determine which edges are included.
+      filter_by      : A Boolean attribute to determine which vertices are eligible as seeds.
+                       Only effective when `input_vertices` is NULL.
       v_types        : Vertex types to be included.
       e_types        : Edge types to be included.
-      seed_types     : Edge types to be included as seeds.
+      seed_types     : Vertex types to be included as seeds.
       kafka_address  : Address of the Kafka cluster to send data to.
       kafka_topic    : The Kafka topic to send data to.
-      kafka_topic_partitions: Number of partitions for the given Kafka topic.
-      kafka_max_size : Maximum Kafka message size.
       security_protocol : Security prototol for Kafka.
       sasl_mechanism : Authentication mechanism for Kafka.
       sasl_username  : SASL username for Kafka. 
       sasl_password  : SASL password for Kafka. 
       ssl_ca_location: Path to CA certificate for verifying the Kafka broker key.
     */
+    TYPEDEF TUPLE<INT tmp_id, VERTEX v> ID_Tuple;
     INT num_vertices;
     INT kafka_errcode;
     SumAccum<INT> @tmp_id;
     SumAccum<STRING> @@kafka_error;
     UINT producer;
+    INT batch_s;
+    OrAccum @prev_sampled;
 
     # Initialize Kafka producer
     IF kafka_address != "" THEN
         producer = init_kafka_producer(
             kafka_address, kafka_max_size, security_protocol, 
             sasl_mechanism, sasl_username, sasl_password, ssl_ca_location,
             ssl_certificate_location, ssl_key_location, ssl_key_password,
             ssl_endpoint_identification_algorithm, sasl_kerberos_service_name,
             sasl_kerberos_keytab, sasl_kerberos_principal);
     END;
 
     # Shuffle vertex ID if needed
-    start = {v_types};
-    IF shuffle THEN
-        num_vertices = start.size();
-        res = SELECT s 
-              FROM start:s
-              POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
-    ELSE
-        res = SELECT s 
-              FROM start:s
-              POST-ACCUM s.@tmp_id = getvid(s);
+    IF input_vertices.size()==0 THEN
+        start = {seed_types};
+        IF filter_by IS NOT NULL THEN
+            start = SELECT s FROM start:s WHERE s.getAttr(filter_by, "BOOL");
+        END;
+        IF shuffle THEN
+            num_vertices = start.size();
+            res = SELECT s 
+                FROM start:s
+                POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
+        ELSE
+            res = SELECT s 
+                FROM start:s
+                POST-ACCUM s.@tmp_id = getvid(s);
+        END;
+    END;
+    IF batch_size IS NULL THEN
+      batch_s = ceil(res.size()/num_batches);
+    ELSE  
+      batch_s = batch_size;
     END;
 
-    # Generate batches
+    # Generate subgraphs
     FOREACH batch_id IN RANGE[0, num_batches-1] DO
-        SetAccum<VERTEX> @@vertices;
-        SumAccum<STRING> @@e_batch;
         SumAccum<STRING> @@v_batch;
+        SumAccum<STRING> @@e_batch;
+        SetAccum<VERTEX> @@printed_vertices;
         SetAccum<EDGE> @@printed_edges;
-       
-        start = {v_types};
-        IF filter_by IS NOT NULL THEN
-            res = 
-                SELECT s
-                FROM start:s -(seed_types:e)- v_types:t
-                WHERE e.getAttr(filter_by, "BOOL") and ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_batches==batch_id
-                ACCUM 
-                    {SEEDEDGEATTRS},
-                    @@printed_edges += e,
-                    @@vertices += s,
-                    @@vertices += t;
+        SetAccum<VERTEX> @@seeds;
+        # Get seeds
+        IF input_vertices.size()==0 THEN
+            start = {seed_types};
+            HeapAccum<ID_Tuple> (1, tmp_id ASC) @@batch_heap;
+            @@batch_heap.resize(batch_s);
+            IF filter_by IS NOT NULL THEN
+                FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
+                  _verts = SELECT s FROM start:s
+                         WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled AND s.getAttr(filter_by, "BOOL")
+                         POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
+                END;
+                FOREACH elem IN @@batch_heap DO
+                  @@seeds += elem.v;
+                END;
+                seeds = {@@seeds};
+                seeds = SELECT s 
+                        FROM seeds:s 
+                        POST-ACCUM 
+                            s.@prev_sampled += TRUE,
+                            {SEEDVERTEXATTRS},
+                            @@printed_vertices += s;
+            ELSE
+                FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
+                  _verts = SELECT s FROM start:s
+                           WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled
+                           POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
+                END;
+                FOREACH elem IN @@batch_heap DO
+                  @@seeds += elem.v;
+                END;
+                seeds = {@@seeds};
+                seeds = SELECT s 
+                        FROM start:s
+                        POST-ACCUM
+                            s.@prev_sampled += TRUE,
+                            {SEEDVERTEXATTRS},
+                            @@printed_vertices += s;
+            END;
         ELSE
-            res = 
-                SELECT s
-                FROM start:s -(seed_types:e)- v_types:t
-                WHERE ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_batches==batch_id
-                ACCUM 
-                    {SEEDEDGEATTRS},
-                    @@printed_edges += e,
-                    @@vertices += s,
-                    @@vertices += t;
+            start = input_vertices;
+            seeds = SELECT s 
+                    FROM start:s 
+                    POST-ACCUM
+                        @@printed_vertices += s,
+                        {SEEDVERTEXATTRS};
         END;
-    
-        # Get seed vertices
-        v_in_batch = @@vertices;
-        seeds = 
-            SELECT s 
-            FROM v_in_batch:s 
-            POST-ACCUM
-                {VERTEXATTRS};
         # Get neighbors of seeeds
         FOREACH i IN RANGE[1, num_hops] DO
-            seeds = SELECT t
-                    FROM seeds:s -(e_types:e)- v_types:t 
-                    SAMPLE num_neighbors EDGE WHEN s.outdegree() >= 1
-                    ACCUM
-                        IF NOT @@printed_edges.contains(e) THEN
-                            {OTHEREDGEATTRS},
-                            @@printed_edges += e
-                        END;
-            attr = 
-                SELECT s
+            {SELECTNEIGHBORS}
+            attr = SELECT s
                 FROM seeds:s 
                 POST-ACCUM 
-                    IF NOT @@vertices.contains(s) THEN
-                        {VERTEXATTRS},
-                        @@vertices += s
+                    IF NOT @@printed_vertices.contains(s) THEN
+                        @@printed_vertices += s,
+                        {OTHERVERTEXATTRS}
                     END;
-        END;        
+        END;
         IF kafka_address != "" THEN
             # Write to kafka
             kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
             IF kafka_errcode!=0 THEN 
                 @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
             END;
             kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "edge_batch_" + stringify(batch_id), @@e_batch);
             IF kafka_errcode!=0 THEN 
                 @@kafka_error += ("Error sending edge batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
             END;
         ELSE
             # Add to response
-            PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch;   
-        END;
+            IF input_vertices.size()==0 THEN
+                PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch;  
+            ELSE
+                MapAccum<UINT, VERTEX> @@id_map;
+                source = @@printed_vertices;
+                res = 
+                    SELECT s 
+                    FROM source:s
+                    POST-ACCUM @@id_map += (getvid(s) -> s);
+                PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch, @@id_map AS pids; 
+            END;
+        END;                          
     END;
     IF kafka_address != "" THEN
         kafka_errcode = close_kafka_producer(producer, kafka_timeout);
         IF kafka_errcode!=0 THEN 
             @@kafka_error += ("Error shutting down Kafka producer: " + stringify(kafka_errcode) + "\n");
         END;
         PRINT @@kafka_error as kafkaError;
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-CREATE QUERY hgt_loader_{QUERYSUFFIX}(
+CREATE QUERY neighbor_loader_{QUERYSUFFIX}(
     SET<VERTEX> input_vertices,
     INT batch_size,
-    INT num_batches=1, 
+    INT num_batches=1,
+    INT num_neighbors=10, 
     INT num_hops=2, 
     BOOL shuffle=FALSE,
     STRING filter_by,
     SET<STRING> v_types,
     SET<STRING> e_types,
     SET<STRING> seed_types,
     STRING delimiter,
@@ -32,23 +33,26 @@
     This query generates the neighborhood subgraphs of given seed vertices (i.e., `input_vertices`).
     If seed vertices are not given, then it will divide all vertices into `num_batches`, and use each 
     batch as seeds.
 
     Parameters :
       input_vertices : Seed vertices to gather neighborhood subgraphs.
       num_batches    : Number of batches to divide all vertices into.
+      num_neighbors  : Number of neighbors to expand from seeds.
       num_hops       : Number of hops to traverse to get neighbors.
       shuffle        : Whether to shuffle vertices before collecting data.
       filter_by      : A Boolean attribute to determine which vertices are eligible as seeds.
                        Only effective when `input_vertices` is NULL.
       v_types        : Vertex types to be included.
       e_types        : Edge types to be included.
       seed_types     : Vertex types to be included as seeds.
       kafka_address  : Address of the Kafka cluster to send data to.
       kafka_topic    : The Kafka topic to send data to.
+      kafka_topic_partitions: Number of partitions for the given Kafka topic.
+      kafka_max_size : Maximum Kafka message size.
       security_protocol : Security prototol for Kafka.
       sasl_mechanism : Authentication mechanism for Kafka.
       sasl_username  : SASL username for Kafka. 
       sasl_password  : SASL password for Kafka. 
       ssl_ca_location: Path to CA certificate for verifying the Kafka broker key.
     */
     TYPEDEF TUPLE<INT tmp_id, VERTEX v> ID_Tuple;
@@ -88,15 +92,14 @@
         END;
     END;
     IF batch_size IS NULL THEN
       batch_s = ceil(res.size()/num_batches);
     ELSE  
       batch_s = batch_size;
     END;
-
     # Generate subgraphs
     FOREACH batch_id IN RANGE[0, num_batches-1] DO
         SumAccum<STRING> @@v_batch;
         SumAccum<STRING> @@e_batch;
         SetAccum<VERTEX> @@printed_vertices;
         SetAccum<EDGE> @@printed_edges;
         SetAccum<VERTEX> @@seeds;
@@ -139,26 +142,33 @@
                             @@printed_vertices += s;
             END;
         ELSE
             start = input_vertices;
             seeds = SELECT s 
                     FROM start:s 
                     POST-ACCUM
-                        @@printed_vertices += s,
-                        {SEEDVERTEXATTRS};
+                        {SEEDVERTEXATTRS},
+                        @@printed_vertices += s;
         END;
         # Get neighbors of seeeds
         FOREACH i IN RANGE[1, num_hops] DO
-            {SELECTNEIGHBORS}
+            seeds = SELECT t
+                    FROM seeds:s -(e_types:e)- v_types:t 
+                    SAMPLE num_neighbors EDGE WHEN s.outdegree() >= 1
+                    ACCUM
+                        IF NOT @@printed_edges.contains(e) THEN
+                            {EDGEATTRS},
+                            @@printed_edges += e
+                        END;
             attr = SELECT s
                 FROM seeds:s 
                 POST-ACCUM 
                     IF NOT @@printed_vertices.contains(s) THEN
-                        @@printed_vertices += s,
-                        {OTHERVERTEXATTRS}
+                        {OTHERVERTEXATTRS},
+                        @@printed_vertices += s
                     END;
         END;
         IF kafka_address != "" THEN
             # Write to kafka
             kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
             IF kafka_errcode!=0 THEN 
                 @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql`

 * *Files 23% similar despite different names*

```diff
@@ -1,202 +1,233 @@
-CREATE QUERY neighbor_loader_{QUERYSUFFIX}(
-    SET<VERTEX> input_vertices,
-    INT batch_size,
-    INT num_batches=1,
-    INT num_neighbors=10, 
-    INT num_hops=2, 
-    BOOL shuffle=FALSE,
-    STRING filter_by,
-    SET<STRING> v_types,
-    SET<STRING> e_types,
-    SET<STRING> seed_types,
-    STRING delimiter,
-    STRING kafka_address="",
-    STRING kafka_topic,
-    INT kafka_topic_partitions=1,
-    STRING kafka_max_size="104857600",
-    INT kafka_timeout=300000,
-    STRING security_protocol="",
-    STRING sasl_mechanism="",
-    STRING sasl_username="",
-    STRING sasl_password="",
-    STRING ssl_ca_location="",
-    STRING ssl_certificate_location="",
-    STRING ssl_key_location="",
-    STRING ssl_key_password="",
-    STRING ssl_endpoint_identification_algorithm="",
-    STRING sasl_kerberos_service_name="",
-    STRING sasl_kerberos_keytab="",
-    STRING sasl_kerberos_principal="",
-    INT num_heap_inserts = 10
-) SYNTAX V1 { 
-    /*
-    This query generates the neighborhood subgraphs of given seed vertices (i.e., `input_vertices`).
-    If seed vertices are not given, then it will divide all vertices into `num_batches`, and use each 
-    batch as seeds.
-
-    Parameters :
-      input_vertices : Seed vertices to gather neighborhood subgraphs.
-      num_batches    : Number of batches to divide all vertices into.
-      num_neighbors  : Number of neighbors to expand from seeds.
-      num_hops       : Number of hops to traverse to get neighbors.
-      shuffle        : Whether to shuffle vertices before collecting data.
-      filter_by      : A Boolean attribute to determine which vertices are eligible as seeds.
-                       Only effective when `input_vertices` is NULL.
-      v_types        : Vertex types to be included.
-      e_types        : Edge types to be included.
-      seed_types     : Vertex types to be included as seeds.
-      kafka_address  : Address of the Kafka cluster to send data to.
-      kafka_topic    : The Kafka topic to send data to.
-      kafka_topic_partitions: Number of partitions for the given Kafka topic.
-      kafka_max_size : Maximum Kafka message size.
-      security_protocol : Security prototol for Kafka.
-      sasl_mechanism : Authentication mechanism for Kafka.
-      sasl_username  : SASL username for Kafka. 
-      sasl_password  : SASL password for Kafka. 
-      ssl_ca_location: Path to CA certificate for verifying the Kafka broker key.
-    */
+CREATE QUERY nodepiece_loader_{QUERYSUFFIX}(
+  SET<VERTEX> input_vertices,
+  SET<STRING> v_types,
+  SET<STRING> e_types,
+  SET<STRING> seed_types,
+  BOOL compute_all = TRUE,
+  BOOL clear_cache = TRUE,
+  BOOL use_cache = TRUE,
+  BOOL precompute = FALSE,
+  STRING filter_by,
+  STRING anchor_attr,
+  INT max_distance,
+  INT max_anchors,
+  INT max_rel_context,
+  INT batch_size,
+  INT num_batches=1,
+  BOOL shuffle=FALSE,
+  STRING delimiter,
+  STRING kafka_address="",
+  STRING kafka_topic,
+  INT kafka_topic_partitions=1,
+  STRING kafka_max_size="104857600",
+  INT kafka_timeout=300000,
+  STRING security_protocol="",
+  STRING sasl_mechanism="",
+  STRING sasl_username="",
+  STRING sasl_password="",
+  STRING ssl_ca_location="",
+  STRING ssl_certificate_location="",
+  STRING ssl_key_location="",
+  STRING ssl_key_password="",
+  STRING ssl_endpoint_identification_algorithm="",
+  STRING sasl_kerberos_service_name="",
+  STRING sasl_kerberos_keytab="",
+  STRING sasl_kerberos_principal="",
+  INT num_heap_inserts=10,
+  INT num_edge_batches=10
+) SYNTAX v1{ 
+    TYPEDEF TUPLE<INT v_id, INT distance> Distance_Tuple;
     TYPEDEF TUPLE<INT tmp_id, VERTEX v> ID_Tuple;
     INT num_vertices;
     INT kafka_errcode;
+    INT batch_s;
     SumAccum<INT> @tmp_id;
     SumAccum<STRING> @@kafka_error;
-    UINT producer;
-    INT batch_s;
+    SetAccum<VERTEX> @next_pass, @to_pass, @received;
+    HeapAccum<Distance_Tuple> (max_anchors, distance ASC) @token_heap;
+    SumAccum<STRING> @rel_context_set;
+    SumAccum<STRING> @ancs;
     OrAccum @prev_sampled;
+    OrAccum @heapFull;
+
+    MapAccum<VERTEX, SumAccum<INT>> @@token_count;
+    MapAccum<INT, MinAccum<INT>> @conv_map;
+    BOOL cache_empty = FALSE;
+    INT distance;
+    UINT producer;
 
     # Initialize Kafka producer
     IF kafka_address != "" THEN
         producer = init_kafka_producer(
             kafka_address, kafka_max_size, security_protocol, 
             sasl_mechanism, sasl_username, sasl_password, ssl_ca_location,
             ssl_certificate_location, ssl_key_location, ssl_key_password,
             ssl_endpoint_identification_algorithm, sasl_kerberos_service_name,
             sasl_kerberos_keytab, sasl_kerberos_principal);
     END;
 
-    # Shuffle vertex ID if needed
-    IF input_vertices.size()==0 THEN
+    start = {v_types};
+    # Perform fetch operation if desired
+    IF clear_cache THEN
+      res = SELECT s FROM start:s POST-ACCUM s.{ANCHOR_CACHE_ATTRIBUTE} = s.@conv_map;
+    END;
+    IF input_vertices.size() != 0 AND NOT compute_all THEN
+      seeds = {input_vertices};
+      res = SELECT s FROM seeds:s -(e_types)- v_types:t
+            ACCUM
+              IF s.{ANCHOR_CACHE_ATTRIBUTE}.size() != 0 THEN
+                FOREACH (key, val) IN s.{ANCHOR_CACHE_ATTRIBUTE} DO  # s.{ANCHOR_CACHE_ATTRIBUTE} should be changed to getAttr() when supported
+                  s.@token_heap += Distance_Tuple(key, val)
+                END
+              ELSE
+                FOREACH (key, val) IN t.{ANCHOR_CACHE_ATTRIBUTE} DO
+                  s.@token_heap += Distance_Tuple(key, val)
+                END
+              END
+            POST-ACCUM
+              IF s.@token_heap.size() == 0 THEN
+                cache_empty = TRUE
+              END;
+    ELSE
+      cache_empty = TRUE;
+    END;
+    IF cache_empty THEN  # computing all, shuffle vertices if needed
+        ancs = SELECT s 
+           FROM start:s 
+           WHERE s.getAttr(anchor_attr, "BOOL")
+           POST-ACCUM s.@token_heap += Distance_Tuple(getvid(s), 0);
         start = {seed_types};
         IF filter_by IS NOT NULL THEN
             start = SELECT s FROM start:s WHERE s.getAttr(filter_by, "BOOL");
         END;
         IF shuffle THEN
             num_vertices = start.size();
             res = SELECT s 
                 FROM start:s
                 POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
         ELSE
             res = SELECT s 
                 FROM start:s
                 POST-ACCUM s.@tmp_id = getvid(s);
         END;
+        FOREACH i IN RANGE [1, max_distance] DO
+          LOG(TRUE, "ANCHOR MESSAGE DISTANCE", i);
+          FOREACH j IN RANGE [0, num_edge_batches-1] DO
+            LOG(TRUE, "ANCHOR BATCH", j);
+            ancs = SELECT t
+                 FROM ancs:s -(e_types:e)-v_types:t WHERE t.@heapFull == False AND ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_edge_batches == j
+                 ACCUM 
+                  FOREACH tup IN s.@token_heap DO 
+                    t.@token_heap += Distance_Tuple(tup.v_id, i)
+                  END
+                POST-ACCUM
+                  IF s.@token_heap.size() == max_anchors THEN
+                    s.@heapFull += TRUE
+                  END;
+          END;
+        END;
     END;
     IF batch_size IS NULL THEN
       batch_s = ceil(res.size()/num_batches);
     ELSE  
       batch_s = batch_size;
     END;
-    # Generate subgraphs
     FOREACH batch_id IN RANGE[0, num_batches-1] DO
-        SumAccum<STRING> @@v_batch;
-        SumAccum<STRING> @@e_batch;
-        SetAccum<VERTEX> @@printed_vertices;
-        SetAccum<EDGE> @@printed_edges;
-        SetAccum<VERTEX> @@seeds;
-        # Get seeds
-        IF input_vertices.size()==0 THEN
-            start = {seed_types};
-            HeapAccum<ID_Tuple> (1, tmp_id ASC) @@batch_heap;
-            @@batch_heap.resize(batch_s);
-            IF filter_by IS NOT NULL THEN
-                FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
-                  _verts = SELECT s FROM start:s
-                         WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled AND s.getAttr(filter_by, "BOOL")
-                         POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
-                END;
-                FOREACH elem IN @@batch_heap DO
-                  @@seeds += elem.v;
-                END;
-                seeds = {@@seeds};
-                seeds = SELECT s 
-                        FROM seeds:s 
-                        POST-ACCUM 
-                            s.@prev_sampled += TRUE,
-                            {SEEDVERTEXATTRS},
-                            @@printed_vertices += s;
-            ELSE
-                FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
-                  _verts = SELECT s FROM start:s
-                           WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled
-                           POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
-                END;
-                FOREACH elem IN @@batch_heap DO
-                  @@seeds += elem.v;
-                END;
-                seeds = {@@seeds};
-                seeds = SELECT s 
-                        FROM start:s
-                        POST-ACCUM
-                            s.@prev_sampled += TRUE,
-                            {SEEDVERTEXATTRS},
-                            @@printed_vertices += s;
+      SumAccum<STRING> @@v_batch;
+      SetAccum<VERTEX> @@printed_vertices;
+      SetAccum<VERTEX> @@seeds;
+      # Get batch seeds
+      IF input_vertices.size()==0 THEN
+        start = {seed_types};
+        HeapAccum<ID_Tuple> (1, tmp_id ASC) @@batch_heap;
+        @@batch_heap.resize(batch_s);
+        IF filter_by IS NOT NULL THEN
+            FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
+              _verts = SELECT s FROM start:s
+                      WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled AND s.getAttr(filter_by, "BOOL")
+                      POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
             END;
+            FOREACH elem IN @@batch_heap DO
+              @@seeds += elem.v;
+            END;
+            seeds = {@@seeds};
+            seeds = SELECT s 
+                    FROM seeds:s 
+                    POST-ACCUM 
+                        s.@prev_sampled += TRUE,
+                        @@printed_vertices += s;
         ELSE
-            start = input_vertices;
+            FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
+              _verts = SELECT s FROM start:s
+                        WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled
+                        POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
+            END;
+            FOREACH elem IN @@batch_heap DO
+              @@seeds += elem.v;
+            END;
+            seeds = {@@seeds};
             seeds = SELECT s 
-                    FROM start:s 
+                    FROM seeds:s
                     POST-ACCUM
-                        {SEEDVERTEXATTRS},
+                        s.@prev_sampled += TRUE,
                         @@printed_vertices += s;
         END;
-        # Get neighbors of seeeds
-        FOREACH i IN RANGE[1, num_hops] DO
-            seeds = SELECT t
-                    FROM seeds:s -(e_types:e)- v_types:t 
-                    SAMPLE num_neighbors EDGE WHEN s.outdegree() >= 1
-                    ACCUM
-                        IF NOT @@printed_edges.contains(e) THEN
-                            {EDGEATTRS},
-                            @@printed_edges += e
-                        END;
-            attr = SELECT s
-                FROM seeds:s 
-                POST-ACCUM 
-                    IF NOT @@printed_vertices.contains(s) THEN
-                        {OTHERVERTEXATTRS},
-                        @@printed_vertices += s
-                    END;
-        END;
+      ELSE
+        start = input_vertices;
+        seeds = SELECT s 
+                FROM start:s
+                ACCUM @@printed_vertices += s;
+      END;
+      # Get relational context
+      
+      IF max_rel_context > 0 THEN
+        seeds = SELECT s FROM seeds:s -(e_types:e)- v_types:t 
+                SAMPLE max_rel_context EDGE WHEN s.outdegree() >= max_rel_context
+                ACCUM s.@rel_context_set += e.type +" ";
+      END;
+    
+      res = SELECT s FROM seeds:s 
+            POST-ACCUM
+              FOREACH tup IN s.@token_heap DO
+                s.@ancs += stringify(tup.v_id)+":"+stringify(tup.distance)+" ",
+                IF use_cache AND cache_empty THEN
+                  s.@conv_map += (tup.v_id -> tup.distance)
+                END
+              END,
+              IF (use_cache AND cache_empty) OR precompute THEN
+                s.{ANCHOR_CACHE_ATTRIBUTE} = s.@conv_map
+              END,
+              {VERTEXATTRS};
+      IF NOT precompute THEN # No Output if precomputing
         IF kafka_address != "" THEN
-            # Write to kafka
-            kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
-            IF kafka_errcode!=0 THEN 
-                @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
-            END;
-            kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "edge_batch_" + stringify(batch_id), @@e_batch);
-            IF kafka_errcode!=0 THEN 
-                @@kafka_error += ("Error sending edge batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
-            END;
-        ELSE
-            # Add to response
-            IF input_vertices.size()==0 THEN
-                PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch;  
-            ELSE
-                MapAccum<UINT, VERTEX> @@id_map;
-                source = @@printed_vertices;
-                res = 
-                    SELECT s 
-                    FROM source:s
-                    POST-ACCUM @@id_map += (getvid(s) -> s);
-                PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch, @@id_map AS pids; 
-            END;
+          # Write to kafka
+          kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
+          IF kafka_errcode!=0 THEN 
+            @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
+          END;
+        ELSE # HTTP mode
+          # Add to response
+          IF input_vertices.size()==0 THEN
+            PRINT @@v_batch AS vertex_batch;  
+          ELSE
+            MapAccum<UINT, VERTEX> @@id_map;
+            MapAccum<UINT, STRING> @@type_map;
+            source = @@printed_vertices;
+            res = 
+              SELECT s 
+              FROM source:s
+              POST-ACCUM @@id_map += (getvid(s) -> s), @@type_map += (getvid(s) -> s.type);
+            PRINT @@v_batch AS vertex_batch, @@id_map AS pids, @@type_map AS types; 
+          END;
         END;                          
+      END;
     END;
+    
     IF kafka_address != "" THEN
-        kafka_errcode = close_kafka_producer(producer, kafka_timeout);
+      kafka_errcode = close_kafka_producer(producer, kafka_timeout);
         IF kafka_errcode!=0 THEN 
             @@kafka_error += ("Error shutting down Kafka producer: " + stringify(kafka_errcode) + "\n");
         END;
         PRINT @@kafka_error as kafkaError;
     END;
 }
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql`

 * *Files 26% similar despite different names*

```diff
@@ -1,233 +1,255 @@
-CREATE QUERY nodepiece_loader_{QUERYSUFFIX}(
-  SET<VERTEX> input_vertices,
-  SET<STRING> v_types,
-  SET<STRING> e_types,
-  SET<STRING> seed_types,
-  BOOL compute_all = TRUE,
-  BOOL clear_cache = TRUE,
-  BOOL use_cache = TRUE,
-  BOOL precompute = FALSE,
-  STRING filter_by,
-  STRING anchor_attr,
-  INT max_distance,
-  INT max_anchors,
-  INT max_rel_context,
-  INT batch_size,
-  INT num_batches=1,
-  BOOL shuffle=FALSE,
-  STRING delimiter,
-  STRING kafka_address="",
-  STRING kafka_topic,
-  INT kafka_topic_partitions=1,
-  STRING kafka_max_size="104857600",
-  INT kafka_timeout=300000,
-  STRING security_protocol="",
-  STRING sasl_mechanism="",
-  STRING sasl_username="",
-  STRING sasl_password="",
-  STRING ssl_ca_location="",
-  STRING ssl_certificate_location="",
-  STRING ssl_key_location="",
-  STRING ssl_key_password="",
-  STRING ssl_endpoint_identification_algorithm="",
-  STRING sasl_kerberos_service_name="",
-  STRING sasl_kerberos_keytab="",
-  STRING sasl_kerberos_principal="",
-  INT num_heap_inserts=10,
-  INT num_edge_batches=10
-) SYNTAX v1{ 
-    TYPEDEF TUPLE<INT v_id, INT distance> Distance_Tuple;
-    TYPEDEF TUPLE<INT tmp_id, VERTEX v> ID_Tuple;
+CREATE QUERY edge_nei_loader_{QUERYSUFFIX}(
+    INT batch_size,
+    INT num_batches=1, 
+    INT num_neighbors=10, 
+    INT num_hops=2, 
+    BOOL shuffle=FALSE,
+    STRING filter_by,
+    SET<STRING> v_types,
+    SET<STRING> e_types,
+    SET<STRING> seed_types,
+    STRING delimiter,
+    STRING kafka_address="",
+    STRING kafka_topic,
+    INT kafka_topic_partitions=1,
+    STRING kafka_max_size="104857600",
+    INT kafka_timeout=300000,
+    STRING security_protocol="",
+    STRING sasl_mechanism="",
+    STRING sasl_username="",
+    STRING sasl_password="",
+    STRING ssl_ca_location="",
+    STRING ssl_certificate_location="",
+    STRING ssl_key_location="",
+    STRING ssl_key_password="",
+    STRING ssl_endpoint_identification_algorithm="",
+    STRING sasl_kerberos_service_name="",
+    STRING sasl_kerberos_keytab="",
+    STRING sasl_kerberos_principal=""
+) SYNTAX V1 { 
+    /*
+    This query generates the batches of edges and vertices attached to those edges.
+
+    Parameters :
+      num_batches    : Number of batches to divide all edges.
+      num_neighbors  : Number of neighbors to expand from seeds.
+      num_hops       : Number of hops to traverse to get neighbors.
+      shuffle        : Whether to shuffle vertices before collecting data.
+      filter_by      : A Boolean attribute to determine which edges are included.
+      v_types        : Vertex types to be included.
+      e_types        : Edge types to be included.
+      seed_types     : Edge types to be included as seeds.
+      kafka_address  : Address of the Kafka cluster to send data to.
+      kafka_topic    : The Kafka topic to send data to.
+      kafka_topic_partitions: Number of partitions for the given Kafka topic.
+      kafka_max_size : Maximum Kafka message size.
+      security_protocol : Security prototol for Kafka.
+      sasl_mechanism : Authentication mechanism for Kafka.
+      sasl_username  : SASL username for Kafka. 
+      sasl_password  : SASL password for Kafka. 
+      ssl_ca_location: Path to CA certificate for verifying the Kafka broker key.
+    */
+    TYPEDEF TUPLE<INT tmp_id, VERTEX src, VERTEX tgt> ID_Tuple;
     INT num_vertices;
     INT kafka_errcode;
-    INT batch_s;
     SumAccum<INT> @tmp_id;
     SumAccum<STRING> @@kafka_error;
-    SetAccum<VERTEX> @next_pass, @to_pass, @received;
-    HeapAccum<Distance_Tuple> (max_anchors, distance ASC) @token_heap;
-    SumAccum<STRING> @rel_context_set;
-    SumAccum<STRING> @ancs;
-    OrAccum @prev_sampled;
-    OrAccum @heapFull;
-
-    MapAccum<VERTEX, SumAccum<INT>> @@token_count;
-    MapAccum<INT, MinAccum<INT>> @conv_map;
-    BOOL cache_empty = FALSE;
-    INT distance;
     UINT producer;
+    MapAccum<INT, BOOL> @@edges_sampled;
+    SetAccum<VERTEX> @valid_v_out;
+    SetAccum<VERTEX> @valid_v_in;
 
     # Initialize Kafka producer
     IF kafka_address != "" THEN
         producer = init_kafka_producer(
             kafka_address, kafka_max_size, security_protocol, 
             sasl_mechanism, sasl_username, sasl_password, ssl_ca_location,
             ssl_certificate_location, ssl_key_location, ssl_key_password,
             ssl_endpoint_identification_algorithm, sasl_kerberos_service_name,
             sasl_kerberos_keytab, sasl_kerberos_principal);
     END;
 
+    # Shuffle vertex ID if needed
     start = {v_types};
-    # Perform fetch operation if desired
-    IF clear_cache THEN
-      res = SELECT s FROM start:s POST-ACCUM s.{ANCHOR_CACHE_ATTRIBUTE} = s.@conv_map;
-    END;
-    IF input_vertices.size() != 0 AND NOT compute_all THEN
-      seeds = {input_vertices};
-      res = SELECT s FROM seeds:s -(e_types)- v_types:t
-            ACCUM
-              IF s.{ANCHOR_CACHE_ATTRIBUTE}.size() != 0 THEN
-                FOREACH (key, val) IN s.{ANCHOR_CACHE_ATTRIBUTE} DO  # s.{ANCHOR_CACHE_ATTRIBUTE} should be changed to getAttr() when supported
-                  s.@token_heap += Distance_Tuple(key, val)
-                END
+    IF shuffle THEN
+        num_vertices = start.size();
+        res = SELECT s 
+              FROM start:s
+              POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
+    ELSE
+        res = SELECT s 
+              FROM start:s
+              POST-ACCUM s.@tmp_id = getvid(s);
+    END;
+
+    SumAccum<INT> @@num_edges;
+    IF filter_by IS NOT NULL THEN
+      res = SELECT s
+            FROM start:s -(seed_types:e)- v_types:t WHERE e.getAttr(filter_by, "BOOL")
+            ACCUM 
+              IF e.isDirected() THEN # we divide by two later to correct for undirected edges being counted twice, need to count directed edges twice to get correct count
+                @@num_edges += 2
               ELSE
-                FOREACH (key, val) IN t.{ANCHOR_CACHE_ATTRIBUTE} DO
-                  s.@token_heap += Distance_Tuple(key, val)
-                END
-              END
-            POST-ACCUM
-              IF s.@token_heap.size() == 0 THEN
-                cache_empty = TRUE
+                @@num_edges += 1
               END;
     ELSE
-      cache_empty = TRUE;
-    END;
-    IF cache_empty THEN  # computing all, shuffle vertices if needed
-        ancs = SELECT s 
-           FROM start:s 
-           WHERE s.getAttr(anchor_attr, "BOOL")
-           POST-ACCUM s.@token_heap += Distance_Tuple(getvid(s), 0);
-        start = {seed_types};
-        IF filter_by IS NOT NULL THEN
-            start = SELECT s FROM start:s WHERE s.getAttr(filter_by, "BOOL");
-        END;
-        IF shuffle THEN
-            num_vertices = start.size();
-            res = SELECT s 
-                FROM start:s
-                POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
-        ELSE
-            res = SELECT s 
-                FROM start:s
-                POST-ACCUM s.@tmp_id = getvid(s);
-        END;
-        FOREACH i IN RANGE [1, max_distance] DO
-          LOG(TRUE, "ANCHOR MESSAGE DISTANCE", i);
-          FOREACH j IN RANGE [0, num_edge_batches-1] DO
-            LOG(TRUE, "ANCHOR BATCH", j);
-            ancs = SELECT t
-                 FROM ancs:s -(e_types:e)-v_types:t WHERE t.@heapFull == False AND ((s.@tmp_id+t.@tmp_id)*(s.@tmp_id+t.@tmp_id+1)/2+t.@tmp_id)%num_edge_batches == j
-                 ACCUM 
-                  FOREACH tup IN s.@token_heap DO 
-                    t.@token_heap += Distance_Tuple(tup.v_id, i)
-                  END
-                POST-ACCUM
-                  IF s.@token_heap.size() == max_anchors THEN
-                    s.@heapFull += TRUE
-                  END;
-          END;
-        END;
+      res = SELECT s 
+            FROM start:s -(seed_types:e)- v_types:t 
+            ACCUM
+              IF e.isDirected() THEN # we divide by two later to correct for undirected edges being counted twice, need to count directed edges twice to get correct count
+                @@num_edges += 2
+              ELSE
+                @@num_edges += 1
+              END;
     END;
+    INT batch_s;     
     IF batch_size IS NULL THEN
-      batch_s = ceil(res.size()/num_batches);
+      batch_s = ceil((@@num_edges/2)/num_batches);
     ELSE  
       batch_s = batch_size;
     END;
+
+    # Generate batches
     FOREACH batch_id IN RANGE[0, num_batches-1] DO
-      SumAccum<STRING> @@v_batch;
-      SetAccum<VERTEX> @@printed_vertices;
-      SetAccum<VERTEX> @@seeds;
-      # Get batch seeds
-      IF input_vertices.size()==0 THEN
-        start = {seed_types};
+        SetAccum<VERTEX> @@vertices;
+        SumAccum<STRING> @@e_batch;
+        SumAccum<STRING> @@v_batch;
+        SetAccum<EDGE> @@printed_edges;
+        SetAccum<VERTEX> @@seeds;
+        SetAccum<VERTEX> @@targets;
         HeapAccum<ID_Tuple> (1, tmp_id ASC) @@batch_heap;
         @@batch_heap.resize(batch_s);
+        
+        start = {v_types};
         IF filter_by IS NOT NULL THEN
-            FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
-              _verts = SELECT s FROM start:s
-                      WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled AND s.getAttr(filter_by, "BOOL")
-                      POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
-            END;
+            res = 
+                SELECT s
+                FROM start:s -(seed_types:e)- v_types:t
+                WHERE e.getAttr(filter_by, "BOOL") 
+                      AND ((t.@tmp_id >= s.@tmp_id AND NOT @@edges_sampled.containsKey((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id)) OR
+                            (t.@tmp_id < s.@tmp_id AND NOT @@edges_sampled.containsKey((s.@tmp_id*s.@tmp_id)+t.@tmp_id)))
+                ACCUM 
+                    IF t.@tmp_id >= s.@tmp_id THEN
+                        @@batch_heap += ID_Tuple(((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id), s, t)
+                    ELSE
+                        @@batch_heap += ID_Tuple(((s.@tmp_id*s.@tmp_id)+t.@tmp_id), s, t)
+                    END;
+            
             FOREACH elem IN @@batch_heap DO
-              @@seeds += elem.v;
+              SetAccum<VERTEX> @@src;
+              @@seeds += elem.src;
+              @@targets += elem.tgt;
+              @@src += elem.src;
+              src = {@@src};
+              res = SELECT s FROM src:s -(seed_types:e)- v_types:t
+                    WHERE t == elem.tgt
+                    ACCUM
+                      s.@valid_v_out += elem.tgt,
+                      t.@valid_v_in += elem.src;
             END;
-            seeds = {@@seeds};
-            seeds = SELECT s 
-                    FROM seeds:s 
-                    POST-ACCUM 
-                        s.@prev_sampled += TRUE,
-                        @@printed_vertices += s;
+            start = {@@seeds};
+            res =
+                SELECT s 
+                FROM start:s -(seed_types:e)- v_types:t 
+                WHERE t in @@targets AND s IN t.@valid_v_in AND t IN s.@valid_v_out
+                ACCUM 
+                    {SEEDEDGEATTRS},
+                    @@printed_edges += e,
+                    @@vertices += s,
+                    @@vertices += t,
+                    IF t.@tmp_id >= s.@tmp_id THEN
+                      @@edges_sampled += (((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id) -> TRUE)
+                    ELSE
+                      @@edges_sampled += (((s.@tmp_id*s.@tmp_id)+t.@tmp_id) -> TRUE)
+                    END;
         ELSE
-            FOREACH iter IN RANGE[0,num_heap_inserts-1] DO 
-              _verts = SELECT s FROM start:s
-                        WHERE s.@tmp_id % num_heap_inserts == iter AND NOT s.@prev_sampled
-                        POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
-            END;
+            res = 
+                SELECT s
+                FROM start:s -(seed_types:e)- v_types:t
+                WHERE ((t.@tmp_id >= s.@tmp_id AND NOT @@edges_sampled.containsKey((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id)) OR
+                        (t.@tmp_id < s.@tmp_id AND NOT @@edges_sampled.containsKey((s.@tmp_id*s.@tmp_id)+t.@tmp_id)))
+                ACCUM 
+                    IF t.@tmp_id >= s.@tmp_id THEN
+                        @@batch_heap += ID_Tuple(((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id), s, t)
+                    ELSE
+                        @@batch_heap += ID_Tuple(((s.@tmp_id*s.@tmp_id)+t.@tmp_id), s, t)
+                    END;
+            
             FOREACH elem IN @@batch_heap DO
-              @@seeds += elem.v;
+              SetAccum<VERTEX> @@src;
+              @@seeds += elem.src;
+              @@targets += elem.tgt;
+              @@src += elem.src;
+              src = {@@src};
+              res = SELECT s FROM src:s -(seed_types:e)- v_types:t
+                    WHERE t == elem.tgt
+                    ACCUM
+                      s.@valid_v_out += elem.tgt,
+                      t.@valid_v_in += elem.src;
             END;
-            seeds = {@@seeds};
-            seeds = SELECT s 
-                    FROM seeds:s
-                    POST-ACCUM
-                        s.@prev_sampled += TRUE,
-                        @@printed_vertices += s;
+            start = {@@seeds};
+            res =
+                SELECT s 
+                FROM start:s -(seed_types:e)- v_types:t 
+                WHERE t in @@targets AND s IN t.@valid_v_in AND t IN s.@valid_v_out
+                ACCUM 
+                    {SEEDEDGEATTRS},
+                    @@printed_edges += e,
+                    @@vertices += s,
+                    @@vertices += t,
+                    IF t.@tmp_id >= s.@tmp_id THEN
+                      @@edges_sampled += (((t.@tmp_id*t.@tmp_id)+s.@tmp_id+t.@tmp_id) -> TRUE)
+                    ELSE
+                      @@edges_sampled += (((s.@tmp_id*s.@tmp_id)+t.@tmp_id) -> TRUE)
+                    END;
         END;
-      ELSE
-        start = input_vertices;
-        seeds = SELECT s 
-                FROM start:s
-                ACCUM @@printed_vertices += s;
-      END;
-      # Get relational context
-      
-      IF max_rel_context > 0 THEN
-        seeds = SELECT s FROM seeds:s -(e_types:e)- v_types:t 
-                SAMPLE max_rel_context EDGE WHEN s.outdegree() >= max_rel_context
-                ACCUM s.@rel_context_set += e.type +" ";
-      END;
     
-      res = SELECT s FROM seeds:s 
+        # Get seed vertices
+        v_in_batch = @@vertices;
+        seeds = 
+            SELECT s 
+            FROM v_in_batch:s 
             POST-ACCUM
-              FOREACH tup IN s.@token_heap DO
-                s.@ancs += stringify(tup.v_id)+":"+stringify(tup.distance)+" ",
-                IF use_cache AND cache_empty THEN
-                  s.@conv_map += (tup.v_id -> tup.distance)
-                END
-              END,
-              IF (use_cache AND cache_empty) OR precompute THEN
-                s.{ANCHOR_CACHE_ATTRIBUTE} = s.@conv_map
-              END,
-              {VERTEXATTRS};
-      IF NOT precompute THEN # No Output if precomputing
+                {VERTEXATTRS};
+        # Get neighbors of seeeds
+        FOREACH i IN RANGE[1, num_hops] DO
+            seeds = SELECT t
+                    FROM seeds:s -(e_types:e)- v_types:t 
+                    SAMPLE num_neighbors EDGE WHEN s.outdegree() >= 1
+                    ACCUM
+                        IF NOT @@printed_edges.contains(e) THEN
+                            {OTHEREDGEATTRS},
+                            @@printed_edges += e
+                        END;
+            attr = 
+                SELECT s
+                FROM seeds:s 
+                POST-ACCUM 
+                    IF NOT @@vertices.contains(s) THEN
+                        {VERTEXATTRS},
+                        @@vertices += s
+                    END;
+        END;        
         IF kafka_address != "" THEN
-          # Write to kafka
-          kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
-          IF kafka_errcode!=0 THEN 
-            @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
-          END;
-        ELSE # HTTP mode
-          # Add to response
-          IF input_vertices.size()==0 THEN
-            PRINT @@v_batch AS vertex_batch;  
-          ELSE
-            MapAccum<UINT, VERTEX> @@id_map;
-            MapAccum<UINT, STRING> @@type_map;
-            source = @@printed_vertices;
-            res = 
-              SELECT s 
-              FROM source:s
-              POST-ACCUM @@id_map += (getvid(s) -> s), @@type_map += (getvid(s) -> s.type);
-            PRINT @@v_batch AS vertex_batch, @@id_map AS pids, @@type_map AS types; 
-          END;
-        END;                          
-      END;
+            # Write to kafka
+            kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "vertex_batch_" + stringify(batch_id), @@v_batch);
+            IF kafka_errcode!=0 THEN 
+                @@kafka_error += ("Error sending vertex batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
+            END;
+            kafka_errcode = write_to_kafka(producer, kafka_topic, batch_id%kafka_topic_partitions, "edge_batch_" + stringify(batch_id), @@e_batch);
+            IF kafka_errcode!=0 THEN 
+                @@kafka_error += ("Error sending edge batch " + stringify(batch_id) + ": "+ stringify(kafka_errcode) + "\n");
+            END;
+        ELSE
+            # Add to response
+            PRINT @@v_batch AS vertex_batch, @@e_batch AS edge_batch;   
+        END;
     END;
-    
     IF kafka_address != "" THEN
-      kafka_errcode = close_kafka_producer(producer, kafka_timeout);
+        kafka_errcode = close_kafka_producer(producer, kafka_timeout);
         IF kafka_errcode!=0 THEN 
             @@kafka_error += ("Error shutting down Kafka producer: " + stringify(kafka_errcode) + "\n");
         END;
         PRINT @@kafka_error as kafkaError;
     END;
 }
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/metrics.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/GraphSAGE.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/GraphSAGE.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/NodePieceMLP.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/NodePieceMLP.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/models/base_model.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/splitters.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/trainer.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     def update_eval_metrics(self, metrics):
         """Update the metrics of an evaluation loop.
         
         Args:
             metrics (dict):
                 Dictionary of calculated metrics.
         """
-        self.eval_metrics = metrics
+        self.eval_metrics.update(metrics)
 
     def get_eval_metrics(self):
         """Get the metrics for an evaluation loop.
         
         Returns:
             Dictionary of evaluation loop metrics results.
         """
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/transforms/nodepiece_transforms.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/nodepiece_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/transforms/pyg_transforms.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/transforms/pyg_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/gds/utilities.py` & `pyTigerGraph-1.4.1/pyTigerGraph/gds/utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraph.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraph.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphAuth.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphBase.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,8 +404,8 @@
                 The timeout value desired in milliseconds. Defaults to 16,000 ms (16 sec)
             responseSize:
                 The size of the response in bytes. Defaults to 3.2E7 bytes (32 MB).
 
         Returns:
             Nothing. Sets `responseConfigHeader` class attribute.
         """
-        self.responseConfigHeader = {"GSQL-TIMEOUT": timeout, "RESPONSE-LIMIT": responseSize}
+        self.responseConfigHeader = {"GSQL-TIMEOUT": str(timeout), "RESPONSE-LIMIT": str(responseSize)}
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphDataset.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphDataset.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphEdge.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphEdge.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphGSQL.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphLoading.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphLoading.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphPath.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphQuery.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphQuery.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphSchema.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphUDT.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphUtils.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphUtils.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/pyTigerGraphVertex.py` & `pyTigerGraph-1.4.1/pyTigerGraph/pyTigerGraphVertex.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph/visualization.py` & `pyTigerGraph-1.4.1/pyTigerGraph/visualization.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/pyTigerGraph.egg-info/PKG-INFO` & `pyTigerGraph-1.4.1/pyTigerGraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.4
+Version: 1.4.1
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.4/pyTigerGraph.egg-info/SOURCES.txt` & `pyTigerGraph-1.4.1/pyTigerGraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/setup.py` & `pyTigerGraph-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/pyTigerGraphUnitTest.py` & `pyTigerGraph-1.4.1/tests/pyTigerGraphUnitTest.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_datasets.py` & `pyTigerGraph-1.4.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_BaseLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_BaseLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_EdgeLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_EdgeLoader.py`

 * *Files 10% similar despite different names*

```diff
@@ -252,51 +252,51 @@
         self.assertEqual(num_batches, 6)
 
     def test_iterate_hetero(self):
         loader = EdgeLoader(
             graph=self.conn,
             attributes={"v0v0": ["is_train", "is_val"], "v2v0": ["is_train", "is_val"]},
             batch_size=200,
-            shuffle=False,
+            shuffle=True, # Needed to get around VID distribution issues
             filter_by=None,
             loader_id=None,
             buffer_size=4,
         )
         num_batches = 0
         for data in loader:
             # print(num_batches, data)
             self.assertEqual(len(data), 2)
             self.assertIsInstance(data["v0v0"], DataFrame)
-            self.assertIsInstance(data["v2v0"], DataFrame)
             self.assertIn("is_val", data["v0v0"])
             self.assertIn("is_train", data["v0v0"])
+            self.assertIsInstance(data["v2v0"], DataFrame)
             self.assertIn("is_val", data["v2v0"])
             self.assertIn("is_train", data["v2v0"])
             num_batches += 1
         self.assertEqual(num_batches, 9)
 
     def test_iterate_hetero_multichar_delimiter(self):
         loader = EdgeLoader(
             graph=self.conn,
             attributes={"v0v0": ["is_train", "is_val"], "v2v0": ["is_train", "is_val"]},
             batch_size=200,
-            shuffle=False,
+            shuffle=True,  # Needed to get around VID distribution issues
             filter_by=None,
             loader_id=None,
             buffer_size=4,
             delimiter="|$"
         )
         num_batches = 0
         for data in loader:
             # print(num_batches, data)
             self.assertEqual(len(data), 2)
             self.assertIsInstance(data["v0v0"], DataFrame)
-            self.assertIsInstance(data["v2v0"], DataFrame)
             self.assertIn("is_val", data["v0v0"])
             self.assertIn("is_train", data["v0v0"])
+            self.assertIsInstance(data["v2v0"], DataFrame)
             self.assertIn("is_val", data["v2v0"])
             self.assertIn("is_train", data["v2v0"])
             num_batches += 1
         self.assertEqual(num_batches, 9)
 
 
 if __name__ == "__main__":
```

### Comparing `pyTigerGraph-1.4/tests/test_gds_EdgeNeighborLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_EdgeNeighborLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_GDS.py` & `pyTigerGraph-1.4.1/tests/test_gds_GDS.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_GraphLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_GraphLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_GraphSAGE.py` & `pyTigerGraph-1.4.1/tests/test_gds_GraphSAGE.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_HGTLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_HGTLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_NeighborLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_NeighborLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_NodePiece.py` & `pyTigerGraph-1.4.1/tests/test_gds_NodePiece.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_NodePieceLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_NodePieceLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_Trainer.py` & `pyTigerGraph-1.4.1/tests/test_gds_Trainer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_VertexLoader.py` & `pyTigerGraph-1.4.1/tests/test_gds_VertexLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_featurizer.py` & `pyTigerGraph-1.4.1/tests/test_gds_featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_metrics.py` & `pyTigerGraph-1.4.1/tests/test_gds_metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_splitters.py` & `pyTigerGraph-1.4.1/tests/test_gds_splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_transforms.py` & `pyTigerGraph-1.4.1/tests/test_gds_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_gds_utilities.py` & `pyTigerGraph-1.4.1/tests/test_gds_utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphAuth.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphBase.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphBase.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphEdge.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphEdge.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphGSQL.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphPath.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphQuery.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphQuery.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphSchema.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphUDT.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphUtils.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphUtils.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.4/tests/test_pyTigerGraphVertex.py` & `pyTigerGraph-1.4.1/tests/test_pyTigerGraphVertex.py`

 * *Files identical despite different names*

