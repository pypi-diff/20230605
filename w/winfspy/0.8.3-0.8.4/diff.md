# Comparing `tmp/winfspy-0.8.3.tar.gz` & `tmp/winfspy-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winfspy-0.8.3.tar", last modified: Fri Mar 18 18:44:12 2022, max compression
+gzip compressed data, was "winfspy-0.8.4.tar", last modified: Mon Jun  5 08:44:29 2023, max compression
```

## Comparing `winfspy-0.8.3.tar` & `winfspy-0.8.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.197634 winfspy-0.8.3/
--rw-rw-rw-   0        0        0      170 2022-03-18 18:43:12.000000 winfspy-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4621 2022-03-18 18:44:12.197634 winfspy-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     3000 2022-03-18 18:43:12.000000 winfspy-0.8.3/README.rst
--rw-rw-rw-   0        0        0       72 2022-03-18 18:43:12.000000 winfspy-0.8.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       36 2022-03-18 18:43:12.000000 winfspy-0.8.3/requirements-test.txt
--rw-rw-rw-   0        0        0       13 2022-03-18 18:43:12.000000 winfspy-0.8.3/requirements.txt
--rw-rw-rw-   0        0        0      406 2022-03-18 18:44:12.198635 winfspy-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1652 2022-03-18 18:43:12.000000 winfspy-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.162629 winfspy-0.8.3/src/
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.168630 winfspy-0.8.3/src/_cffi_src/
--rw-rw-rw-   0        0        0    16952 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/_cffi_src/build_bindings.py
--rw-rw-rw-   0        0        0    27217 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/_cffi_src/winfsp.cdef.h
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.171634 winfspy-0.8.3/src/winfspy/
--rw-rw-rw-   0        0        0     1101 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/__init__.py
--rw-rw-rw-   0        0        0       23 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/_version.py
--rw-rw-rw-   0        0        0     6807 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/file_system.py
--rw-rw-rw-   0        0        0    20450 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/memfs.py
--rw-rw-rw-   0        0        0    28069 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/operations.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.182632 winfspy-0.8.3/src/winfspy/plumbing/
--rw-rw-rw-   0        0        0     1811 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/__init__.py
--rw-rw-rw-   0        0        0     1310 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/bindings.py
--rw-rw-rw-   0        0        0      990 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/exceptions.py
--rw-rw-rw-   0        0        0     2428 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/file_attribute.py
--rw-rw-rw-   0        0        0    10383 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/file_system_interface.py
--rw-rw-rw-   0        0        0     2122 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/get_winfsp_dir.py
--rw-rw-rw-   0        0        0     2822 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/security_descriptor.py
--rw-rw-rw-   0        0        0     2786 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/service.py
--rw-rw-rw-   0        0        0    92338 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/status.py
--rw-rw-rw-   0        0        0     4421 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/plumbing/win32_filetime.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.185630 winfspy-0.8.3/src/winfspy/tests/
--rw-rw-rw-   0        0        0      267 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1754 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     1586 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/test_bindings.py
--rw-rw-rw-   0        0        0      236 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/test_security_descriptor.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.187632 winfspy-0.8.3/src/winfspy/tests/winfsp_tests/
--rw-rw-rw-   0        0        0      437 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfsp_tests/__init__.py
--rw-rw-rw-   0        0        0      243 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfsp_tests/__main__.py
--rw-rw-rw-   0        0        0      250 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfsp_tests/conftest.py
--rw-rw-rw-   0        0        0     2178 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfsp_tests/test_winfsp_tests.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.189633 winfspy-0.8.3/src/winfspy/tests/winfstest/
--rw-rw-rw-   0        0        0       74 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/__init__.py
--rw-rw-rw-   0        0        0      234 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/__main__.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.196635 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/
--rw-rw-rw-   0        0        0     1944 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/00_CreateFile_Dispositions.t
--rw-rw-rw-   0        0        0     1238 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/01_CreateFile_Attributes.t
--rw-rw-rw-   0        0        0     1167 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/02_CreateRemoveDirectory.t
--rw-rw-rw-   0        0        0     1282 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/03_FindFiles.t
--rw-rw-rw-   0        0        0     2762 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/04_MoveFile.t
--rw-rw-rw-   0        0        0     1636 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/05_CreateFile_Truncation.t
--rw-rw-rw-   0        0        0      642 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/06_FileTimes.t
--rw-rw-rw-   0        0        0      898 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/07_SetGetFileAttributes.t
--rw-rw-rw-   0        0        0     1386 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/08_CreateFile_Delete.t
--rw-rw-rw-   0        0        0     2213 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/09_CreateFile_Sharing.t
--rw-rw-rw-   0        0        0     1490 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/cases/10_GetSetSecurity.t
--rw-rw-rw-   0        0        0      147 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/conftest.py
--rw-rw-rw-   0        0        0    12585 2022-03-18 18:43:12.000000 winfspy-0.8.3/src/winfspy/tests/winfstest/test_winfs.py
-drwxrwxrwx   0        0        0        0 2022-03-18 18:44:12.175630 winfspy-0.8.3/src/winfspy.egg-info/
--rw-rw-rw-   0        0        0     4621 2022-03-18 18:44:11.000000 winfspy-0.8.3/src/winfspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1967 2022-03-18 18:44:12.000000 winfspy-0.8.3/src/winfspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-18 18:44:11.000000 winfspy-0.8.3/src/winfspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-18 18:44:11.000000 winfspy-0.8.3/src/winfspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2022-03-18 18:44:11.000000 winfspy-0.8.3/src/winfspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-03-18 18:44:11.000000 winfspy-0.8.3/src/winfspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:29.209026 winfspy-0.8.4/
+-rw-rw-rw-   0        0        0      170 2023-06-05 08:43:58.000000 winfspy-0.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4621 2023-06-05 08:44:29.209026 winfspy-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2023-06-05 08:43:58.000000 winfspy-0.8.4/README.rst
+-rw-rw-rw-   0        0        0       72 2023-06-05 08:43:58.000000 winfspy-0.8.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       36 2023-06-05 08:43:58.000000 winfspy-0.8.4/requirements-test.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 08:43:58.000000 winfspy-0.8.4/requirements.txt
+-rw-rw-rw-   0        0        0      406 2023-06-05 08:44:29.209026 winfspy-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-06-05 08:43:58.000000 winfspy-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.385181 winfspy-0.8.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.385181 winfspy-0.8.4/src/_cffi_src/
+-rw-rw-rw-   0        0        0    16952 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/_cffi_src/build_bindings.py
+-rw-rw-rw-   0        0        0    27217 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/_cffi_src/winfsp.cdef.h
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.385181 winfspy-0.8.4/src/winfspy/
+-rw-rw-rw-   0        0        0     1101 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/_version.py
+-rw-rw-rw-   0        0        0     7687 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/file_system.py
+-rw-rw-rw-   0        0        0    20553 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/memfs.py
+-rw-rw-rw-   0        0        0    28224 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/operations.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.400804 winfspy-0.8.4/src/winfspy/plumbing/
+-rw-rw-rw-   0        0        0     1811 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/__init__.py
+-rw-rw-rw-   0        0        0     1310 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/bindings.py
+-rw-rw-rw-   0        0        0      990 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/exceptions.py
+-rw-rw-rw-   0        0        0     2428 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/file_attribute.py
+-rw-rw-rw-   0        0        0    10465 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/file_system_interface.py
+-rw-rw-rw-   0        0        0     2120 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/get_winfsp_dir.py
+-rw-rw-rw-   0        0        0     2822 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/security_descriptor.py
+-rw-rw-rw-   0        0        0     2786 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/service.py
+-rw-rw-rw-   0        0        0    92338 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/status.py
+-rw-rw-rw-   0        0        0     4446 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/plumbing/win32_filetime.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.400804 winfspy-0.8.4/src/winfspy/tests/
+-rw-rw-rw-   0        0        0      267 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1793 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     1586 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/test_bindings.py
+-rw-rw-rw-   0        0        0      236 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/test_security_descriptor.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.400804 winfspy-0.8.4/src/winfspy/tests/winfsp_tests/
+-rw-rw-rw-   0        0        0      437 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfsp_tests/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfsp_tests/__main__.py
+-rw-rw-rw-   0        0        0      250 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfsp_tests/conftest.py
+-rw-rw-rw-   0        0        0     2178 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfsp_tests/test_winfsp_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.400804 winfspy-0.8.4/src/winfspy/tests/winfstest/
+-rw-rw-rw-   0        0        0       74 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:29.209026 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/
+-rw-rw-rw-   0        0        0     1944 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/00_CreateFile_Dispositions.t
+-rw-rw-rw-   0        0        0     1238 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/01_CreateFile_Attributes.t
+-rw-rw-rw-   0        0        0     1167 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/02_CreateRemoveDirectory.t
+-rw-rw-rw-   0        0        0     1282 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/03_FindFiles.t
+-rw-rw-rw-   0        0        0     2762 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/04_MoveFile.t
+-rw-rw-rw-   0        0        0     1636 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/05_CreateFile_Truncation.t
+-rw-rw-rw-   0        0        0      642 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/06_FileTimes.t
+-rw-rw-rw-   0        0        0      898 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/07_SetGetFileAttributes.t
+-rw-rw-rw-   0        0        0     1386 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/08_CreateFile_Delete.t
+-rw-rw-rw-   0        0        0     2213 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/09_CreateFile_Sharing.t
+-rw-rw-rw-   0        0        0     1490 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/cases/10_GetSetSecurity.t
+-rw-rw-rw-   0        0        0      147 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/conftest.py
+-rw-rw-rw-   0        0        0    12751 2023-06-05 08:43:58.000000 winfspy-0.8.4/src/winfspy/tests/winfstest/test_winfs.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:44:28.385181 winfspy-0.8.4/src/winfspy.egg-info/
+-rw-rw-rw-   0        0        0     4621 2023-06-05 08:44:27.000000 winfspy-0.8.4/src/winfspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1967 2023-06-05 08:44:28.000000 winfspy-0.8.4/src/winfspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:44:27.000000 winfspy-0.8.4/src/winfspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 08:44:27.000000 winfspy-0.8.4/src/winfspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2023-06-05 08:44:27.000000 winfspy-0.8.4/src/winfspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 08:44:27.000000 winfspy-0.8.4/src/winfspy.egg-info/top_level.txt
```

### Comparing `winfspy-0.8.3/PKG-INFO` & `winfspy-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winfspy
-Version: 0.8.3
+Version: 0.8.4
 Summary: CFFI bindings for WinFSP
 Home-page: https://github.com/Scille/winfspy
 Author: Emmanuel Leblond
 Author-email: emmanuel.leblond@gmail.com
 License: UNKNOWN
 Description: ===============================
         WinFSPy
