# Comparing `tmp/manubot-ai-editor-0.4.5.tar.gz` & `tmp/manubot-ai-editor-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manubot-ai-editor-0.4.5.tar", last modified: Fri Jun  2 14:13:38 2023, max compression
+gzip compressed data, was "manubot-ai-editor-0.4.6.tar", last modified: Mon Jun  5 14:58:45 2023, max compression
```

## Comparing `manubot-ai-editor-0.4.5.tar` & `manubot-ai-editor-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.5/README.md
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/__init__.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     3399 2023-06-02 13:56:51.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/env_vars.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20582 2023-06-01 16:43:05.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/models.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor/utils.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      498 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/SOURCES.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/dependency_links.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/requires.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-02 14:13:38.000000 manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/top_level.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/setup.cfg
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-02 14:13:22.000000 manubot-ai-editor-0.4.5/setup.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-02 14:13:38.236326 manubot-ai-editor-0.4.5/tests/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    61034 2023-06-01 15:22:56.000000 manubot-ai-editor-0.4.5/tests/test_completion_model.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.5/tests/test_editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     7738 2023-06-01 16:46:08.000000 manubot-ai-editor-0.4.5/tests/test_model_get_prompt.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.6/README.md
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.707883 manubot-ai-editor-0.4.6/libs/
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/__init__.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     3604 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/env_vars.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20468 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/models.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/utils.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      523 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/requires.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/top_level.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/setup.cfg
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-05 14:58:43.000000 manubot-ai-editor-0.4.6/setup.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/tests/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.6/tests/test_editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     8306 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_basics.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    10320 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_get_prompt.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    51084 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_revision.py
```

### Comparing `manubot-ai-editor-0.4.5/PKG-INFO` & `manubot-ai-editor-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.5/README.md` & `manubot-ai-editor-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/editor.py` & `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/env_vars.py` & `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/env_vars.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     AI_EDITOR_CUSTOM_PROMPT="proofread the following paragraph"
 """
 
 # OpenAI API key to use
 OPENAI_API_KEY = "OPENAI_API_KEY"
 
 # Language model to use. For example, "text-davinci-003", "gpt-3.5-turbo", "gpt-3.5-turbo-0301", etc
+# The tool currently supports the "chat/completions", "completions", and "edits" endpoints, and you can check
+# compatible models here: https://platform.openai.com/docs/models/model-endpoint-compatibility
 LANGUAGE_MODEL = "AI_EDITOR_LANGUAGE_MODEL"
 
 # Model parameter: max_tokens
 MAX_TOKENS_PER_REQUEST = "AI_EDITOR_MAX_TOKENS_PER_REQUEST"
 
 # Model parameter: temperature
 TEMPERATURE = "AI_EDITOR_TEMPERATURE"
```

### Comparing `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/models.py` & `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,14 @@
         model_engine: str = "text-davinci-003",
         temperature: float = 0.5,
         presence_penalty: float = None,
         frequency_penalty: float = None,
         best_of: int = None,
         top_p: float = None,
         retry_count: int = 5,
-        edit_endpoint: bool = False,
     ):
         super().__init__()
 
         # make sure the OpenAI API key is set
         openai.api_key = openai_api_key
 
         if openai.api_key is None:
@@ -215,28 +214,24 @@
                 # if it is not an int, we ignore it
                 pass
 
         self.title = title
         self.keywords = keywords
 
         # adjust options if edits or chat endpoint was selected
-        self.edit_endpoint = edit_endpoint
-        self.chat_endpoint = False
+        self.endpoint = "chat"
 
-        if self.edit_endpoint and model_engine == "text-davinci-003":
-            model_engine = "text-davinci-edit-001"
+        if model_engine.startswith(("text-davinci-", "text-curie-", "text-babbage-", "text-ada-")):
+            self.endpoint = "completions"
 
-        if model_engine == "text-davinci-edit-001":
-            self.edit_endpoint = True
+            if "-edit-" in model_engine:
+                self.endpoint = "edits"
 
-        if model_engine == "gpt-3.5-turbo":
-            self.edit_endpoint = False
-            self.chat_endpoint = True
-
-        print("Language model: ", model_engine)
+        print(f"Language model: {model_engine}")
+        print(f"Model endpoint used: {self.endpoint}")
 
         self.model_parameters = {
             "model": model_engine,
             "temperature": temperature,
             "top_p": top_p,
             "presence_penalty": presence_penalty,
             "frequency_penalty": frequency_penalty,
@@ -262,19 +257,19 @@
         Results, Discussion, etc.).
 
         Args:
             paragraph_text: text of the paragraph to revise.
             section_name: name of the section the paragraph belongs to.
 
         Returns:
-            If self.edit_endpoint is False, then returns a string with the prompt to be used by the model for the revision of the paragraph.
+            If self.endpoint != "edits", then returns a string with the prompt to be used by the model for the revision of the paragraph.
             It contains two paragraphs of text: the command for the model
             ("Revise...") and the paragraph to revise.
 
-            If self.edit_endpoint is True, then returns a tuple with two strings:
+            If self.endpoint == "edits", then returns a tuple with two strings:
              1) the instructions to be used by the model for the revision of the paragraph,
              2) the paragraph to revise.
         """
 
         if env_vars.CUSTOM_PROMPT in os.environ:
             prompt = os.environ[env_vars.CUSTOM_PROMPT]
             print(
@@ -352,15 +347,15 @@
                     the text minimizes the use of jargon,
                     the text grammar is correct, spelling errors are fixed,
                     and the text has a clear sentence structure
             """
 
         prompt = self.several_spaces_pattern.sub(" ", prompt).strip()
 
-        if not self.edit_endpoint:
+        if self.endpoint != "edits":
             return f"{prompt}.\n\n{paragraph_text.strip()}"
         else:
             prompt = prompt.replace("the following paragraph", "this paragraph")
             return f"{prompt}.", paragraph_text.strip()
 
     def get_max_tokens(self, paragraph_text: str, fraction: float = 2.0) -> int:
         """
@@ -449,22 +444,22 @@
         max_tokens = self.get_max_tokens(paragraph_text)
         prompt = self.get_prompt(paragraph_text, section_name)
 
         params = {
             "n": 1,
         }
 
-        if self.edit_endpoint:
+        if self.endpoint == "edits":
             params.update(
                 {
                     "instruction": prompt[0],
                     "input": prompt[1],
                 }
             )
-        elif self.chat_endpoint:
+        elif self.endpoint == "chat":
             params.update(
                 {
                     "messages": [
                         {"role": "user", "content": prompt},
                     ],
                     "max_tokens": max_tokens,
                     "stop": None,
@@ -486,22 +481,22 @@
         while message == "" and retry_count < self.retry_count:
             try:
                 print(
                     f"[Attempt #{retry_count}] Revising paragraph '{paragraph_text[:20]}'...",
                     flush=True,
                 )
 
-                if self.edit_endpoint:
+                if self.endpoint == "edits":
                     completions = openai.Edit.create(**params)
-                elif self.chat_endpoint:
+                elif self.endpoint == "chat":
                     completions = openai.ChatCompletion.create(**params)
                 else:
                     completions = openai.Completion.create(**params)
 
-                if self.chat_endpoint:
+                if self.endpoint == "chat":
                     message = completions.choices[0].message.content.strip()
                 else:
                     message = completions.choices[0].text.strip()
             except Exception as e:
                 error_message = str(e)
                 print(f"Error: {error_message}")
```

### Comparing `manubot-ai-editor-0.4.5/libs/manubot_ai_editor/utils.py` & `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/utils.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.5/libs/manubot_ai_editor.egg-info/PKG-INFO` & `manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.5/setup.py` & `manubot-ai-editor-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="manubot-ai-editor",
-    version="0.4.5",
+    version="0.4.6",
     author="Milton Pividori",
     author_email="miltondp@gmail.com",
     description="A Manubot plugin to revise a manuscript using GPT-3",
     license="BSD-2-Clause Plus Patent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greenelab/manubot-ai-editor",
```

### Comparing `manubot-ai-editor-0.4.5/tests/test_completion_model.py` & `manubot-ai-editor-0.4.6/tests/test_model_revision.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,296 +1,22 @@
-import os
-from pathlib import Path
-from unittest import mock
-
+"""
+These tests need to call the OpenAI API, so they are in a separate file and can incur costs.
+"""
 import pytest
 
-from manubot_ai_editor.editor import ManuscriptEditor, env_vars
-from manubot_ai_editor import models
-from manubot_ai_editor.models import GPT3CompletionModel, RandomManuscriptRevisionModel
+from manubot_ai_editor.editor import ManuscriptEditor
+from manubot_ai_editor.models import GPT3CompletionModel
 from manubot_ai_editor.utils import starts_with_similar
 
-MANUSCRIPTS_DIR = Path(__file__).parent / "manuscripts"
-
-
-def test_model_object_init_without_openai_api_key():
-    _environ = os.environ.copy()
-    try:
-        if env_vars.OPENAI_API_KEY in os.environ:
-            os.environ.pop(env_vars.OPENAI_API_KEY)
-
-        with pytest.raises(ValueError):
-            GPT3CompletionModel(
-                title="Test title",
-                keywords=["test", "keywords"],
-            )
-    finally:
-        os.environ = _environ
-
-
-@mock.patch.dict("os.environ", {env_vars.OPENAI_API_KEY: "env_var_test_value"})
-def test_model_object_init_with_openai_api_key_as_environment_variable():
-    GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    assert models.openai.api_key == "env_var_test_value"
-
-
-def test_model_object_init_with_openai_api_key_as_parameter():
-    _environ = os.environ.copy()
-    try:
-        if env_vars.OPENAI_API_KEY in os.environ:
-            os.environ.pop(env_vars.OPENAI_API_KEY)
-
-        GPT3CompletionModel(
-            title="Test title",
-            keywords=["test", "keywords"],
-            openai_api_key="test_value",
-        )
-
-        from manubot_ai_editor import models
-
-        assert models.openai.api_key == "test_value"
-    finally:
-        os.environ = _environ
-
-
-@mock.patch.dict("os.environ", {env_vars.OPENAI_API_KEY: "env_var_test_value"})
-def test_model_object_init_with_openai_api_key_as_parameter_has_higher_priority():
-    GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-        openai_api_key="test_value",
-    )
-
-    from manubot_ai_editor import models
-
-    assert models.openai.api_key == "test_value"
-
-
-def test_model_object_init_default_language_model():
-    model = GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    assert model.model_parameters["model"] == "text-davinci-003"
-
-
-@mock.patch.dict("os.environ", {env_vars.LANGUAGE_MODEL: "text-curie-001"})
-def test_model_object_init_read_language_model_from_environment():
-    model = GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    assert model.model_parameters["model"] == "text-curie-001"
-
-
-@mock.patch.dict("os.environ", {env_vars.LANGUAGE_MODEL: ""})
-def test_model_object_init_read_language_model_from_environment_is_empty():
-    model = GPT3CompletionModel(
-        title="Test title",
-        keywords=["test", "keywords"],
-    )
-
-    assert model.model_parameters["model"] == "text-davinci-003"
-
-
-def test_get_prompt_for_abstract():
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    paragraph_text = "Text of the abstract"
-
-    prompt = model.get_prompt(paragraph_text, "abstract")
-    assert prompt is not None
-    assert isinstance(prompt, str)
-    assert "abstract" in prompt
-    assert f"'{me.title}'" in prompt
-    assert f"{me.keywords[0]}" in prompt
-    assert f"{me.keywords[1]}" in prompt
-    assert f"{me.keywords[2]}" in prompt
-    assert paragraph_text in prompt
-    assert prompt.startswith("Revise")
-    assert "  " not in prompt
-
-
-def test_get_prompt_for_abstract_edit_endpoint():
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-        edit_endpoint=True,
-    )
-
-    paragraph_text = "Text of the abstract. "
-
-    instruction, paragraph = model.get_prompt(paragraph_text, "abstract")
-    assert instruction is not None
-    assert isinstance(instruction, str)
-    assert paragraph is not None
-    assert isinstance(paragraph, str)
-
-    assert "this paragraph" in instruction
-    assert "abstract" in instruction
-    assert f"'{me.title}'" in instruction
-    assert f"{me.keywords[0]}" in instruction
-    assert f"{me.keywords[1]}" in instruction
-    assert f"{me.keywords[2]}" in instruction
-    assert "  " not in instruction
-    assert instruction.startswith("Revise")
-
-    assert paragraph_text.strip() == paragraph
-
-
-def test_get_prompt_for_introduction():
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    paragraph_text = "Text of the initial part"
-
-    prompt = model.get_prompt(paragraph_text, "introduction")
-    assert prompt is not None
-    assert isinstance(prompt, str)
-    assert "Introduction" in prompt
-    assert f"'{me.title}'" in prompt
-    assert f"{me.keywords[0]}" in prompt
-    assert f"{me.keywords[1]}" in prompt
-    assert f"{me.keywords[2]}" in prompt
-    assert paragraph_text in prompt
-    assert prompt.startswith("Revise")
-    assert "  " not in prompt
-
-
-def test_get_max_tokens_fraction_is_one():
-    paragraph = r"""
-Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
-In transcriptomics, genes with correlated expression often share functions or are part of disease-relevant biological processes.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    paragraph_text = " ".join(paragraph)
-
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    max_tokens = model.get_max_tokens(paragraph_text, 1.0)
-    assert max_tokens is not None
-    assert isinstance(max_tokens, int)
-    assert 50 < max_tokens < 60
-
-
-def test_get_max_tokens_using_fraction_is_two():
-    paragraph = r"""
-Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
-In transcriptomics, genes with correlated expression often share functions or are part of disease-relevant biological processes.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    paragraph_text = " ".join(paragraph)
-
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    max_tokens = model.get_max_tokens(paragraph_text, 2.0)
-    assert max_tokens is not None
-    assert isinstance(max_tokens, int)
-    assert 110 < max_tokens < 120
-
-
-@mock.patch.dict("os.environ", {env_vars.MAX_TOKENS_PER_REQUEST: "0.5"})
-def test_get_max_tokens_using_fraction_is_given_by_environment_and_is_float():
-    paragraph = r"""
-Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
-In transcriptomics, genes with correlated expression often share functions or are part of disease-relevant biological processes.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    paragraph_text = " ".join(paragraph)
-
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    max_tokens = model.get_max_tokens(paragraph_text)
-    assert max_tokens is not None
-    assert isinstance(max_tokens, int)
-    assert 25 < max_tokens < 35
-
-
-@mock.patch.dict("os.environ", {env_vars.MAX_TOKENS_PER_REQUEST: "779"})
-def test_get_max_tokens_using_fraction_is_given_by_environment_and_is_int():
-    paragraph = r"""
-Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
-In transcriptomics, genes with correlated expression often share functions or are part of disease-relevant biological processes.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    paragraph_text = " ".join(paragraph)
-
-    me = ManuscriptEditor(
-        content_dir=MANUSCRIPTS_DIR / "ccc",
-    )
-
-    model = GPT3CompletionModel(
-        title=me.title,
-        keywords=me.keywords,
-    )
-
-    # parameter 'fraction' is ignored when environment variable is set
-    max_tokens = model.get_max_tokens(paragraph_text, 2.0)
-    assert max_tokens is not None
-    assert isinstance(max_tokens, int)
-    assert max_tokens == 779
-
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_abstract_ccc(model):
     # from CCC manuscript
     paragraph = r"""
 Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
@@ -342,15 +68,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_abstract_phenoplier(model):
     # from PhenoPLIER manuscript
     paragraph = r"""
 Genes act in concert with each other in specific contexts to perform their functions.
@@ -405,15 +131,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_abstract_ai_revision(model):
     # from LLM for articles revision manuscript
     paragraph = r"""
 Academics often communicate through scholarly manuscripts.
@@ -463,15 +189,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_introduction_paragraph_with_single_and_multiple_citations_together(
     model,
 ):
     # from CCC manuscript
@@ -524,15 +250,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_introduction_paragraph_with_citations_and_paragraph_is_the_first(model):
     # from PhenoPLIER manuscript
     paragraph = r"""
 Genes work together in context-specific networks to carry out different functions [@pmid:19104045; @doi:10.1038/ng.3259].
@@ -582,15 +308,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_introduction_paragraph_with_citations_and_paragraph_is_the_last(model):
     # from LLM for articles revision manuscript
     paragraph = r"""
 We developed a software publishing platform that imagines a future where authors co-write their manuscripts with the support of large language models.
@@ -639,15 +365,15 @@
     assert "$" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_results_paragraph_with_short_inline_formulas_and_refs_to_figures_and_citations(
     model,
 ):
     # from CCC manuscript
@@ -691,15 +417,15 @@
     assert "Figure @fig:datasets_rel" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_results_paragraph_with_lists_and_refs_to_sections_and_subfigs(model):
     # from PhenoPLIER manuscript
     paragraph = r"""
 PhenoPLIER is a flexible computational framework that combines gene-trait and gene-drug associations with gene modules expressed in specific contexts (Figure {@fig:entire_process}a).
@@ -753,15 +479,15 @@
     assert "[Supplementary Note 2](#sm:clustering:null_sim)" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_results_paragraph_is_too_long(model):
     # from CCC manuscript
     paragraph = r"""
 We sought to systematically analyze discrepant scores to assess whether associations were replicated in other datasets besides GTEx.
@@ -807,15 +533,15 @@
     assert "\n".join(paragraph) == paragraph_revised_without_error
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_discussion_paragraph_with_markdown_formatting_and_citations(model):
     # from CCC manuscript
     paragraph = r"""
 It is well-known that biomedical research is biased towards a small fraction of human genes [@pmid:17620606; @pmid:17472739].
@@ -861,15 +587,15 @@
     assert "*" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_discussion_paragraph_with_minor_math_and_refs_to_sections_and_websites(
     model,
 ):
     # from PhenoPLIER manuscript
@@ -922,15 +648,15 @@
     )
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_conclusions_paragraph_with_simple_text(model):
     # conclusions is the same as discussion in CCC/PhenoPLIER
 
     # from LLM for articles revision manuscript
