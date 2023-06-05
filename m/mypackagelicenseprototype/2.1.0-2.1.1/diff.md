# Comparing `tmp/mypackagelicenseprototype-2.1.0.tar.gz` & `tmp/mypackagelicenseprototype-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-2.1.0.tar", last modified: Mon Jun  5 14:58:40 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-2.1.1.tar", last modified: Mon Jun  5 15:33:59 2023, max compression
```

## Comparing `mypackagelicenseprototype-2.1.0.tar` & `mypackagelicenseprototype-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:58:40.381866 mypackagelicenseprototype-2.1.0/
--rw-rw-rw-   0        0        0       51 2023-06-05 14:56:48.000000 mypackagelicenseprototype-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0       72 2023-06-05 14:58:40.381866 mypackagelicenseprototype-2.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 14:58:40.274699 mypackagelicenseprototype-2.1.0/dist/
-drwxrwxrwx   0        0        0        0 2023-06-05 14:58:40.327341 mypackagelicenseprototype-2.1.0/dist/mypackagelicenseprototype.egg-info/
--rw-rw-rw-   0        0        0       72 2023-06-05 14:58:40.000000 mypackagelicenseprototype-2.1.0/dist/mypackagelicenseprototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-05 14:58:40.000000 mypackagelicenseprototype-2.1.0/dist/mypackagelicenseprototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:58:40.000000 mypackagelicenseprototype-2.1.0/dist/mypackagelicenseprototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-05 14:58:40.000000 mypackagelicenseprototype-2.1.0/dist/mypackagelicenseprototype.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 14:58:40.330512 mypackagelicenseprototype-2.1.0/dist/parent/
--rw-rw-rw-   0        0        0     2494 2023-06-05 14:56:09.000000 mypackagelicenseprototype-2.1.0/dist/parent/PackageContent.py
--rw-rw-rw-   0        0        0     1351 2023-06-05 14:56:09.000000 mypackagelicenseprototype-2.1.0/dist/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:58:40.381866 mypackagelicenseprototype-2.1.0/dist/pyarmor_runtime_000000/
--rw-rw-rw-   0        0        0      103 2023-06-05 14:56:09.000000 mypackagelicenseprototype-2.1.0/dist/pyarmor_runtime_000000/__init__.py
--rw-rw-rw-   0        0        0   616960 2023-06-05 14:56:09.000000 mypackagelicenseprototype-2.1.0/dist/pyarmor_runtime_000000/pyarmor_runtime.pyd
--rw-rw-rw-   0        0        0      103 2023-06-05 13:06:06.000000 mypackagelicenseprototype-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      221 2023-06-05 14:58:40.381866 mypackagelicenseprototype-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 15:33:59.001543 mypackagelicenseprototype-2.1.1/
+-rw-rw-rw-   0        0        0       58 2023-06-05 15:29:39.000000 mypackagelicenseprototype-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0       72 2023-06-05 15:33:59.001543 mypackagelicenseprototype-2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.921442 mypackagelicenseprototype-2.1.1/dist3/
+drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.985594 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0       72 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 15:33:58.000000 mypackagelicenseprototype-2.1.1/dist3/mypackagelicenseprototype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.993496 mypackagelicenseprototype-2.1.1/dist3/parent/
+-rw-rw-rw-   0        0        0     2646 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.1/dist3/parent/PackageContent.py
+-rw-rw-rw-   0        0        0     1399 2023-06-05 15:29:08.000000 mypackagelicenseprototype-2.1.1/dist3/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:33:58.997540 mypackagelicenseprototype-2.1.1/dist3/parent/pyarmor_runtime_000000/
+-rw-rw-rw-   0        0        0      103 2023-06-05 15:29:07.000000 mypackagelicenseprototype-2.1.1/dist3/parent/pyarmor_runtime_000000/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-06-05 13:06:06.000000 mypackagelicenseprototype-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      229 2023-06-05 15:33:59.009750 mypackagelicenseprototype-2.1.1/setup.cfg
```

