# Comparing `tmp/fau_tools-1.4.3.1.tar.gz` & `tmp/fau_tools-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fau_tools-1.4.3.1.tar", max compression
+gzip compressed data, was "fau_tools-1.4.4.tar", max compression
```

## Comparing `fau_tools-1.4.3.1.tar` & `fau_tools-1.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.3.1/Fau_tools/__init__.py
--rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.3.1/Fau_tools/data_structure/__init__.py
--rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.py
--rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.pyi
--rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.3.1/Fau_tools/torch_tools/__init__.py
--rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.py
--rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.pyi
--rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.3.1/Fau_tools/utility/__init__.py
--rw-r--r--   0        0        0     8727 2023-03-24 06:33:55.632551 fau_tools-1.4.3.1/Fau_tools/utility/utility.py
--rw-r--r--   0        0        0      797 2023-03-24 02:36:31.555258 fau_tools-1.4.3.1/Fau_tools/utility/utility.pyi
--rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.3.1/README.md
--rw-r--r--   0        0        0     1150 2023-04-20 07:15:06.555876 fau_tools-1.4.3.1/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 fau_tools-1.4.3.1/PKG-INFO
+-rw-r--r--   0        0        0      179 2022-09-17 06:01:57.485247 fau_tools-1.4.4/Fau_tools/__init__.py
+-rw-r--r--   0        0        0       30 2022-11-07 07:34:00.261010 fau_tools-1.4.4/Fau_tools/data_structure/__init__.py
+-rw-r--r--   0        0        0     3420 2023-04-20 02:46:11.824418 fau_tools-1.4.4/Fau_tools/data_structure/data_structure.py
+-rw-r--r--   0        0        0      914 2023-04-20 02:46:11.824752 fau_tools-1.4.4/Fau_tools/data_structure/data_structure.pyi
+-rw-r--r--   0        0        0       27 2022-09-17 05:48:40.673809 fau_tools-1.4.4/Fau_tools/torch_tools/__init__.py
+-rw-r--r--   0        0        0    10050 2023-04-20 02:47:54.439467 fau_tools-1.4.4/Fau_tools/torch_tools/torch_tools.py
+-rw-r--r--   0        0        0     1440 2023-04-20 02:46:11.825456 fau_tools-1.4.4/Fau_tools/torch_tools/torch_tools.pyi
+-rw-r--r--   0        0        0       23 2022-09-17 05:58:01.298778 fau_tools-1.4.4/Fau_tools/utility/__init__.py
+-rw-r--r--   0        0        0     9338 2023-06-05 07:21:35.127414 fau_tools-1.4.4/Fau_tools/utility/utility.py
+-rw-r--r--   0        0        0      823 2023-06-05 07:21:12.849504 fau_tools-1.4.4/Fau_tools/utility/utility.pyi
+-rw-r--r--   0        0        0     2680 2023-04-20 02:37:45.625671 fau_tools-1.4.4/README.md
+-rw-r--r--   0        0        0     1148 2023-06-05 07:35:53.101686 fau_tools-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 fau_tools-1.4.4/PKG-INFO
```

### Comparing `fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.py` & `fau_tools-1.4.4/Fau_tools/data_structure/data_structure.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3.1/Fau_tools/data_structure/data_structure.pyi` & `fau_tools-1.4.4/Fau_tools/data_structure/data_structure.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.py` & `fau_tools-1.4.4/Fau_tools/torch_tools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3.1/Fau_tools/torch_tools/torch_tools.pyi` & `fau_tools-1.4.4/Fau_tools/torch_tools/torch_tools.pyi`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3.1/Fau_tools/utility/utility.py` & `fau_tools-1.4.4/Fau_tools/utility/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,47 +55,59 @@
   return "minor"
 
 
 
 # ------------------------------------------------------------
 # --------------- color print function
 # ------------------------------------------------------------
+# \033[{style=0};{fg=0};{bg}m
 __COLOR_DICT = {
   'black' : "\033[90m", "B": "\033[90m",
   'red'   : "\033[91m", 'r': "\033[91m",  # default
   'green' : "\033[92m", 'g': "\033[92m",
   'yellow': "\033[93m", 'y': "\033[93m",
   'blue'  : "\033[94m", 'b': "\033[94m",
   'purple': "\033[95m", 'p': "\033[95m",
   'cyan'  : "\033[96m", 'c': "\033[96m",
   'white' : "\033[97m", 'w': "\033[97m",
+
+  'solid_black' : "\033[0;97;100m", "sB": "\033[0;97;100m",
+  'solid_red'   : "\033[0;97;101m", 'sr': "\033[0;97;101m",
+  'solid_green' : "\033[0;90;102m", 'sg': "\033[0;90;102m",
+  'solid_yellow': "\033[0;90;103m", 'sy': "\033[0;90;103m",
+  'solid_blue'  : "\033[0;97;104m", 'sb': "\033[0;97;104m",
+  'solid_purple': "\033[0;97;105m", 'sp': "\033[0;97;105m",
+  'solid_cyan'  : "\033[0;90;106m", 'sc': "\033[0;90;106m",
+  'solid_white' : "\033[0;90;107m", 'sw': "\033[0;90;107m",
 }
 
-def cprint(text, color='red', sep='\n', ret=False):
+
+def cprint(*values, color='red', show=True, sep=' ', end='\n', **kwargs):
   """
   Colorful printer.
 
   Parameters
   ----------
-  text : the content needs to be printed
-  color : a string representing color; all the valid values shown in `__COLOR_DICT`
-  sep : a kwarg in `print()` function
-  ret : if True, the colorful string will not be print, but will be returned.
+  values : the contents need to be printed
+  color  : a string representing color; all the valid values shown in `__COLOR_DICT`
+  show   : if True, the colorful string will be printed; otherwise, will be returned.
+  sep    : a kwarg in `print()` function
+  end    : a kwarg in `print()` function
 
   Returns
   -------
-  If `ret=True`, will return the colorful string.
+  return the colorful string.
 
   """
   HEAD, TAIL = "\033[91m", "\033[0m"
   if color in __COLOR_DICT: HEAD = __COLOR_DICT[color]
 
-  color_string = f"{HEAD}{text}{TAIL}"
-  if not ret: print(color_string, sep=sep)
-  else: return color_string
+  color_string = HEAD + sep.join(str(value) for value in values) + TAIL
+  if show: show(color_string, sep=sep, end=end, **kwargs)
+  return color_string
 
 
 
 
 # ------------------------------------------------------------
 # --------------- auto calculate feature size
 # ------------------------------------------------------------
```

