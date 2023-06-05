# Comparing `tmp/iris_pex_embedded_python-2.3.2.tar.gz` & `tmp/iris_pex_embedded_python-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.2.tar", last modified: Fri Jun  2 07:52:45 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.3.tar", last modified: Mon Jun  5 14:57:35 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.2.tar` & `iris_pex_embedded_python-2.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.902573 iris_pex_embedded_python-2.3.2/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.2/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-02 07:52:45.901644 iris_pex_embedded_python-2.3.2/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.2/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.2/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-06-02 07:52:45.902858 iris_pex_embedded_python-2.3.2/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2295 2023-06-02 07:52:21.000000 iris_pex_embedded_python-2.3.2/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.841233 iris_pex_embedded_python-2.3.2/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.840175 iris_pex_embedded_python-2.3.2/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.850172 iris_pex_embedded_python-2.3.2/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.886553 iris_pex_embedded_python-2.3.2/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112     5471 2023-05-31 16:30:39.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     8057 2023-05-31 15:44:03.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.899649 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112      933 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       47 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/entry_points.txt
--rw-r--r--   0 grongier (902446405) 1252422112       43 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.713297 iris_pex_embedded_python-2.3.3/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.3/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49406 2023-06-05 14:57:35.712189 iris_pex_embedded_python-2.3.3/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.3/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.3/pyproject.toml
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-06-05 14:57:35.713620 iris_pex_embedded_python-2.3.3/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2295 2023-06-05 14:57:10.000000 iris_pex_embedded_python-2.3.3/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.650513 iris_pex_embedded_python-2.3.3/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.649877 iris_pex_embedded_python-2.3.3/src/grongier/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.659170 iris_pex_embedded_python-2.3.3/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.696950 iris_pex_embedded_python-2.3.3/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5320 2023-06-02 13:11:45.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.709898 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49406 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      933 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       47 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.2/LICENSE` & `iris_pex_embedded_python-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/PKG-INFO` & `iris_pex_embedded_python-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.2
+Version: 2.3.3
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.2/README.md` & `iris_pex_embedded_python-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/setup.py` & `iris_pex_embedded_python-2.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.2',
+        version='2.3.3',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,18 +48,16 @@
         # display list of productions
         dikt = _Director.list_productions()
         print(json.dumps(dikt, indent=4))
 
     elif args.start:
         if args.start == 'not_set':
             # start default production
-            _Director.start_production(_Director.get_default_production())
-        else:
-            # start a production
-            _Director.start_production(args.start)
+            args.start = _Director.get_default_production()
+        _Director.start_production_with_log(args.start)
 
     elif args.kill:
         # kill a production
         _Director.shutdown_production()
 
     elif args.restart:
         # restart a production
@@ -71,32 +69,31 @@
 
     elif args.version:
         # display version
         print(version('iris-pex-embedded-python'))
 
     elif args.log:
         # display log
-        _Director.start_log_production()
+        _Director.log_production()
 
     elif args.stop:
         # stop a production
         _Director.stop_production()
 
     elif args.status:
         dikt=_Director.status_production()
         print(json.dumps(dikt, indent=4))
 
     elif args.export:
-        dikt = {}
+
         if args.export == 'not_set':
             # export default production
-            dikt = _Utils.export_production(_Director.get_default_production())
-        else:
-            # export a production
-            dikt = _Utils.export_production(args.export)
+            args.export= _Director.get_default_production()
+
+        dikt = _Utils.export_production(args.export)
         print(json.dumps(dikt, indent=4))
 
     else:
         # display help and default production name
         print("usage: iop [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]")
         print("optional arguments:")
         print("  -h, --help            display help and default production name")
