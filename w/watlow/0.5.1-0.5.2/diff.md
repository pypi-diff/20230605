# Comparing `tmp/watlow-0.5.1.tar.gz` & `tmp/watlow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watlow-0.5.1.tar", last modified: Thu Dec 15 18:45:04 2022, max compression
+gzip compressed data, was "watlow-0.5.2.tar", last modified: Mon Jun  5 21:33:22 2023, max compression
```

## Comparing `watlow-0.5.1.tar` & `watlow-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2022-12-15 18:45:04.159506 watlow-0.5.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2021-07-06 15:20:32.000000 watlow-0.5.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2021-07-06 15:20:32.000000 watlow-0.5.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3003 2022-12-15 18:45:04.159594 watlow-0.5.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.5.1/README.md
--rw-r--r--   0 a.ruddick   (502) staff       (20)      172 2022-12-15 18:45:04.159893 watlow-0.5.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1840 2022-12-15 18:37:36.000000 watlow-0.5.1/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2022-12-15 18:45:04.158297 watlow-0.5.1/watlow/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2022-11-16 23:55:15.000000 watlow-0.5.1/watlow/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     7767 2022-11-16 23:55:15.000000 watlow-0.5.1/watlow/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2050 2022-11-16 23:55:15.000000 watlow-0.5.1/watlow/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5582 2022-12-15 18:37:36.000000 watlow-0.5.1/watlow/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2022-12-15 18:45:04.159347 watlow-0.5.1/watlow.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3003 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      237 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2022-12-15 18:45:04.000000 watlow-0.5.1/watlow.egg-info/top_level.txt
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.256345 watlow-0.5.2/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-06-05 17:03:36.000000 watlow-0.5.2/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-06-05 17:03:36.000000 watlow-0.5.2/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-05 21:33:22.256409 watlow-0.5.2/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.5.2/README.md
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      110 2023-06-05 21:33:22.256599 watlow-0.5.2/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1990 2023-06-05 21:32:55.000000 watlow-0.5.2/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.255332 watlow-0.5.2/watlow/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1830 2023-06-05 15:40:30.000000 watlow-0.5.2/watlow/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     9120 2023-06-05 17:03:36.000000 watlow-0.5.2/watlow/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2120 2023-06-05 21:32:01.000000 watlow-0.5.2/watlow/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     6071 2023-06-05 21:32:01.000000 watlow-0.5.2/watlow/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:33:22.256214 watlow-0.5.2/watlow.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      270 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-06-05 21:33:22.000000 watlow-0.5.2/watlow.egg-info/top_level.txt
```

### Comparing `watlow-0.5.1/LICENSE` & `watlow-0.5.2/LICENSE`

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

### Comparing `watlow-0.5.1/PKG-INFO` & `watlow-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
-Home-page: http://github.com/numat/watlow/
+Home-page: https://github.com/numat/watlow/
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

### Comparing `watlow-0.5.1/README.md` & `watlow-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `watlow-0.5.1/setup.py` & `watlow-0.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 """Install parameters for CLI and python import."""
 from sys import version_info
+
 from setuptools import setup
 
-if version_info < (3, 7):
+if version_info < (3, 7):  # noqa: UP036
     raise ImportError("This module requires Python >=3.7.  Use 0.3.1 for Python3.6")
 
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="watlow",
-    version="0.5.1",
+    version="0.5.2",
     description="Python driver for Watlow EZ-Zone temperature controllers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="http://github.com/numat/watlow/",
