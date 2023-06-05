# Comparing `tmp/chatgpt-klient-0.0.2.tar.gz` & `tmp/chatgpt-klient-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.2.tar", last modified: Fri Jun  2 10:22:06 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.0.3.tar", last modified: Mon Jun  5 11:40:09 2023, max compression
```

## Comparing `chatgpt-klient-0.0.2.tar` & `chatgpt-klient-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.494628 chatgpt-klient-0.0.2/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.2/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-06-02 10:20:12.000000 chatgpt-klient-0.0.2/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-02 10:22:06.494628 chatgpt-klient-0.0.2/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.486628 chatgpt-klient-0.0.2/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-06-02 10:20:30.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5338 2023-06-02 10:11:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.2/src/chatgpt_klient/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-02 10:22:06.490628 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-06-02 10:22:06.000000 chatgpt-klient-0.0.2/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-05 11:40:09.042482 chatgpt-klient-0.0.3/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-05 11:40:09.042482 chatgpt-klient-0.0.3/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.3/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-06-05 11:01:26.000000 chatgpt-klient-0.0.3/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-06-05 11:40:09.042482 chatgpt-klient-0.0.3/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-05 11:40:09.034482 chatgpt-klient-0.0.3/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-05 11:40:09.042482 chatgpt-klient-0.0.3/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-06-05 11:01:36.000000 chatgpt-klient-0.0.3/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5457 2023-06-05 11:01:01.000000 chatgpt-klient-0.0.3/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.3/src/chatgpt_klient/consts.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-06-05 11:40:09.042482 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-06-05 11:40:09.000000 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-06-05 11:40:09.000000 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-06-05 11:40:09.000000 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-06-05 11:40:09.000000 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-06-05 11:40:09.000000 chatgpt-klient-0.0.3/src/chatgpt_klient.egg-info/top_level.txt
```

### Comparing `chatgpt-klient-0.0.2/src/chatgpt_klient/client.py` & `chatgpt-klient-0.0.3/src/chatgpt_klient/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,28 @@
         if engine not in ENGINES0 + ENGINES1:
             logger.error(f"Engine {engine} is not supported")
             raise Exception("Engine not supported")
         self.engine = engine
         self.encoding = tiktoken.encoding_for_model(self.engine)
         self.max_tokens = int(MAX_TOKENS[self.engine] / 2)
 
+
+    def set_system_directive(self, directive: str):
+        self.msg_history = {"messages": [], "tokens": []}
+        self.msg_history["messages"].append(
+            {
+                "role": "system",
+                "content": directive,
+            }
+        )
+        self.msg_history["tokens"].append(
+            len(self.encoding.encode(directive))
+        )
+
+
     def get_max_tokens_allowed(self):
         return min(self.max_tokens, MAX_TOKENS[self.engine])
 
     def send_prompt(self, text=None, max_tokens=None):
         response = "No response"
         if self.engine in ENGINES0:
             r = self.openai.Completion.create(
@@ -88,23 +102,15 @@
 
         else:
             logger.warning(f"Engine {self.engine} not supported")
         return response
 
     def interactive_prompt(self, system_directive: str | None = None, max_tokens=None):
         if system_directive:
-            self.msg_history["messages"].append(
-                {
-                    "role": "system",
-                    "content": system_directive,
-                }
-            )
-            self.msg_history["tokens"].append(
-                len(self.encoding.encode(system_directive))
-            )
+            self.set_system_directive(system_directive)
         console.print("###########", style="bold")
         console.print("# ChatGPT #", style="bold")
         console.print("###########", style="bold")
         console.print(
             f"[bold yellow]Engine:[/bold yellow] {self.engine}", highlight=False
         )
         console.print("[bold cyan]Enter 'q'/'quit' to exit the chat[/]")
```

### Comparing `chatgpt-klient-0.0.2/src/chatgpt_klient/consts.py` & `chatgpt-klient-0.0.3/src/chatgpt_klient/consts.py`

 * *Files identical despite different names*