### Comparing `fau_tools-1.4.3.1/Fau_tools/utility/utility.pyi` & `fau_tools-1.4.4/Fau_tools/utility/utility.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def calc_time(function): ...
 
 def time_to_human(time: float|int) -> str: ...
 
 # def show_progress(now: int, total: int, time_manager: TimeManager=None, length: int=30, icons: str='█ ') -> None: ...
 
-def cprint(text: str, color: str='red', sep: str='\n', ret: bool=False) -> None|str: ...
+def cprint(*values: *object, color: str='red', show: bool=True, sep: str=' ', end: str='\n', **kwargs) -> str: ...
 
 
 def __get_value_in_height_and_width(value: tuple[int, int]|int, value_name: str) -> tuple[int, int]: ...
 
 def _calc_value_after_layer(x: int, k_size: int, stride: int, padding: int) -> int: ...
 
 def calc_feature_size(channel: int, height: int, width: int, sequential: torch.nn.Sequential) -> int: ...
```

### Comparing `fau_tools-1.4.3.1/README.md` & `fau_tools-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fau_tools-1.4.3.1/pyproject.toml` & `fau_tools-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 reportUnusedExpression  = false
 
 # useLibraryCodeForTypes = false
 
 
 [tool.poetry]
 name = "Fau-tools"
-version = "1.4.3.1"
+version = "1.4.4"
 description = "A python module. The main function is for pytorch training."
 authors = ["Fau <Fau818@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "Fau_tools"}]
 homepage   = "https://github.com/Fau818/Fau_tools"
 repository = "https://github.com/Fau818/Fau_tools"
```

### Comparing `fau_tools-1.4.3.1/PKG-INFO` & `fau_tools-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fau-tools
-Version: 1.4.3.1
+Version: 1.4.4
 Summary: A python module. The main function is for pytorch training.
 Home-page: https://github.com/Fau818/Fau_tools
 License: MIT
 Author: Fau
 Author-email: Fau818@qq.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

