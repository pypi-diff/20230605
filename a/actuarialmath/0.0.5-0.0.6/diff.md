# Comparing `tmp/actuarialmath-0.0.5.tar.gz` & `tmp/actuarialmath-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actuarialmath-0.0.5.tar", last modified: Sun Jun  4 15:40:09 2023, max compression
+gzip compressed data, was "actuarialmath-0.0.6.tar", last modified: Mon Jun  5 17:57:36 2023, max compression
```

## Comparing `actuarialmath-0.0.5.tar` & `actuarialmath-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,13 @@
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-04 15:40:09.437494 actuarialmath-0.0.5/
--rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.5/LICENSE
--rw-rw-r--   0 terence   (1000) terence   (1000)      960 2023-06-04 15:40:09.437494 actuarialmath-0.0.5/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)      458 2023-06-04 15:37:18.000000 actuarialmath-0.0.5/README.md
--rw-rw-r--   0 terence   (1000) terence   (1000)      574 2023-06-04 15:39:39.000000 actuarialmath-0.0.5/pyproject.toml
--rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-04 15:40:09.437494 actuarialmath-0.0.5/setup.cfg
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-04 15:40:09.433494 actuarialmath-0.0.5/src/
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-04 15:40:09.437494 actuarialmath-0.0.5/src/actuarialmath/
--rw-rw-r--   0 terence   (1000) terence   (1000)        0 2023-05-25 13:19:02.000000 actuarialmath-0.0.5/src/actuarialmath/__init__.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     4958 2023-06-04 12:06:44.000000 actuarialmath-0.0.5/src/actuarialmath/actuarial.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    15123 2023-06-04 13:28:04.000000 actuarialmath-0.0.5/src/actuarialmath/annuity.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9333 2023-06-04 14:59:30.000000 actuarialmath-0.0.5/src/actuarialmath/constantforce.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     3638 2023-06-04 15:05:12.000000 actuarialmath-0.0.5/src/actuarialmath/extrarisk.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9482 2023-06-04 12:58:13.000000 actuarialmath-0.0.5/src/actuarialmath/fractional.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21112 2023-06-04 13:13:54.000000 actuarialmath-0.0.5/src/actuarialmath/insurance.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6029 2023-06-04 12:21:48.000000 actuarialmath-0.0.5/src/actuarialmath/interest.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6906 2023-06-04 12:26:59.000000 actuarialmath-0.0.5/src/actuarialmath/life.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11663 2023-06-04 14:21:25.000000 actuarialmath-0.0.5/src/actuarialmath/lifetable.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     2706 2023-06-04 12:39:39.000000 actuarialmath-0.0.5/src/actuarialmath/lifetime.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12048 2023-06-04 14:53:49.000000 actuarialmath-0.0.5/src/actuarialmath/mortalitylaws.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12454 2023-06-04 15:08:44.000000 actuarialmath-0.0.5/src/actuarialmath/mthly.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21134 2023-06-04 14:09:48.000000 actuarialmath-0.0.5/src/actuarialmath/policyvalues.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8833 2023-06-04 13:33:45.000000 actuarialmath-0.0.5/src/actuarialmath/premiums.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    60668 2023-06-04 14:42:14.000000 actuarialmath-0.0.5/src/actuarialmath/recursion.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11689 2023-06-04 14:13:35.000000 actuarialmath-0.0.5/src/actuarialmath/reserves.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    19575 2023-06-04 14:36:57.000000 actuarialmath-0.0.5/src/actuarialmath/selectlife.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9499 2023-06-04 14:31:45.000000 actuarialmath-0.0.5/src/actuarialmath/sult.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8390 2023-06-04 12:50:08.000000 actuarialmath-0.0.5/src/actuarialmath/survival.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9937 2023-06-04 15:15:45.000000 actuarialmath-0.0.5/src/actuarialmath/udd.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8112 2023-06-04 15:16:53.000000 actuarialmath-0.0.5/src/actuarialmath/woolhouse.py
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-04 15:40:09.437494 actuarialmath-0.0.5/src/actuarialmath.egg-info/
--rw-rw-r--   0 terence   (1000) terence   (1000)      960 2023-06-04 15:40:09.000000 actuarialmath-0.0.5/src/actuarialmath.egg-info/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)      863 2023-06-04 15:40:09.000000 actuarialmath-0.0.5/src/actuarialmath.egg-info/SOURCES.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-04 15:40:09.000000 actuarialmath-0.0.5/src/actuarialmath.egg-info/dependency_links.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-04 15:40:09.000000 actuarialmath-0.0.5/src/actuarialmath.egg-info/top_level.txt
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 17:57:36.499751 actuarialmath-0.0.6/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.6/LICENSE
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4193 2023-06-05 17:57:36.499751 actuarialmath-0.0.6/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4674 2023-06-05 17:43:14.000000 actuarialmath-0.0.6/README.md
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 17:57:36.499751 actuarialmath-0.0.6/actuarialmath.egg-info/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4193 2023-06-05 17:57:36.000000 actuarialmath-0.0.6/actuarialmath.egg-info/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)      199 2023-06-05 17:57:36.000000 actuarialmath-0.0.6/actuarialmath.egg-info/SOURCES.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-05 17:57:36.000000 actuarialmath-0.0.6/actuarialmath.egg-info/dependency_links.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-05 17:57:36.000000 actuarialmath-0.0.6/actuarialmath.egg-info/top_level.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3695 2023-06-05 17:52:31.000000 actuarialmath-0.0.6/index.rst
+-rw-rw-r--   0 terence   (1000) terence   (1000)      573 2023-06-05 17:57:12.000000 actuarialmath-0.0.6/pyproject.toml
+-rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-05 17:57:36.499751 actuarialmath-0.0.6/setup.cfg
+-rw-rw-r--   0 terence   (1000) terence   (1000)      128 2023-06-05 16:33:30.000000 actuarialmath-0.0.6/setup.py
```

### Comparing `actuarialmath-0.0.5/LICENSE` & `actuarialmath-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.5/pyproject.toml` & `actuarialmath-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "actuarialmath"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Terence Lim"},
 ]
-description = "A package for solving actuarial math"
-readme = "README.md"
+description = "A package for life contingent risks"
+readme = "index.rst"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

