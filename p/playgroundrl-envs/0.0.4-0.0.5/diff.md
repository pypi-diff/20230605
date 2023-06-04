# Comparing `tmp/playgroundrl_envs-0.0.4.tar.gz` & `tmp/playgroundrl_envs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl_envs-0.0.4.tar", last modified: Sun Jun  4 23:48:09 2023, max compression
+gzip compressed data, was "playgroundrl_envs-0.0.5.tar", last modified: Sun Jun  4 23:51:46 2023, max compression
```

## Comparing `playgroundrl_envs-0.0.4.tar` & `playgroundrl_envs-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.316194 playgroundrl_envs-0.0.4/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:48:09.316249 playgroundrl_envs-0.0.4/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.4/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 23:48:09.316408 playgroundrl_envs-0.0.4/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      610 2023-06-04 23:47:48.000000 playgroundrl_envs-0.0.4/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.311213 playgroundrl_envs-0.0.4/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.312608 playgroundrl_envs-0.0.4/src/playgroundrl_envs/
--rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/game_interface.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.314893 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:35:42.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/__init__.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.315353 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:19.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     5442 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/catan.py
--rw-r--r--   0 rayan      (501) staff       (20)     9605 2023-05-07 04:36:31.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/encoder.py
--rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/chess.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.315710 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/codenames/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:18.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/codenames/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     8023 2023-06-03 21:24:11.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/codenames/codenames.py
--rw-r--r--   0 rayan      (501) staff       (20)      517 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/coup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.316033 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/go/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:16.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/go/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     3656 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/go/go.py
--rw-r--r--   0 rayan      (501) staff       (20)     4033 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/mining_decarbonization.py
--rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/petting_zoo.py
--rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-04 23:24:02.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/poker.py
--rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/snake.py
--rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/tic_tac_toe.py
--rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs/sid_util.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:48:09.313353 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:48:09.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      968 2023-06-04 23:48:09.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:48:09.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 23:48:09.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:48:09.000000 playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/top_level.txt
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.241563 playgroundrl_envs-0.0.5/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:51:46.241643 playgroundrl_envs-0.0.5/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.5/README.md
+-rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 23:51:46.241819 playgroundrl_envs-0.0.5/setup.cfg
+-rw-r--r--   0 rayan      (501) staff       (20)      664 2023-06-04 23:51:40.000000 playgroundrl_envs-0.0.5/setup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.235897 playgroundrl_envs-0.0.5/src/
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.237276 playgroundrl_envs-0.0.5/src/playgroundrl_envs/
+-rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/game_interface.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.239447 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:35:42.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/__init__.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.239908 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:19.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     5442 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/catan.py
+-rw-r--r--   0 rayan      (501) staff       (20)     9605 2023-05-07 04:36:31.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/encoder.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/chess.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.240260 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/codenames/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:18.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/codenames/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     8023 2023-06-03 21:24:11.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/codenames/codenames.py
+-rw-r--r--   0 rayan      (501) staff       (20)      517 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/coup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.240644 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:39:16.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/__init__.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.241415 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/engine/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:50:47.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/engine/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)    14656 2023-04-08 22:28:50.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/engine/gogame.py
+-rw-r--r--   0 rayan      (501) staff       (20)      117 2023-04-08 22:28:50.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/engine/govars.py
+-rw-r--r--   0 rayan      (501) staff       (20)    10833 2023-04-08 22:28:50.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/engine/state_utils.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3656 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/go.py
+-rw-r--r--   0 rayan      (501) staff       (20)     4033 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/mining_decarbonization.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/petting_zoo.py
+-rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-04 23:24:02.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/poker.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/snake.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/tic_tac_toe.py
+-rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs/sid_util.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:51:46.238043 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:51:46.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)     1167 2023-06-04 23:51:46.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/SOURCES.txt
+-rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:51:46.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/dependency_links.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 23:51:46.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/requires.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-04 23:51:46.000000 playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/top_level.txt
```

### Comparing `playgroundrl_envs-0.0.4/setup.py` & `playgroundrl_envs-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
    name='playgroundrl_envs',
-   version='0.0.4',
+   version='0.0.5',
    author='Rayan Krishnan',
-   # packages=['playgroundrl_envs', 'playgroundrl_envs.games', 'playgroundrl_envs.games.go', 'playgroundrl_envs.games.codenames', 'playgroundrl_envs.games.catan'],
-   packages=find_packages(),
+   # TODO: figure out systematic way to do this
+   packages=['playgroundrl_envs', 'playgroundrl_envs.games', 'playgroundrl_envs.games.go', 'playgroundrl_envs.games.go.engine', 'playgroundrl_envs.games.codenames', 'playgroundrl_envs.games.catan'],
    package_dir={'':'src'},
    scripts=[],
    url='http://pypi.python.org/pypi/playgroundrl_envs/',
    description='The environments hosted on Playground RL',
    # long_description=open('README.txt').read(),
    install_requires=[
         'attrs==22.2.0',
```

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/game_interface.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/game_interface.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/catan.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/catan.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/catan/encoder.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/catan/encoder.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/chess.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/chess.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/codenames/codenames.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/codenames/codenames.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/coup.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/coup.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/go/go.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/go/go.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/mining_decarbonization.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/mining_decarbonization.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/petting_zoo.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/petting_zoo.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/poker.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/poker.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/snake.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/snake.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/games/tic_tac_toe.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/games/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs/sid_util.py` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs/sid_util.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.4/src/playgroundrl_envs.egg-info/SOURCES.txt` & `playgroundrl_envs-0.0.5/src/playgroundrl_envs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,8 +18,12 @@
 src/playgroundrl_envs/games/tic_tac_toe.py
 src/playgroundrl_envs/games/catan/__init__.py
 src/playgroundrl_envs/games/catan/catan.py
 src/playgroundrl_envs/games/catan/encoder.py
 src/playgroundrl_envs/games/codenames/__init__.py
 src/playgroundrl_envs/games/codenames/codenames.py
 src/playgroundrl_envs/games/go/__init__.py
-src/playgroundrl_envs/games/go/go.py
+src/playgroundrl_envs/games/go/go.py
+src/playgroundrl_envs/games/go/engine/__init__.py
+src/playgroundrl_envs/games/go/engine/gogame.py
+src/playgroundrl_envs/games/go/engine/govars.py
+src/playgroundrl_envs/games/go/engine/state_utils.py
```

