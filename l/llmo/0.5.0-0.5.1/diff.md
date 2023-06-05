# Comparing `tmp/llmo-0.5.0.tar.gz` & `tmp/llmo-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.5.0.tar", last modified: Sat May 27 20:01:25 2023, max compression
+gzip compressed data, was "llmo-0.5.1.tar", last modified: Mon Jun  5 21:55:12 2023, max compression
```

## Comparing `llmo-0.5.0.tar` & `llmo-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.5.0/LICENSE
--rw-r--r--   0        0        0     2374 2023-05-26 15:57:37.255918 llmo-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.5.0/llmo/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.5.0/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.5.0/llmo/constants.py
--rw-r--r--   0        0        0     9835 2023-05-27 19:43:28.486609 llmo-0.5.0/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.5.0/llmo/layout.css
--rw-r--r--   0        0        0     5957 2023-05-27 19:43:28.491411 llmo-0.5.0/llmo/llms.py
--rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.5.0/llmo/shell_mode.py
--rw-r--r--   0        0        0      722 2023-05-27 20:01:25.439524 llmo-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.5.0/tests/test_openai.py
--rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 llmo-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2374 2023-05-26 15:57:37.255918 llmo-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.5.1/llmo/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.5.1/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.5.1/llmo/constants.py
+-rw-r--r--   0        0        0     9835 2023-06-05 21:39:29.568488 llmo-0.5.1/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.5.1/llmo/layout.css
+-rw-r--r--   0        0        0     5945 2023-06-05 21:39:47.303463 llmo-0.5.1/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.5.1/llmo/shell_mode.py
+-rw-r--r--   0        0        0      722 2023-06-05 21:55:12.133340 llmo-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      844 2023-06-05 21:39:47.300280 llmo-0.5.1/tests/test_openai.py
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 llmo-0.5.1/PKG-INFO
```

### Comparing `llmo-0.5.0/LICENSE` & `llmo-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.5.0/README.md` & `llmo-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.5.0/llmo/cli.py` & `llmo-0.5.1/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.5.0/llmo/gui.py` & `llmo-0.5.1/llmo/gui.py`

 * *Files identical despite different names*

### Comparing `llmo-0.5.0/llmo/llms.py` & `llmo-0.5.1/llmo/llms.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                     # If a file message was removed, continue to the next iteration
                     continue
 
                 estimated_tokens -= (
                     len(removed_message["content"]) / ESTIMATED_CHAR_PER_TOKEN
                 )
 
-    async def _prepare_messages(self, files, prompt):
+    def _prepare_messages(self, files, prompt):
         for file in files or []:
             # remove any existing messages with the same file content
             temp_messages = copy(self.messages)
             for msg in temp_messages:
                 if msg["role"] == "user" and msg["content"].startswith(f"`{file}`"):
                     self.messages.remove(msg)
             # add file content to messages
@@ -123,15 +123,15 @@
     @retry_openai_call
     async def asubmit(self, prompt: str, files: Iterable[Path] = None):
         """
         Submit a prompt to the OpenAI API and asynchronously yield tokens.
 
         If files are provided, they will be added to the prompt as part of the submission.
         """
-        messages = await self._prepare_messages(files, prompt)
+        messages = self._prepare_messages(files, prompt)
 
         events = openai.ChatCompletion.create(
             messages=messages,
             model=self.model,
             temperature=self.temperature,
             stream=True,
         )
```

### Comparing `llmo-0.5.0/llmo/shell_mode.py` & `llmo-0.5.1/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.5.0/tests/test_openai.py` & `llmo-0.5.1/tests/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def test_remove_personality(openai):
     openai.add_personality()
     openai.remove_personality()
     assert openai.personality_prompt not in openai.system_prompt
 
 
-def test_submit(openai, monkeypatch):
+async def test_submit(openai, monkeypatch):
     def mock_completion(*args, **kwargs):
         return {"choices": [
             {"message": {"role": "assistant", "content": "Python:\n```python\nprint('Hello, World!')\n```"}}]}
 
     monkeypatch.setattr("llmo.llms.openai.ChatCompletion.create", mock_completion)
     response = openai.submit("How to print 'Hello, World!' in Python?")
     assert "Python:\n```python\nprint('Hello, World!')\n```" in response
```

### Comparing `llmo-0.5.0/PKG-INFO` & `llmo-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.5.0
+Version: 0.5.1
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