```

### Comparing `winfspy-0.8.3/README.rst` & `winfspy-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/setup.py` & `winfspy-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/_cffi_src/build_bindings.py` & `winfspy-0.8.4/src/_cffi_src/build_bindings.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/_cffi_src/winfsp.cdef.h` & `winfspy-0.8.4/src/_cffi_src/winfsp.cdef.h`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/__init__.py` & `winfspy-0.8.4/src/winfspy/__init__.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/file_system.py` & `winfspy-0.8.4/src/winfspy/file_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import os
+import time
+import errno
+
 from .plumbing import ffi, lib, cook_ntstatus, nt_success, file_system_interface_trampoline_factory
 from .plumbing import WinFSPyError, FileSystemAlreadyStarted, FileSystemNotStarted
 from .operations import BaseFileSystemOperations
 
 
 def _volume_params_factory(
     sector_size=0,
@@ -146,15 +150,18 @@
         # Network drive if prefix is provided
         if self.volume_params.get("prefix"):
             device_path = lib.WFSPY_FSP_FSCTL_NET_DEVICE_NAME
         else:
             device_path = lib.WFSPY_FSP_FSCTL_DISK_DEVICE_NAME
 
         result = lib.FspFileSystemCreate(
-            device_path, self._volume_params, self._file_system_interface, self._file_system_ptr,
+            device_path,
+            self._volume_params,
+            self._file_system_interface,
+            self._file_system_ptr,
         )
         if not nt_success(result):
             raise WinFSPyError(f"Cannot create file system: {cook_ntstatus(result).name}")
 
         # Avoid GC on the handle
         self._operations_handle = ffi.new_handle(self.operations)
         self._file_system_ptr[0].UserContext = self._operations_handle
@@ -169,14 +176,29 @@
 
         result = lib.FspFileSystemSetMountPoint(self._file_system_ptr[0], self.mountpoint)
         if not nt_success(result):
             raise WinFSPyError(f"Cannot mount file system: {cook_ntstatus(result).name}")
         result = lib.FspFileSystemStartDispatcher(self._file_system_ptr[0], 0)
         if not nt_success(result):
             raise WinFSPyError(f"Cannot start file system dispatcher: {cook_ntstatus(result).name}")
+        # Since winfsp 1.12.22301 (2022-2), the file system might not be reachable as soon as the dispatcher is started.
+        # Instead a request might fail with the following error:
+        # [WinError 995] The I/O operation has been aborted because of either a thread exit or an application request
+        # In order to avoid this issue, we simply stat the mountpoint until it responds, with a maximum of 10 attempts.
+        attemps = 10
+        delay = 0.01  # seconds
+        for i in range(attemps):
+            try:
+                os.stat(self.mountpoint)
+                break
+            except OSError as e:
+                if e.errno == errno.EINVAL and e.winerror in (995, 1005):
+                    time.sleep(delay)
+                    continue
+                raise
 
     def restart(self, **volume_params):
         self.stop()
         self.volume_params.update(volume_params)
         self._apply_volume_params()
         self._create_file_system()
         self.start()
```

