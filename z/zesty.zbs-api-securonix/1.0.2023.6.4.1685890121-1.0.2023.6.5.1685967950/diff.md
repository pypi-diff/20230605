# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar", last modified: Sun Jun  4 14:48:41 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar", last modified: Mon Jun  5 12:25:51 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13458 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    12497 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7199 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13458 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    12497 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.4.1685890121
+Version: 1.0.2023.6.5.1685967950
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/README.md` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/step_instructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             and self.dev_iops is None \
             and self.dev_throughput is None:
             raise Exception(f"Must modify at least one attribute")
 
 
 @dataclass
 class DetachDiskCloud(CloudInstruction):
-    dev_id: str
+    volume_id: str
 
 
 @dataclass
 class TakeSnapshotCloud(CloudInstruction):
     dev_id: str
     snapshot_id: str
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.4.1685890121
+Version: 1.0.2023.6.5.1685967950
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

