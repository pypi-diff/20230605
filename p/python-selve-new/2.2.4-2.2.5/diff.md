# Comparing `tmp/python-selve-new-2.2.4.tar.gz` & `tmp/python-selve-new-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.2.4.tar", last modified: Sun Jun  4 22:22:01 2023, max compression
+gzip compressed data, was "python-selve-new-2.2.5.tar", last modified: Sun Jun  4 22:46:50 2023, max compression
```

## Comparing `python-selve-new-2.2.4.tar` & `python-selve-new-2.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:22:01.832495 python-selve-new-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 22:22:01.832495 python-selve-new-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:22:01.828495 python-selve-new-2.2.4/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 22:22:01.000000 python-selve-new-2.2.4/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-04 22:22:01.000000 python-selve-new-2.2.4/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:22:01.000000 python-selve-new-2.2.4/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 22:22:01.000000 python-selve-new-2.2.4/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 22:22:01.000000 python-selve-new-2.2.4/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:22:01.828495 python-selve-new-2.2.4/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    66112 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:22:01.832495 python-selve-new-2.2.4/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:22:01.832495 python-selve-new-2.2.4/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:22:01.832495 python-selve-new-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-04 22:21:54.000000 python-selve-new-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:50.764261 python-selve-new-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 22:46:50.760261 python-selve-new-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:50.756261 python-selve-new-2.2.5/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 22:46:50.000000 python-selve-new-2.2.5/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-04 22:46:50.000000 python-selve-new-2.2.5/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:46:50.000000 python-selve-new-2.2.5/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 22:46:50.000000 python-selve-new-2.2.5/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 22:46:50.000000 python-selve-new-2.2.5/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:50.756261 python-selve-new-2.2.5/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    66154 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:50.760261 python-selve-new-2.2.5/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:46:50.760261 python-selve-new-2.2.5/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:46:50.764261 python-selve-new-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-04 22:46:43.000000 python-selve-new-2.2.5/setup.py
```

### Comparing `python-selve-new-2.2.4/LICENSE` & `python-selve-new-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/PKG-INFO` & `python-selve-new-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.4/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.2.5/python_selve_new.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.4/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.2.5/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/__init__.py` & `python-selve-new-2.2.5/selve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
                                     await self.processResponse(msg)
 
                                     # if msg.rstrip() == b' ':
                                     self._LOGGER.debug(f'(Selve Worker): Worker received: {msg}')
                 if self._stopThread.is_set():
                     self._LOGGER.debug("(Selve Worker): " + 'Exiting worker loop...')
                     break
+                await asyncio.sleep(0.01)
             return True
         # serial port exceptions, all of these notify that we are in some
         # serious trouble
         except serial.SerialException:
             # log message
             self._LOGGER.error("(Selve Worker): " + 'Serial Port RX error')
```

### Comparing `python-selve-new-2.2.4/selve/commands/command.py` & `python-selve-new-2.2.5/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/device.py` & `python-selve-new-2.2.5/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/event.py` & `python-selve-new-2.2.5/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/group.py` & `python-selve-new-2.2.5/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/iveo.py` & `python-selve-new-2.2.5/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/param.py` & `python-selve-new-2.2.5/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/senSim.py` & `python-selve-new-2.2.5/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/sender.py` & `python-selve-new-2.2.5/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/sensor.py` & `python-selve-new-2.2.5/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/commands/service.py` & `python-selve-new-2.2.5/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/device.py` & `python-selve-new-2.2.5/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/group.py` & `python-selve-new-2.2.5/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/iveo.py` & `python-selve-new-2.2.5/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/senSim.py` & `python-selve-new-2.2.5/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/sender.py` & `python-selve-new-2.2.5/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/sensor.py` & `python-selve-new-2.2.5/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/util/__init__.py` & `python-selve-new-2.2.5/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/util/errors.py` & `python-selve-new-2.2.5/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/selve/util/protocol.py` & `python-selve-new-2.2.5/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.4/setup.py` & `python-selve-new-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.2.4',  # Required
+    version='2.2.5',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