### Comparing `winfspy-0.8.3/src/winfspy/memfs.py` & `winfspy-0.8.4/src/winfspy/memfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,23 +191,27 @@
         self._thread_lock = threading.Lock()
 
     # Debugging helpers
 
     def _create_directory(self, path):
         path = self._root_path / path
         obj = FolderObj(
-            path, FILE_ATTRIBUTE.FILE_ATTRIBUTE_DIRECTORY, self._root_obj.security_descriptor,
+            path,
+            FILE_ATTRIBUTE.FILE_ATTRIBUTE_DIRECTORY,
+            self._root_obj.security_descriptor,
         )
         self._entries[path] = obj
 
     def _import_files(self, file_path):
         file_path = Path(file_path)
         path = self._root_path / file_path.name
         obj = FileObj(
-            path, FILE_ATTRIBUTE.FILE_ATTRIBUTE_ARCHIVE, self._root_obj.security_descriptor,
+            path,
+            FILE_ATTRIBUTE.FILE_ATTRIBUTE_ARCHIVE,
+            self._root_obj.security_descriptor,
         )
         self._entries[path] = obj
         obj.write(file_path.read_bytes(), 0, False)
 
     # Winfsp operations
 
     @operation
@@ -266,15 +270,18 @@
 
         if create_options & CREATE_FILE_CREATE_OPTIONS.FILE_DIRECTORY_FILE:
             file_obj = self._entries[file_name] = FolderObj(
                 file_name, file_attributes, security_descriptor
             )
         else:
             file_obj = self._entries[file_name] = FileObj(
-                file_name, file_attributes, security_descriptor, allocation_size,
+                file_name,
+                file_attributes,
+                security_descriptor,
+                allocation_size,
             )
 
         return OpenedObj(file_obj)
 
     @operation
     def get_security(self, file_context):
         return file_context.file_obj.security_descriptor
