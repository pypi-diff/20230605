# Comparing `tmp/fukkatsu-0.0.2.tar.gz` & `tmp/fukkatsu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.2.tar", last modified: Mon May 22 22:35:32 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.3.tar", last modified: Mon Jun  5 00:23:53 2023, max compression
```

## Comparing `fukkatsu-0.0.2.tar` & `fukkatsu-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.320587 fukkatsu-0.0.2/
--rw-rw-rw-   0        0        0      377 2023-05-22 21:56:00.000000 fukkatsu-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9618 2023-05-22 22:35:32.304972 fukkatsu-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8977 2023-05-22 22:17:18.000000 fukkatsu-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.195587 fukkatsu-0.0.2/fukkatsu/
--rw-rw-rw-   0        0        0     6790 2023-05-22 22:11:23.000000 fukkatsu-0.0.2/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.258082 fukkatsu-0.0.2/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.2/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.2/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.2/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.289340 fukkatsu-0.0.2/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.2/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     2573 2023-05-22 21:23:31.000000 fukkatsu-0.0.2/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     2241 2023-05-22 22:11:23.000000 fukkatsu-0.0.2/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     1583 2023-05-20 04:08:40.000000 fukkatsu-0.0.2/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.242463 fukkatsu-0.0.2/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0     9618 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 22:35:32.320587 fukkatsu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-05-19 01:33:19.000000 fukkatsu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.512154 fukkatsu-0.0.3/
+-rw-rw-rw-   0        0        0      519 2023-06-04 23:17:03.000000 fukkatsu-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10488 2023-06-05 00:23:53.506492 fukkatsu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9849 2023-06-05 00:14:18.000000 fukkatsu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.422550 fukkatsu-0.0.3/fukkatsu/
+-rw-rw-rw-   0        0        0     7833 2023-06-05 00:09:44.000000 fukkatsu-0.0.3/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.469382 fukkatsu-0.0.3/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.3/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.3/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.3/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.494481 fukkatsu-0.0.3/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.3/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2023-06-04 21:33:13.000000 fukkatsu-0.0.3/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     2241 2023-06-05 00:09:44.000000 fukkatsu-0.0.3/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     1583 2023-05-20 04:08:40.000000 fukkatsu-0.0.3/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.453760 fukkatsu-0.0.3/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    10488 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-05 00:23:53.000000 fukkatsu-0.0.3/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 00:23:53.000000 fukkatsu-0.0.3/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 00:23:53.512154 fukkatsu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-04 21:25:11.000000 fukkatsu-0.0.3/setup.py
```

### Comparing `fukkatsu-0.0.2/LICENSE` & `fukkatsu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.2/PKG-INFO` & `fukkatsu-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: fukkatsu
-Version: 0.0.2
-Summary: A python library for runtime LLM supported code corrections.
-Home-page: https://github.com/maxmekiska/fukkatsu
-Author: Maximilian Mekiska
-Author-email: maxmekiska@gmail.com
-Keywords: machinelearning,llm,runtime,codecorrection
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -113,26 +97,26 @@
 ```
 
 The above example will allow the LLM to attempt to fix the function twice. If the LLM fails to fix the function after two attempts, a `flatline error` will be raised which indicates that the LLM was not able to fix the function during runtime.
 
 </details>
 
 
-## fukkatsu 0.0.1
+## fukkatsu 0.0.1 - `Extra Life`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 
 fukkatsu 0.0.1 incorporates all the features demonstrated within the MVP section and introduces the concept of additional requests. Additional requests provide users with an alternative means of giving specific instructions to the LLM when a correction to a function is required. These additional requests act as a safeguard against potential misinterpretations by the LLM.
 
 
 ```python
-@resurrect(lives=1, additional_req = "multiply any result by 1000")
+@resurrect(lives=1, additional_req = "add to any result 1000")
 def my_function(x, y, z):
     """
     function to divide x by y and add to the result z. Should return z if y is 0.
     """
     result = x / y + z
     return result
 
@@ -212,15 +196,15 @@
 ```
 1002
 1002
 ```
 </details>
 
 
-## fukkatsu 0.0.2
+## fukkatsu 0.0.2 - `The Ghost in the Machine`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
 
@@ -231,10 +215,29 @@
     """
     function to read files and output a dataframes.
     """
     pd.read_csv(file_path)
     
 my_mutated_function("test_file.xlsx")
 ```
+</details>
+
+## fukkatsu 0.0.3 - `Laissez-faire`
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The `mutate` and `resurrect` decorators now support a new argument called allow_installs. By default, `allow_installs` is set to `False`. However, when set to `True`, the LLM will be able to test whether suggested or used python libraries are installed on the system. If any of the libraries are not installed, the LLM will install them before continuing code execution. This argument enables the LLM to have even more freedom. Therefore, setting the argument to True should be considered carefully.
 
+### `resurrect`
+```python
+def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
+  ...
+```
 
+### `mutate`
+```python
+def mutate(request: str = "", allow_installs: bool = False):
+  ...
+```
 </details>
```

