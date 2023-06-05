# Comparing `tmp/midas-0.6.1.tar.gz` & `tmp/midas-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-0.6.1.tar", last modified: Mon May  1 20:37:34 2023, max compression
+gzip compressed data, was "midas-0.6.2.tar", last modified: Mon Jun  5 20:56:39 2023, max compression
```

## Comparing `midas-0.6.1.tar` & `midas-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.117861 midas-0.6.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-05-01 20:37:34.117926 midas-0.6.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.116945 midas-0.6.1/midas/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-05-01 20:34:55.000000 midas-0.6.1/midas/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.1/midas/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.1/midas/faults.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1811 2023-05-01 20:34:55.000000 midas-0.6.1/midas/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.1/midas/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5738 2023-05-01 20:34:55.000000 midas-0.6.1/midas/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:37:34.117732 midas-0.6.1/midas.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3205 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      254 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-05-01 20:37:34.000000 midas-0.6.1/midas.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-05-01 20:37:34.118144 midas-0.6.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1804 2023-05-01 20:35:04.000000 midas-0.6.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.407750 midas-0.6.2/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.2/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.2/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-05 20:56:39.407813 midas-0.6.2/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.2/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.406760 midas-0.6.2/midas/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-06-02 19:43:38.000000 midas-0.6.2/midas/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.2/midas/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.2/midas/faults.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1889 2023-06-05 20:43:02.000000 midas-0.6.2/midas/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.2/midas/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     6137 2023-06-05 20:43:02.000000 midas-0.6.2/midas/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.407650 midas-0.6.2/midas.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-06-05 20:56:39.408040 midas-0.6.2/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2023-06-05 20:56:20.000000 midas-0.6.2/setup.py
```

### Comparing `midas-0.6.1/LICENSE` & `midas-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-0.6.1/PKG-INFO` & `midas-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python driver for Honeywell Midas gas detectors.
-Home-page: http://github.com/numat/midas/
+Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
+Maintainer: Alex Ruddick
+Maintainer-email: alex@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `midas-0.6.1/README.md` & `midas-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `midas-0.6.1/midas/__init__.py` & `midas-0.6.2/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.1/midas/driver.py` & `midas-0.6.2/midas/driver.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.1/midas/faults.csv` & `midas-0.6.2/midas/faults.csv`

 * *Files identical despite different names*

### Comparing `midas-0.6.1/midas/mock.py` & `midas-0.6.2/midas/mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
     async def __call__(self, *args, **kwargs):  # type: ignore
         """Convert regular mocks into into an async coroutine."""
         return super().__call__(*args, **kwargs)
 
+    def close(self) -> None:
+        """Close the connection."""
+        ...
+
 
 class GasDetector(realGasDetector):
     """Mock interface to the Midas gas detector."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Set an inital mocked state."""
         self.client = AsyncClientMock()
```

### Comparing `midas-0.6.1/midas/util.py` & `midas-0.6.2/midas/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 """Base functionality for modbus communication.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2022 NuMat Technologies
 """
 import asyncio
-from typing import Any, Literal, Union, overload
+from typing import Any, Literal, TypeVar, Union, overload
 
 try:
     from pymodbus.client import AsyncModbusTcpClient  # 3.x
     from pymodbus.pdu import ModbusResponse
     from pymodbus.register_read_message import ReadHoldingRegistersResponse
 except ImportError:  # 2.4.x - 2.5.x
     from pymodbus.client.asynchronous.async_io import (  # type: ignore
         ReconnectingAsyncioModbusTcpClient,
     )
+    ReadHoldingRegistersResponse = TypeVar('ReadHoldingRegistersResponse')  # type: ignore
+    ModbusResponse = TypeVar('ModbusResponse')  # type: ignore
+
 import pymodbus.exceptions
 
 
 class AsyncioModbusClient:
     """A generic asyncio client.
 
     This expands upon the pymodbus AsyncModbusTcpClient by
     including standard timeouts, async context manager, and queued requests.
     """
 
     def __init__(self, address: str, timeout: float = 1) -> None:
         """Set up communication parameters."""
         self.ip = address
         self.timeout = timeout
-        try:
-            self.client = AsyncModbusTcpClient(address, timeout=timeout)  # 3.0
-            self.pymodbus32plus = not hasattr(self.client, 'protocol')  # >= 3.2.0
-        except NameError:
-            self.client = ReconnectingAsyncioModbusTcpClient()  # 2.4.x - 2.5.x
+        self.pymodbus30plus = int(pymodbus.__version__[0]) == 3
+        self.pymodbus32plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 2
+        self.pymodbus33plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 3
+        if self.pymodbus30plus:
+            self.client = AsyncModbusTcpClient(address, timeout=timeout)
+        else:  # 2.x
+            self.client = ReconnectingAsyncioModbusTcpClient()
         self.lock = asyncio.Lock()
         self.connectTask = asyncio.create_task(self._connect())
 
     async def __aenter__(self) -> Any:
         """Asynchronously connect with the context manager."""
         return self
 
@@ -44,17 +49,17 @@
         """Provide exit to the context manager."""
         await self._close()
 
     async def _connect(self) -> None:
         """Start asynchronous reconnect loop."""
         async with self.lock:
             try:
-                try:
-                    await asyncio.wait_for(self.client.connect(), timeout=self.timeout)  # 3.x
-                except AttributeError:  # 2.4.x - 2.5.x
+                if self.pymodbus30plus:
+                    await asyncio.wait_for(self.client.connect(), timeout=self.timeout)
+                else:  # 2.x
                     await self.client.start(self.ip)  # type: ignore
             except Exception as e:
                 raise OSError(f"Could not connect to '{self.ip}'.") from e
 
     async def read_registers(self, address: int, count: int) -> list:
         """Read modbus registers.
 
@@ -130,11 +135,13 @@
                     future = getattr(self.client.protocol, method)  # type: ignore
                 return await future(*args, **kwargs)
             except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException) as e:
                 raise TimeoutError("Not connected to Midas.") from e
 
     async def _close(self) -> None:
         """Close the TCP connection."""
-        try:
-            await self.client.close()  # 3.x
-        except AttributeError:  # 2.4.x - 2.5.x
+        if self.pymodbus33plus:
+            self.client.close()  # 3.3.x
+        elif self.pymodbus30plus:
+            await self.client.close()  # type: ignore  # 3.0.x - 3.2.x
+        else:  # 2.4.x - 2.5.x
             self.client.stop()  # type: ignore
```

### Comparing `midas-0.6.1/midas.egg-info/PKG-INFO` & `midas-0.6.2/midas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python driver for Honeywell Midas gas detectors.
-Home-page: http://github.com/numat/midas/
+Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
+Maintainer: Alex Ruddick
+Maintainer-email: alex@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `midas-0.6.1/setup.py` & `midas-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,36 +7,37 @@
     raise ImportError("This module requires Python >=3.8.  Use 0.5.1 for Python3.7")
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="midas",
-    version="0.6.1",
+    version="0.6.2",
     description="Python driver for Honeywell Midas gas detectors.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="http://github.com/numat/midas/",
+    url="https://github.com/numat/midas/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
+    maintainer="Alex Ruddick",
+    maintainer_email="alex@numat-tech.com",
     packages=['midas'],
     package_data={'midas': ['faults.csv', 'py.typed']},
     install_requires=[
-        'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.3.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
             'mypy>=1.1.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.263',
+            'ruff==0.0.270',
         ],
     },
     entry_points={
         'console_scripts': [('midas = midas:command_line')]
     },
     license='GPLv2',
     classifiers=[
```