```

### Comparing `winfspy-0.8.3/src/winfspy/operations.py` & `winfspy-0.8.4/src/winfspy/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,24 +248,31 @@
     ) -> NTSTATUS:
         """
         Overwrite a file.
         """
         cooked_file_context = ffi.from_handle(file_context)
         try:
             self.overwrite(
-                cooked_file_context, file_attributes, replace_file_attributes, allocation_size,
+                cooked_file_context,
+                file_attributes,
+                replace_file_attributes,
+                allocation_size,
             )
 
         except NTStatusError as exc:
             return exc.value
 
         return self.ll_get_file_info(file_context, file_info)
 
     def overwrite(
-        self, file_context, file_attributes, replace_file_attributes: bool, allocation_size: int,
+        self,
+        file_context,
+        file_attributes,
+        replace_file_attributes: bool,
+        allocation_size: int,
     ) -> None:
         raise NotImplementedError()
 
     # ~~~ CLEANUP ~~~
 
     @_catch_unhandled_exceptions
     def ll_cleanup(self, file_context, file_name, flags: int) -> None:
@@ -346,15 +353,19 @@
         Write a file.
         """
         cooked_file_context = ffi.from_handle(file_context)
         cooked_buffer = ffi.buffer(buffer, length)
 
         try:
             p_bytes_transferred[0] = self.write(
-                cooked_file_context, cooked_buffer, offset, write_to_end_of_file, constrained_io,
+                cooked_file_context,
+                cooked_buffer,
+                offset,
+                write_to_end_of_file,
+                constrained_io,
             )
 
         except NTStatusError as exc:
             return exc.value
 
         return self.ll_get_file_info(file_context, file_info)
```

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/__init__.py` & `winfspy-0.8.4/src/winfspy/plumbing/__init__.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/bindings.py` & `winfspy-0.8.4/src/winfspy/plumbing/bindings.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/exceptions.py` & `winfspy-0.8.4/src/winfspy/plumbing/exceptions.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/file_attribute.py` & `winfspy-0.8.4/src/winfspy/plumbing/file_attribute.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/file_system_interface.py` & `winfspy-0.8.4/src/winfspy/plumbing/file_system_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     FileName,
     PFileAttributesOrReparsePointIndex,
     SecurityDescriptor,
     PSecurityDescriptorSize,
 ):
     user_context = ffi.from_handle(FileSystem.UserContext)
     return user_context.ll_get_security_by_name(
-        FileName, PFileAttributesOrReparsePointIndex, SecurityDescriptor, PSecurityDescriptorSize,
+        FileName,
+        PFileAttributesOrReparsePointIndex,
+        SecurityDescriptor,
+        PSecurityDescriptorSize,
     )
 
 
 @ffi.def_extern()
 def _trampolin_fs_Create(
     FileSystem,
     FileName,
@@ -56,15 +59,20 @@
 def _trampolin_fs_Open(FileSystem, FileName, CreateOptions, GrantedAccess, PFileContext, FileInfo):
     user_context = ffi.from_handle(FileSystem.UserContext)
     return user_context.ll_open(FileName, CreateOptions, GrantedAccess, PFileContext, FileInfo)
 
 
 @ffi.def_extern()
 def _trampolin_fs_Overwrite(
-    FileSystem, FileContext, FileAttributes, ReplaceFileAttributes, AllocationSize, FileInfo,
+    FileSystem,
+    FileContext,
+    FileAttributes,
+    ReplaceFileAttributes,
+    AllocationSize,
+    FileInfo,
 ):
     user_context = ffi.from_handle(FileSystem.UserContext)
     return user_context.ll_overwrite(
         FileContext, FileAttributes, ReplaceFileAttributes, AllocationSize, FileInfo
     )
 
 
@@ -184,15 +192,21 @@
     return user_context.ll_read_directory(
         FileContext, Pattern, Marker, Buffer, Length, PBytesTransferred
     )
 
 
 @ffi.def_extern()
 def _trampolin_fs_ResolveReparsePoints(
-    FileSystem, FileName, ReparsePointIndex, ResolveLastPathComponent, PIoStatus, Buffer, PSize,
+    FileSystem,
+    FileName,
+    ReparsePointIndex,
+    ResolveLastPathComponent,
+    PIoStatus,
+    Buffer,
+    PSize,
 ):
     user_context = ffi.from_handle(FileSystem.UserContext)
     return user_context.ll_resolve_reparse_points(
         FileName, ReparsePointIndex, ResolveLastPathComponent, PIoStatus, Buffer, PSize
     )
```

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/get_winfsp_dir.py` & `winfspy-0.8.4/src/winfspy/plumbing/get_winfsp_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,9 +57,9 @@
 
     return path
 
 
 def get_winfsp_library_name():
     # See:
     # https://docs.python.org/3/library/platform.html#platform.architecture
-    is_64bits = sys.maxsize > 2 ** 32
+    is_64bits = sys.maxsize > 2**32
     return "winfsp-" + ("x64" if is_64bits else "x86")
```

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/security_descriptor.py` & `winfspy-0.8.4/src/winfspy/plumbing/security_descriptor.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/service.py` & `winfspy-0.8.4/src/winfspy/plumbing/service.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/status.py` & `winfspy-0.8.4/src/winfspy/plumbing/status.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/plumbing/win32_filetime.py` & `winfspy-0.8.4/src/winfspy/plumbing/win32_filetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,18 @@
     >>> filetime_to_dt(128930364000000000)
     datetime.datetime(2009, 7, 25, 23, 0, tzinfo=datetime.timezone.utc)
 
     >>> now = filetime_now() // 10 * 10  # Only precise to the usec
     >>> assert dt_to_filetime(filetime_to_dt(now)) == now, now
     """
     milliseconds = (ft - EPOCH_AS_FILETIME) // MILLISEDCONDS_TO_HNS