@@ -973,15 +699,15 @@
     assert "@" not in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_methods_paragraph_with_inline_equations_and_figure_refs(model):
     # from CCC manuscript
     paragraph = r"""
 The Clustermatch Correlation Coefficient (CCC) computes a similarity value $c \in \left[0,1\right]$ between any pair of numerical or categorical features/variables $\mathbf{x}$ and $\mathbf{y}$ measured on $n$ objects.
@@ -1029,15 +755,15 @@
     assert "Figure @fig:datasets_rel" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_methods_paragraph_with_figure_table_and_equation_refs(model):
     # from PhenoPLIER manuscript:
     paragraph = r"""
 Note that, since we used the MultiXcan regression model (Equation (@eq:multixcan)), $\mathbf{R}$ is only an approximation of gene correlations in S-MultiXcan.
@@ -1091,15 +817,15 @@
     assert "[Supplementary Note 1](#sm:reg:null_sim)" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_methods_paragraph_with_inline_math_and_equations(model):
     # from PhenoPLIER manuscript:
     paragraph = r"""
 S-PrediXcan [@doi:10.1038/s41467-018-03621-1] is the summary version of PrediXcan [@doi:10.1038/ng.3367].
@@ -1156,15 +882,15 @@
     assert "$\hat{\sigma}_a$" in paragraph_revised
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_methods_paragraph_without_fig_table_reference(model):
     # from LLM for articles revision manuscript
     paragraph = r"""
 We used the OpenAI API for access to large language models, with a focus on the completion endpoints.
