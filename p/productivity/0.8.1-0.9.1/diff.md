# Comparing `tmp/productivity-0.8.1.tar.gz` & `tmp/productivity-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "productivity-0.8.1.tar", last modified: Mon Mar  6 17:21:24 2023, max compression
+gzip compressed data, was "productivity-0.9.1.tar", last modified: Mon Jun  5 21:05:14 2023, max compression
```

## Comparing `productivity-0.8.1.tar` & `productivity-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 17:21:24.765636 productivity-0.8.1/
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 17:21:24.763359 productivity-0.8.1/.github/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      153 2021-07-02 03:58:52.000000 productivity-0.8.1/.github/dependabot.yaml
--rw-r--r--   0 a.ruddick   (502) staff       (20)       65 2022-11-17 00:08:20.000000 productivity-0.8.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2021-07-02 03:58:52.000000 productivity-0.8.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2021-07-02 03:58:52.000000 productivity-0.8.1/MANIFEST.in
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3091 2023-03-06 17:21:24.765707 productivity-0.8.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2186 2022-11-17 00:08:20.000000 productivity-0.8.1/README.md
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1361 2022-11-17 00:08:20.000000 productivity-0.8.1/azure-pipelines.yml
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 17:21:24.764136 productivity-0.8.1/productivity/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1197 2022-11-17 00:08:20.000000 productivity-0.8.1/productivity/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    15466 2023-03-06 16:45:26.000000 productivity-0.8.1/productivity/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3381 2022-11-17 00:08:20.000000 productivity-0.8.1/productivity/mock.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 17:21:24.765509 productivity-0.8.1/productivity/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2021-07-02 03:58:52.000000 productivity-0.8.1/productivity/tests/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1246 2021-07-02 03:58:52.000000 productivity-0.8.1/productivity/tests/bad_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1211 2021-09-09 18:54:10.000000 productivity-0.8.1/productivity/tests/plc_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5525 2022-11-17 00:08:20.000000 productivity-0.8.1/productivity/tests/test_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     7401 2023-03-06 17:20:57.000000 productivity-0.8.1/productivity/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-06 17:21:24.764825 productivity-0.8.1/productivity.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3091 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      540 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      235 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       13 2023-03-06 17:21:24.000000 productivity-0.8.1/productivity.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      255 2023-03-06 17:21:24.765918 productivity-0.8.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1800 2023-03-06 17:20:57.000000 productivity-0.8.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.243499 productivity-0.9.1/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       80 2023-04-25 18:53:08.000000 productivity-0.9.1/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-18 00:56:18.000000 productivity-0.9.1/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2021-07-02 03:58:52.000000 productivity-0.9.1/MANIFEST.in
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3155 2023-06-05 21:05:14.243563 productivity-0.9.1/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2186 2023-04-11 05:00:34.000000 productivity-0.9.1/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.241815 productivity-0.9.1/productivity/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1197 2022-11-17 00:08:20.000000 productivity-0.9.1/productivity/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    15410 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3368 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/mock.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.243366 productivity-0.9.1/productivity/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2021-07-02 03:58:52.000000 productivity-0.9.1/productivity/tests/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1246 2021-07-02 03:58:52.000000 productivity-0.9.1/productivity/tests/bad_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1211 2021-09-09 18:54:10.000000 productivity-0.9.1/productivity/tests/plc_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5564 2023-04-18 00:56:18.000000 productivity-0.9.1/productivity/tests/test_driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     7434 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.242556 productivity-0.9.1/productivity.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3155 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      496 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      274 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       13 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      270 2023-06-05 21:05:14.243800 productivity-0.9.1/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1955 2023-06-05 21:04:21.000000 productivity-0.9.1/setup.py
```

### Comparing `productivity-0.8.1/LICENSE` & `productivity-0.9.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -333,8 +333,7 @@
   Ty Coon, President of Vice
 
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
-
```

### Comparing `productivity-0.8.1/PKG-INFO` & `productivity-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: productivity
-Version: 0.8.1
+Version: 0.9.1
 Summary: Python driver for AutomationDirect Productivity Series PLCs.
