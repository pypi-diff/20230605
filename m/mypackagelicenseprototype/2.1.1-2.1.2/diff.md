# Comparing `tmp/mypackagelicenseprototype-2.1.1.tar.gz` & `tmp/mypackagelicenseprototype-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-2.1.1.tar", last modified: Mon Jun  5 15:33:59 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-2.1.2.tar", last modified: Mon Jun  5 15:39:23 2023, max compression
```

## Comparing `mypackagelicenseprototype-2.1.1.tar` & `mypackagelicenseprototype-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:59.001543 mypackagelicenseprototype-2.1.1/
--rw-rw-rw-   0        0        0       58 2023-06-05 15:29:39.000000 mypackagelicenseprototype-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0       72 2023-06-05 15:33:59.001543 mypackagelicenseprototype-2.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.921442 mypackagelicenseprototype-2.1.1/dist3/
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.985594 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/
--rw-rw-rw-   0        0        0       72 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.993496 mypackagelicenseprototype-2.1.1/dist3/parent/
--rw-rw-rw-   0        0        0     2646 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.1/dist3/parent/PackageContent.py
--rw-rw-rw-   0        0        0     1399 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.1/dist3/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.997540 mypackagelicenseprototype-2.1.1/dist3/parent/pyarmor_runtime_000000/
--rw-rw-rw-   0        0        0      103 2023-06-05 15:29:07.000000 mypackagelicenseprototype-2.1.1/dist3/parent/pyarmor_runtime_000000/__init__.py
--rw-rw-rw-   0        0        0      103 2023-06-05 13:06:06.000000 mypackagelicenseprototype-2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      229 2023-06-05 15:33:59.009750 mypackagelicenseprototype-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:23.527158 mypackagelicenseprototype-2.1.2/
+-rw-rw-rw-   0        0        0       59 2023-06-05 15:38:28.000000 mypackagelicenseprototype-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       72 2023-06-05 15:39:23.527158 mypackagelicenseprototype-2.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:23.430699 mypackagelicenseprototype-2.1.2/dist3/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:23.470814 mypackagelicenseprototype-2.1.2/dist3/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0       72 2023-06-05 15:39:23.000000 mypackagelicenseprototype-2.1.2/dist3/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-05 15:39:23.000000 mypackagelicenseprototype-2.1.2/dist3/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:39:23.000000 mypackagelicenseprototype-2.1.2/dist3/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 15:39:23.000000 mypackagelicenseprototype-2.1.2/dist3/mypackagelicenseprototype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:23.478745 mypackagelicenseprototype-2.1.2/dist3/parent/
+-rw-rw-rw-   0        0        0     2646 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.2/dist3/parent/PackageContent.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.2/dist3/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:39:23.525129 mypackagelicenseprototype-2.1.2/dist3/parent/pyarmor_runtime_000000/
+-rw-rw-rw-   0        0        0      103 2023-06-05 15:29:07.000000 mypackagelicenseprototype-2.1.2/dist3/parent/pyarmor_runtime_000000/__init__.py
+-rw-rw-rw-   0        0        0   616960 2023-06-05 15:29:07.000000 mypackagelicenseprototype-2.1.2/dist3/parent/pyarmor_runtime_000000/pyarmor_runtime.pyd
+-rw-rw-rw-   0        0        0      103 2023-06-05 13:06:06.000000 mypackagelicenseprototype-2.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      229 2023-06-05 15:39:23.527158 mypackagelicenseprototype-2.1.2/setup.cfg
```

### Comparing `mypackagelicenseprototype-2.1.1/dist3/parent/PackageContent.py` & `mypackagelicenseprototype-2.1.2/dist3/parent/PackageContent.py`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-2.1.1/dist3/parent/__init__.py` & `mypackagelicenseprototype-2.1.2/dist3/parent/__init__.py`

 * *Files identical despite different names*