+    url="https://github.com/numat/watlow/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
+    maintainer="Alex Ruddick",
+    maintainer_email="alex@numat-tech.com",
     packages=["watlow"],
     install_requires=[
         'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
         "pyserial",
         "crcmod"],
     extras_require={
         'test': [
+            'mypy==1.3.0',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
+            'ruff==0.0.270',
         ],
     },
     entry_points={
         "console_scripts": [("watlow = watlow:command_line")]
     },
     license="GPLv2",
     classifiers=[
```

### Comparing `watlow-0.5.1/watlow/__init__.py` & `watlow-0.5.2/watlow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Python driver for Watlow EZ-Zone temperature controllers.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2019 NuMat Technologies
 """
-from watlow.driver import TemperatureController, Gateway
 from watlow import mock  # noqa: F401
+from watlow.driver import Gateway, TemperatureController
 
 
 def command_line(args=None):
     """CLI interface, accessible when installed through pip."""
     import argparse
     import asyncio
     import json
@@ -21,15 +21,15 @@
     parser.add_argument('--set-setpoint', '-f', default=None, type=float,
                         help="Sets the setpoint temperature.")
     parser.add_argument('--zone', '-z', default=None, type=int,
                         help="Specify zone in case of gateway")
     args = parser.parse_args(args)
 
     async def run():
-        async with Gateway(args) as gateway:
+        async with Gateway(args.port) as gateway:
             if args.set_setpoint:
                 await gateway.set_setpoint(args.zone, args.set_setpoint)
             d = await gateway.get(args.zone)
             print(json.dumps(d, indent=4))
 
     if args.zone:
         loop = asyncio.new_event_loop()
```

### Comparing `watlow-0.5.1/watlow/driver.py` & `watlow-0.5.2/watlow/driver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 """Drivers for Watlow EZ-Zone temperature controllers."""
+from __future__ import annotations
+
+import logging
+import re
 import struct
 from binascii import unhexlify
-import re
 
-import crcmod
+import crcmod  # type: ignore
 import serial
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder, BinaryPayloadDecoder
 
 from .util import AsyncioModbusClient
 
-crc = crcmod.mkCrcFun(0b10001000000100001)
+# BACnet CRC: https://sourceforge.net/p/bacnet/mailman/message/1259086/
+# CRC8 polynominal: X^8 + X^7 + 1 (110000001)
+crc8 = crcmod.mkCrcFun(0b110000001)
+# CRC16 polynominal: X^16 + X^12 + X^5 + 1 (10001000000100001)
+crc16 = crcmod.mkCrcFun(0b10001000000100001)
 
 
 def f_to_c(f):
     """Convert Fahrenheit to Celsius."""
     return (f - 32.0) / 1.8
 
 
 def c_to_f(c):
     """Convert Celsius to Fahrenheit."""
     return c * 1.8 + 32.0
 
 
-class TemperatureController(object):
+class TemperatureController:
     """Driver for the Watlow EZ-ZONE temperature controller.
 
     This driver borrows heavily from this StackOverflow post:
         https://reverseengineering.stackexchange.com/questions/8303/
         rs-485-checksum-reverse-engineering-watlow-ez-zone-pm
 
     The EZ-Zone communication protocol is Bacnet MS/TP over a serial line.
@@ -48,18 +55,25 @@
      * First checksum is a custom protocol.
      * Only known registers are 0401 for PV and 0701 for SP. Other registers
        return data, so we could hunt around for PID params if needed.
      * Instance, only 01 works. Current understanding is similar to zone.
      * Second checksum is a custom CRC-16 following Bacnet spec.
     """
 
-    commands = {'actual': unhexlify('55ff0510000006e8010301040101e399'),
-                'setpoint': unhexlify('55ff0510000006e80103010701018776'),
-                'set': {'header': unhexlify('55ff051000000aec'),
-                        'body': unhexlify('010407010108')}}
+    commands = {
+        'actual':
+            {'header': unhexlify('0510000006'),
+             'body':   unhexlify('010301040101')},
+        'setpoint':
+            {'header': unhexlify('0510000006'),
+             'body':   unhexlify('010301070101')},
+        'set':
+            {'header': unhexlify('051000000a'),
+             'body':   unhexlify('010407010108')},
+    }
     responses = {
         'actual': re.compile('^55ff060010000b8802030104010108'
                              '([0-9a-f]{8})([0-9a-f]{4})$'),
         'setpoint': re.compile('^55ff060010000b8802030107010108'
                                '([0-9a-f]{8})([0-9a-f]{4})$'),
         'set': re.compile('^55ff060010000a76020407010108'
                           '([0-9a-f]{8})([0-9a-f]{4})$')
@@ -70,52 +84,66 @@
 
         This device uses RS-422 instead of RS-232. You will likely need a
         custom converter.
         """
         self.port = port
         self.baudrate = 38400
         self.timeout = timeout
-        self.connection = None
-        self.open()
+        self.connection = self.open()
 
     def open(self):
         """Open up a serial connection to the oven."""
-        self.connection = serial.Serial(
+        return serial.Serial(
             self.port,
             self.baudrate,
             timeout=self.timeout
         )
 
     def close(self):
         """Close the serial connection. Use on cleanup."""
         self.connection.flush()
         self.connection.close()
 
     def get(self):
         """Get the current temperature and setpoint, in C."""
+        preamble = unhexlify('55ff')
         output = {'actual': None, 'setpoint': None}
         for key in output:
+            header = self.commands[key]['header']
+            body = self.commands[key]['body']
+            # Calculate header and data checksums based on BACnet CRC
+            header_checksum = struct.pack('<H', ~crc8(self.commands[key]['header']) & 0xff)
+            data_checksum = struct.pack('<H', ~crc16(self.commands[key]['body']) & 0xffff)
+
+            # send command to controller, formatting preamble, header, crc8, body and crc16
             output[key] = self._write_and_read(
-                request=self.commands[key],
+                request=preamble + header + header_checksum[:1] + body + data_checksum,
                 length=21,
                 check=self.responses[key]
             )
         return output
 
     def set(self, setpoint):
         """Set the setpoint temperature, in C."""
+        preamble = unhexlify('55ff')
+        header = self.commands['set']['header']
         body = self.commands['set']['body'] + struct.pack('>f', c_to_f(setpoint))
-        checksum = struct.pack('<H', ~crc(body) & 0xffff)
+        # Calculate header and data checksums based on BACnet CRC
+        header_checksum = struct.pack('<H', ~crc8(self.commands['set']['header']) & 0xff)
+        data_checksum = struct.pack('<H', ~crc16(body) & 0xffff)
+
         response = self._write_and_read(
-            request=self.commands['set']['header'] + body + checksum,
+            request=preamble + header + header_checksum[:1] + body + data_checksum,
             length=20,
             check=self.responses['set']
         )
+
+        # check setpoint versus response, if not the same raise an error
         if round(setpoint, 2) != round(response, 2):
-            raise IOError(f"Could not change setpoint from "
+            raise OSError(f"Could not change setpoint from "
                           f"{response:.2f}°C to {setpoint:.2f}°C.")
 
     def _write_and_read(self, request, length, check, retries=3):
         """Write to and read from the device.
 
         This function abstracts a whole lot of validation checks and error
         handling. The goal is for this driver to be stable to both incomplete
@@ -126,22 +154,24 @@
             http://www.bacnet.org/Addenda/Add-135-2010an-APR1-1_chair-approved.pdf
         However, my attempts at reproducing did not go well.
         """
         if not self.connection.is_open:
             self.open()
         if retries <= 0:
             self.close()
-            raise IOError("Could not communicate with Watlow.")
+            raise OSError("Could not communicate with Watlow.")
         self.connection.flush()
         try:
+            logging.debug('Formatted Request: ' + str(bytes.hex(request)))
             self.connection.write(request)
             response = self.connection.read(length)
         except serial.serialutil.SerialException:
             return self._write_and_read(request, length, check, retries - 1)
         match = check.match(bytes.hex(response))
+        logging.debug('Formatted Response: ' + str(bytes.hex(response)))
         if not match:
             return self._write_and_read(request, length, check, retries - 1)
         value = match.group(1)
         # From docstring, `checksum = match.group(2)` could be added and checked.
         temperature = f_to_c(struct.unpack('>f', unhexlify(value))[0])
         if temperature < 0 or temperature > 250:
             return self._write_and_read(request, length, check, retries - 1)
@@ -161,15 +191,15 @@
         self.setpoint_range = (10, max_temp)
 
     async def get(self, zone: int):
         """Get oven data for a zone.
 
         For more information on a 'Zone', refer to Watlow manuals.
         """
-        output = {
+        output: dict[str, int | None] = {
             'actual': self.actual_temp_address,
             'setpoint': self.setpoint_address,
             'output': self.output_address,
         }
         for k, v in output.items():
             address = (zone - 1) * self.modbus_offset + v
             try:
@@ -189,9 +219,9 @@
         """
         if not self.setpoint_range[0] <= setpoint <= self.setpoint_range[1]:
             raise ValueError(f"Setpoint ({setpoint}) is not in the valid range from"
                              f" {self.setpoint_range[0]} to {self.setpoint_range[1]}")
         address = (zone - 1) * self.modbus_offset + self.setpoint_address
         builder = BinaryPayloadBuilder(byteorder=Endian.Big)
         builder.add_32bit_float(setpoint)
-        await self.client.protocol.write_registers(address, builder.build(),
-                                                   skip_encode=True)
+        await self.write_registers(address, builder.build(),
+                                   skip_encode=True)
```

### Comparing `watlow-0.5.1/watlow/mock.py` & `watlow-0.5.2/watlow/mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Mock Watlow interface. Use for debugging systems."""
 
 import asyncio
-from random import random
 from copy import deepcopy
+from random import random
 from unittest.mock import MagicMock
 
 from watlow.driver import Gateway as realGateway
 
 
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
     async def __call__(self, *args, **kwargs):
         """Convert regular mocks into into an async coroutine."""
         return super().__call__(*args, **kwargs)
 
+    def close(self):
+        """Close the connection."""
+        ...
+
 
 class Gateway(realGateway):
     """Mock interface to the Watlow Gateway used to communicate with ovens."""
 
     def __init__(self, *args, max_temp=220, **kwargs):
         """Set random data."""
         self.setpoint_range = (10, max_temp)
```

### Comparing `watlow-0.5.1/watlow/util.py` & `watlow-0.5.2/watlow/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,54 +4,62 @@
 Copyright (C) 2022 NuMat Technologies
 """
 import asyncio
 
 try:
     from pymodbus.client import AsyncModbusTcpClient  # 3.x
 except ImportError:  # 2.4.x - 2.5.x
-    from pymodbus.client.asynchronous.async_io import ReconnectingAsyncioModbusTcpClient
+    from pymodbus.client.asynchronous.async_io import (  # type: ignore
+        ReconnectingAsyncioModbusTcpClient,
+    )
 import pymodbus.exceptions
 
 
-class AsyncioModbusClient(object):
+class AsyncioModbusClient:
     """A generic asyncio client.
 
     This expands upon the pymodbus AsyncModbusTcpClient by
     including standard timeouts, async context manager, and queued requests.
     """
 
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
             except Exception:
-                raise IOError(f"Could not connect to '{self.ip}'.")
+                raise OSError(f"Could not connect to '{self.ip}'.")
 
     async def read_coils(self, address, count):
         """Read modbus output coils (0 address prefix)."""
         return await self._request('read_coils', address, count)
 
     async def read_registers(self, address, count):
         """Read modbus registers.
@@ -124,13 +132,15 @@
                     self.client.protocol_lost_connection(self.modbus)
                 raise TimeoutError(e)
             except pymodbus.exceptions.ConnectionException as e:
                 if self.client.connected and hasattr(self, 'modbus'):
                     self.client.protocol_lost_connection(self.modbus)
                 raise ConnectionError(e)
 
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
```

### Comparing `watlow-0.5.1/watlow.egg-info/PKG-INFO` & `watlow-0.5.2/watlow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
-Home-page: http://github.com/numat/watlow/
+Home-page: https://github.com/numat/watlow/
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