-Home-page: http://github.com/numat/productivity/
+Home-page: https://github.com/numat/productivity/
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
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `productivity-0.8.1/README.md` & `productivity-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `productivity-0.8.1/productivity/__init__.py` & `productivity-0.9.1/productivity/__init__.py`

 * *Files identical despite different names*

### Comparing `productivity-0.8.1/productivity/driver.py` & `productivity-0.9.1/productivity/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import logging
 import pydoc
 from copy import deepcopy
 from math import ceil
 from string import digits
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from pymodbus.bit_write_message import (WriteMultipleCoilsResponse,
-                                        WriteSingleCoilResponse)
+from pymodbus.bit_write_message import WriteMultipleCoilsResponse, WriteSingleCoilResponse
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder, BinaryPayloadDecoder
 from pymodbus.pdu import ExceptionResponse
 from pymodbus.register_write_message import WriteMultipleRegistersResponse
 
 from productivity.util import DATA_TYPES, TYPE_START, AsyncioModbusClient
 
@@ -93,37 +92,37 @@
         discrete_to_write, registers_to_write = await self._parse_set_args(data_dict,
                                                                            args, kwargs)
 
         responses: List[str] = []
         if discrete_to_write:
             discrete_resp = await self._write_discrete_values(discrete_to_write)
             if any(r.isError() for r in discrete_resp):
-                raise RuntimeError(f"Setting discrete values failed: {str(discrete_resp)}")
+                raise RuntimeError(f"Setting discrete values failed: {discrete_resp!s}")
             responses.extend(str(r) for r in discrete_resp)
 
         if registers_to_write:
             for key, value in registers_to_write.items():
                 register_resp = await self._write_register_value(key, value)
                 if register_resp.isError():
-                    raise RuntimeError(f"Setting {key} failed: {str(register_resp)}")
+                    raise RuntimeError(f"Setting {key} failed: {register_resp!s}")
                 responses.append(str(register_resp))
         return responses
 
     async def _parse_set_args(self, data_dict: Optional[dict],
                               args: tuple, kwargs: dict) -> Tuple[dict, dict]:
         """Parse and validate input to the set function."""
         if isinstance(data_dict, dict):
             kwargs.update(data_dict)
         if args or (data_dict and not isinstance(data_dict, dict)):
             raise TypeError(f"Invalid input. See the following docstring:\n"
                             f"{self.set.__doc__}")
         if not kwargs:
             raise TypeError(f"No settings provided. See the following docstring:\n"
                             f"{self.set.__doc__}")
-        to_write = {key: value for key, value in kwargs.items()}
+        to_write = dict(kwargs.items())
         unsupported = set(to_write) - set(self.tags)
         if unsupported:
             raise ValueError(f"The tags file is missing the following tags:"
                              f" {', '.join(unsupported)}")
         discrete_to_write, registers_to_write = {}, {}
         for key, value in to_write.items():
             start_address = self.tags[key]['address']['start']
@@ -150,25 +149,25 @@
 
         """
         start_address = self.tags[key]['address']['start'] - 400001
         builder = BinaryPayloadBuilder(byteorder=Endian.Big,
                                        wordorder=Endian.Little)
         data_type = self.tags[key]['type']
         if data_type == 'float':
-            builder.add_32bit_float(value)
+            builder.add_32bit_float(float(value))
         elif data_type == 'str' and isinstance(value, str):
             chars = self.tags[key]['length']
             if len(value) > chars:
                 raise ValueError(f'{value} is too long for {key}. '
                                  f'Max: {chars} chars')
             builder.add_string(value.ljust(chars))
         elif data_type == 'int16':
-            builder.add_16bit_int(value)
+            builder.add_16bit_int(int(value))
         elif data_type == 'int32':
-            builder.add_32bit_int(value)
+            builder.add_32bit_int(int(value))
         else:
             raise ValueError("Missing data type.")
         resp = await self.write_registers(start_address,
                                           builder.build(),
                                           skip_encode=True)
         return resp[0]
```

### Comparing `productivity-0.8.1/productivity/mock.py` & `productivity-0.9.1/productivity/mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 Distributed under the GNU General Public License v2
 Copyright (C) 2022 NuMat Technologies
 """
 
 from collections import defaultdict
 from unittest.mock import MagicMock
 
-from pymodbus.bit_read_message import (ReadCoilsResponse,
-                                       ReadDiscreteInputsResponse)
-from pymodbus.bit_write_message import (WriteMultipleCoilsResponse,
-                                        WriteSingleCoilResponse)
+from pymodbus.bit_read_message import ReadCoilsResponse, ReadDiscreteInputsResponse
+from pymodbus.bit_write_message import WriteMultipleCoilsResponse, WriteSingleCoilResponse
 from pymodbus.register_read_message import ReadHoldingRegistersResponse
