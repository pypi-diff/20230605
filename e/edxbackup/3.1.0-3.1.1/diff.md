# Comparing `tmp/edxbackup-3.1.0.tar.gz` & `tmp/edxbackup-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxbackup-3.1.0.tar", last modified: Fri Jun  2 09:42:23 2023, max compression
+gzip compressed data, was "edxbackup-3.1.1.tar", last modified: Mon Jun  5 12:59:05 2023, max compression
```

## Comparing `edxbackup-3.1.0.tar` & `edxbackup-3.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.839717 edxbackup-3.1.0/
--rw-r--r--   0 snglth    (1000) users      (100)        8 2023-01-31 10:12:41.000000 edxbackup-3.1.0/.dockerignore
--rw-r--r--   0 snglth    (1000) users      (100)      395 2023-05-23 14:56:08.000000 edxbackup-3.1.0/.envrc
--rw-r--r--   0 snglth    (1000) users      (100)      125 2023-01-31 10:12:41.000000 edxbackup-3.1.0/.flake8
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.831717 edxbackup-3.1.0/.github/
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.835717 edxbackup-3.1.0/.github/workflows/
--rw-r--r--   0 snglth    (1000) users      (100)      809 2023-05-23 14:56:08.000000 edxbackup-3.1.0/.github/workflows/lint.yml
--rw-r--r--   0 snglth    (1000) users      (100)      100 2023-05-23 14:56:08.000000 edxbackup-3.1.0/.gitignore
--rw-r--r--   0 snglth    (1000) users      (100)      173 2023-01-31 10:12:41.000000 edxbackup-3.1.0/.isort.cfg
--rw-r--r--   0 snglth    (1000) users      (100)      598 2023-05-23 14:56:08.000000 edxbackup-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 snglth    (1000) users      (100)     1060 2023-05-23 14:56:08.000000 edxbackup-3.1.0/Dockerfile
--rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-05-23 14:56:33.000000 edxbackup-3.1.0/LICENSE
--rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-02 09:42:23.839717 edxbackup-3.1.0/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      849 2023-05-23 14:56:08.000000 edxbackup-3.1.0/README.md
--rw-r--r--   0 snglth    (1000) users      (100)      876 2023-06-02 09:40:17.000000 edxbackup-3.1.0/README.rst
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.835717 edxbackup-3.1.0/contrib/
--rw-r--r--   0 snglth    (1000) users      (100)     1443 2023-05-23 14:56:08.000000 edxbackup-3.1.0/contrib/delete_old.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.835717 edxbackup-3.1.0/edxbackup/
--rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-02 09:42:15.000000 edxbackup-3.1.0/edxbackup/__init__.py
--rw-r--r--   0 snglth    (1000) users      (100)     1679 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/backup.py
--rw-r--r--   0 snglth    (1000) users      (100)      637 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/cli.py
--rw-r--r--   0 snglth    (1000) users      (100)      278 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/config.py
--rw-r--r--   0 snglth    (1000) users      (100)     2871 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/context.py
--rw-r--r--   0 snglth    (1000) users      (100)      837 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/info.py
--rw-r--r--   0 snglth    (1000) users      (100)     1831 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/mongo.py
--rw-r--r--   0 snglth    (1000) users      (100)     1857 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/mysql.py
--rw-r--r--   0 snglth    (1000) users      (100)      447 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/options.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.837717 edxbackup-3.1.0/edxbackup/restic/
--rw-r--r--   0 snglth    (1000) users      (100)      952 2023-06-02 09:41:20.000000 edxbackup-3.1.0/edxbackup/restic/backup.py
--rw-r--r--   0 snglth    (1000) users      (100)      627 2023-06-02 09:41:20.000000 edxbackup-3.1.0/edxbackup/restic/restore.py
--rw-r--r--   0 snglth    (1000) users      (100)     1189 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/restic/snapshot.py
--rw-r--r--   0 snglth    (1000) users      (100)     2664 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/restore.py
--rw-r--r--   0 snglth    (1000) users      (100)     1744 2023-06-02 09:41:20.000000 edxbackup-3.1.0/edxbackup/s3.py
--rw-r--r--   0 snglth    (1000) users      (100)      384 2023-05-23 14:56:08.000000 edxbackup-3.1.0/edxbackup/utils.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.837717 edxbackup-3.1.0/edxbackup.egg-info/
--rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      943 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/SOURCES.txt
--rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/dependency_links.txt
--rw-r--r--   0 snglth    (1000) users      (100)       49 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/entry_points.txt
--rw-r--r--   0 snglth    (1000) users      (100)       28 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/requires.txt
--rw-r--r--   0 snglth    (1000) users      (100)       45 2023-06-02 09:42:23.000000 edxbackup-3.1.0/edxbackup.egg-info/top_level.txt
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.837717 edxbackup-3.1.0/example/
--rw-r--r--   0 snglth    (1000) users      (100)      560 2023-05-23 14:56:08.000000 edxbackup-3.1.0/example/edxbackup.json
--rw-r--r--   0 snglth    (1000) users      (100)      612 2023-06-02 09:41:24.000000 edxbackup-3.1.0/pyproject.toml
--rw-r--r--   0 snglth    (1000) users      (100)       37 2023-06-01 16:33:13.000000 edxbackup-3.1.0/pytest.ini
--rw-r--r--   0 snglth    (1000) users      (100)      538 2023-06-02 09:41:20.000000 edxbackup-3.1.0/requirements.txt
--rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-02 09:42:23.839717 edxbackup-3.1.0/setup.cfg
--rw-r--r--   0 snglth    (1000) users      (100)       98 2023-06-02 09:41:24.000000 edxbackup-3.1.0/shell.nix
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.837717 edxbackup-3.1.0/systemd/
--rw-r--r--   0 snglth    (1000) users      (100)      288 2023-05-23 14:56:08.000000 edxbackup-3.1.0/systemd/edxbackup.service
--rw-r--r--   0 snglth    (1000) users      (100)      131 2023-05-23 14:56:08.000000 edxbackup-3.1.0/systemd/edxbackup.timer
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-02 09:42:23.837717 edxbackup-3.1.0/tests/
--rw-r--r--   0 snglth    (1000) users      (100)       20 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/README.md
--rw-r--r--   0 snglth    (1000) users      (100)     1180 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/docker-compose.yml
--rw-r--r--   0 snglth    (1000) users      (100)      438 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/edxbackup.json
--rwxr-xr-x   0 snglth    (1000) users      (100)      370 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/integration.sh
--rw-r--r--   0 snglth    (1000) users      (100)     1157 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/populate.sh
--rw-r--r--   0 snglth    (1000) users      (100)      330 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/retention.py
--rw-r--r--   0 snglth    (1000) users      (100)      391 2023-05-23 14:56:08.000000 edxbackup-3.1.0/tests/testenv.sh
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/
+-rw-r--r--   0 snglth    (1000) users      (100)        8 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.dockerignore
+-rw-r--r--   0 snglth    (1000) users      (100)      395 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.envrc
+-rw-r--r--   0 snglth    (1000) users      (100)      125 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.flake8
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.986704 edxbackup-3.1.1/.github/
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.988704 edxbackup-3.1.1/.github/workflows/
+-rw-r--r--   0 snglth    (1000) users      (100)      809 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.github/workflows/lint.yml
+-rw-r--r--   0 snglth    (1000) users      (100)      100 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.gitignore
+-rw-r--r--   0 snglth    (1000) users      (100)      173 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.isort.cfg
+-rw-r--r--   0 snglth    (1000) users      (100)      598 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 snglth    (1000) users      (100)     1060 2023-05-23 14:56:08.000000 edxbackup-3.1.1/Dockerfile
+-rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-06-05 12:45:15.000000 edxbackup-3.1.1/LICENSE
+-rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-05 12:59:05.992704 edxbackup-3.1.1/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)      849 2023-05-23 14:56:08.000000 edxbackup-3.1.1/README.md
+-rw-r--r--   0 snglth    (1000) users      (100)      876 2023-06-05 12:45:15.000000 edxbackup-3.1.1/README.rst
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.988704 edxbackup-3.1.1/contrib/
+-rw-r--r--   0 snglth    (1000) users      (100)     1443 2023-05-23 14:56:08.000000 edxbackup-3.1.1/contrib/delete_old.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.990704 edxbackup-3.1.1/edxbackup/
+-rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-05 12:58:04.000000 edxbackup-3.1.1/edxbackup/__init__.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1679 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/backup.py
+-rw-r--r--   0 snglth    (1000) users      (100)      637 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/cli.py
+-rw-r--r--   0 snglth    (1000) users      (100)      278 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/config.py
+-rw-r--r--   0 snglth    (1000) users      (100)     2871 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/context.py
+-rw-r--r--   0 snglth    (1000) users      (100)      837 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/info.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1831 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/mongo.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1857 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/mysql.py
+-rw-r--r--   0 snglth    (1000) users      (100)      447 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/options.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/edxbackup/restic/
+-rw-r--r--   0 snglth    (1000) users      (100)      912 2023-06-05 12:56:46.000000 edxbackup-3.1.1/edxbackup/restic/backup.py
+-rw-r--r--   0 snglth    (1000) users      (100)      587 2023-06-05 12:56:57.000000 edxbackup-3.1.1/edxbackup/restic/restore.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1189 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/restic/snapshot.py
+-rw-r--r--   0 snglth    (1000) users      (100)     2664 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/restore.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1744 2023-06-05 12:45:15.000000 edxbackup-3.1.1/edxbackup/s3.py
+-rw-r--r--   0 snglth    (1000) users      (100)      384 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/utils.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.990704 edxbackup-3.1.1/edxbackup.egg-info/
+-rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)      943 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       49 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/entry_points.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       29 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/requires.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       45 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/top_level.txt
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/example/
+-rw-r--r--   0 snglth    (1000) users      (100)      560 2023-05-23 14:56:08.000000 edxbackup-3.1.1/example/edxbackup.json
+-rw-r--r--   0 snglth    (1000) users      (100)      606 2023-06-05 12:55:53.000000 edxbackup-3.1.1/pyproject.toml
+-rw-r--r--   0 snglth    (1000) users      (100)       37 2023-06-01 16:33:13.000000 edxbackup-3.1.1/pytest.ini
+-rw-r--r--   0 snglth    (1000) users      (100)      495 2023-06-05 12:55:58.000000 edxbackup-3.1.1/requirements.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-05 12:59:05.992704 edxbackup-3.1.1/setup.cfg
+-rw-r--r--   0 snglth    (1000) users      (100)       98 2023-06-05 12:45:27.000000 edxbackup-3.1.1/shell.nix
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/systemd/
+-rw-r--r--   0 snglth    (1000) users      (100)      288 2023-05-23 14:56:08.000000 edxbackup-3.1.1/systemd/edxbackup.service
+-rw-r--r--   0 snglth    (1000) users      (100)      131 2023-05-23 14:56:08.000000 edxbackup-3.1.1/systemd/edxbackup.timer
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/tests/
+-rw-r--r--   0 snglth    (1000) users      (100)       20 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/README.md
+-rw-r--r--   0 snglth    (1000) users      (100)     1180 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/docker-compose.yml
+-rw-r--r--   0 snglth    (1000) users      (100)      438 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/edxbackup.json
+-rwxr-xr-x   0 snglth    (1000) users      (100)      370 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/integration.sh
+-rw-r--r--   0 snglth    (1000) users      (100)     1157 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/populate.sh
+-rw-r--r--   0 snglth    (1000) users      (100)      330 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/retention.py
+-rw-r--r--   0 snglth    (1000) users      (100)      391 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/testenv.sh
```

### Comparing `edxbackup-3.1.0/.github/workflows/lint.yml` & `edxbackup-3.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/.pre-commit-config.yaml` & `edxbackup-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/Dockerfile` & `edxbackup-3.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/LICENSE` & `edxbackup-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/PKG-INFO` & `edxbackup-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edxbackup
-Version: 3.1.0
+Version: 3.1.1
 Summary: My package description
 Author-email: Illia Shestakov <i.shestakov@abstract-technology.de>
 License: Apache-2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `edxbackup-3.1.0/README.md` & `edxbackup-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/README.rst` & `edxbackup-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/contrib/delete_old.py` & `edxbackup-3.1.1/contrib/delete_old.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/backup.py` & `edxbackup-3.1.1/edxbackup/backup.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/cli.py` & `edxbackup-3.1.1/edxbackup/cli.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/context.py` & `edxbackup-3.1.1/edxbackup/context.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/info.py` & `edxbackup-3.1.1/edxbackup/info.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/mongo.py` & `edxbackup-3.1.1/edxbackup/mongo.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/mysql.py` & `edxbackup-3.1.1/edxbackup/mysql.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/restic/backup.py` & `edxbackup-3.1.1/edxbackup/restic/backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from datetime import datetime
 from subprocess import PIPE
 from subprocess import Popen
-import tarfile
-
-from minio import Minio
 
 
 def backup_stdin(
     backup_args: list[str],
     filename: str,
     hostname: str,
     tags: list[str],
```

