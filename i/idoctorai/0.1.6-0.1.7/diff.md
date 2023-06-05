# Comparing `tmp/idoctorai-0.1.6.tar.gz` & `tmp/idoctorai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.1.6.tar", max compression
+gzip compressed data, was "idoctorai-0.1.7.tar", max compression
```

## Comparing `idoctorai-0.1.6.tar` & `idoctorai-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.1.6/LICENSE
--rw-r--r--   0        0        0    16565 2023-06-02 04:05:23.763126 idoctorai-0.1.6/pandasai/__init__.py
--rw-r--r--   0        0        0     1200 2023-06-02 03:38:48.762886 idoctorai-0.1.6/pandasai/constants.py
--rw-r--r--   0        0        0     1001 2023-06-02 03:38:48.762886 idoctorai-0.1.6/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.1.6/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0      593 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.1.6/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     2723 2023-05-31 07:10:59.364569 idoctorai-0.1.6/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.1.6/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.1.6/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11245 2023-06-02 03:38:48.763883 idoctorai-0.1.6/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.1.6/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.1.6/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.1.6/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.1.6/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.1.6/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.1.6/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.1.6/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.1.6/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.1.6/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-02 04:03:56.645964 idoctorai-0.1.6/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1093 2023-06-02 03:41:13.186309 idoctorai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-02 03:40:47.303734 idoctorai-0.1.6/README.md
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 idoctorai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.1.7/LICENSE
+-rw-r--r--   0        0        0    16574 2023-06-05 11:32:52.312900 idoctorai-0.1.7/pandasai/__init__.py
+-rw-r--r--   0        0        0     1200 2023-06-05 10:38:51.205810 idoctorai-0.1.7/pandasai/constants.py
+-rw-r--r--   0        0        0     1001 2023-06-05 10:38:51.206807 idoctorai-0.1.7/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.1.7/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.1.7/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0      593 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.1.7/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     2723 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.1.7/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.1.7/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11269 2023-06-05 11:26:38.666244 idoctorai-0.1.7/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.1.7/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.1.7/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.1.7/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.1.7/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.1.7/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.1.7/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.1.7/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.1.7/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1455 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1093 2023-06-05 12:53:10.833279 idoctorai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-05 10:50:23.961401 idoctorai-0.1.7/README.md
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 idoctorai-0.1.7/PKG-INFO
```

### Comparing `idoctorai-0.1.6/LICENSE` & `idoctorai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/__init__.py` & `idoctorai-0.1.7/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
     _enforce_privacy: bool = False
-    _max_retries: int = 3
+    _max_retries: int = 1
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
@@ -217,15 +217,15 @@
                 df_head = data_frame.head(rows_to_display)
                 if anonymize_df:
                     df_head = anonymize_dataframe_head(df_head)
 
                 code = self._llm.generate_code(
                     GeneratePythonCodePrompt(
                         prompt=prompt,
-                        df_head=df_head.to_string(),
+                        df_head=df_head,
                         num_rows=data_frame.shape[0],
                         num_columns=data_frame.shape[1],
                         rows_to_display=rows_to_display,
                     ),
                     prompt,
                 )
 
@@ -381,14 +381,15 @@
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
             code = add_save_chart(code)
 
         # Get the code to run removing unsafe imports and df overwrites
+        print(code)
         code_to_run = self.clean_code(code)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
```

### Comparing `idoctorai-0.1.6/pandasai/constants.py` & `idoctorai-0.1.7/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/exceptions.py` & `idoctorai-0.1.7/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/helpers/anonymizer.py` & `idoctorai-0.1.7/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/helpers/from_excel.py` & `idoctorai-0.1.7/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/helpers/notebook.py` & `idoctorai-0.1.7/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/helpers/save_chart.py` & `idoctorai-0.1.7/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/azure_openai.py` & `idoctorai-0.1.7/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/base.py` & `idoctorai-0.1.7/pandasai/llm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,16 @@
                 }
             ],
         }
 
         if self.stop is not None:
             params["stop"] = [self.stop]
 
+        print(value)
+
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
```

### Comparing `idoctorai-0.1.6/pandasai/llm/fake.py` & `idoctorai-0.1.7/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/google_palm.py` & `idoctorai-0.1.7/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/open_assistant.py` & `idoctorai-0.1.7/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/openai.py` & `idoctorai-0.1.7/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/llm/starcoder.py` & `idoctorai-0.1.7/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/base.py` & `idoctorai-0.1.7/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.1.7/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.1.7/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/generate_python_code.py` & `idoctorai-0.1.7/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/generate_response.py` & `idoctorai-0.1.7/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.6/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.1.7/pandasai/prompts/multiple_dataframes.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,20 +21,18 @@
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
-            data_text = dataframe.head().to_string()
-
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the result of `print(df{i}.head())`:
-{data_text}"""
+{dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
         )
```

### Comparing `idoctorai-0.1.6/pyproject.toml` & `idoctorai-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.1.6"
+version = "0.1.7"
 description = "this is idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `idoctorai-0.1.6/PKG-INFO` & `idoctorai-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.1.6
+Version: 0.1.7
 Summary: this is idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