-from pymodbus.register_write_message import (WriteMultipleRegistersResponse,
-                                             WriteSingleRegisterResponse)
+from pymodbus.register_write_message import WriteMultipleRegistersResponse, WriteSingleRegisterResponse
 
 from productivity.driver import ProductivityPLC as realProductivityPLC
 
 
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
@@ -37,14 +34,17 @@
         self.tags = self._load_tags(tag_filepath)
         self.addresses = self._calculate_addresses(self.tags)
         self.map = {data['address']['start']: tag for tag, data in self.tags.items()}
         self.client = AsyncClientMock()
         self._coils = defaultdict(bool)
         self._discrete_inputs = defaultdict(bool)
         self._registers = defaultdict(bytes)
+        self._detect_pymodbus_version()
+        if self.pymodbus33plus:
+            self.client.close = lambda: None
 
     async def _request(self, method, *args, **kwargs):
         if method == 'read_coils':
             address, count = args
             return ReadCoilsResponse([self._coils[address + i] for i in range(count)])
         if method == 'read_discrete_inputs':
             address, count = args
```

### Comparing `productivity-0.8.1/productivity/tests/bad_tags.csv` & `productivity-0.9.1/productivity/tests/bad_tags.csv`

 * *Files identical despite different names*

### Comparing `productivity-0.8.1/productivity/tests/plc_tags.csv` & `productivity-0.9.1/productivity/tests/plc_tags.csv`

 * *Files identical despite different names*

### Comparing `productivity-0.8.1/productivity/tests/test_driver.py` & `productivity-0.9.1/productivity/tests/test_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from productivity import command_line
 from productivity.mock import ProductivityPLC
 
 
 @pytest.fixture
 def plc_driver():
     """Confirm the driver correctly initializes with a good tags file."""
-    return ProductivityPLC('fake ip', 'tests/plc_tags.csv')
+    return ProductivityPLC('fake ip', 'productivity/tests/plc_tags.csv')
 
 
 def test_init():
     """Confirm the driver detects an improper tags file."""
     with pytest.raises(TypeError, match='unsupported data type'):
-        ProductivityPLC('fake ip', 'tests/bad_tags.csv')
+        ProductivityPLC('fake ip', 'productivity/tests/bad_tags.csv')
 
 
 @mock.patch('productivity.ProductivityPLC', ProductivityPLC)
 def test_driver_cli_tags(capsys):
     """Confirm the commandline interface works with a tags file."""
-    command_line(['fakeip', 'tests/plc_tags.csv'])
+    command_line(['fakeip', 'productivity/tests/plc_tags.csv'])
     captured = capsys.readouterr()
     assert 'AV-101' in captured.out
     assert 'GAS-101' in captured.out
     assert 'TI-101' in captured.out
     with pytest.raises(SystemExit):
         command_line(['fakeip', 'tags', 'bogus'])
```

### Comparing `productivity-0.8.1/productivity/util.py` & `productivity-0.9.1/productivity/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 Copyright (C) 2022 NuMat Technologies
 """
 import asyncio
 
 try:
     from pymodbus.client import AsyncModbusTcpClient  # 3.x
 except ImportError:  # 2.4.x - 2.5.x
-    from pymodbus.client.asynchronous.async_io import (   # type: ignore
-        ReconnectingAsyncioModbusTcpClient)
+    from pymodbus.client.asynchronous.async_io import ReconnectingAsyncioModbusTcpClient  # type: ignore
 import pymodbus.exceptions
 
 TYPE_START = {
     'discrete_output': 0,
     'discrete_input': 100000,
     'input': 300000,
     'holding': 400000,
@@ -35,54 +34,60 @@
     'STR': 'str',      # STRing
     'SSTR': 'str',     # System STRing
     'SWR': 'int16',    # System Word Read-only
     'SWRW': 'int16'    # System Word Read-Write
 }
 
 
-class AsyncioModbusClient(object):
+class AsyncioModbusClient:
     """A generic asyncio client.
 
     This expands upon the pymodbus AsyncModbusTcpClient by
     including standard timeouts, async context manager, and queued requests.
     """
 
     _register_types = ['holding', 'input']
 
     def __init__(self, address, timeout=1):
         """Set up communication parameters."""
         self.ip = address
         self.timeout = timeout
-        try:
-            self.client = AsyncModbusTcpClient(address, timeout=timeout)  # 3.0
-        except NameError:
-            self.client = ReconnectingAsyncioModbusTcpClient()  # 2.4.x - 2.5.x
+        self._detect_pymodbus_version()
+        if self.pymodbus30plus:
+            self.client = AsyncModbusTcpClient(address, timeout=timeout)
+        else:  # 2.x
+            self.client = ReconnectingAsyncioModbusTcpClient()
         self.lock = asyncio.Lock()
         self.connectTask = asyncio.create_task(self._connect())
         self.open = False
 
     async def __aenter__(self):
         """Asynchronously connect with the context manager."""
         return self
 
     async def __aexit__(self, *args):
         """Provide exit to the context manager."""
         await self._close()
 
+    def _detect_pymodbus_version(self) -> None:
+        self.pymodbus30plus = int(pymodbus.__version__[0]) == 3
+        self.pymodbus32plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 2
+        self.pymodbus33plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 3
+
     async def _connect(self):
         """Start asynchronous reconnect loop."""
         async with self.lock:
             try:
-                try:
+                if self.pymodbus30plus:
                     await asyncio.wait_for(self.client.connect(), timeout=self.timeout)  # 3.x
-                except AttributeError:
-                    await self.client.start(self.ip)  # 2.4.x - 2.5.x
+                else:  # 2.4.x - 2.5.x
+                    await self.client.start(self.ip)  # type: ignore
                 self.open = True
             except Exception:
-                raise IOError(f"Could not connect to '{self.ip}'.")
+                raise OSError(f"Could not connect to '{self.ip}'.")
 
     async def read_coils(self, address, count):
         """Read modbus output coils (0 address prefix)."""
         return await self._request('read_coils', address, count)
 
     async def read_discrete_inputs(self, address, count):
         """Read modbus discrete inputs (1 address prefix)."""
@@ -151,30 +156,25 @@
         request sent while it's processing something). The driver handles this
         by assuming there is only one client instance. If other clients
         exist, other logic will have to be added to either prevent or manage
         race conditions.
         """
         await self.connectTask
         async with self.lock:
