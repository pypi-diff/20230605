# Comparing `tmp/fwhunt_scan-2.2.6.tar.gz` & `tmp/fwhunt_scan-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwhunt_scan-2.2.6.tar", last modified: Tue May  9 10:56:23 2023, max compression
+gzip compressed data, was "fwhunt_scan-2.3.0.tar", last modified: Mon Jun  5 17:51:58 2023, max compression
```

## Comparing `fwhunt_scan-2.2.6.tar` & `fwhunt_scan-2.3.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087656 fwhunt_scan-2.2.6/
--rw-r--r--   0 yv         (501) staff       (20)    35149 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.6/LICENSE
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-09 10:56:23.087706 fwhunt_scan-2.2.6/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)     3728 2023-03-17 22:44:15.000000 fwhunt_scan-2.2.6/README.md
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.086642 fwhunt_scan-2.2.6/fwhunt_scan/
--rw-r--r--   0 yv         (501) staff       (20)      615 2023-05-09 10:54:32.000000 fwhunt_scan-2.2.6/fwhunt_scan/__init__.py
--rw-r--r--   0 yv         (501) staff       (20)      362 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/__init__.pyi
--rw-r--r--   0 yv         (501) staff       (20)       64 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.6/fwhunt_scan/py.typed
--rw-r--r--   0 yv         (501) staff       (20)      817 2023-02-20 11:45:24.000000 fwhunt_scan-2.2.6/fwhunt_scan/test_internal.py
--rw-r--r--   0 yv         (501) staff       (20)    27487 2023-05-09 10:54:10.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     2686 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5237 2023-02-20 13:44:10.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_extractor.py
--rw-r--r--   0 yv         (501) staff       (20)   304114 2022-05-30 08:29:58.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.py
--rw-r--r--   0 yv         (501) staff       (20)      218 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.pyi
--rw-r--r--   0 yv         (501) staff       (20)    36316 2023-03-06 19:27:41.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.py
--rw-r--r--   0 yv         (501) staff       (20)     2634 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.pyi
--rw-r--r--   0 yv         (501) staff       (20)     9985 2022-09-20 15:07:51.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.py
--rw-r--r--   0 yv         (501) staff       (20)     1337 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_smm.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5596 2022-05-30 08:30:06.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.py
--rw-r--r--   0 yv         (501) staff       (20)      280 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3035 2022-07-27 15:10:58.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.py
--rw-r--r--   0 yv         (501) staff       (20)      727 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3875 2022-04-13 18:03:37.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.py
--rw-r--r--   0 yv         (501) staff       (20)     1596 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_types.pyi
--rw-r--r--   0 yv         (501) staff       (20)     2112 2022-07-15 12:35:57.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.py
--rw-r--r--   0 yv         (501) staff       (20)      418 2023-05-09 10:56:13.000000 fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.pyi
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087317 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)      888 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/SOURCES.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/dependency_links.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2022-05-30 08:58:37.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/not-zip-safe
--rw-r--r--   0 yv         (501) staff       (20)      127 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/requires.txt
--rw-r--r--   0 yv         (501) staff       (20)       12 2023-05-09 10:56:23.000000 fwhunt_scan-2.2.6/fwhunt_scan.egg-info/top_level.txt
--rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-08 17:59:45.000000 fwhunt_scan-2.2.6/fwhunt_scan_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     3860 2023-03-17 22:40:12.000000 fwhunt_scan-2.2.6/fwhunt_scan_docker.py
--rw-r--r--   0 yv         (501) staff       (20)      116 2023-05-09 10:56:23.087889 fwhunt_scan-2.2.6/setup.cfg
--rw-r--r--   0 yv         (501) staff       (20)     1408 2023-02-20 17:31:56.000000 fwhunt_scan-2.2.6/setup.py
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-09 10:56:23.087538 fwhunt_scan-2.2.6/test/
--rw-r--r--   0 yv         (501) staff       (20)     1208 2022-05-30 08:09:52.000000 fwhunt_scan-2.2.6/test/test.py
--rw-r--r--   0 yv         (501) staff       (20)      230 2022-08-03 15:21:16.000000 fwhunt_scan-2.2.6/test/test_variants.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.222045 fwhunt_scan-2.3.0/
+-rw-r--r--   0 yv         (501) staff       (20)    35149 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/LICENSE
+-rw-r--r--   0 yv         (501) staff       (20)     4411 2023-06-05 17:51:58.222085 fwhunt_scan-2.3.0/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)     3837 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/README.md
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221191 fwhunt_scan-2.3.0/fwhunt_scan/
+-rw-r--r--   0 yv         (501) staff       (20)      615 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/__init__.py
+-rw-r--r--   0 yv         (501) staff       (20)      362 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/__init__.pyi
+-rw-r--r--   0 yv         (501) staff       (20)       64 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/py.typed
+-rw-r--r--   0 yv         (501) staff       (20)      817 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/test_internal.py
+-rw-r--r--   0 yv         (501) staff       (20)    30184 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     2728 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5494 2023-05-09 12:22:20.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_extractor.py
+-rw-r--r--   0 yv         (501) staff       (20)   305195 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_protocols.py
+-rw-r--r--   0 yv         (501) staff       (20)    35819 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.py
+-rw-r--r--   0 yv         (501) staff       (20)     2592 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.pyi
+-rw-r--r--   0 yv         (501) staff       (20)    14733 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.py
+-rw-r--r--   0 yv         (501) staff       (20)     1430 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_smm.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5508 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.py
+-rw-r--r--   0 yv         (501) staff       (20)      280 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3035 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.py
+-rw-r--r--   0 yv         (501) staff       (20)      727 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     4277 2023-06-05 17:49:00.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.py
+-rw-r--r--   0 yv         (501) staff       (20)     1922 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_types.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     2112 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.py
+-rw-r--r--   0 yv         (501) staff       (20)      418 2023-06-05 17:51:41.000000 fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.pyi
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221781 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/
+-rw-r--r--   0 yv         (501) staff       (20)     4411 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)      857 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-06-05 12:35:02.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/not-zip-safe
+-rw-r--r--   0 yv         (501) staff       (20)      127 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/requires.txt
+-rw-r--r--   0 yv         (501) staff       (20)       12 2023-06-05 17:51:58.000000 fwhunt_scan-2.3.0/fwhunt_scan.egg-info/top_level.txt
+-rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-13 18:05:03.000000 fwhunt_scan-2.3.0/fwhunt_scan_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     3860 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/fwhunt_scan_docker.py
+-rw-r--r--   0 yv         (501) staff       (20)      116 2023-06-05 17:51:58.222247 fwhunt_scan-2.3.0/setup.cfg
+-rw-r--r--   0 yv         (501) staff       (20)     1408 2023-05-09 11:57:34.000000 fwhunt_scan-2.3.0/setup.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-06-05 17:51:58.221964 fwhunt_scan-2.3.0/test/
+-rw-r--r--   0 yv         (501) staff       (20)     1208 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.0/test/test.py
+-rw-r--r--   0 yv         (501) staff       (20)      230 2023-05-09 11:57:50.000000 fwhunt_scan-2.3.0/test/test_variants.py
```

### Comparing `fwhunt_scan-2.2.6/LICENSE` & `fwhunt_scan-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/PKG-INFO` & `fwhunt_scan-2.3.0/fwhunt_scan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fwhunt_scan
-Version: 2.2.6
+Name: fwhunt-scan
+Version: 2.3.0
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -24,28 +24,28 @@
 
 # FwHunt Community Scanner
 
 Tools for analyzing UEFI firmware and checking UEFI modules with [FwHunt rules](https://github.com/binarly-io/fwhunt).
 
 # Dependencies
 
-rizin (v0.4.1)
+rizin (v0.5.2)
 
 # Installation
 
 Install with `pip` (tested on `python3.6` and above):
 
 ```
 $ python -m pip install fwhunt-scan
 ```
 
 Install manually:
 
 ```
-$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt_scan
+$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt-scan
 $ python setup.py install
 ```
 
 # Example
 
 ### With script
 
@@ -68,14 +68,16 @@
 
 You can build a docker image locally as follows:
 
 ```
 docker build -t fwhunt_scan .
 ```
 
+Or pull the latest image from [ghcr](https://github.com/binarly-io/fwhunt-scan/pkgs/container/fwhunt-scan).
+
 Example of use:
 
 ```
 docker run --rm -it -v {module_path}:/tmp/image:ro \
   fwhunt_scan analyze-module /tmp/image # to analyze EFI module
 
 docker run --rm -it -v {module_path}:/tmp/image:ro -v {rule_path}:/tmp/rule.yml:ro \
```

### Comparing `fwhunt_scan-2.2.6/README.md` & `fwhunt_scan-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 # FwHunt Community Scanner
 
 Tools for analyzing UEFI firmware and checking UEFI modules with [FwHunt rules](https://github.com/binarly-io/fwhunt).
 
 # Dependencies
 
-rizin (v0.4.1)
+rizin (v0.5.2)
 
 # Installation
 
 Install with `pip` (tested on `python3.6` and above):
 
 ```
 $ python -m pip install fwhunt-scan
 ```
 
 Install manually:
 
 ```
-$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt_scan
+$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt-scan
 $ python setup.py install
 ```
 
 # Example
 
 ### With script
 
@@ -52,14 +52,16 @@
 
 You can build a docker image locally as follows:
 
 ```
 docker build -t fwhunt_scan .
 ```
 
+Or pull the latest image from [ghcr](https://github.com/binarly-io/fwhunt-scan/pkgs/container/fwhunt-scan).
+
 Example of use:
 
 ```
 docker run --rm -it -v {module_path}:/tmp/image:ro \
   fwhunt_scan analyze-module /tmp/image # to analyze EFI module
 
 docker run --rm -it -v {module_path}:/tmp/image:ro -v {rule_path}:/tmp/rule.yml:ro \
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/test_internal.py` & `fwhunt_scan-2.3.0/fwhunt_scan/test_internal.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # pylint: disable=too-few-public-methods,too-many-arguments,too-many-instance-attributes
 
 """
 Tools for analyzing UEFI firmware using radare2/rizin
 """
 
 import json
+import string
 import sys
 import uuid
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type
 
 import rzpipe
 
@@ -24,21 +25,21 @@
     EFI_RUNTIME_SERVICES_64_BIT,
     OFFSET_TO_SERVICE,
 )
 from fwhunt_scan.uefi_te import TerseExecutableError, TerseExecutableParser
 from fwhunt_scan.uefi_types import (
     ChildSwSmiHandler,
     NvramVariable,
-    SwSmiHandler,
+    SmiHandler,
     UefiGuid,
     UefiProtocol,
     UefiProtocolGuid,
     UefiService,
 )
-from fwhunt_scan.uefi_utils import get_int
+from fwhunt_scan.uefi_utils import get_current_insn_index, get_int
 
 if sys.version_info.major == 3 and sys.version_info.minor >= 8:
     from multiprocessing import shared_memory
 if sys.version_info.major == 3 and (
     sys.version_info.minor >= 6 and sys.version_info.minor < 8
 ):
     import shared_memory  # type: ignore # noqa: F811
@@ -118,16 +119,20 @@
         self._sections: Optional[List[Any]] = None
         self._functions: Optional[List[Any]] = None
         self._insns: Optional[List[Any]] = None
         self._g_bs: Optional[List[int]] = None
         self._g_rt: Optional[List[int]] = None
         self._smst_list: Optional[List[int]] = None
 
+        self._rt_filter_list: List[int] = list()
+        self._bs_filter_list: List[int] = list()
+        self._pei_filter_list: List[int] = list()
+
         # SMI handlers addresses
-        self._swsmi_handlers: Optional[List[SwSmiHandler]] = None
+        self._smi_handlers: Optional[List[SmiHandler]] = None
         self._child_swsmi_handlers: Optional[List[ChildSwSmiHandler]] = None
 
     def __enter__(self):
         return self
 
     def _section_paddr(self, section_name: str) -> int:
         for section in self.sections:
@@ -211,19 +216,17 @@
 
         if self._functions is None:
             self._functions = self._rz.cmdj("aflj") or []
         return self._functions
 
     def _get_insns(self) -> List[Any]:
         insns = list()
-        target_sections = [".text"]
-        for section in self.sections:
-            if section["name"] in target_sections:
-                self._rz.cmd("s {:#x}".format(section["vaddr"]))
-                insns = self._rz.cmdj("pDj {:#x}".format(section["vsize"]))
+        for function in self.functions:
+            self._rz.cmd("s {:#x}".format(function["offset"]))
+            insns += self._rz.cmdj("pDj {:#x}".format(function["size"]))
         return insns
 
     @property
     def insns(self) -> List[Any]:
         """Get instructions"""
 
         if self._insns is None:
@@ -329,69 +332,72 @@
             # if current instriction is "mov rax, qword [g_bs]"
             index = self.insns.index(insn)
             for g_bs_area_insn in self.insns[index : index + 0x10]:
                 if "esil" not in g_bs_area_insn.keys():
                     continue
                 g_bs_area_esil = g_bs_area_insn["esil"].split(",")
                 if not (
-                    (g_bs_area_insn["type"] == "ucall")
+                    (g_bs_area_insn["type"] in ["ucall", "ircall", "ujmp", "irjmp"])
                     and (g_bs_area_esil[1] == "rax")
                     and (g_bs_area_esil[2] == "+")
                     and (g_bs_area_esil[3] == "[8]")
                     and (g_bs_area_esil[-1] == "=")
                 ):
                     continue
                 if "ptr" not in g_bs_area_insn:
                     continue
                 service_offset = g_bs_area_insn["ptr"]
                 if service_offset in EFI_BOOT_SERVICES_64_BIT:
                     if g_bs_area_insn["offset"] in addrs:
                         break
-                    bs_list.append(
-                        UefiService(
-                            address=g_bs_area_insn["offset"],
-                            name=EFI_BOOT_SERVICES_64_BIT[service_offset],
+                    if g_bs_area_insn["offset"] not in self._bs_filter_list:
+                        bs_list.append(
+                            UefiService(
+                                address=g_bs_area_insn["offset"],
+                                name=EFI_BOOT_SERVICES_64_BIT[service_offset],
+                            )
                         )
-                    )
+                        self._bs_filter_list.append(g_bs_area_insn["offset"])
                     break
 
         return bs_list
 
     def _get_boot_services_prot_64bit(self) -> List[UefiService]:
         bs_prot: List[UefiService] = list()
 
         for insn in self.insns:
             if "esil" not in insn:
                 continue
             esil = insn["esil"].split(",")
             if not (
-                (insn["type"] == "ucall")
+                (insn["type"] in ["ucall", "ircall", "ujmp", "irjmp"])
                 and (esil[1] == "rax")
                 and (esil[2] == "+")
                 and (esil[3] == "[8]")
             ):
                 continue
             if "ptr" not in insn:
                 continue
             service_offset = insn["ptr"]
             if service_offset in OFFSET_TO_SERVICE:
                 name = OFFSET_TO_SERVICE[service_offset]
                 # found boot service that work with protocol
-                bs_prot.append(UefiService(address=insn["offset"], name=name))
-
+                if insn["offset"] not in self._bs_filter_list:
+                    bs_prot.append(UefiService(address=insn["offset"], name=name))
+                    self._bs_filter_list.append(insn["offset"])
         return bs_prot
 
     @property
     def boot_services(self) -> List[UefiService]:
         """Find boot services using g_bs"""
 
-        if self._bs_list_g_bs is None:
-            self._bs_list_g_bs = self._get_boot_services_bs_64bit()
         if self._bs_prot is None:
             self._bs_prot = self._get_boot_services_prot_64bit()
+        if self._bs_list_g_bs is None:
+            self._bs_list_g_bs = self._get_boot_services_bs_64bit()
         return self._bs_list_g_bs + self._bs_prot
 
     @property
     def boot_services_protocols(self) -> List[Any]:
         """Find boot service that work with protocols"""
 
         if self._bs_prot is None:
@@ -421,31 +427,33 @@
             if not found:
                 continue
 
             index = self.insns.index(insn)
             for g_rt_area_insn in self.insns[index : index + 0x10]:
                 g_rt_area_esil = g_rt_area_insn["esil"].split(",")
                 if not (
-                    (g_rt_area_insn["type"] == "ucall")
+                    (g_rt_area_insn["type"] in ["ucall", "ircall", "ujmp", "irjmp"])
                     and (g_rt_area_esil[1] == "rax")
                     and (g_rt_area_esil[2] == "+")
                     and (g_rt_area_esil[3] == "[8]")
                     and (g_rt_area_esil[-1] == "=")
                 ):
                     continue
                 if "ptr" not in g_rt_area_insn:
                     continue
                 service_offset = g_rt_area_insn["ptr"]
                 if service_offset in EFI_RUNTIME_SERVICES_64_BIT:
-                    rt_list.append(
-                        UefiService(
-                            address=g_rt_area_insn["offset"],
-                            name=EFI_RUNTIME_SERVICES_64_BIT[service_offset],
+                    if g_rt_area_insn["offset"] not in self._rt_filter_list:
+                        rt_list.append(
+                            UefiService(
+                                address=g_rt_area_insn["offset"],
+                                name=EFI_RUNTIME_SERVICES_64_BIT[service_offset],
+                            )
                         )
-                    )
+                        self._rt_filter_list.append(g_rt_area_insn["offset"])
                     break
         return rt_list
 
     @property
     def runtime_services(self) -> List[UefiService]:
         """Find all runtime services"""
 
@@ -478,15 +486,15 @@
                     p_guid_b = bytes(self._rz.cmdj("xj 16"))
 
                     # look up in known list
                     guid = GUID_FROM_BYTES.get(p_guid_b)
                     if not guid:
                         guid = UefiGuid(
                             value=str(uuid.UUID(bytes_le=p_guid_b)).upper(),
-                            name="proprietary_protocol",
+                            name="UNKNOWN_PROTOCOL",
                         )
 
                     protocols.append(
                         UefiProtocol(
                             name=guid.name,
                             value=guid.value,
                             guid_address=p_guid_addr,
@@ -533,53 +541,123 @@
     def protocol_guids(self) -> List[UefiProtocolGuid]:
         """Find protocols GUIDs"""
 
         if self._protocol_guids is None:
             self._protocol_guids = self._get_protocol_guids()
         return self._protocol_guids
 
+    @staticmethod
+    def _name_is_valid(name: str) -> bool:
+        for c in name:
+            if c not in string.printable:
+                return False
+        return True
+
     def r2_get_nvram_vars_64bit(self) -> List[NvramVariable]:
+        # to fix FPs need to apply filtering
+        # of the extracted Runtime Services (from self.runtime_services)
+
         nvram_vars = list()
         for service in self.runtime_services:
-            if service.name in ["GetVariable", "SetVariable"]:
-                # disassemble 16 instructions backward
-                block_insns = self._rz.cmdj("pdj -16 @ {:#x}".format(service.address))
-                name: str = str()
-                p_guid_b: bytes = bytes()
-                for index in range(len(block_insns) - 2, -1, -1):
-                    if "xrefs_from" not in block_insns[index]:
-                        continue
-                    ref_addr = block_insns[index]["xrefs_from"][0]["addr"]
-                    if "esil" not in block_insns[index]:
-                        continue
-                    esil = block_insns[index]["esil"].split(",")
-                    if (
-                        (esil[-1] == "=")
-                        and (esil[-2] == "rcx")
-                        and (esil[-3] == "+")
-                        and (esil[-4] == "rip")
-                    ):
-                        name = self._rz.cmd("psw @ {:#x}".format(ref_addr))[:-1]
-                    if (
-                        (esil[-1] == "=")
-                        and (esil[-2] == "rdx")
-                        and (esil[-3] == "+")
-                        and (esil[-4] == "rip")
-                    ):
-                        p_guid_b = bytes(
-                            self._rz.cmdj("xj 16 @ {:#x}".format(ref_addr))
-                        )
-                    if not name:
-                        name = "Unknown"
-                    if p_guid_b:
-                        guid = str(uuid.UUID(bytes_le=p_guid_b)).upper()
-                        nvram_vars.append(
-                            NvramVariable(name=name, guid=guid, service=service)
-                        )
-                        break
+            if service.name not in ["GetVariable", "SetVariable"]:
+                continue
+
+            # disassemble current function
+            func_insns = self._rz.cmdj("pdfj @ {:#x}".format(service.address))
+            if "ops" not in func_insns:
+                continue
+
+            insns = func_insns["ops"]
+            index = get_current_insn_index(insns, service.address)
+            if index is None:
+                continue
+
+            name: Optional[str] = None
+            name_addr_reg: Optional[str] = None
+            p_guid_b: Optional[bytes] = None
+            stack_guid: bool = False
+            for i in range(index - 1, -1, -1):
+                insn = insns[i]
+                if name is not None and p_guid_b is not None:
+                    break
+
+                if "esil" not in insn:
+                    continue
+                esil = insn["esil"].split(",")
+
+                # handle case when we have:
+                # NAME_ADDR,rip,+,REG,=
+                # REG,rcx,=
+                if (
+                    name is None
+                    and name_addr_reg is None
+                    and len(esil) == 3
+                    and (esil[-1] == "=" and esil[-2] == "rcx")
+                ):
+                    name_addr_reg = esil[0]
+
+                ptr = insn.get("ptr", None)
+                if ptr is None:
+                    continue
+
+                if (
+                    name is None
+                    and name_addr_reg
+                    and len(esil) == 5
+                    and esil[-1] == "="
+                    and esil[-2] == name_addr_reg
+                    and esil[-3] == "+"
+                    and esil[-4] == "rip"
+                ):
+                    tmp_name = self._rz.cmd("psw @ {:#x}".format(ptr))[:-1]
+                    if UefiAnalyzer._name_is_valid(tmp_name):
+                        name = tmp_name
+
+                if (
+                    name is None
+                    and len(esil) == 5
+                    and (esil[-1] == "=")
+                    and (esil[-2] == "rcx")
+                    and (esil[-3] == "+")
+                    and (esil[-4] == "rip")
+                ):
+                    tmp_name = self._rz.cmd("psw @ {:#x}".format(ptr))[:-1]
+                    if UefiAnalyzer._name_is_valid(tmp_name):
+                        name = tmp_name
+
+                if (
+                    p_guid_b is None
+                    and len(esil) == 5
+                    and (esil[-1] == "=")
+                    and (esil[-2] == "rdx")
+                    and (esil[-4] in ["rsp", "rbp"])
+                ):
+                    stack_guid = True
+
+                if (
+                    not stack_guid
+                    and p_guid_b is None
+                    and len(esil) == 5
+                    and (esil[-1] == "=")
+                    and (esil[-2] == "rdx")
+                    and (esil[-3] == "+")
+                    and (esil[-4] == "rip")
+                ):
+                    p_guid_b = bytes(self._rz.cmdj("xj 16 @ {:#x}".format(ptr)))
+
+            if not name:
+                name = "Unknown"
+
+            if p_guid_b is not None:
+                guid = str(uuid.UUID(bytes_le=p_guid_b)).upper()
+            else:
+                guid = "Unknown"
+
+            nvram_vars.append(NvramVariable(name=name, guid=guid, service=service))
+
         return nvram_vars
 
     @property
     def nvram_vars(self) -> List[NvramVariable]:
         """Find NVRAM variables passed to GetVariable and SetVariable services"""
 
         if self._nvram_vars is None:
@@ -606,17 +684,19 @@
 
                     # found potential pei service, compare number of arguments
                     arg_num: Any = self._pei_service_args_num(reg, insn["offset"])
                     if arg_num < service["arg_num"]:
                         continue
 
                     # wrong addresses in r2 in case of TE
-                    pei_list.append(
-                        UefiService(address=insn["offset"], name=service["name"])
-                    )
+                    if insn["offset"] not in self._pei_filter_list:
+                        pei_list.append(
+                            UefiService(address=insn["offset"], name=service["name"])
+                        )
+                        self._pei_filter_list.append(insn["offset"])
 
         return pei_list
 
     @property
     def pei_services(self) -> List[UefiService]:
         """Find all PEI services"""
 
@@ -669,20 +749,20 @@
         """Find all PPIs"""
 
         if self._ppi_list is None:
             self._ppi_list = self._get_ppi_list()
         return self._ppi_list
 
     @property
-    def swsmi_handlers(self) -> List[SwSmiHandler]:
+    def smi_handlers(self) -> List[SmiHandler]:
         """Find software SMI handlers"""
 
-        if self._swsmi_handlers is None:
-            self._swsmi_handlers = uefi_smm.get_sw_smi_handlers(self._rz)
-        return self._swsmi_handlers
+        if self._smi_handlers is None:
+            self._smi_handlers = uefi_smm.get_smi_handlers(self._rz)
+        return self._smi_handlers
 
     @property
     def child_swsmi_handlers(self) -> List[ChildSwSmiHandler]:
         """Find child software SMI handlers"""
 
         if self._child_swsmi_handlers is None:
             self._child_swsmi_handlers = uefi_smm.get_child_sw_smi_handlers(
@@ -719,21 +799,21 @@
             summary["pei_list"] = [x.__dict__ for x in self.pei_services]
             summary["ppi_list"] = [x.__dict__ for x in self.ppi_list]
             summary["nvram_vars"] = [x.__dict__ for x in self.nvram_vars]
 
         elif self.info["bin"]["arch"] == "x86" and self.info["bin"]["bits"] == 64:
             summary["g_bs"] = self.g_bs
             summary["g_rt"] = self.g_rt
-            summary["g_smst"] = [x for x in self.smst_list]
+            summary["g_smst"] = self.smst_list
             summary["bs_list"] = [x.__dict__ for x in self.boot_services]
             summary["rt_list"] = [x.__dict__ for x in self.runtime_services]
             summary["protocols"] = [x.__dict__ for x in self.protocols]
             summary["nvram_vars"] = [x.__dict__ for x in self.nvram_vars]
-            if len(self.swsmi_handlers) > 0:
-                summary["swsmi_handlers"] = [x.__dict__ for x in self.swsmi_handlers]
+            if len(self.smi_handlers) > 0:
+                summary["smi_handlers"] = [x.__dict__ for x in self.smi_handlers]
             if len(self.child_swsmi_handlers) > 0:
                 summary["child_swsmi_handlers"] = [
                     x.__dict__ for x in self.child_swsmi_handlers
                 ]
 
         summary["p_guids"] = [x.__dict__ for x in self.protocol_guids]
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_analyzer.pyi` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_analyzer.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from _typeshed import Incomplete
 from fwhunt_scan.uefi_protocols import GUID_FROM_BYTES as GUID_FROM_BYTES
 from fwhunt_scan.uefi_tables import BS_PROTOCOLS_INFO_64_BIT as BS_PROTOCOLS_INFO_64_BIT, EFI_BOOT_SERVICES_64_BIT as EFI_BOOT_SERVICES_64_BIT, EFI_PEI_SERVICES_32_BIT as EFI_PEI_SERVICES_32_BIT, EFI_RUNTIME_SERVICES_64_BIT as EFI_RUNTIME_SERVICES_64_BIT, OFFSET_TO_SERVICE as OFFSET_TO_SERVICE
 from fwhunt_scan.uefi_te import TerseExecutableError as TerseExecutableError, TerseExecutableParser as TerseExecutableParser
-from fwhunt_scan.uefi_types import ChildSwSmiHandler as ChildSwSmiHandler, NvramVariable as NvramVariable, SwSmiHandler as SwSmiHandler, UefiGuid as UefiGuid, UefiProtocol as UefiProtocol, UefiProtocolGuid as UefiProtocolGuid, UefiService as UefiService
-from fwhunt_scan.uefi_utils import get_int as get_int
+from fwhunt_scan.uefi_types import ChildSwSmiHandler as ChildSwSmiHandler, NvramVariable as NvramVariable, SmiHandler as SmiHandler, UefiGuid as UefiGuid, UefiProtocol as UefiProtocol, UefiProtocolGuid as UefiProtocolGuid, UefiService as UefiService
+from fwhunt_scan.uefi_utils import get_current_insn_index as get_current_insn_index, get_int as get_int
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type
 
 class UefiAnalyzerError(Exception):
     value: Incomplete
     def __init__(self, value: str) -> None: ...
 
@@ -42,15 +42,15 @@
     @property
     def nvram_vars(self) -> List[NvramVariable]: ...
     @property
     def pei_services(self) -> List[UefiService]: ...
     @property
     def ppi_list(self) -> List[UefiProtocol]: ...
     @property
-    def swsmi_handlers(self) -> List[SwSmiHandler]: ...
+    def smi_handlers(self) -> List[SmiHandler]: ...
     @property
     def child_swsmi_handlers(self) -> List[ChildSwSmiHandler]: ...
     @property
     def smst_list(self) -> List[int]: ...
     def get_summary(self) -> Dict[str, Any]: ...
     def get_protocols_info(self) -> Dict[str, Any]: ...
     def close(self) -> None: ...
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_extractor.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import contextlib
+import os
 from typing import Any, Dict, List, Optional
 
 import uefi_firmware
 
 
 class UefiBinary:
     def __init__(
@@ -118,20 +120,23 @@
         for parser in self._parsers:
             firmware = parser.parse()
             self._append_binaries(firmware)
 
         return True
 
     def extract_all(self, ignore_guid: bool = False) -> None:
-        self._extract()
-        for guid in self._info:
-            if ignore_guid or (
-                self._info[guid]["content"] is not None and (guid in self._file_guids)
-            ):
-                self.binaries.append(
-                    UefiBinary(
-                        content=self._info[guid]["content"],
-                        name=self._info[guid]["name"],
-                        guid=guid,
-                        ext=self._info[guid]["ext"],
-                    )
-                )
+        with open(os.devnull, "w") as devnull:
+            with contextlib.redirect_stderr(devnull):
+                self._extract()
+                for guid in self._info:
+                    if ignore_guid or (
+                        self._info[guid]["content"] is not None
+                        and (guid in self._file_guids)
+                    ):
+                        self.binaries.append(
+                            UefiBinary(
+                                content=self._info[guid]["content"],
+                                name=self._info[guid]["name"],
+                                guid=guid,
+                                ext=self._info[guid]["ext"],
+                            )
+                        )
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_protocols.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -6406,14 +6406,18 @@
         "B709EFA0-47A6-4B41-B93112ECE7A8EE56",
         name="EFI_SMM_POWER_BUTTON_DISPATCH_PROTOCOL_GUID",
     ),
     UefiGuid(
         "C50B323E-9075-4F2A-AC8ED2596A1085CC",
         name="EFI_SMM_ICHN_DISPATCH_PROTOCOL_GUID",
     ),
+    UefiGuid(
+        "ADF3A128-416D-4060-8DDF-30A1D7AAB699",
+        name="EFI_SMM_ICHN_DISPATCH2_PROTOCOL_GUID",
+    ),
     UefiGuid("5F439A0B-45D8-4682-A4F4F0576B513441", name="EFI_SMM_CPU_IO_GUID"),
     UefiGuid(
         "F3E4543D-CF35-6CEF-35C44FE6344DFC54", name="EFI_FORM_CALLBACK_PROTOCOL_GUID"
     ),
     UefiGuid(
         "E5A1333E-E1B4-4D55-CEEB35C3EF133443", name="EFI_FORM_BROWSER_PROTOCOL_GUID"
     ),
@@ -6883,14 +6887,45 @@
         "03FDF171-1D67-4ACE-A9043E36D338FA74", name="SE_C_PLATFORM_READY_TO_BOOT_GUID"
     ),
     UefiGuid("40B09B5A-F0EF-4627-93D527F04B754D05", name="AMT_READY_TO_BOOT_GUID"),
     UefiGuid("10BA6BBE-A97E-41C3-9A07607AD9BD60E5", name="EFI_VLV2_VARIABLE_GUID"),
     UefiGuid(
         "BFD02359-8DFE-459A-8B69-A73A6BAFADC0", name="LENOVO_VARIABLE_PROTOCOL_GUID"
     ),
+    UefiGuid(
+        "9E71D609-6D24-47FD-B572-6140F8D9C2A4",
+        name="PCH_TCO_SMI_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "3e7d2b56-3f47-42aa-8f6b-22f519818dab",
+        name="PCH_PCIE_SMI_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "d52bb262-f022-49ec-86d2-7a293a7a054b",
+        name="PCH_ACPI_SMI_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "83339ef7-9392-4716-8d3a-d1fc67cd55db",
+        name="PCH_GPIO_UNLOCK_SMI_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "e6a81bbf-873d-47fd-b6be-61b3e5720993", name="PCH_SMI_DISPATCH_PROTOCOL_GUID"
+    ),
+    UefiGuid(
+        "b3c14ff3-bae8-456c-8631-27fe0ceb340c",
+        name="PCH_ESPI_SMI_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "bd88ec68-ebe4-4f7b-935a-4f666642e75f",
+        name="EFI_ACPI_EN_DISPATCH_PROTOCOL_GUID",
+    ),
+    UefiGuid(
+        "9c939ba6-1fcc-46f6-b4e1-102dbe186567",
+        name="EFI_ACPI_DIS_DISPATCH_PROTOCOL_GUID",
+    ),
 ]
 
 GUID_FROM_VALUE: Dict[str, UefiGuid] = dict(
     [(guid.value, guid) for guid in PROTOCOLS_GUIDS]
 )
 GUID_FROM_BYTES: Dict[bytes, UefiGuid] = dict(
     [(guid.bytes, guid) for guid in PROTOCOLS_GUIDS]
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,28 +22,23 @@
 
 class CodePattern:
     """Code pattern"""
 
     def __init__(self, pattern: str, place: Optional[str]) -> None:
         self.pattern: str = str(pattern)
         self.place: Optional[str] = place
-
-        # if True, scan in all SW SMI handlers
-        self.sw_smi_handlers: bool = place == "sw_smi_handlers"
-
-        # if True, scan in all child SW SMI handlers
-        self.child_sw_smi_handlers: bool = place == "child_sw_smi_handlers"
+        # if True, scan the whole binary
+        self.unspecified: bool = place is None
 
     @property
     def __dict__(self):
         return dict(
             {
                 "pattern": self.pattern,
-                "sw_smi_handlers": self.sw_smi_handlers,
-                "child_sw_smi_handlers": self.child_sw_smi_handlers,
+                "unspecified": self.unspecified,
             }
         )
 
 
 class UefiRuleVariant:
     """A rule for scanning EFI image (content without meta and variants)"""
 
@@ -490,15 +485,15 @@
         self._valid_rules: bool = self._check_rules()
         if not self._valid_rules:
             raise UefiScannerError(
                 "Invalid rule format. Visit https://github.com/binarly-io/FwHunt to find the latest version of the rules format."
             )
         self._results: Optional[List[UefiScannerRes]] = None
 
-    def _check_rule(self, rule: UefiRule):
+    def _check_rule(self, rule: UefiRule) -> bool:
         variants: Optional[Dict[str, UefiRuleVariant]] = None
         try:
             variants = rule.variants
         except KeyError:
             return False
 
         if not isinstance(variants, dict):
@@ -508,15 +503,15 @@
             if not isinstance(label, str):
                 return False
             if not isinstance(variants[label], UefiRuleVariant):
                 return False
 
         return True
 
-    def _check_rules(self):
+    def _check_rules(self) -> bool:
         for rule in self._uefi_rules:
             if not self._check_rule(rule):
                 return False
         return True
 
     def _and_strings(self, strings: List[str]) -> bool:
         res = True
@@ -595,15 +590,14 @@
         return res
 
     def _strings_scanner(self, rule_strings: Dict[str, List[str]]) -> bool:
         """Match strings"""
 
         final_res = True
         for op in rule_strings:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -628,15 +622,14 @@
     def _wide_strings_scanner(
         self, rule_wide_strings: Dict[str, List[Dict[str, str]]]
     ) -> bool:
         """Match wide strings"""
 
         final_res = True
         for op in rule_wide_strings:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -659,15 +652,14 @@
         return final_res
 
     def _hex_strings_scanner(self, rule_hex_strings: Dict[str, List[str]]) -> bool:
         """Match hex strings"""
 
         final_res = True
         for op in rule_hex_strings:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -716,15 +708,14 @@
         return res
 
     def _compare_nvram_vars(self, rule_nvram: Dict[str, List[NvramVariable]]) -> bool:
         """Compare NVRAM variables"""
 
         final_res = True
         for op in rule_nvram:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -778,15 +769,14 @@
     def _compare_protocols(
         self, rule_protocol: Dict[str, List[UefiProtocol]], mode: int
     ) -> bool:
         """Compare protocols"""
 
         final_res = True
         for op in rule_protocol:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -833,15 +823,14 @@
         return res
 
     def _compare_guids(self, rule_guid: Dict[str, List[UefiGuid]]) -> bool:
         """Compare GUIDs"""
 
         final_res = True
         for op in rule_guid:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
@@ -965,79 +954,72 @@
         return False
 
     def _clear_cache(self) -> None:
         self._funcs_bounds: List[Any] = list()
         self._rec_addrs: List[Any] = list()
 
     def _code_scan_rec(self, address: int, pattern: str) -> bool:
-
         self._clear_cache()
 
         self._get_bounds_rec(address, depth=0, debug=False)
         if not len(self._funcs_bounds):
             return False
 
         for start, end in self._funcs_bounds:
             if self._hex_strings_scanner_bounds(pattern, start, end):
                 # Debug
                 # print(f"Matched: {start:#x} - {end:#x}")
                 return True
 
         return False
 
+    def _get_handlers(self, c: CodePattern) -> List[Any]:
+        if c.place == "child_sw_smi_handlers":
+            return self._uefi_analyzer.child_swsmi_handlers
+        if c.place == "smi_handlers":
+            return self._uefi_analyzer.smi_handlers
+        return [
+            handler
+            for handler in self._uefi_analyzer.smi_handlers
+            if handler.place == c.place
+        ]
+
+    def _single_code_scan(self, c: CodePattern) -> bool:
+        search_res = False
+        if c.unspecified:
+            return not not self._uefi_analyzer._rz.cmdj("/xj {}".format(c.pattern))
+        for handler in self._get_handlers(c):
+            search_res = self._code_scan_rec(handler.address, c.pattern)
+            if search_res:
+                break
+        return search_res
+
     def _and_code(self, cs: List[CodePattern]) -> bool:
         res = True
         for c in cs:
-            handlers: Optional[List[Any]] = None
-            if c.sw_smi_handlers:
-                handlers = self._uefi_analyzer.swsmi_handlers
-            elif c.child_sw_smi_handlers:
-                handlers = self._uefi_analyzer.child_swsmi_handlers
-            else:
-                raise UefiScannerError("The search place is incorrect")
-            search_res = False
-            for handler in handlers:
-                search_res = self._code_scan_rec(handler.address, c.pattern)
-                if search_res:
-                    break
-
-            res &= search_res
+            res &= self._single_code_scan(c)
             if not res:
                 break
 
         return res
 
     def _or_code(self, cs: List[CodePattern]) -> bool:
         res = False
         for c in cs:
-            handlers: Optional[List[Any]] = None
-            if c.sw_smi_handlers:
-                handlers = self._uefi_analyzer.swsmi_handlers
-            elif c.child_sw_smi_handlers:
-                handlers = self._uefi_analyzer.child_swsmi_handlers
-            else:
-                raise UefiScannerError("The search place is incorrect")
-            search_res = False
-            for handler in handlers:
-                search_res = self._code_scan_rec(handler.address, c.pattern)
-                if search_res:
-                    break
-
-            res |= search_res
+            res |= self._single_code_scan(c)
             if res:
                 break
 
         return res
 
     def _code_scanner(self, rule_code: Dict[str, List[CodePattern]]) -> bool:
         """Compare code patterns"""
 
         final_res = True
         for op in rule_code:
-
             # check kind of matches
             if op not in ["and", "or", "not-any", "not-all"]:
                 raise UefiScannerError(
                     f"Invalid kind of matches: {op} (possible kinds of matches: and, or, not-any, not-all)"
                 )
 
             res = True
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_scanner.pyi` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_scanner.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from _typeshed import Incomplete
 from fwhunt_scan.uefi_analyzer import NvramVariable as NvramVariable, UefiAnalyzer as UefiAnalyzer, UefiGuid as UefiGuid, UefiProtocol as UefiProtocol, UefiService as UefiService
 from typing import Any, Dict, List, Optional
 
 class CodePattern:
     pattern: Incomplete
     place: Incomplete
-    sw_smi_handlers: Incomplete
-    child_sw_smi_handlers: Incomplete
+    unspecified: Incomplete
     def __init__(self, pattern: str, place: Optional[str]) -> None: ...
     @property
     def __dict__(self): ...
 
 class UefiRuleVariant:
     def __init__(self, rule_content: Dict[str, Any]) -> None: ...
     @property
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_tables.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 # SPDX-License-Identifier: GPL-3.0+
 #
 # pylint: disable=consider-using-dict-comprehension
 
-"""
-Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
-"""
-
-
 EFI_BOOT_SERVICES_64_BIT = {
     0x00000018: "RaiseTPL",
     0x00000020: "RestoreTPL",
     0x00000028: "AllocatePages",
     0x00000030: "FreePages",
     0x00000038: "GetMemoryMap",
     0x00000040: "AllocatePool",
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_te.pyi` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_te.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan/uefi_utils.py` & `fwhunt_scan-2.3.0/fwhunt_scan/uefi_utils.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan.egg-info/PKG-INFO` & `fwhunt_scan-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fwhunt-scan
-Version: 2.2.6
+Name: fwhunt_scan
+Version: 2.3.0
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -24,28 +24,28 @@
 
 # FwHunt Community Scanner
 
 Tools for analyzing UEFI firmware and checking UEFI modules with [FwHunt rules](https://github.com/binarly-io/fwhunt).
 
 # Dependencies
 
-rizin (v0.4.1)
+rizin (v0.5.2)
 
 # Installation
 
 Install with `pip` (tested on `python3.6` and above):
 
 ```
 $ python -m pip install fwhunt-scan
 ```
 
 Install manually:
 
 ```
-$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt_scan
+$ git clone https://github.com/binarly-io/fwhunt-scan.git && cd fwhunt-scan
 $ python setup.py install
 ```
 
 # Example
 
 ### With script
 
@@ -68,14 +68,16 @@
 
 You can build a docker image locally as follows:
 
 ```
 docker build -t fwhunt_scan .
 ```
 
+Or pull the latest image from [ghcr](https://github.com/binarly-io/fwhunt-scan/pkgs/container/fwhunt-scan).
+
 Example of use:
 
 ```
 docker run --rm -it -v {module_path}:/tmp/image:ro \
   fwhunt_scan analyze-module /tmp/image # to analyze EFI module
 
 docker run --rm -it -v {module_path}:/tmp/image:ro -v {rule_path}:/tmp/rule.yml:ro \
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan.egg-info/SOURCES.txt` & `fwhunt_scan-2.3.0/fwhunt_scan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 fwhunt_scan/__init__.pyi
 fwhunt_scan/py.typed
 fwhunt_scan/test_internal.py
 fwhunt_scan/uefi_analyzer.py
 fwhunt_scan/uefi_analyzer.pyi
 fwhunt_scan/uefi_extractor.py
 fwhunt_scan/uefi_protocols.py
-fwhunt_scan/uefi_protocols.pyi
 fwhunt_scan/uefi_scanner.py
 fwhunt_scan/uefi_scanner.pyi
 fwhunt_scan/uefi_smm.py
 fwhunt_scan/uefi_smm.pyi
 fwhunt_scan/uefi_tables.py
 fwhunt_scan/uefi_tables.pyi
 fwhunt_scan/uefi_te.py
```

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan_analyzer.py` & `fwhunt_scan-2.3.0/fwhunt_scan_analyzer.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/fwhunt_scan_docker.py` & `fwhunt_scan-2.3.0/fwhunt_scan_docker.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/setup.py` & `fwhunt_scan-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.6/test/test.py` & `fwhunt_scan-2.3.0/test/test.py`

 * *Files identical despite different names*

