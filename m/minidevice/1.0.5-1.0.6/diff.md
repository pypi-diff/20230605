# Comparing `tmp/minidevice-1.0.5.tar.gz` & `tmp/minidevice-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.5.tar", last modified: Sat Jun  3 06:33:32 2023, max compression
+gzip compressed data, was "minidevice-1.0.6.tar", last modified: Mon Jun  5 08:23:41 2023, max compression
```

## Comparing `minidevice-1.0.5.tar` & `minidevice-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.636500 minidevice-1.0.5/
--rw-rw-rw-   0        0        0     1373 2023-06-03 06:33:32.633518 minidevice-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.579619 minidevice-1.0.5/minidevice/
--rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.5/minidevice/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-06-02 05:28:24.000000 minidevice-1.0.5/minidevice/adb.py
-drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.614520 minidevice-1.0.5/minidevice/bin/
--rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/AdbWinApi.dll
--rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/AdbWinUsbApi.dll
--rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/adb.exe
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.5/minidevice/config.py
--rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.5/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.5/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.5/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.5/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.603057 minidevice-1.0.5/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1373 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 06:33:32.636995 minidevice-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-06-03 06:32:42.000000 minidevice-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.168431 minidevice-1.0.6/
+-rw-rw-rw-   0        0        0     1394 2023-06-05 08:23:41.166478 minidevice-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.017789 minidevice-1.0.6/minidevice/
+-rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.6/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-06-02 05:28:24.000000 minidevice-1.0.6/minidevice/adb.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.157651 minidevice-1.0.6/minidevice/bin/
+-rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/AdbWinApi.dll
+-rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/AdbWinUsbApi.dll
+-rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/adb.exe
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.6/minidevice/config.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 08:21:57.000000 minidevice-1.0.6/minidevice/device.py
+-rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.6/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.6/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.6/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.049750 minidevice-1.0.6/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1394 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 08:23:41.168431 minidevice-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-06-05 08:22:12.000000 minidevice-1.0.6/setup.py
```

### Comparing `minidevice-1.0.5/PKG-INFO` & `minidevice-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.5
+Version: 1.0.6
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # minidevice 
 
 ## CaptureScreen类
 初始化时会判断minicap在该设备是否可用 不可用时则抛出异常
@@ -47,7 +48,8 @@
     - `adb.exe`
     - `__init__.py`
     - `adb.py`
     - `AdbWinApi.dll`
     - `AdbWinUsbApi.dll`
     - `utils.py`
 项目结构
+
```

### Comparing `minidevice-1.0.5/README.md` & `minidevice-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice/adb.py` & `minidevice-1.0.6/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice/bin/AdbWinApi.dll` & `minidevice-1.0.6/minidevice/bin/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice/bin/AdbWinUsbApi.dll` & `minidevice-1.0.6/minidevice/bin/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice/bin/adb.exe` & `minidevice-1.0.6/minidevice/bin/adb.exe`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice/device.py` & `minidevice-1.0.6/minidevice/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self.sdk = get_sdk(device)
         self.vmszie = get_vmsize(device)
         if not minicap_available(device, self.vmszie):
             try:
                 minicap_install(device, self.sdk, self.abi)
             except:
                 print("minicap isn't available")
+                raise Exception
 
     def adb_screen(self):
         return raw2opencv(adb_screen(self.device))
 
     def minicap_screen(self):
         return raw2opencv(minicap_screen(self.device, self.sdk, self.vmszie))
```

### Comparing `minidevice-1.0.5/minidevice/minicap.py` & `minidevice-1.0.6/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.5/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.6/minidevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.5
+Version: 1.0.6
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
+Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # minidevice 
 
 ## CaptureScreen类
 初始化时会判断minicap在该设备是否可用 不可用时则抛出异常
@@ -47,7 +48,8 @@
     - `adb.exe`
     - `__init__.py`
     - `adb.py`
     - `AdbWinApi.dll`
     - `AdbWinUsbApi.dll`
     - `utils.py`
 项目结构
+
```

### Comparing `minidevice-1.0.5/setup.py` & `minidevice-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.5',
+      version='1.0.6',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
```

