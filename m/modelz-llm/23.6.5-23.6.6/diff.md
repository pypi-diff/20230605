# Comparing `tmp/modelz-llm-23.6.5.tar.gz` & `tmp/modelz-llm-23.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.5.tar", last modified: Fri Jun  2 08:42:08 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.6.tar", last modified: Mon Jun  5 07:32:08 2023, max compression
```

## Comparing `modelz-llm-23.6.5.tar` & `modelz-llm-23.6.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.351405 modelz-llm-23.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 07:31:49.000000 modelz-llm-23.6.6/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:32:08.355405 modelz-llm-23.6.6/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 07:32:08.000000 modelz-llm-23.6.6/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.5/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.6/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/.github/workflows/gcr.yml` & `modelz-llm-23.6.6/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/.github/workflows/python-check.yml` & `modelz-llm-23.6.6/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/.github/workflows/python-publish.yml` & `modelz-llm-23.6.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/.gitignore` & `modelz-llm-23.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/PKG-INFO` & `modelz-llm-23.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.5
+Version: 23.6.6
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.5 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.6 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.5/README.md` & `modelz-llm-23.6.6/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/build.envd` & `modelz-llm-23.6.6/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/client.py` & `modelz-llm-23.6.6/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/images/base/Dockerfile` & `modelz-llm-23.6.6/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.6/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.6/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/images/llama-7b/Dockerfile` & `modelz-llm-23.6.6/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.6/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/pyproject.toml` & `modelz-llm-23.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/src/modelz_llm/cli.py` & `modelz-llm-23.6.6/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.6/src/modelz_llm/falcon_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,27 +47,41 @@
 
 
 class LLM:
     def __init__(self, model_name: str, device: str) -> None:
         self.model_name = model_name
         self.model_spec = LanguageModels.find(model_name).value
         tokenizer_cls = getattr(transformers, self.model_spec.tokenizer_cls)
+
         self.tokenizer = tokenizer_cls.from_pretrained(
-            model_name, trust_remote_code=True, low_cpu_mem_usage=True
+            model_name,
+            trust_remote_code=True,
+            low_cpu_mem_usage=self.model_spec.low_cpu_mem_usage,
         )
         model_cls = getattr(transformers, self.model_spec.transformer_model_cls)
         self.model = model_cls.from_pretrained(
-            model_name, trust_remote_code=True, low_cpu_mem_usage=True
+            model_name,
+            trust_remote_code=True,
+            low_cpu_mem_usage=self.model_spec.low_cpu_mem_usage,
         )
         if device == "auto":
             self.device = (
                 torch.cuda.current_device() if torch.cuda.is_available() else "cpu"
             )
         else:
             self.device = device
+
+        try:
+            if self.device == "cpu":
+                self.model = self.model.float()
+            else:
+                self.model = self.model.half()
+        except Exception as err:
+            logger.debug("failed to convert the model: %s", err)
+
         self.model = self.model.to(self.device)
         self.model.eval()
 
     def __str__(self) -> str:
         return f"LLM(model={self.model}, tokenizer={self.tokenizer})"
 
     def token_encode(self, text: str):
@@ -82,14 +96,32 @@
 
     def generate(self, tokens, **kwargs):
         """Generate content with model."""
         inputs = tokens.to(self.device)
         outputs = self.model.generate(inputs, **kwargs).tolist()
         return outputs
 
+    def chat_completion(self, req: ChatCompletionRequest) -> ChatResponse:
+        """Generate ChatCompletionResponse for ChatCompletionRequest."""
+        if self.model_spec is not LanguageModels.CHAT_GLM.value:
+            return list(self.step_generate(req))[0]
+
+        tokens = self.token_encode(req.get_prompt(self.model_name))
+        input_length = len(tokens[0])
+        outputs = self.generate(tokens, **req.get_inference_args(self.model_name))[0]
+        message = self.token_decode(outputs[input_length:])
+        return ChatResponse.from_message(
+            message=message,
+            role=Role.ASSISTANT,
+            model=self.model_name,
+            finish_reason=None,
+            prompt_token=input_length,
+            completion_token=len(outputs) - input_length,
+        )
+
     def step_generate(self, req: ChatCompletionRequest, echo=False, stream_interval=1):
         """Ref to FastChat.
 
         https://github.com/lm-sys/FastChat/blob/8e38141ff5dd15f3138ccfd312dd73a471e986a1/fastchat/serve/inference.py#L58
         """
         prompt = req.get_prompt(self.model_name)
         input_ids = self.token_encode(prompt)