-    return datetime.fromtimestamp(milliseconds / MILLISECONDS, timezone.utc,)
+    return datetime.fromtimestamp(
+        milliseconds / MILLISECONDS,
+        timezone.utc,
+    )
 
 
 def filetime_now():
     return time_ns() // 100 + EPOCH_AS_FILETIME
 
 
 if __name__ == "__main__":
```

### Comparing `winfspy-0.8.3/src/winfspy/tests/fixtures.py` & `winfspy-0.8.4/src/winfspy/tests/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
             "--file-system-path",
             action="store",
             type=str,
             default=None,
             help="A path to the file system to test",
         )
         parser.addoption(
-            "--enable-stream-tests", action="store_true", default=False, help="Enable stream tests",
+            "--enable-stream-tests",
+            action="store_true",
+            default=False,
+            help="Enable stream tests",
         )
     # Options already added (via the pluging module)
     except ValueError:
         pass
 
 
 def get_available_drive():
```

### Comparing `winfspy-0.8.3/src/winfspy/tests/test_bindings.py` & `winfspy-0.8.4/src/winfspy/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfsp_tests/test_winfsp_tests.py` & `winfspy-0.8.4/src/winfspy/tests/winfsp_tests/test_winfsp_tests.py`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/00_CreateFile_Dispositions.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/00_CreateFile_Dispositions.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/01_CreateFile_Attributes.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/01_CreateFile_Attributes.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/02_CreateRemoveDirectory.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/02_CreateRemoveDirectory.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/03_FindFiles.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/03_FindFiles.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/04_MoveFile.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/04_MoveFile.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/05_CreateFile_Truncation.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/05_CreateFile_Truncation.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/06_FileTimes.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/06_FileTimes.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/07_SetGetFileAttributes.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/07_SetGetFileAttributes.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/08_CreateFile_Delete.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/08_CreateFile_Delete.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/09_CreateFile_Sharing.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/09_CreateFile_Sharing.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/cases/10_GetSetSecurity.t` & `winfspy-0.8.4/src/winfspy/tests/winfstest/cases/10_GetSetSecurity.t`

 * *Files identical despite different names*