### Comparing `fukkatsu-0.0.2/README.md` & `fukkatsu-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: fukkatsu
+Version: 0.0.3
+Summary: A python library for runtime LLM supported code corrections.
+Home-page: https://github.com/maxmekiska/fukkatsu
+Author: Maximilian Mekiska
+Author-email: maxmekiska@gmail.com
+Keywords: machinelearning,llm,runtime,codecorrection
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -97,26 +113,26 @@
 ```
 
 The above example will allow the LLM to attempt to fix the function twice. If the LLM fails to fix the function after two attempts, a `flatline error` will be raised which indicates that the LLM was not able to fix the function during runtime.
 
 </details>
 
 
-## fukkatsu 0.0.1
+## fukkatsu 0.0.1 - `Extra Life`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 
 fukkatsu 0.0.1 incorporates all the features demonstrated within the MVP section and introduces the concept of additional requests. Additional requests provide users with an alternative means of giving specific instructions to the LLM when a correction to a function is required. These additional requests act as a safeguard against potential misinterpretations by the LLM.
 
 
 ```python
-@resurrect(lives=1, additional_req = "multiply any result by 1000")
+@resurrect(lives=1, additional_req = "add to any result 1000")
 def my_function(x, y, z):
     """
     function to divide x by y and add to the result z. Should return z if y is 0.
     """
     result = x / y + z
     return result
 
@@ -196,15 +212,15 @@
 ```
 1002
 1002
 ```
 </details>
 
 
-## fukkatsu 0.0.2
+## fukkatsu 0.0.2 - `The Ghost in the Machine`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
 
@@ -215,10 +231,29 @@
     """
     function to read files and output a dataframes.
     """
     pd.read_csv(file_path)
     
 my_mutated_function("test_file.xlsx")
 ```
+</details>
+
+## fukkatsu 0.0.3 - `Laissez-faire`
+
+<details>
+  <summary>Expand</summary>
+  <br>
 
+The `mutate` and `resurrect` decorators now support a new argument called allow_installs. By default, `allow_installs` is set to `False`. However, when set to `True`, the LLM will be able to test whether suggested or used python libraries are installed on the system. If any of the libraries are not installed, the LLM will install them before continuing code execution. This argument enables the LLM to have even more freedom. Therefore, setting the argument to True should be considered carefully.
 
-</details>
+### `resurrect`
+```python
+def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
+  ...
+```
+
+### `mutate`
+```python
+def mutate(request: str = "", allow_installs: bool = False):
+  ...
+```
+</details>
```

