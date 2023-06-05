# Comparing `tmp/chappie-rl-0.0.1.tar.gz` & `tmp/chappie_rl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chappie-rl-0.0.1.tar", last modified: Mon Jun  5 02:06:50 2023, max compression
+gzip compressed data, was "chappie_rl-0.0.2.tar", last modified: Mon Jun  5 02:46:13 2023, max compression
```

## Comparing `chappie-rl-0.0.1.tar` & `chappie_rl-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:06:50.722105 chappie-rl-0.0.1/
--rw-r--r--   0 benbellerose   (501) staff       (20)     1070 2021-12-02 23:49:25.000000 chappie-rl-0.0.1/LICENSE
--rw-r--r--   0 benbellerose   (501) staff       (20)      664 2023-06-05 02:06:50.721975 chappie-rl-0.0.1/PKG-INFO
--rw-r--r--   0 benbellerose   (501) staff       (20)     1029 2022-11-05 20:42:47.000000 chappie-rl-0.0.1/README.md
-drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:06:50.721812 chappie-rl-0.0.1/chappie_rl.egg-info/
--rw-r--r--   0 benbellerose   (501) staff       (20)      664 2023-06-05 02:06:50.000000 chappie-rl-0.0.1/chappie_rl.egg-info/PKG-INFO
--rw-r--r--   0 benbellerose   (501) staff       (20)      195 2023-06-05 02:06:50.000000 chappie-rl-0.0.1/chappie_rl.egg-info/SOURCES.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:06:50.000000 chappie-rl-0.0.1/chappie_rl.egg-info/dependency_links.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)       31 2023-06-05 02:06:50.000000 chappie-rl-0.0.1/chappie_rl.egg-info/requires.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:06:50.000000 chappie-rl-0.0.1/chappie_rl.egg-info/top_level.txt
--rw-r--r--   0 benbellerose   (501) staff       (20)       38 2023-06-05 02:06:50.722149 chappie-rl-0.0.1/setup.cfg
--rw-r--r--   0 benbellerose   (501) staff       (20)      895 2023-06-05 02:03:12.000000 chappie-rl-0.0.1/setup.py
+drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:46:13.978285 chappie_rl-0.0.2/
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 02:46:13.978173 chappie_rl-0.0.2/PKG-INFO
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1029 2022-11-05 20:42:47.000000 chappie_rl-0.0.2/README.md
+drwxr-xr-x   0 benbellerose   (501) staff       (20)        0 2023-06-05 02:46:13.978025 chappie_rl-0.0.2/chappie_rl.egg-info/
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1568 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/PKG-INFO
+-rw-r--r--   0 benbellerose   (501) staff       (20)      187 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)       31 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/requires.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)        1 2023-06-05 02:46:13.000000 chappie_rl-0.0.2/chappie_rl.egg-info/top_level.txt
+-rw-r--r--   0 benbellerose   (501) staff       (20)       38 2023-06-05 02:46:13.978331 chappie_rl-0.0.2/setup.cfg
+-rw-r--r--   0 benbellerose   (501) staff       (20)     1016 2023-06-05 02:46:03.000000 chappie_rl-0.0.2/setup.py
```

### Comparing `chappie-rl-0.0.1/README.md` & `chappie_rl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chappie-rl-0.0.1/setup.py` & `chappie_rl-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="chappie-rl",
-    version="0.0.1",
+    name="chappie_rl",
+    version="0.0.2",
     author="Ben Bellerose",
     author_email="benbellerose@gmail.com",
     description="Machine learning agent",
-    long_description="The Chappie agent is built to be a generalized reinforcement learning AI. This AI is trained using a combination of reinforcement learning and evolutionary learning.",
+    long_description=open('README.md').read(),  # Read the README file
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         "torch",
         "pandas",
         "numpy",
         "tdqm",
         "einops"
@@ -23,9 +24,14 @@
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ]
+    ],
+    url="https://github.com/bellerb/chappie.ai",
+    bugtrack_url="https://github.com/bellerb/chappie.ai/issues",
+    license="MIT",
+    platforms=["Any"],
+    license_file="LICENSE.txt",
 )
```

