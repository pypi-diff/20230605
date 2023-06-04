# Comparing `tmp/playgroundrl_envs-0.0.2.tar.gz` & `tmp/playgroundrl_envs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl_envs-0.0.2.tar", last modified: Sun Jun  4 23:36:19 2023, max compression
+gzip compressed data, was "playgroundrl_envs-0.0.3.tar", last modified: Sun Jun  4 23:41:43 2023, max compression
```

## Comparing `playgroundrl_envs-0.0.2.tar` & `playgroundrl_envs-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.859143 playgroundrl_envs-0.0.2/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:36:19.859207 playgroundrl_envs-0.0.2/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.2/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 23:36:19.859390 playgroundrl_envs-0.0.2/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      464 2023-06-04 23:36:05.000000 playgroundrl_envs-0.0.2/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.854267 playgroundrl_envs-0.0.2/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.855316 playgroundrl_envs-0.0.2/src/playgroundrl_envs/
--rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/game_interface.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.858950 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:35:42.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/chess.py
--rw-r--r--   0 rayan      (501) staff       (20)      517 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/coup.py
--rw-r--r--   0 rayan      (501) staff       (20)     4033 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/mining_decarbonization.py
--rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/petting_zoo.py
--rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-04 23:24:02.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/poker.py
--rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/snake.py
--rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/tic_tac_toe.py
--rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/sid_util.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.856076 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      653 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/top_level.txt
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.309877 playgroundrl_envs-0.0.3/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:41:43.309970 playgroundrl_envs-0.0.3/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.3/README.md
+-rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 23:41:43.310226 playgroundrl_envs-0.0.3/setup.cfg
+-rw-r--r--   0 rayan      (501) staff       (20)      564 2023-06-04 23:40:55.000000 playgroundrl_envs-0.0.3/setup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.305104 playgroundrl_envs-0.0.3/src/
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.306224 playgroundrl_envs-0.0.3/src/playgroundrl_envs/
+-rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/game_interface.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.308458 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:35:42.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/__init__.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.308935 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/catan/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:19.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/catan/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     5442 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/catan/catan.py
+-rw-r--r--   0 rayan      (501) staff       (20)     9605 2023-05-07 04:36:31.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/catan/encoder.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/chess.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.309289 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/codenames/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:18.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/codenames/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     8023 2023-06-03 21:24:11.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/codenames/codenames.py
+-rw-r--r--   0 rayan      (501) staff       (20)      517 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/coup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.309616 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/go/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:16.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/go/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3656 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/go/go.py
+-rw-r--r--   0 rayan      (501) staff       (20)     4033 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/mining_decarbonization.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/petting_zoo.py
+-rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-04 23:24:02.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/poker.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/snake.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/tic_tac_toe.py
+-rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs/sid_util.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:41:43.306918 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:41:43.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      968 2023-06-04 23:41:43.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/SOURCES.txt
+-rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:41:43.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/dependency_links.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 23:41:43.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/requires.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-04 23:41:43.000000 playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/top_level.txt
```

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/game_interface.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/game_interface.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/chess.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/chess.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/coup.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/coup.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/mining_decarbonization.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/mining_decarbonization.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/petting_zoo.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/petting_zoo.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/poker.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/poker.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/snake.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/snake.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/tic_tac_toe.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/games/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs/sid_util.py` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs/sid_util.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/SOURCES.txt` & `playgroundrl_envs-0.0.3/src/playgroundrl_envs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,8 +11,15 @@
 src/playgroundrl_envs/games/__init__.py
 src/playgroundrl_envs/games/chess.py
 src/playgroundrl_envs/games/coup.py
 src/playgroundrl_envs/games/mining_decarbonization.py
 src/playgroundrl_envs/games/petting_zoo.py
 src/playgroundrl_envs/games/poker.py
 src/playgroundrl_envs/games/snake.py
-src/playgroundrl_envs/games/tic_tac_toe.py
+src/playgroundrl_envs/games/tic_tac_toe.py
+src/playgroundrl_envs/games/catan/__init__.py
+src/playgroundrl_envs/games/catan/catan.py
+src/playgroundrl_envs/games/catan/encoder.py
+src/playgroundrl_envs/games/codenames/__init__.py
+src/playgroundrl_envs/games/codenames/codenames.py
+src/playgroundrl_envs/games/go/__init__.py
+src/playgroundrl_envs/games/go/go.py
```