### Comparing `fukkatsu-0.0.2/fukkatsu/__init__.py` & `fukkatsu-0.0.3/fukkatsu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
-import ast
 import functools
 import logging
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
-from fukkatsu.utils import (extract_imports, extract_text_between_backticks,
+from fukkatsu.utils import (check_and_install_libraries, extract_imports,
+                            extract_text_between_backticks,
                             insert_string_after_colon, remove_trace_lines,
                             remove_wrapper_name, return_input_arguments,
                             return_source_code)
 from fukkatsu.utils.medic import defibrillate, enhance
 
 
-def resurrect(lives: int = 1, additional_req: str = ""):
+def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
     def _resurrect(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
 
             try:
                 result = func(*args, **kwargs)
                 return result
@@ -45,18 +45,26 @@
                     logging.warning("Requesting INITIAL correction\n")
                     suggested_code = defibrillate(
                         inputs=input_args,
                         faulty_function=source,
                         error_trace=trace,
                         additional_req=additional_req,
                     )
+                    logging.warning(
+                        f"Received INITIAL RAW suggestion: {suggested_code}\n"
+                    )
                     suggested_code = extract_text_between_backticks(suggested_code)
-                    logging.warning(f"Received INITIAL suggestion: {suggested_code}\n")
+                    logging.warning(
+                        f"Received INITIAL CLEANED suggestion: {suggested_code}\n"
+                    )
 
                     import_block = extract_imports(suggested_code)
+                    if allow_installs == True:
+                        check_and_install_libraries(import_statements=import_block)
+
                     suggested_code = insert_string_after_colon(
                         suggested_code, import_block
                     )
                     logging.warning(
                         f"Import block added to suggested code:\n {suggested_code}\n"
                     )
 
@@ -97,37 +105,45 @@
                         else:
                             suggested_code = defibrillate(
                                 inputs=input_args,
                                 faulty_function=suggested_code,
                                 error_trace=trace,
                                 additional_req=additional_req,
                             )
+                            logging.warning(
+                                f"Received attempt RAW suggestion: {suggested_code}\n"
+                            )
                             suggested_code = extract_text_between_backticks(
                                 suggested_code
                             )
                             logging.warning(
-                                f"Received attempt {i} suggestion: {suggested_code}\n"
+                                f"Received attempt CLEANED suggestion: {suggested_code}\n"
                             )
 
                             import_block = extract_imports(suggested_code)
+                            if allow_installs == True:
+                                check_and_install_libraries(
+                                    import_statements=import_block
+                                )
+
                             suggested_code = insert_string_after_colon(
                                 suggested_code, import_block
                             )
                             logging.warning(
                                 f"Import block added to suggested code:\n {suggested_code}\n"
                             )
 
                 raise Exception(f"|__|__|______ {func.__name__} flatlined")
 
         return wrapper
 
     return _resurrect
 
 
-def mutate(request: str = ""):
+def mutate(request: str = "", allow_installs: bool = False):
     def _mutate(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
 
             input_args = return_input_arguments(func, *args, **kwargs)
             source = return_source_code(func)
             source = remove_wrapper_name(source)
@@ -137,21 +153,25 @@
 
             logging.warning("Requesting mutation\n")
             suggested_code = enhance(
                 inputs=input_args,
                 target_function=source,
                 request=request,
             )
+            logging.warning(f"Received RAW suggestion mutation: {suggested_code}\n")
             suggested_code = extract_text_between_backticks(suggested_code)
-            logging.warning(f"Received suggestion mutation: {suggested_code}\n")
+            logging.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
 
             global_dict = globals()
             local_dict = locals()
 
             import_block = extract_imports(suggested_code)
+            if allow_installs == True:
+                check_and_install_libraries(import_statements=import_block)
+
             suggested_code = insert_string_after_colon(suggested_code, import_block)
             logging.warning(
                 f"Import block added to suggested code:\n {suggested_code}\n"
             )
 
             compiled_code = compile(suggested_code, "<string>", "exec")
```

### Comparing `fukkatsu-0.0.2/fukkatsu/memory/manage.py` & `fukkatsu-0.0.3/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.2/fukkatsu/utils/medic.py` & `fukkatsu-0.0.3/fukkatsu/utils/medic.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.2/fukkatsu/utils/prompt.py` & `fukkatsu-0.0.3/fukkatsu/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.2/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.3/fukkatsu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -113,26 +113,26 @@
 ```
 
 The above example will allow the LLM to attempt to fix the function twice. If the LLM fails to fix the function after two attempts, a `flatline error` will be raised which indicates that the LLM was not able to fix the function during runtime.
 
 </details>
 
 
-## fukkatsu 0.0.1
+## fukkatsu 0.0.1 - `Extra Life`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 
 fukkatsu 0.0.1 incorporates all the features demonstrated within the MVP section and introduces the concept of additional requests. Additional requests provide users with an alternative means of giving specific instructions to the LLM when a correction to a function is required. These additional requests act as a safeguard against potential misinterpretations by the LLM.
 
 
 ```python
-@resurrect(lives=1, additional_req = "multiply any result by 1000")
+@resurrect(lives=1, additional_req = "add to any result 1000")
 def my_function(x, y, z):
     """
     function to divide x by y and add to the result z. Should return z if y is 0.
     """
     result = x / y + z
     return result
 
@@ -212,15 +212,15 @@
 ```
 1002
 1002
 ```
 </details>
 
 
-## fukkatsu 0.0.2
+## fukkatsu 0.0.2 - `The Ghost in the Machine`
 
 <details>
   <summary>Expand</summary>
   <br>
 
 The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
 
@@ -231,10 +231,29 @@
     """
     function to read files and output a dataframes.
     """
     pd.read_csv(file_path)
     
 my_mutated_function("test_file.xlsx")
 ```
+</details>
+
+## fukkatsu 0.0.3 - `Laissez-faire`
+
+<details>
+  <summary>Expand</summary>
+  <br>
 
+The `mutate` and `resurrect` decorators now support a new argument called allow_installs. By default, `allow_installs` is set to `False`. However, when set to `True`, the LLM will be able to test whether suggested or used python libraries are installed on the system. If any of the libraries are not installed, the LLM will install them before continuing code execution. This argument enables the LLM to have even more freedom. Therefore, setting the argument to True should be considered carefully.
 
+### `resurrect`
+```python
+def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
+  ...
+```
+
+### `mutate`
+```python
+def mutate(request: str = "", allow_installs: bool = False):
+  ...
+```
 </details>
```

### Comparing `fukkatsu-0.0.2/setup.py` & `fukkatsu-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