-            if not self.client.connected or not self.open:
-                raise TimeoutError("Not connected to PLC.")
-            future = getattr(self.client.protocol, method)(*args, **kwargs)
             try:
-                return await asyncio.wait_for(future, timeout=self.timeout)
-            except asyncio.TimeoutError as e:
-                if self.open:
-                    # This came from reading through the pymodbus@python3 source
-                    # Problem was that the driver was not detecting disconnect
-                    if hasattr(self, 'modbus'):
-                        self.client.protocol_lost_connection(self.modbus)
-                    self.open = False
-                raise TimeoutError(e)
-            except pymodbus.exceptions.ConnectionException as e:
-                raise ConnectionError(e)
+                if self.pymodbus32plus:
+                    future = getattr(self.client, method)
+                else:
+                    future = getattr(self.client.protocol, method)  # type: ignore
+                return await future(*args, **kwargs)
+            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException):
+                raise TimeoutError("Not connected to PLC.")
 
-    async def _close(self):
+    async def _close(self) -> None:
         """Close the TCP connection."""
-        try:
-            await self.client.close()  # 3.x
-        except AttributeError:
-            self.client.stop()  # 2.4.x - 2.5.x
+        if self.pymodbus33plus:
+            self.client.close()  # 3.3.x
+        elif self.pymodbus30plus:
+            await self.client.close()  # type: ignore  # 3.0.x - 3.2.x
+        else:  # 2.4.x - 2.5.x
+            self.client.stop()  # type: ignore
         self.open = False
```

### Comparing `productivity-0.8.1/productivity.egg-info/PKG-INFO` & `productivity-0.9.1/productivity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: productivity
-Version: 0.8.1
+Version: 0.9.1
 Summary: Python driver for AutomationDirect Productivity Series PLCs.
-Home-page: http://github.com/numat/productivity/
+Home-page: https://github.com/numat/productivity/
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
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `productivity-0.8.1/setup.py` & `productivity-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """Python driver for AutomationDirect Productivity Series PLCs."""
 from sys import version_info
+
 from setuptools import setup
 
 if version_info < (3, 7):
     raise ImportError("This module requires Python >=3.7.  Use 0.6.0 for Python3.6")
 
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name='productivity',
-    version='0.8.1',
+    version='0.9.1',
     description="Python driver for AutomationDirect Productivity Series PLCs.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='http://github.com/numat/productivity/',
+    url='https://github.com/numat/productivity/',
     author='Patrick Fuller',
     author_email='pat@numat-tech.com',
+    maintainer="Alex Ruddick",
+    maintainer_email="alex@numat-tech.com",
     packages=['productivity'],
     entry_points={
         'console_scripts': [('productivity = productivity:command_line')]
     },
     install_requires=[
         'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.2.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
         'PyYAML',
     ],
     extras_require={
         'test': [
+            'mypy==1.3.0',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
+            'ruff==0.0.270',
+            'types-PyYAML'
         ],
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
```

