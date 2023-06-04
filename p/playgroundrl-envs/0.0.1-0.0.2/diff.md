# Comparing `tmp/playgroundrl_envs-0.0.1.tar.gz` & `tmp/playgroundrl_envs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl_envs-0.0.1.tar", last modified: Sun Jun  4 00:29:22 2023, max compression
+gzip compressed data, was "playgroundrl_envs-0.0.2.tar", last modified: Sun Jun  4 23:36:19 2023, max compression
```

## Comparing `playgroundrl_envs-0.0.1.tar` & `playgroundrl_envs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 00:29:22.055399 playgroundrl_envs-0.0.1/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 00:29:22.055451 playgroundrl_envs-0.0.1/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.1/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 00:29:22.055595 playgroundrl_envs-0.0.1/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      437 2023-06-04 00:25:37.000000 playgroundrl_envs-0.0.1/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 00:29:22.053687 playgroundrl_envs-0.0.1/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 00:29:22.054569 playgroundrl_envs-0.0.1/src/playgroundrl_envs/
--rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs/game_interface.py
--rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs/sid_util.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 00:29:22.055296 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 00:29:22.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      326 2023-06-04 00:29:22.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 00:29:22.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 00:29:22.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-04 00:29:22.000000 playgroundrl_envs-0.0.1/src/playgroundrl_envs.egg-info/top_level.txt
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.859143 playgroundrl_envs-0.0.2/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:36:19.859207 playgroundrl_envs-0.0.2/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.2/README.md
+-rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-04 23:36:19.859390 playgroundrl_envs-0.0.2/setup.cfg
+-rw-r--r--   0 rayan      (501) staff       (20)      464 2023-06-04 23:36:05.000000 playgroundrl_envs-0.0.2/setup.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.854267 playgroundrl_envs-0.0.2/src/
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.855316 playgroundrl_envs-0.0.2/src/playgroundrl_envs/
+-rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/game_interface.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.858950 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/
+-rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-04 23:35:42.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/__init__.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/chess.py
+-rw-r--r--   0 rayan      (501) staff       (20)      517 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/coup.py
+-rw-r--r--   0 rayan      (501) staff       (20)     4033 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/mining_decarbonization.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/petting_zoo.py
+-rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-04 23:24:02.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/poker.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/snake.py
+-rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/games/tic_tac_toe.py
+-rw-r--r--   0 rayan      (501) staff       (20)      873 2023-05-16 00:49:24.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs/sid_util.py
+drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-04 23:36:19.856076 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/
+-rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/PKG-INFO
+-rw-r--r--   0 rayan      (501) staff       (20)      653 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/SOURCES.txt
+-rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/dependency_links.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/requires.txt
+-rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-04 23:36:19.000000 playgroundrl_envs-0.0.2/src/playgroundrl_envs.egg-info/top_level.txt
```

### Comparing `playgroundrl_envs-0.0.1/src/playgroundrl_envs/game_interface.py` & `playgroundrl_envs-0.0.2/src/playgroundrl_envs/game_interface.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.1/src/playgroundrl_envs/sid_util.py` & `playgroundrl_envs-0.0.2/src/playgroundrl_envs/sid_util.py`

 * *Files identical despite different names*