### Comparing `edxbackup-3.1.0/edxbackup/restic/restore.py` & `edxbackup-3.1.1/edxbackup/restic/restore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from subprocess import PIPE
 from subprocess import Popen
 
-from minio import Minio
-import tarfile
-
 
 def restore_stream(restore_args: list[str], snapshot_id: str, path: str) -> bool:
     download_args = [
         "restic",
         "dump",
         snapshot_id,
         path,
```

### Comparing `edxbackup-3.1.0/edxbackup/restic/snapshot.py` & `edxbackup-3.1.1/edxbackup/restic/snapshot.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/restore.py` & `edxbackup-3.1.1/edxbackup/restore.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup/s3.py` & `edxbackup-3.1.1/edxbackup/s3.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/edxbackup.egg-info/PKG-INFO` & `edxbackup-3.1.1/edxbackup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edxbackup
-Version: 3.1.0
+Version: 3.1.1
 Summary: My package description
 Author-email: Illia Shestakov <i.shestakov@abstract-technology.de>
 License: Apache-2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `edxbackup-3.1.0/edxbackup.egg-info/SOURCES.txt` & `edxbackup-3.1.1/edxbackup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/example/edxbackup.json` & `edxbackup-3.1.1/example/edxbackup.json`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/pyproject.toml` & `edxbackup-3.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,16 @@
     {name = "Illia Shestakov", email = "i.shestakov@abstract-technology.de"},
 ]
 description = "My package description"
 requires-python = ">=3.11"
 license = {text = "Apache-2.0"}
 dependencies = [
     "click",
-    "minio",
     "pydantic",
-	"s3ball",
+	"s3ball>=0.1.1",
 ]
 dynamic = ["version", "readme"]
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools.dynamic]
```

### Comparing `edxbackup-3.1.0/tests/docker-compose.yml` & `edxbackup-3.1.1/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.0/tests/populate.sh` & `edxbackup-3.1.1/tests/populate.sh`

 * *Files identical despite different names*

