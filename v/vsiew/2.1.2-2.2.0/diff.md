# Comparing `tmp/vsiew-2.1.2.tar.gz` & `tmp/vsiew-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.1.2.tar", last modified: Wed May 24 17:17:18 2023, max compression
+gzip compressed data, was "vsiew-2.2.0.tar", last modified: Mon Jun  5 20:46:33 2023, max compression
```

## Comparing `vsiew-2.1.2.tar` & `vsiew-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:17:18.334321 vsiew-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-24 17:16:56.000000 vsiew-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 17:17:18.330321 vsiew-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 17:16:56.000000 vsiew-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:17:18.334321 vsiew-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 17:16:56.000000 vsiew-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:17:18.330321 vsiew-2.1.2/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 17:16:56.000000 vsiew-2.1.2/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-24 17:16:56.000000 vsiew-2.1.2/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-24 17:16:56.000000 vsiew-2.1.2/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-24 17:16:56.000000 vsiew-2.1.2/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:17:18.330321 vsiew-2.1.2/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:17:18.000000 vsiew-2.1.2/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.976798 vsiew-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 20:46:08.000000 vsiew-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-05 20:46:33.976798 vsiew-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 20:46:08.000000 vsiew-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:46:33.976798 vsiew-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-05 20:46:08.000000 vsiew-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.972798 vsiew-2.2.0/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.976798 vsiew-2.2.0/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.1.2/LICENSE` & `vsiew-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.1.2/PKG-INFO` & `vsiew-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.1.2
+Version: 2.2.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.1.2/setup.py` & `vsiew-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,11 +30,11 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     entry_points={
         'console_scripts': [
-            'iew-update=vsiew:update'
+            'vsiew=vsiew:update_packages'
         ]
     },
 )
```

### Comparing `vsiew-2.1.2/vsiew/init.py` & `vsiew-2.2.0/vsiew/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # Shrimply
 
 from typing import Iterator
 
 base_org = 'Irrational-Encoding-Wizardry'
 
 
-def update(action: str) -> None:
+def update(action_: list[str] | None) -> None:
     import sys
 
+    action = 'update'
+
+    if action_:
+        if action_[-1] == 'latest':
+            action = 'update-git'
+        elif 'Scripts' not in action_[-1] or '.py' not in action_[-1]:
+            action = action_[-1].strip()
+
     def _get_install_call(package: str, do_git: bool) -> int:
         from subprocess import check_call
 
         args = list[str]()
 
         if do_git:
             package = f'git+https://github.com/{base_org}/{package}.git'
```

### Comparing `vsiew-2.1.2/vsiew.egg-info/PKG-INFO` & `vsiew-2.2.0/vsiew.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.1.2
+Version: 2.2.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

