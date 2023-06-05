# Comparing `tmp/mastf-libscout-0.1.0a0.tar.gz` & `tmp/mastf-libscout-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastf-libscout-0.1.0a0.tar", last modified: Mon Jun  5 08:16:05 2023, max compression
+gzip compressed data, was "mastf-libscout-0.1.1a0.tar", last modified: Mon Jun  5 08:19:10 2023, max compression
```

## Comparing `mastf-libscout-0.1.0a0.tar` & `mastf-libscout-0.1.1a0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.662922 mastf-libscout-0.1.0a0/
--rw-rw-rw-   0        0        0    11560 2023-05-27 11:12:32.000000 mastf-libscout-0.1.0a0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.086315 mastf-libscout-0.1.0a0/LibScout/
--rw-rw-rw-   0        0        0       48 2023-05-28 09:11:37.000000 mastf-libscout-0.1.0a0/LibScout/__init__.py
--rw-rw-rw-   0        0        0    11771 2023-06-05 07:24:32.000000 mastf-libscout-0.1.0a0/LibScout/ch.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.171738 mastf-libscout-0.1.0a0/LibScout/cli/
--rw-rw-rw-   0        0        0        0 2023-05-28 10:30:52.000000 mastf-libscout-0.1.0a0/LibScout/cli/__init__.py
--rw-rw-rw-   0        0        0    10903 2023-06-05 06:19:55.000000 mastf-libscout-0.1.0a0/LibScout/cli/entry_points.py
--rw-rw-rw-   0        0        0     6883 2023-06-05 07:56:42.000000 mastf-libscout-0.1.0a0/LibScout/cli/main.py
--rw-rw-rw-   0        0        0      769 2023-06-05 07:24:07.000000 mastf-libscout-0.1.0a0/LibScout/config.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.272676 mastf-libscout-0.1.0a0/LibScout/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 09:15:19.000000 mastf-libscout-0.1.0a0/LibScout/core/__init__.py
--rw-rw-rw-   0        0        0    23009 2023-06-05 08:05:58.000000 mastf-libscout-0.1.0a0/LibScout/core/matcher.py
--rw-rw-rw-   0        0        0     3881 2023-06-05 06:19:55.000000 mastf-libscout-0.1.0a0/LibScout/core/profiler.py
--rw-rw-rw-   0        0        0     8455 2023-06-05 06:19:55.000000 mastf-libscout-0.1.0a0/LibScout/core/robot.py
--rw-rw-rw-   0        0        0     4413 2023-06-05 06:19:56.000000 mastf-libscout-0.1.0a0/LibScout/files.py
--rw-rw-rw-   0        0        0     8409 2023-06-05 07:24:59.000000 mastf-libscout-0.1.0a0/LibScout/hashtree.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.375258 mastf-libscout-0.1.0a0/LibScout/pkg/
--rw-rw-rw-   0        0        0      698 2023-05-27 19:33:25.000000 mastf-libscout-0.1.0a0/LibScout/pkg/__init__.py
--rw-rw-rw-   0        0        0    17984 2023-06-05 07:25:52.000000 mastf-libscout-0.1.0a0/LibScout/pkg/tree.py
--rw-rw-rw-   0        0        0     3269 2023-05-31 16:59:05.000000 mastf-libscout-0.1.0a0/LibScout/pkg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.537179 mastf-libscout-0.1.0a0/LibScout/profile/
--rw-rw-rw-   0        0        0      721 2023-05-28 10:42:40.000000 mastf-libscout-0.1.0a0/LibScout/profile/__init__.py
--rw-rw-rw-   0        0        0    11087 2023-06-05 07:04:01.000000 mastf-libscout-0.1.0a0/LibScout/profile/base.py
--rw-rw-rw-   0        0        0     5431 2023-06-05 06:25:07.000000 mastf-libscout-0.1.0a0/LibScout/profile/caches.py
--rw-rw-rw-   0        0        0     5627 2023-06-05 06:19:56.000000 mastf-libscout-0.1.0a0/LibScout/profile/match.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:16:05.620985 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/
--rw-rw-rw-   0        0        0      801 2023-06-05 08:16:04.000000 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-06-05 08:16:04.000000 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 08:16:04.000000 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-05 08:16:04.000000 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 08:16:04.000000 mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      801 2023-06-05 08:16:05.656920 mastf-libscout-0.1.0a0/PKG-INFO
--rw-rw-rw-   0        0        0     4592 2023-06-05 08:10:35.000000 mastf-libscout-0.1.0a0/README.md
--rw-rw-rw-   0        0        0     1173 2023-06-05 08:11:10.000000 mastf-libscout-0.1.0a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 08:16:05.663924 mastf-libscout-0.1.0a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:10.287417 mastf-libscout-0.1.1a0/
+-rw-rw-rw-   0        0        0    11560 2023-05-27 11:12:32.000000 mastf-libscout-0.1.1a0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:09.832017 mastf-libscout-0.1.1a0/LibScout/
+-rw-rw-rw-   0        0        0       48 2023-05-28 09:11:37.000000 mastf-libscout-0.1.1a0/LibScout/__init__.py
+-rw-rw-rw-   0        0        0    11771 2023-06-05 07:24:32.000000 mastf-libscout-0.1.1a0/LibScout/ch.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:09.905093 mastf-libscout-0.1.1a0/LibScout/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-28 10:30:52.000000 mastf-libscout-0.1.1a0/LibScout/cli/__init__.py
+-rw-rw-rw-   0        0        0    10903 2023-06-05 06:19:55.000000 mastf-libscout-0.1.1a0/LibScout/cli/entry_points.py
+-rw-rw-rw-   0        0        0     6883 2023-06-05 07:56:42.000000 mastf-libscout-0.1.1a0/LibScout/cli/main.py
+-rw-rw-rw-   0        0        0      769 2023-06-05 07:24:07.000000 mastf-libscout-0.1.1a0/LibScout/config.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:09.995890 mastf-libscout-0.1.1a0/LibScout/core/
+-rw-rw-rw-   0        0        0        0 2023-05-28 09:15:19.000000 mastf-libscout-0.1.1a0/LibScout/core/__init__.py
+-rw-rw-rw-   0        0        0    23009 2023-06-05 08:05:58.000000 mastf-libscout-0.1.1a0/LibScout/core/matcher.py
+-rw-rw-rw-   0        0        0     3881 2023-06-05 06:19:55.000000 mastf-libscout-0.1.1a0/LibScout/core/profiler.py
+-rw-rw-rw-   0        0        0     8455 2023-06-05 06:19:55.000000 mastf-libscout-0.1.1a0/LibScout/core/robot.py
+-rw-rw-rw-   0        0        0     4413 2023-06-05 06:19:56.000000 mastf-libscout-0.1.1a0/LibScout/files.py
+-rw-rw-rw-   0        0        0     8409 2023-06-05 07:24:59.000000 mastf-libscout-0.1.1a0/LibScout/hashtree.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:10.076710 mastf-libscout-0.1.1a0/LibScout/pkg/
+-rw-rw-rw-   0        0        0      698 2023-05-27 19:33:25.000000 mastf-libscout-0.1.1a0/LibScout/pkg/__init__.py
+-rw-rw-rw-   0        0        0    17984 2023-06-05 07:25:52.000000 mastf-libscout-0.1.1a0/LibScout/pkg/tree.py
+-rw-rw-rw-   0        0        0     3269 2023-05-31 16:59:05.000000 mastf-libscout-0.1.1a0/LibScout/pkg/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:10.176183 mastf-libscout-0.1.1a0/LibScout/profile/
+-rw-rw-rw-   0        0        0      721 2023-05-28 10:42:40.000000 mastf-libscout-0.1.1a0/LibScout/profile/__init__.py
+-rw-rw-rw-   0        0        0    11087 2023-06-05 07:04:01.000000 mastf-libscout-0.1.1a0/LibScout/profile/base.py
+-rw-rw-rw-   0        0        0     5431 2023-06-05 06:25:07.000000 mastf-libscout-0.1.1a0/LibScout/profile/caches.py
+-rw-rw-rw-   0        0        0     5627 2023-06-05 06:19:56.000000 mastf-libscout-0.1.1a0/LibScout/profile/match.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:19:10.250580 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/
+-rw-rw-rw-   0        0        0     5436 2023-06-05 08:19:09.000000 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2023-06-05 08:19:09.000000 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:19:09.000000 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-05 08:19:09.000000 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 08:19:09.000000 mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5436 2023-06-05 08:19:10.282418 mastf-libscout-0.1.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     4592 2023-06-05 08:10:35.000000 mastf-libscout-0.1.1a0/README.md
+-rw-rw-rw-   0        0        0     1195 2023-06-05 08:18:46.000000 mastf-libscout-0.1.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:19:10.288776 mastf-libscout-0.1.1a0/setup.cfg
```

### Comparing `mastf-libscout-0.1.0a0/LICENSE` & `mastf-libscout-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/ch.py` & `mastf-libscout-0.1.1a0/LibScout/ch.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/cli/entry_points.py` & `mastf-libscout-0.1.1a0/LibScout/cli/entry_points.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/cli/main.py` & `mastf-libscout-0.1.1a0/LibScout/cli/main.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/config.py` & `mastf-libscout-0.1.1a0/LibScout/config.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/core/matcher.py` & `mastf-libscout-0.1.1a0/LibScout/core/matcher.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/core/profiler.py` & `mastf-libscout-0.1.1a0/LibScout/core/profiler.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/core/robot.py` & `mastf-libscout-0.1.1a0/LibScout/core/robot.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/files.py` & `mastf-libscout-0.1.1a0/LibScout/files.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/hashtree.py` & `mastf-libscout-0.1.1a0/LibScout/hashtree.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/pkg/__init__.py` & `mastf-libscout-0.1.1a0/LibScout/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/pkg/tree.py` & `mastf-libscout-0.1.1a0/LibScout/pkg/tree.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/pkg/utils.py` & `mastf-libscout-0.1.1a0/LibScout/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/profile/__init__.py` & `mastf-libscout-0.1.1a0/LibScout/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/profile/base.py` & `mastf-libscout-0.1.1a0/LibScout/profile/base.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/profile/caches.py` & `mastf-libscout-0.1.1a0/LibScout/profile/caches.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/LibScout/profile/match.py` & `mastf-libscout-0.1.1a0/LibScout/profile/match.py`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/MASTF_LibScout.egg-info/SOURCES.txt` & `mastf-libscout-0.1.1a0/MASTF_LibScout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/README.md` & `mastf-libscout-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `mastf-libscout-0.1.0a0/pyproject.toml` & `mastf-libscout-0.1.1a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "mastf-libscout"
-version = "0.1.0-alpha"
+version = "0.1.1-alpha"
 description="Modified fork of LibScout for integration into MAST-F"
+readme = "README.md"
 authors = [
   { name="MatrixEditor", email="not@supported.com" },
 ]
 classifiers = [
      # How mature is this project? Common values are
       #   3 - Alpha
       #   4 - Beta
```

