# Comparing `tmp/chappie_rl-0.0.2.tar.gz` & `tmp/chappie_rl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chappie_rl-0.0.2.tar", last modified: Mon Jun  5 02:46:13 2023, max compression
+gzip compressed data, was "chappie_rl-0.0.3.tar", last modified: Mon Jun  5 03:06:56 2023, max compression
```

## Comparing `chappie_rl-0.0.2.tar` & `chappie_rl-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:46:13.978285 chappie_rl-0.0.2/
--rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 02:46:13.978173 chappie_rl-0.0.2/PKG-INFO
--rw-r--r--   0 benbellerose   (501) staff       (20)     1029 2022-11-05 20:42:47.000000 chappie_rl-0.0.2/README.md
-drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:46:13.978025 chappie_rl-0.0.2/chappie_rl.egg-info/
--rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/PKG-INFO
--rw-r--r--   0 benbellerose   (501) staff       (20)      187 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/SOURCES.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/dependency_links.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)       31 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/requires.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/top_level.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)       38 2023-06-05 02:46:13.978331 chappie_rl-0.0.2/setup.cfg
--rw-r--r--   0 benbellerose   (501) staff       (20)     1016 2023-06-05 02:46:03.000000 chappie_rl-0.0.2/setup.py
+drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 03:06:56.558394 chappie_rl-0.0.3/
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 03:06:56.558277 chappie_rl-0.0.3/PKG-INFO
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1029 2022-11-05 20:42:47.000000 chappie_rl-0.0.3/README.md
+drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 03:06:56.558136 chappie_rl-0.0.3/chappie_rl.egg-info/
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 03:06:56.000000 chappie_rl-0.0.3/chappie_rl.egg-info/PKG-INFO
+-rw-r--r--   0 benbellerose   (501) staff       (20)      187 2023-06-05 03:06:56.000000 chappie_rl-0.0.3/chappie_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 03:06:56.000000 chappie_rl-0.0.3/chappie_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)       31 2023-06-05 03:06:56.000000 chappie_rl-0.0.3/chappie_rl.egg-info/requires.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 03:06:56.000000 chappie_rl-0.0.3/chappie_rl.egg-info/top_level.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)       38 2023-06-05 03:06:56.558439 chappie_rl-0.0.3/setup.cfg
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1016 2023-06-05 03:06:54.000000 chappie_rl-0.0.3/setup.py
```

### Comparing `chappie_rl-0.0.2/PKG-INFO` & `chappie_rl-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chappie_rl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine learning agent
 Home-page: https://github.com/bellerb/chappie.ai
 Author: Ben Bellerose
 Author-email: benbellerose@gmail.com
 License: MIT
 Keywords: python,Chappie,MuZero,RETRO
 Platform: Any
```

### Comparing `chappie_rl-0.0.2/README.md` & `chappie_rl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chappie_rl-0.0.2/chappie_rl.egg-info/PKG-INFO` & `chappie_rl-0.0.3/chappie_rl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chappie-rl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine learning agent
 Home-page: https://github.com/bellerb/chappie.ai
 Author: Ben Bellerose
 Author-email: benbellerose@gmail.com
 License: MIT
 Keywords: python,Chappie,MuZero,RETRO
 Platform: Any
```

### Comparing `chappie_rl-0.0.2/setup.py` & `chappie_rl-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chappie_rl",
-    version="0.0.2",
+    version="0.0.3",
     author="Ben Bellerose",
     author_email="benbellerose@gmail.com",
     description="Machine learning agent",
     long_description=open('README.md').read(),  # Read the README file
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

