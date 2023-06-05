# Comparing `tmp/clickplc-0.7.0.tar.gz` & `tmp/clickplc-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickplc-0.7.0.tar", last modified: Tue Feb 28 22:35:46 2023, max compression
+gzip compressed data, was "clickplc-0.7.1.tar", last modified: Mon Jun  5 21:17:35 2023, max compression
```

## Comparing `clickplc-0.7.0.tar` & `clickplc-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 22:35:46.166242 clickplc-0.7.0/
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 22:35:46.163614 clickplc-0.7.0/.github/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      153 2021-09-24 00:06:19.000000 clickplc-0.7.0/.github/dependabot.yaml
--rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2022-11-17 00:56:19.000000 clickplc-0.7.0/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2021-09-24 00:06:19.000000 clickplc-0.7.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2023-02-06 20:30:11.000000 clickplc-0.7.0/MANIFEST.in
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3817 2023-02-28 22:35:46.166308 clickplc-0.7.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2938 2022-05-18 14:45:44.000000 clickplc-0.7.0/README.md
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1371 2022-11-17 00:56:19.000000 clickplc-0.7.0/azure-pipelines.yml
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 22:35:46.164580 clickplc-0.7.0/clickplc/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1354 2022-11-17 00:56:19.000000 clickplc-0.7.0/clickplc/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    22190 2023-02-28 22:35:22.000000 clickplc-0.7.0/clickplc/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2947 2022-11-17 00:56:19.000000 clickplc-0.7.0/clickplc/mock.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 22:35:46.165997 clickplc-0.7.0/clickplc/tests/
--rw-------   0 a.ruddick   (502) staff       (20)        0 2021-09-24 00:06:19.000000 clickplc-0.7.0/clickplc/tests/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)      190 2021-09-24 00:06:19.000000 clickplc-0.7.0/clickplc/tests/bad_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2306 2022-05-18 14:45:44.000000 clickplc-0.7.0/clickplc/tests/plc_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)    10481 2022-10-24 18:01:53.000000 clickplc-0.7.0/clickplc/tests/test_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5126 2023-02-28 22:35:22.000000 clickplc-0.7.0/clickplc/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-02-28 22:35:46.165424 clickplc-0.7.0/clickplc.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3817 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      484 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      264 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-02-28 22:35:46.000000 clickplc-0.7.0/clickplc.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      206 2023-02-28 22:35:46.166514 clickplc-0.7.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1821 2023-02-28 22:35:22.000000 clickplc-0.7.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.041057 clickplc-0.7.1/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:38:49.000000 clickplc-0.7.1/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 23:33:43.000000 clickplc-0.7.1/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2023-02-06 20:30:11.000000 clickplc-0.7.1/MANIFEST.in
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3694 2023-06-05 21:17:35.041118 clickplc-0.7.1/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2751 2023-04-11 05:40:45.000000 clickplc-0.7.1/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.039119 clickplc-0.7.1/clickplc/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1354 2022-11-17 00:56:19.000000 clickplc-0.7.1/clickplc/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    22132 2023-04-10 23:33:43.000000 clickplc-0.7.1/clickplc/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3065 2023-06-05 21:17:10.000000 clickplc-0.7.1/clickplc/mock.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.040640 clickplc-0.7.1/clickplc/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      190 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/bad_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2306 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/plc_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    10508 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/test_driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5541 2023-06-05 21:17:10.000000 clickplc-0.7.1/clickplc/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.039980 clickplc-0.7.1/clickplc.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3694 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      440 2023-06-05 21:17:35.000000 clickplc-0.7.1/clickplc.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      254 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      161 2023-06-05 21:17:35.041323 clickplc-0.7.1/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1741 2023-06-05 21:17:13.000000 clickplc-0.7.1/setup.py
```

### Comparing `clickplc-0.7.0/LICENSE` & `clickplc-0.7.1/LICENSE`

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

### Comparing `clickplc-0.7.0/PKG-INFO` & `clickplc-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python driver for Koyo Ethernet ClickPLCs.
-Home-page: http://github.com/numat/clickplc/
+Home-page: https://github.com/numat/clickplc/
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
@@ -17,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-clickplc [![Build Status](https://dev.azure.com/numat/NuMat/_apis/build/status/numat.clickplc?branchName=master)](https://dev.azure.com/numat/NuMat/_build/latest?definitionId=3&branchName=master)
+clickplc
 ========
 
 Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
```

### Comparing `clickplc-0.7.0/README.md` & `clickplc-0.7.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-clickplc [![Build Status](https://dev.azure.com/numat/NuMat/_apis/build/status/numat.clickplc?branchName=master)](https://dev.azure.com/numat/NuMat/_build/latest?definitionId=3&branchName=master)
+clickplc
 ========
 
 Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
```

### Comparing `clickplc-0.7.0/clickplc/__init__.py` & `clickplc-0.7.1/clickplc/__init__.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.0/clickplc/driver.py` & `clickplc-0.7.1/clickplc/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 A Python driver for Koyo ClickPLC ethernet units.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2020 NuMat Technologies
 """
+from __future__ import annotations
+
 import copy
 import csv
 import pydoc
 from collections import defaultdict
 from string import digits
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder, BinaryPayloadDecoder
 
 from clickplc.util import AsyncioModbusClient
 
 
@@ -55,15 +57,15 @@
 
         Returns:
             A dictionary containing information associated with each tag name.
 
         """
         return copy.deepcopy(self.tags)
 
-    async def get(self, address: Optional[str] = None) -> dict:
+    async def get(self, address: str | None = None) -> dict:
         """Get variables from the ClickPLC.
 
         Args:
             address: ClickPLC address(es) to get. Specify a range with a
                 hyphen, e.g. 'DF1-DF40'
 
         If driver is loaded with a tags file this can be called without an
@@ -100,15 +102,15 @@
         i = next(i for i, s in enumerate(start) if s.isdigit())
         category, start_index = start[:i].lower(), int(start[i:])
         end_index = None if end is None else int(end[i:])
 
         if end_index is not None and end_index < start_index:
             raise ValueError("End address must be greater than start address.")
         if category not in self.data_types:
-            raise ValueError("{} currently unsupported.".format(category))
+            raise ValueError(f"{category} currently unsupported.")
         if end is not None and end[:i].lower() != category:
             raise ValueError("Inter-category ranges are unsupported.")
         return await getattr(self, '_get_' + category)(start_index, end_index)
 
     async def set(self, address: str, data):
         """Set values on the ClickPLC.
 
@@ -241,15 +243,15 @@
             elif current % 100 <= 16:
                 output[f'y{current:03}'] = bit
             elif current % 100 == 32:
                 current += 100 - 32
             current += 1
         return output
 
-    async def _get_c(self, start: int, end: int) -> Union[dict, bool]:
+    async def _get_c(self, start: int, end: int) -> dict | bool:
         """Read C addresses. Called by `get`.
 
         C entries start at 16384 (16385 in the Click software's 1-indexed
         notation). This continues for 2000 bits, ending at 18383.
 
         The response always returns a full byte of data. If you request
         a number of addresses not divisible by 8, it will have extra data. The
@@ -268,15 +270,15 @@
             count = end_coil - start_coil + 1
 
         coils = await self.read_coils(start_coil, count)
         if count == 1:
             return coils.bits[0]
         return {f'c{(start + i)}': bit for i, bit in enumerate(coils.bits) if i < count}
 
-    async def _get_df(self, start: int, end: int) -> Union[dict, float]:
+    async def _get_df(self, start: int, end: int) -> dict | float:
         """Read DF registers. Called by `get`.
 
         DF entries start at Modbus address 28672 (28673 in the Click software's
         1-indexed notation). Each DF entry takes 32 bits, or 2 16-bit
         registers.
         """
         if start < 1 or start > 500:
@@ -290,15 +292,15 @@
         decoder = BinaryPayloadDecoder.fromRegisters(registers,
                                                      byteorder=Endian.Big,
                                                      wordorder=Endian.Little)
         if end is None:
             return decoder.decode_32bit_float()
         return {f'df{n}': decoder.decode_32bit_float() for n in range(start, end + 1)}
 
-    async def _get_ds(self, start: int, end: int) -> Union[dict, int]:
+    async def _get_ds(self, start: int, end: int) -> dict | int:
         """Read DS registers. Called by `get`.
 
         DS entries start at Modbus address 0 (1 in the Click software's
         1-indexed notation). Each DS entry takes 16 bits.
         """
         if start < 1 or start > 4500:
             raise ValueError('DS must be in [1, 4500]')
@@ -311,15 +313,15 @@
         decoder = BinaryPayloadDecoder.fromRegisters(registers,
                                                      byteorder=Endian.Big,
                                                      wordorder=Endian.Little)
         if end is None:
             return decoder.decode_16bit_int()
         return {f'ds{n}': decoder.decode_16bit_int() for n in range(start, end + 1)}
 
-    async def _get_sd(self, start: int, end: int) -> Union[dict, int]:
+    async def _get_sd(self, start: int, end: int) -> dict | int:
         """Read SD registers. Called by `get`.
 
         SD entries start at Modbus address 361440 (361441 in the Click software's
         1-indexed notation). Each SD entry takes 16 bits.
         """
         if start < 1 or start > 4500:
             raise ValueError('SD must be in [1, 4500]')
@@ -353,15 +355,15 @@
         decoder = BinaryPayloadDecoder.fromRegisters(registers,
                                                      byteorder=Endian.Big,
                                                      wordorder=Endian.Little)
         if end is None:
             return decoder.decode_32bit_int()
         return {f'ctd{n}': decoder.decode_32bit_int() for n in range(start, end + 1)}
 
-    async def _set_x(self, start: int, data: Union[List[bool], bool]):
+    async def _set_x(self, start: int, data: list[bool] | bool):
         """Set X addresses. Called by `set`.
 
         For more information on the quirks of X coils, read the `_get_x`
         docstring.
         """
         if start % 100 == 0 or start % 100 > 16:
             raise ValueError('X start address must be *01-*16.')
@@ -381,15 +383,15 @@
                 payload += data[:16] + [False] * 16
                 data = data[16:]
             payload += data
             await self.write_coils(coil, payload)
         else:
             await self.write_coil(coil, data)
 
-    async def _set_y(self, start: int, data: Union[List[bool], bool]):
+    async def _set_y(self, start: int, data: list[bool] | bool):
         """Set Y addresses. Called by `set`.
 
         For more information on the quirks of Y coils, read the `_get_y`
         docstring.
         """
         if start % 100 == 0 or start % 100 > 16:
             raise ValueError('Y start address must be *01-*16.')
@@ -409,15 +411,15 @@
                 payload += data[:16] + [False] * 16
                 data = data[16:]
             payload += data
             await self.write_coils(coil, payload)
         else:
             await self.write_coil(coil, data)
 
-    async def _set_c(self, start: int, data: Union[List[bool], bool]):
+    async def _set_c(self, start: int, data: list[bool] | bool):
         """Set C addresses. Called by `set`.
 
         For more information on the quirks of C coils, read the `_get_c`
         docstring.
         """
         if start < 1 or start > 2000:
             raise ValueError('C start address must be 1-2000.')
@@ -426,54 +428,54 @@
         if isinstance(data, list):
             if len(data) > (2000 - start):
                 raise ValueError('Data list longer than available addresses.')
             await self.write_coils(coil, data)
         else:
             await self.write_coil(coil, data)
 
-    async def _set_df(self, start: int, data: Union[List[float], float]):
+    async def _set_df(self, start: int, data: list[float] | float):
         """Set DF registers. Called by `set`.
 
         The ClickPLC is little endian, but on registers ("words") instead
         of bytes. As an example, take a random floating point number:
             Input: 0.1
             Hex: 3dcc cccd (IEEE-754 float32)
             Click: -1.076056E8
             Hex: cccd 3dcc
         To fix, we need to flip the registers. Implemented below in `pack`.
         """
         if start < 1 or start > 500:
             raise ValueError('DF must be in [1, 500]')
         address = 28672 + 2 * (start - 1)
 
-        def _pack(values: List[float]):
+        def _pack(values: list[float]):
             builder = BinaryPayloadBuilder(byteorder=Endian.Big,
                                            wordorder=Endian.Little)
             for value in values:
                 builder.add_32bit_float(float(value))
             return builder.build()
 
         if isinstance(data, list):
             if len(data) > 500 - start:
                 raise ValueError('Data list longer than available addresses.')
             payload = _pack(data)
             await self.write_registers(address, payload, skip_encode=True)
         else:
             await self.write_register(address, _pack([data]), skip_encode=True)
 
-    async def _set_ds(self, start: int, data: Union[List[int], int]):
+    async def _set_ds(self, start: int, data: list[int] | int):
         """Set DS registers. Called by `set`.
 
         See _get_ds for more information.
         """
         if start < 1 or start > 4500:
             raise ValueError('DS must be in [1, 4500]')
         address = (start - 1)
 
-        def _pack(values: List[int]):
+        def _pack(values: list[int]):
             builder = BinaryPayloadBuilder(byteorder=Endian.Big,
                                            wordorder=Endian.Little)
             for value in values:
                 builder.add_16bit_int(int(value))
             return builder.build()
 
         if isinstance(data, list):
@@ -492,15 +494,15 @@
 
         """
         if not tag_filepath:
             return {}
         with open(tag_filepath) as csv_file:
             csv_data = csv_file.read().splitlines()
         csv_data[0] = csv_data[0].lstrip('## ')
-        parsed: Dict[str, Dict[str, Any]] = {
+        parsed: dict[str, dict[str, Any]] = {
             row['Nickname']: {
                 'address': {
                     'start': int(row['Modbus Address']),
                 },
                 'id': row['Address'],
                 'comment': row['Address Comment'],
                 'type': self.data_types.get(
@@ -519,15 +521,15 @@
                     "github issue at numat/clickplc to get it added."
                 )
         sorted_tags = {k: parsed[k] for k in
                        sorted(parsed, key=lambda k: parsed[k]['address']['start'])}
         return sorted_tags
 
     @staticmethod
-    def _get_address_ranges(tags: dict) -> Dict[str, Dict]:
+    def _get_address_ranges(tags: dict) -> dict[str, dict]:
         """Determine range of addresses required.
 
         Parse the loaded tags to determine the range of addresses that must be
         queried to return all values
         """
         address_dict: dict = defaultdict(lambda: {'min': 1, 'max': 1})
         for tag_info in tags.values():
```

### Comparing `clickplc-0.7.0/clickplc/mock.py` & `clickplc-0.7.1/clickplc/mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2021 NuMat Technologies
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
 from pymodbus.register_write_message import WriteMultipleRegistersResponse
 
 from clickplc.driver import ClickPLC as realClickPLC
 
 
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
     async def __call__(self, *args, **kwargs):
         """Convert regular mocks into into an async coroutine."""
         return super().__call__(*args, **kwargs)
 
+    def stop(self) -> None:
+        """Close the connection (2.5.3)."""
+        ...
 
 class ClickPLC(realClickPLC):
     """A version of the driver replacing remote communication with local storage for testing."""
 
     def __init__(self, address, tag_filepath='', timeout=1):
         self.tags = self._load_tags(tag_filepath)
         self.active_addresses = self._get_address_ranges(self.tags)
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

### Comparing `clickplc-0.7.0/clickplc/tests/plc_tags.csv` & `clickplc-0.7.1/clickplc/tests/plc_tags.csv`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.0/clickplc/tests/test_driver.py` & `clickplc-0.7.1/clickplc/tests/test_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Confirm the driver correctly initializes without a tags file."""
     return ClickPLC('fake ip')
 
 
 @pytest.fixture
 def tagged_driver():
     """Confirm the driver correctly initializes with a good tags file."""
-    return ClickPLC('fake ip', 'tests/plc_tags.csv')
+    return ClickPLC('fake ip', 'clickplc/tests/plc_tags.csv')
 
 
 @pytest.fixture
 def expected_tags():
     """Return the tags defined in the tags file."""
     return {
         'IO2_24V_OK': {'address': {'start': 16397}, 'id': 'C13', 'type': 'bool'},
@@ -53,15 +53,15 @@
     assert 'c100' in captured.out
     assert 'df100' in captured.out
 
 
 @mock.patch('clickplc.ClickPLC', ClickPLC)
 def test_driver_cli_tags(capsys):
     """Confirm the commandline interface works with a tags file."""
-    command_line(['fakeip', 'tests/plc_tags.csv'])
+    command_line(['fakeip', 'clickplc/tests/plc_tags.csv'])
     captured = capsys.readouterr()
     assert 'P_101' in captured.out
     assert 'VAHH_101_OK' in captured.out
     assert 'TI_101' in captured.out
     with pytest.raises(SystemExit):
         command_line(['fakeip', 'tags', 'bogus'])
 
@@ -70,15 +70,15 @@
     """Confirm that the driver returns correct values on get() calls."""
     assert expected_tags == tagged_driver.get_tags()
 
 
 def test_unsupported_tags():
     """Confirm the driver detects an improper tags file."""
     with pytest.raises(TypeError, match='unsupported data type'):
-        ClickPLC('fake ip', 'tests/bad_tags.csv')
+        ClickPLC('fake ip', 'clickplc/tests/bad_tags.csv')
 
 
 @pytest.mark.asyncio
 async def test_tagged_driver(tagged_driver, expected_tags):
     """Test a roundtrip with the driver using a tags file."""
     await tagged_driver.set('VAH_101_OK', True)
     state = await tagged_driver.get()
```

### Comparing `clickplc-0.7.0/clickplc/util.py` & `clickplc-0.7.1/clickplc/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 """Base functionality for modbus communication.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2022 NuMat Technologies
 """
+from __future__ import annotations
+
 import asyncio
 
 try:
     from pymodbus.client import AsyncModbusTcpClient  # 3.x
 except ImportError:  # 2.4.x - 2.5.x
     from pymodbus.client.asynchronous.async_io import (  # type: ignore
-        ReconnectingAsyncioModbusTcpClient)
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
-            self.pymodbus32plus = not hasattr(self.client, 'protocol')  # >= 3.2.0
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
 
+    def _detect_pymodbus_version(self):
+        """Detect various pymodbus versions."""
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
-                except AttributeError:  # 2.4.x - 2.5.x
+                else:  # 2.4.x - 2.5.x
                     await self.client.start(self.ip)  # type: ignore
                 self.open = True
             except Exception:
-                raise IOError(f"Could not connect to '{self.ip}'.")
+                raise OSError(f"Could not connect to '{self.ip}'.")
 
     async def read_coils(self, address: int, count):
         """Read modbus output coils (0 address prefix)."""
         return await self._request('read_coils', address, count)
 
     async def read_registers(self, address: int, count):
         """Read modbus registers.
@@ -118,12 +127,14 @@
                     future = getattr(self.client.protocol, method)  # type: ignore
                 return await future(*args, **kwargs)
             except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException):
                 raise TimeoutError("Not connected to PLC.")
 
     async def _close(self):
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
         self.open = False
```

### Comparing `clickplc-0.7.0/clickplc.egg-info/PKG-INFO` & `clickplc-0.7.1/clickplc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python driver for Koyo Ethernet ClickPLCs.
-Home-page: http://github.com/numat/clickplc/
+Home-page: https://github.com/numat/clickplc/
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
@@ -17,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-clickplc [![Build Status](https://dev.azure.com/numat/NuMat/_apis/build/status/numat.clickplc?branchName=master)](https://dev.azure.com/numat/NuMat/_build/latest?definitionId=3&branchName=master)
+clickplc
 ========
 
 Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
```

### Comparing `clickplc-0.7.0/setup.py` & `clickplc-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 """Python driver for AutomationDirect (formerly Koyo) Ethernet ClickPLCs."""
-from sys import version_info
 
 from setuptools import setup
 
-if version_info < (3, 7):
-    raise ImportError("This module requires Python >=3.7.  Use 0.4.1 for Python3.6")
-
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name='clickplc',
-    version='0.7.0',
+    version='0.7.1',
     description="Python driver for Koyo Ethernet ClickPLCs.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='http://github.com/numat/clickplc/',
+    url='https://github.com/numat/clickplc/',
     author='Patrick Fuller',
     author_email='pat@numat-tech.com',
+    maintainer='Alex Ruddick',
+    maintainer_email='alex@numat-tech.com',
     packages=['clickplc'],
     entry_points={
         'console_scripts': [('clickplc = clickplc:command_line')]
     },
     install_requires=[
         'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.3.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'flake8>=3,<7',
-            'flake8-docstrings==1.*',
+            'mypy==1.3.0',
+            'ruff==0.0.270',
         ],
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
```

