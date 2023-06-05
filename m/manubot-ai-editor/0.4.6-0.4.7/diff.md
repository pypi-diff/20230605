# Comparing `tmp/manubot-ai-editor-0.4.6.tar.gz` & `tmp/manubot-ai-editor-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manubot-ai-editor-0.4.6.tar", last modified: Mon Jun  5 14:58:45 2023, max compression
+gzip compressed data, was "manubot-ai-editor-0.4.7.tar", last modified: Mon Jun  5 16:22:40 2023, max compression
```

## Comparing `manubot-ai-editor-0.4.6.tar` & `manubot-ai-editor-0.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.6/README.md
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.707883 manubot-ai-editor-0.4.6/libs/
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/__init__.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     3604 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/env_vars.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20468 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/models.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor/utils.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/PKG-INFO
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      523 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/SOURCES.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/dependency_links.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/requires.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-05 14:58:45.000000 manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/top_level.txt
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/setup.cfg
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-05 14:58:43.000000 manubot-ai-editor-0.4.6/setup.py
-drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 14:58:45.711883 manubot-ai-editor-0.4.6/tests/
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.6/tests/test_editor.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     8306 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_basics.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    10320 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_get_prompt.py
--rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    51084 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.6/tests/test_model_revision.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2062 2023-06-01 16:26:59.000000 manubot-ai-editor-0.4.7/README.md
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/libs/
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        0 2023-01-26 21:56:19.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/__init__.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    16883 2023-06-01 19:57:14.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     3604 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/env_vars.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    20603 2023-06-05 15:42:37.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/models.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      632 2023-06-05 15:49:50.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor/utils.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     2544 2023-06-05 16:22:40.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/PKG-INFO
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      523 2023-06-05 16:22:40.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/SOURCES.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)        1 2023-06-05 16:22:40.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/dependency_links.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       20 2023-06-05 16:22:40.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/requires.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       19 2023-06-05 16:22:40.000000 manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/top_level.txt
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)       38 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/setup.cfg
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)      938 2023-06-05 16:22:33.000000 manubot-ai-editor-0.4.7/setup.py
+drwxrwxr-x   0 miltondp  (1000) miltondp  (1000)        0 2023-06-05 16:22:40.236614 manubot-ai-editor-0.4.7/tests/
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    41575 2023-06-01 19:57:26.000000 manubot-ai-editor-0.4.7/tests/test_editor.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)     8306 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.7/tests/test_model_basics.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    10320 2023-06-05 14:55:25.000000 manubot-ai-editor-0.4.7/tests/test_model_get_prompt.py
+-rw-rw-r--   0 miltondp  (1000) miltondp  (1000)    54774 2023-06-05 16:21:14.000000 manubot-ai-editor-0.4.7/tests/test_model_revision.py
```

### Comparing `manubot-ai-editor-0.4.6/PKG-INFO` & `manubot-ai-editor-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.6/README.md` & `manubot-ai-editor-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/editor.py` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor/editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/env_vars.py` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor/env_vars.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/models.py` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,33 +266,31 @@
             ("Revise...") and the paragraph to revise.
 
             If self.endpoint == "edits", then returns a tuple with two strings:
              1) the instructions to be used by the model for the revision of the paragraph,
              2) the paragraph to revise.
         """
 
-        if env_vars.CUSTOM_PROMPT in os.environ:
+        if env_vars.CUSTOM_PROMPT in os.environ and os.environ[env_vars.CUSTOM_PROMPT].strip() != "":
             prompt = os.environ[env_vars.CUSTOM_PROMPT]
             print(
                 f"Using custom prompt from environment variable '{env_vars.CUSTOM_PROMPT}'"
             )
 
             placeholders = {
                 "paragraph_text": paragraph_text,
                 "section_name": section_name,
                 "title": self.title,
                 "keywords": ", ".join(self.keywords),
             }
 
-            if "{paragraph_text}" not in prompt:
-                prompt += ":\n\n{paragraph_text}"
-
-            return prompt.format(**placeholders)
-
-        if section_name in ("abstract",):
+            # FIXME: if {paragraph_text} is in the prompt, this won't work for the edits endpoint
+            #  a simple workaround is to remove {paragraph_text} from the prompt
+            prompt = prompt.format(**placeholders)
+        elif section_name in ("abstract",):
             prompt = f"""
                 Revise the following paragraph from the {section_name} of an academic paper (with the title '{self.title}' and keywords '{", ".join(self.keywords)}')
                 so the research problem/question is clear,
                    the solution proposed is clear,
                    the text grammar is correct, spelling errors are fixed,
                    and the text is in active voice and has a clear sentence structure
             """
```

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor/utils.py` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor/utils.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/PKG-INFO` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manubot-ai-editor
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Manubot plugin to revise a manuscript using GPT-3
 Home-page: https://github.com/greenelab/manubot-ai-editor
 Author: Milton Pividori
 Author-email: miltondp@gmail.com
 License: BSD-2-Clause Plus Patent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `manubot-ai-editor-0.4.6/libs/manubot_ai_editor.egg-info/SOURCES.txt` & `manubot-ai-editor-0.4.7/libs/manubot_ai_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/setup.py` & `manubot-ai-editor-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # twine upload dist/*
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="manubot-ai-editor",
-    version="0.4.6",
+    version="0.4.7",
     author="Milton Pividori",
     author_email="miltondp@gmail.com",
     description="A Manubot plugin to revise a manuscript using GPT-3",
     license="BSD-2-Clause Plus Patent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greenelab/manubot-ai-editor",
```

