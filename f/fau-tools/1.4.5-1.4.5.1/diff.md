# Comparing `tmp/fau_tools-1.4.5.tar.gz` & `tmp/fau_tools-1.4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fau_tools-1.4.5.tar", max compression
+gzip compressed data, was "fau_tools-1.4.5.1.tar", max compression
```

## Comparing `fau_tools-1.4.5.tar` & `fau_tools-1.4.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.5/Fau_tools/__init__.py
--rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.5/Fau_tools/data_structure/__init__.py
--rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.5/Fau_tools/data_structure/data_structure.py
--rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.5/Fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.5/Fau_tools/torch_tools/__init__.py
--rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.5/Fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.5/Fau_tools/torch_tools/torch_tools.pyi
--rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.5/Fau_tools/utility/__init__.py
--rw-r--r--   0        0        0    10983 2023-06-05 09:17:34.068974 fau_tools-1.4.5/Fau_tools/utility/utility.py
--rw-r--r--   0        0        0      823 2023-06-05 07:21:12.849504 fau_tools-1.4.5/Fau_tools/utility/utility.pyi
--rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.5/README.md
--rw-r--r--   0        0        0     1148 2023-06-05 09:18:53.893648 fau_tools-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 fau_tools-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.5.1/Fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.5.1/Fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.5.1/Fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.5.1/Fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0    10983 2023-06-05 09:17:34.068974 fau_tools-1.4.5.1/Fau_tools/utility/utility.py
+-rw-r--r--   0        0        0     1008 2023-06-05 09:23:30.478542 fau_tools-1.4.5.1/Fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.5.1/README.md
+-rw-r--r--   0        0        0     1150 2023-06-05 09:21:13.564634 fau_tools-1.4.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.5.1/PKG-INFO
```

### Comparing `fau_tools-1.4.5/Fau_tools/data_structure/data_structure.py` & `fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/Fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.4.5.1/Fau_tools/data_structure/data_structure.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/Fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/Fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.4.5.1/Fau_tools/torch_tools/torch_tools.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/Fau_tools/utility/utility.py` & `fau_tools-1.4.5.1/Fau_tools/utility/utility.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/Fau_tools/utility/utility.pyi` & `fau_tools-1.4.5.1/Fau_tools/utility/utility.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 def calc_time(function): ...
 
 def time_to_human(time: float|int) -> str: ...
 
 # def show_progress(now: int, total: int, time_manager: TimeManager=None, length: int=30, icons: str='█ ') -> None: ...
 
 def cprint(*values: *object, color: str='red', show: bool=True, sep: str=' ', end: str='\n', **kwargs) -> str: ...
-
+def custom_notify(title: str, content: str, title_color: str, content_color: str, show: bool=True): ...
+def notify(title: str, content: str, level: str|int="info", show: bool=True): ...
 
 def __get_value_in_height_and_width(value: tuple[int, int]|int, value_name: str) -> tuple[int, int]: ...
 
 def _calc_value_after_layer(x: int, k_size: int, stride: int, padding: int) -> int: ...
 
 def calc_feature_size(channel: int, height: int, width: int, sequential: torch.nn.Sequential) -> int: ...
```

### Comparing `fau_tools-1.4.5/README.md` & `fau_tools-1.4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.5/pyproject.toml` & `fau_tools-1.4.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 reportUnusedExpression  = false
 
 # useLibraryCodeForTypes = false
 
 
 [tool.poetry]
 name = "Fau-tools"
-version = "1.4.5"
+version = "1.4.5.1"
 description = "A python module. The main function is for pytorch training."
 authors = ["Fau <Fau818@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "Fau_tools"}]
 homepage   = "https://github.com/Fau818/Fau_tools"
 repository = "https://github.com/Fau818/Fau_tools"
```

### Comparing `fau_tools-1.4.5/PKG-INFO` & `fau_tools-1.4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fau-tools
-Version: 1.4.5
+Version: 1.4.5.1
 Summary: A python module. The main function is for pytorch training.
 Home-page: https://github.com/Fau818/Fau_tools
 License: MIT
 Author: Fau
 Author-email: Fau818@qq.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