### Comparing `winfspy-0.8.3/src/winfspy/tests/winfstest/test_winfs.py` & `winfspy-0.8.4/src/winfspy/tests/winfstest/test_winfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,19 @@
     raise_last_error=False,
 ):
     # Create security attributes
     assert zero == 0
     security_attributes = win32security.SECURITY_ATTRIBUTES()
     security_attributes.bInheritHandle = 0
     if sddl:
-        security_attributes.SECURITY_DESCRIPTOR = win32security.ConvertStringSecurityDescriptorToSecurityDescriptor(
-            sddl, win32security.SDDL_REVISION_1,
+        security_attributes.SECURITY_DESCRIPTOR = (
+            win32security.ConvertStringSecurityDescriptorToSecurityDescriptor(
+                sddl,
+                win32security.SDDL_REVISION_1,
+            )
         )
 
     # Windows API call
     handle = win32file.CreateFile(
         path,
         desired_access,
         share_mode,
@@ -168,16 +171,19 @@
 
 
 def create_directory(path, sddl):
     # Create security attributes
     security_attributes = win32security.SECURITY_ATTRIBUTES()
     security_attributes.bInheritHandle = 0
     if sddl:
-        security_attributes.SECURITY_DESCRIPTOR = win32security.ConvertStringSecurityDescriptorToSecurityDescriptor(
-            sddl, win32security.SDDL_REVISION_1,
+        security_attributes.SECURITY_DESCRIPTOR = (
+            win32security.ConvertStringSecurityDescriptorToSecurityDescriptor(
+                sddl,
+                win32security.SDDL_REVISION_1,
+            )
         )
 
     # Windows API call
     win32file.CreateDirectory(path, security_attributes)
 
 
 def remove_directory(path):
@@ -209,15 +215,17 @@
         SYMBOLS.FILE_FLAG_OPEN_REPARSE_POINT | SYMBOLS.FILE_FLAG_BACKUP_SEMANTICS,
         0,
     )
 
     # Second windows API call
     assert handle != win32file.INVALID_HANDLE_VALUE
     win32file.SetFileInformationByHandle(
-        handle, SYMBOLS.FileEndOfFileInfo, length,
+        handle,
+        SYMBOLS.FileEndOfFileInfo,
+        length,
     )
 
     # Close the handle
     # This is necessary since we use a single process
     # for running all the commands from a single test case
     win32file.CloseHandle(handle)
 
@@ -247,15 +255,18 @@
     creation_time = prepare(creation_time)
     last_access_time = prepare(last_access_time)
     last_write_time = prepare(last_write_time)
 
     # Second windows API call
     assert handle != win32file.INVALID_HANDLE_VALUE
     win32file.SetFileTime(
-        handle, creation_time, last_access_time, last_write_time,
+        handle,
+        creation_time,
+        last_access_time,
+        last_write_time,
     )
 
     # Close the handle
     # This is necessary since we use a single process
     # for running all the commands from a single test case
     win32file.CloseHandle(handle)
 
@@ -276,15 +287,16 @@
 
     return {"Sddl": sddl}
 
 
 def set_file_security(path, info, sddl):
     # Create security descriptor
     descriptor = win32security.ConvertStringSecurityDescriptorToSecurityDescriptor(
-        sddl, win32security.SDDL_REVISION_1,
+        sddl,
+        win32security.SDDL_REVISION_1,
     )
 
     # Windows api call
     win32security.SetFileSecurity(path, info, descriptor)
 
 
 OPERATIONS = {
@@ -424,15 +436,17 @@
         def runner(fn, *args, **kwargs):
             return executor.submit(fn, *args, **kwargs).result()
 
         yield runner
 
 
 @pytest.mark.parametrize(
-    "test_module_path", TEST_MODULES, ids=[path.name for path in TEST_MODULES],
+    "test_module_path",
+    TEST_MODULES,
+    ids=[path.name for path in TEST_MODULES],
 )
 def test_winfs(test_module_path, file_system_path, process_runner):
     parser = partial(parse_argument, file_system_path)
     do_expect = partial(expect, parser, process_runner)
     do_expect_task = partial(expect_task, parser, process_runner)
     globs = {
         "uniqname": unique_name,
```

### Comparing `winfspy-0.8.3/src/winfspy.egg-info/PKG-INFO` & `winfspy-0.8.4/src/winfspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winfspy
-Version: 0.8.3
+Version: 0.8.4
 Summary: CFFI bindings for WinFSP
 Home-page: https://github.com/Scille/winfspy
 Author: Emmanuel Leblond
 Author-email: emmanuel.leblond@gmail.com
 License: UNKNOWN
 Description: ===============================
         WinFSPy
```

### Comparing `winfspy-0.8.3/src/winfspy.egg-info/SOURCES.txt` & `winfspy-0.8.4/src/winfspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