### Comparing `manubot-ai-editor-0.4.6/tests/test_editor.py` & `manubot-ai-editor-0.4.7/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/tests/test_model_basics.py` & `manubot-ai-editor-0.4.7/tests/test_model_basics.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/tests/test_model_get_prompt.py` & `manubot-ai-editor-0.4.7/tests/test_model_get_prompt.py`

 * *Files identical despite different names*

### Comparing `manubot-ai-editor-0.4.6/tests/test_model_revision.py` & `manubot-ai-editor-0.4.7/tests/test_model_revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """
 These tests need to call the OpenAI API, so they are in a separate file and can incur costs.
 """
+import difflib
+from unittest import mock
+
 import pytest
 
+from manubot_ai_editor import env_vars
 from manubot_ai_editor.editor import ManuscriptEditor
 from manubot_ai_editor.models import GPT3CompletionModel
 from manubot_ai_editor.utils import starts_with_similar
 
 
 @pytest.mark.parametrize(
     "model",
@@ -48,14 +52,86 @@
     assert paragraph_text is not None
     assert paragraph_revised is not None
     assert isinstance(paragraph_revised, str)
     assert paragraph_revised != paragraph_text
     assert len(paragraph_revised) > 100
     assert "<!--\nERROR:" not in paragraph_revised
 
+    # # original and revised paragraph should be quite different
+    # _ratio = difflib.SequenceMatcher(lambda x: x in (" ", "\n",), paragraph_text, paragraph_revised).ratio()
+    # assert _ratio < 0.10 if model.endpoint != "edits" else 1.0, _ratio
+
+    # revised paragraph was finished (no incomplete sentences, which could happen
+    # if the max_tokens parameter is too low)
+    assert paragraph_revised[-1] == "."
+
+    # most citations were kept in the revised text
+    assert "[" not in paragraph_revised
+    assert "@" not in paragraph_revised
+
+    # no references to figures or tables
+    assert "Figure" not in paragraph_revised
+    assert "Table" not in paragraph_revised
+
+    # no math
+    assert "$" not in paragraph_revised
+
+
+@mock.patch.dict(
+    "os.environ",
+    {env_vars.CUSTOM_PROMPT: "proofread the following paragraph"},
+)
+@pytest.mark.parametrize(
+    "model",
+    [
+        GPT3CompletionModel(None, None),
+        GPT3CompletionModel(None, None, model_engine="text-davinci-edit-001"),
+        GPT3CompletionModel(None, None, model_engine="gpt-3.5-turbo"),
+    ],
+)
+def test_revise_abstract_ccc_with_custom_prompt(model):
+    # from CCC manuscript
+    paragraph = r"""
+Correlation coefficients are widely used to identify patterns in data that may be of particular interest.
+In transcriptomics, genes with correlated expression often share functions or are part of disease-relevant biological processes.
+Here we introduce the Clustermatch Correlation Coefficient (CCC), an efficient, easy-to-use and not-only-linear coefficient based on machine learning models.
+CCC reveals biologically meaningful linear and nonlinear patterns missed by standard, linear-only correlation coefficients.
+CCC captures general patterns in data by comparing clustering solutions while being much faster than state-of-the-art coefficients such as the Maximal Information Coefficient.
+When applied to human gene expression data, CCC identifies robust linear relationships while detecting nonlinear patterns associated, for example, with sex differences that are not captured by linear-only coefficients.
+Gene pairs highly ranked by CCC were enriched for interactions in integrated networks built from protein-protein interaction, transcription factor regulation, and chemical and genetic perturbations, suggesting that CCC could detect functional relationships that linear-only methods missed.
+CCC is a highly-efficient, next-generation not-only-linear correlation coefficient that can readily be applied to genome-scale data and other domains across different data types.
+        """.strip().split(
+        "\n"
+    )
+    paragraph = [sentence.strip() for sentence in paragraph]
+    assert len(paragraph) == 8
+
+    model.title = (
+        "An efficient not-only-linear correlation coefficient based on machine learning"
+    )
+    model.keywords = [
+        "correlation coefficient",
+        "nonlinear relationships",
+        "gene expression",
+    ]
+
+    paragraph_text, paragraph_revised = ManuscriptEditor.revise_and_write_paragraph(
+        paragraph, model, "abstract"
+    )
+    assert paragraph_text is not None
+    assert paragraph_revised is not None
+    assert isinstance(paragraph_revised, str)
+    assert paragraph_revised != paragraph_text
+    assert len(paragraph_revised) > 100
+    assert "<!--\nERROR:" not in paragraph_revised
+
+    # # since the custom prompt also "proofreads", the similarity between input and revised text should be very high
+    # _ratio = difflib.SequenceMatcher(lambda x: x in (" ", "\n",), paragraph_text, paragraph_revised).ratio()
+    # assert _ratio > 0.50, _ratio
+
     # revised paragraph was finished (no incomplete sentences, which could happen
     # if the max_tokens parameter is too low)
     assert paragraph_revised[-1] == "."
 
     # most citations were kept in the revised text
     assert "[" not in paragraph_revised
     assert "@" not in paragraph_revised
```