```

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_director.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import iris
 import datetime
-import time
 import intersystems_iris.dbapi._DBAPI as irisdbapi
 import signal
-import sys
+import functools
 import asyncio
+from dataclasses import dataclass
 
 class _Director():
     """ The Directorclass is used for nonpolling business services, that is, business services which are not automatically
     called by the production framework (through the inbound adapter) at the call interval.
     Instead these business services are created by a custom application by calling the Director.CreateBusinessService() method.
     """
 
@@ -53,40 +53,43 @@
         """
         iris_object = iris.cls("Grongier.PEX.Director").dispatchCreateBusinessService(target)
         return iris_object.GetClass()
     
     ### List of function to manage the production
     ### start production
     @staticmethod
-    def start_production(production_name=None): 
+    def start_production_with_log(production_name=None):
         if production_name is None or production_name == '':
             production_name = _Director.get_default_production()
         # create two async task
         loop = asyncio.get_event_loop()
-        handler = SIGINT_handler()
-        print('start production')
+        # add signal handler
+        handler = SigintHandler()
+        loop.add_signal_handler(signal.SIGINT, functools.partial(handler.signal_handler, signal.SIGINT, loop))
         loop.run_until_complete(asyncio.gather(
-            _Director.start_production_async(production_name, handler),
-            _Director.log_production(handler)
+            _Director._start_production_async(production_name, handler),
+            _Director._log_production_async(handler)
         ))
+        loop.close()
 
     @staticmethod
-    async def start_production_async(production_name=None, handler=None):
-        if production_name is None or production_name == '':
-            production_name = _Director.get_default_production()
-        signal.signal(signal.SIGINT, handler.signal_handler)
-        iris.cls('Ens.Director').StartProduction(production_name)
+    async def _start_production_async(production_name=None, handler=None):
+        _Director.start_production(production_name)
         while True:
-            if handler.SIGINT:
-                print('try to stop production')
+            if handler.sigint:
                 _Director.stop_production()
-                print('production stopped')
                 break
             await asyncio.sleep(1)
 
+    @staticmethod
+    def start_production(production_name=None):
+        if production_name is None or production_name == '':
+            production_name = _Director.get_default_production()
+        iris.cls('Ens.Director').StartProduction(production_name)
+
     ### stop production
     @staticmethod
     def stop_production():
         iris.cls('Ens.Director').StopProduction()
 
     ### restart production
     @staticmethod
@@ -129,73 +132,100 @@
         glb = iris.gref("^Ens.Configuration")
         default_production_name = glb['csp', "LastProduction"]
         if default_production_name is None or default_production_name == '':
             default_production_name = 'Not defined'
         return default_production_name
 
     @staticmethod
-    def read_log(handler):
+    def format_log(row: list) -> str:
+        # 0,  1,          2,   3,         4,         5,           6,            7,     8,    9,          10,       11
+        # ID, ConfigName, Job, MessageId, SessionId, SourceClass, SourceMethod, Stack, Text, TimeLogged, TraceCat, Type
+        # yield all except stack aand tracecat
+        # in first position, the timelogged
+        # cast the result to string
+        # convert Type to its string value
+            # Assert,Error,Warning,Info,Trace,Alert
+        typ = row[11]
+        if typ == 1:
+            typ = 'Assert'
+        elif typ == 2:
+            typ = 'Error'
+        elif typ == 3:
+            typ = 'Warning'
+        elif typ == 4:
+            typ = 'Info'
+        elif typ == 5:
+            typ = 'Trace'
+        elif typ == 6:
+            typ = 'Alert'
+        return str(row[9]) + ' ' + typ + ' ' + str(row[1]) + ' ' + str(row[2]) + ' ' + str(row[3]) + ' ' + str(row[4]) + ' ' + str(row[5]) + ' ' + str(row[6]) + ' ' + str(row[8])
+
+    @staticmethod
+    def read_top_log(cursor,top) -> list:
+        sql = """
+        SELECT top ?
+        ID, ConfigName, Job, MessageId, SessionId, SourceClass, SourceMethod, Stack, Text, TimeLogged, TraceCat, Type
+        FROM Ens_Util.Log
+        order by id desc
+        """
+        result = []
+        cursor.execute(sql, top)
+        for row in cursor:
+            result.append(_Director.format_log(row))
+        return result
+
+    @staticmethod
+    def read_log(cursor) -> list:
         sql = """
         SELECT 
         ID, ConfigName, Job, MessageId, SessionId, SourceClass, SourceMethod, Stack, Text, TimeLogged, TraceCat, Type
         FROM Ens_Util.Log
         where TimeLogged >= ?
         order by id desc
         """
-        signal.signal(signal.SIGINT, handler.signal_handler)
-        with irisdbapi.connect(embedded=True) as connection:
-            with connection.cursor() as cursor:
-                while True:
-                    cursor.execute(sql, (datetime.datetime.now() - datetime.timedelta(seconds=1),))
-                    for row in cursor:
-                        #ID, ConfigName, Job, MessageId, SessionId, SourceClass, SourceMethod, Stack, Text, TimeLogged, TraceCat, Type
-                        # 0,  1,          2,   3,         4,         5,           6,            7,     8,    9,          10,       11
-                        # yield all except stack aand tracecat
-                        # in first position, the timelogged
-                        # cast the result to string
-                        # convert Type to its string value
-                            # Assert,Error,Warning,Info,Trace,Alert
-                            # 1,    2,    3,      4,   5,    6
-                        typ = row[11]
-                        if typ == 1:
-                            typ = 'Assert'
-                        elif typ == 2:
-                            typ = 'Error'
-                        elif typ == 3:
-                            typ = 'Warning'
-                        elif typ == 4:
-                            typ = 'Info'
-                        elif typ == 5:
-                            typ = 'Trace'
-                        elif typ == 6:
-                            typ = 'Alert'
-                        yield str(row[9]) + ' ' + typ + ' ' + str(row[1]) + ' ' + str(row[2]) + ' ' + str(row[3]) + ' ' + str(row[4]) + ' ' + str(row[5]) + ' ' + str(row[6]) + ' ' + str(row[8])
-                    time.sleep(1)
-                    if handler.SIGINT:
-                        break
+        result = []
+        cursor.execute(sql, (datetime.datetime.now() - datetime.timedelta(seconds=1),))
+        for row in cursor:
+            result.append(_Director.format_log(row))
+        return result
 
     @staticmethod
-    async def log_production(handler):
+    async def _log_production_async(handler):
         """ Log production 
             if ctrl+c is pressed, the log is stopped
         """
-        for line in _Director.read_log(handler):
-            print(line)
-            sys.stdout.flush()
+        with irisdbapi.connect(embedded=True) as conn:
+            with conn.cursor() as cursor:
+                while True:
+                    for row in reversed(_Director.read_log(cursor)):
+                        print(row)
+                    if handler.sigint_log:
+                        break
+                    await asyncio.sleep(1)
 
     @staticmethod
-    def start_log_production():
+    def log_production():
         """ Log production 
             if ctrl+c is pressed, the log is stopped
         """
         loop = asyncio.get_event_loop()
-        handler = SIGINT_handler()
-        loop.run_until_complete(_Director.log_production(handler))
+        handler = SigintHandler(log_only=True)
+        loop.add_signal_handler(signal.SIGINT, functools.partial(handler.signal_handler, signal.SIGINT, loop))
+        with irisdbapi.connect(embedded=True) as conn:
+            with conn.cursor() as cursor:
+                for row in reversed(_Director.read_top_log(cursor, 10)):
+                    print(row)
+        loop.run_until_complete(_Director._log_production_async(handler))
+        loop.close()
 
             
-
-class SIGINT_handler():
-    def __init__(self):
-        self.SIGINT = False
+@dataclass
+class SigintHandler():
+    
+    sigint: bool = False
+    sigint_log: bool = False
+    log_only: bool = False
 
     def signal_handler(self, signal, frame):
-        self.SIGINT = True
+        if self.sigint or self.log_only:
+            self.sigint_log = True
+        self.sigint = True
```

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.3/src/grongier/pex/_utils.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.2
+Version: 2.3.3
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