@@ -1208,15 +934,15 @@
     assert "@" not in paragraph_revised.lower()
 
 
 @pytest.mark.parametrize(
     "model",
     [
         GPT3CompletionModel(None, None),
-        GPT3CompletionModel(None, None, edit_endpoint=True),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
         GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
     ],
 )
 def test_revise_methods_paragraph_with_many_tokens(model):
     # from PhenoPLIER manuscript:
     paragraph = r"""
 Since the error terms $\bm{\epsilon}$ could be correlated, we cannot assume they have independent normal distributions as in a standard linear regression model.
@@ -1302,59 +1028,7 @@
     # revised paragraph was finished (no incomplete sentences, which could happen
     # if the max_tokens parameter is too low)
     assert (paragraph_revised[-1] == ".") or (paragraph_revised[-1] == "}")
 
     # some equations are referenced in the revised text
     assert "$$ {#eq:reg:r}" in paragraph_revised
     assert "$Cor(\mathbf{P}_{i}, \mathbf{P}_{j})" in paragraph_revised
-
-
-def test_revise_paragraph_too_few_sentences():
-    # from LLM for articles revision manuscript
-    paragraph = r"""
-Since the gold standard of drug-disease medical indications is described with Disease Ontology IDs (DOID) [@doi:10.1093/nar/gky1032], we mapped PhenomeXcan traits to the Experimental Factor Ontology [@doi:10.1093/bioinformatics/btq099] using [@url:https://github.com/EBISPOT/EFO-UKB-mappings], and then to DOID.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    assert len(paragraph) == 1
-
-    model = RandomManuscriptRevisionModel()
-
-    paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, model, "methods"
-    )
-    assert paragraph_text is not None
-    assert isinstance(paragraph_text, str)
-
-    assert paragraph_revised is not None
-    assert isinstance(paragraph_revised, str)
-    assert paragraph_revised == paragraph_text
-    assert len(paragraph_revised) > 10
-    assert "<!--\nERROR:" not in paragraph_revised
-
-
-def test_revise_paragraph_too_few_words():
-    # from LLM for articles revision manuscript
-    paragraph = r"""
-We ran our regression model for all 987 LVs across the 4,091 traits in PhenomeXcan.
-For replication, we ran the model in the 309 phecodes in eMERGE.
-We adjusted the $p$-values using the Benjamini-Hochberg procedure.
-    """.strip().split(
-        "\n"
-    )
-    paragraph = [sentence.strip() for sentence in paragraph]
-    assert len(paragraph) == 3
-
-    model = RandomManuscriptRevisionModel()
-
-    paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
-        paragraph, model, "methods"
-    )
-    assert paragraph_text is not None
-    assert isinstance(paragraph_text, str)
-
-    assert paragraph_revised is not None
-    assert isinstance(paragraph_revised, str)
-    assert paragraph_revised == paragraph_text
-    assert len(paragraph_revised) > 10
-    assert "<!--\nERROR:" not in paragraph_revised
```

### Comparing `manubot-ai-editor-0.4.5/tests/test_editor.py` & `manubot-ai-editor-0.4.6/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.5/tests/test_model_get_prompt.py` & `manubot-ai-editor-0.4.6/tests/test_model_get_prompt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,91 @@
 from unittest import mock
 
 from manubot_ai_editor import env_vars
 from manubot_ai_editor.models import GPT3CompletionModel
 
 