@@ -108,16 +140,19 @@
         else:
             stop_token_ids = self.token_encode(req.stop).tolist()[0]
         stop_token_ids.append(self.tokenizer.eos_token_id)
         stop_token = req.stop or self.tokenizer.eos_token
 
         output_ids = input_ids.tolist()[0]
 
+        is_encoder_decoder = getattr(self.model, "encoder", None) and getattr(
+            self.model, "decoder", None
+        )
         # encoding
-        if self.model_spec.is_encoder_decoder:
+        if is_encoder_decoder:
             max_src_len = CONTEXT_LEN
             input_ids = input_ids[-max_src_len:]
             encoder_output = self.model.encoder(
                 input_ids=torch.as_tensor(input_ids, device=self.device)
             )[0]
             start_ids = torch.as_tensor(
                 [[self.model.generation_config.decoder_start_token_id]],
@@ -126,29 +161,29 @@
             )
         else:
             max_src_len = CONTEXT_LEN - req.max_tokens - 8
 
         past_key_values = out = token = None
         for i in range(req.max_tokens):
             if i == 0:
-                if self.model_spec.is_encoder_decoder:
+                if is_encoder_decoder:
                     out = self.model.decoder(
                         input_ids=start_ids,
                         encoder_hidden_states=encoder_output,
                         use_cache=True,
                     )
                     logits = self.model.lm_head(out[0])
                 else:
                     out = self.model(
                         torch.as_tensor(input_ids, device=self.device), use_cache=True
                     )
                     logits = out.logits
                 past_key_values = out.past_key_values
             else:
-                if self.model_spec.is_encoder_decoder:
+                if is_encoder_decoder:
                     out = self.model.decoder(
                         input_ids=torch.as_tensor([[token]], device=self.device),
                         encoder_hidden_states=encoder_output,
                         use_cache=True,
                         past_key_values=past_key_values,
                     )
 
@@ -213,22 +248,14 @@
                                     break
                     else:
                         raise ValueError("Invalid stop field type.")
 
                 # prevent yielding partial stop sequence
                 if not partially_stopped:
                     pass
-                    # yield ChatResponse.from_message(
-                    #     output,
-                    #     Role.ASSISTANT,
-                    #     self.model_name,
-                    #     None,
-                    #     input_length,
-                    #     i,
-                    # )
 
             if stopped:
                 break
 
         # finish stream event, which contains finish reason
         if i == req.max_tokens - 1:
             finish_reason = "length"
@@ -271,27 +298,17 @@
         except msgspec.ValidationError as err:
             logger.info(f"Failed to parse request: {err}")
             # return 400 otherwise the client will retry
             resp.status = falcon.HTTP_400
             resp.data = ErrorResponse.from_validation_err(err, str(buf)).to_json()
             return
 
-        for comp in self.model.step_generate(chat_req):
-            logger.info(comp)
-            resp.data = comp.to_json()
-
-        # tokens = self.model.token_encode(chat_req.get_prompt(self.model_name))
-        # input_length = len(tokens[0])
-        # outputs = self.model.generate(tokens=tokens)[0]
-        # res = outputs[input_length:]
-        # msg = self.model.token_decode(res)
-        # completion = ChatResponse.from_message(
-        #     msg, Role.ASSISTANT, self.model_name, None, input_length, len(res)
-        # )
-        # resp.data = completion.to_json()
+        comp = self.model.chat_completion(chat_req)
+        logger.debug(comp)
+        resp.data = comp.to_json()
 
 
 class Completions:
     def __init__(self, model: LLM) -> None:
         self.model = model
         self.model_name = model.model_name
```

### Comparing `modelz-llm-23.6.5/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.6/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/src/modelz_llm/utils.py` & `modelz-llm-23.6.6/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.5/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.6/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.5
+Version: 23.6.6
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.5 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.6 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.5/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.6/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