+def test_get_prompt_for_abstract():
+    manuscript_title = "Title of the manuscript to be revised"
+    manuscript_keywords = ["keyword0", "keyword1", "keyword2"]
+
+    model = GPT3CompletionModel(
+        title=manuscript_title,
+        keywords=manuscript_keywords,
+    )
+
+    paragraph_text = "Text of the abstract"
+
+    prompt = model.get_prompt(paragraph_text, "abstract")
+    assert prompt is not None
+    assert isinstance(prompt, str)
+    assert "abstract" in prompt
+    assert f"'{manuscript_title}'" in prompt
+    assert f"{manuscript_keywords[0]}" in prompt
+    assert f"{manuscript_keywords[1]}" in prompt
+    assert f"{manuscript_keywords[2]}" in prompt
+    assert paragraph_text in prompt
+    assert prompt.startswith("Revise")
+    assert "  " not in prompt
+
+
+def test_get_prompt_for_abstract_edit_endpoint():
+    manuscript_title = "Title of the manuscript to be revised"
+    manuscript_keywords = ["keyword0", "keyword1", "keyword2"]
+
+    model = GPT3CompletionModel(
+        title=manuscript_title,
+        keywords=manuscript_keywords,
+        model_engine="text-davinci-edit-001",
+    )
+
+    paragraph_text = "Text of the abstract. "
+
+    instruction, paragraph = model.get_prompt(paragraph_text, "abstract")
+    assert instruction is not None
+    assert isinstance(instruction, str)
+    assert paragraph is not None
+    assert isinstance(paragraph, str)
+
+    assert "this paragraph" in instruction
+    assert "abstract" in instruction
+    assert f"'{manuscript_title}'" in instruction
+    assert f"{manuscript_keywords[0]}" in instruction
+    assert f"{manuscript_keywords[1]}" in instruction
+    assert f"{manuscript_keywords[2]}" in instruction
+    assert "  " not in instruction
+    assert instruction.startswith("Revise")
+
+    assert paragraph_text.strip() == paragraph
+
+
+def test_get_prompt_for_introduction():
+    manuscript_title = "Title of the manuscript to be revised"
+    manuscript_keywords = ["keyword0", "keyword1", "keyword2"]
+
+    model = GPT3CompletionModel(
+        title=manuscript_title,
+        keywords=manuscript_keywords,
+    )
+
+    paragraph_text = "Text of the initial part"
+
+    prompt = model.get_prompt(paragraph_text, "introduction")
+    assert prompt is not None
+    assert isinstance(prompt, str)
+    assert "Introduction" in prompt
+    assert f"'{manuscript_title}'" in prompt
+    assert f"{manuscript_keywords[0]}" in prompt
+    assert f"{manuscript_keywords[1]}" in prompt
+    assert f"{manuscript_keywords[2]}" in prompt
+    assert paragraph_text in prompt
+    assert prompt.startswith("Revise")
+    assert "  " not in prompt
+
+
 def test_get_prompt_section_is_abstract():
     model = GPT3CompletionModel(
         title="Test title",
         keywords=["test", "keywords"],
     )
 
     paragraph_text = """
```

