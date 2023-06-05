# Comparing `tmp/gpt4-api-0.1.6.tar.gz` & `tmp/gpt4-api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.6.tar", last modified: Mon Jun  5 02:38:41 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.1.7.tar", last modified: Mon Jun  5 10:25:37 2023, max compression
```

## Comparing `gpt4-api-0.1.6.tar` & `gpt4-api-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.6/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    16649 2023-06-05 02:35:42.000000 gpt4-api-0.1.6/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.6/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.7/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    16557 2023-06-05 10:25:20.000000 gpt4-api-0.1.7/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.7/setup.py
```

### Comparing `gpt4-api-0.1.6/api/gpt.py` & `gpt4-api-0.1.7/api/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,46 +43,52 @@
         # 要生成的文本的数量。默认为1，表示生成一段文本
         self.n = n
         # 是否将生成的文本作为流返回，而不是一次性返回所有文本。默认为False，表示一次性返回所有文本
         # 系统默认内容
         self.system_content = system_content
         self.total_tokens = 0
         self.call_back = call_back
+        self.threads = []
 
     def __worker(self, run_func):
         logging.disable(logging.NOTSET)
         while True:
             try:
                 task = self.task_queue.get(timeout=1)
                 content = task.get("ask")
                 messages = task.get("messages")
                 if "retry" not in task:
                     task["retry"] = False
+                logging.info("active threads: %s" % self.get_active_thread_count())
                 run_func(task, content, messages)
                 self.task_queue.task_done()
             except Empty:
-                logging.info("The queue has no content anymore")
                 break
             except Exception as e:
                 logging.error(e)
                 break
 
     def __run_tasks(self, tasks, run_func):
-        threads = []
-        logging.info("Total threads: %s" % self.num_threads)
-        for _ in range(self.num_threads):
-            thread = threading.Thread(target=self.__worker, args=(run_func,))
-            thread.start()
-            threads.append(thread)
-        logging.info("Total tasks: %s" % len(tasks))
-        for task in tasks:
-            self.task_queue.put(task)
-        # self.task_queue.join()
-        for thread in threads:
-            thread.join()
+        if len(self.threads) == 0:
+            logging.info("Total threads: %s" % self.num_threads)
+            for _ in range(self.num_threads):
+                thread = threading.Thread(target=self.__worker, args=(run_func,))
+                thread.start()
+                self.threads.append(thread)
+            logging.info("Total tasks: %s" % len(tasks))
+            for task in tasks:
+                self.task_queue.put(task)
+            # self.task_queue.join()
+            for thread in self.threads:
+                thread.join()
+            logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
+        else:
+            logging.info("Successfully added tasks for the second time, totaling: %s" % len(tasks))
+            for task in tasks:
+                self.task_queue.put(task)
 
     @staticmethod
     def process_token(keys):
         usable_openai_keys = []
         for key in keys:
             usable_openai_keys.append({"api_key": key, "token_limit": 0})
         if len(usable_openai_keys) == 0:
@@ -127,20 +133,15 @@
         return self.task_queue.empty()
 
     def add_task(self, tasks):
         if tasks is None:
             tasks = []
         if len(tasks) == 0:
             logging.info("The second additional task is empty")
-        logging.info("Successfully added tasks for the second time, totaling: %s" % len(tasks))
-        if self.get_active_thread_count() <= 0 or self.task_is_empty():
-            self.task_run_tasks(tasks=tasks)
-        else:
-            for task in tasks:
-                self.task_queue.put(task)
+        self.task_run_tasks(tasks=tasks)
 
     def __process_task(self, task, ask_content, messages, retries=1):
         open_ai_key = self.__get_key()
         if open_ai_key:
             case_name = task.get("case", None)
             need_system = task.get("need_system", False)
             call_back_func = task.get("call_back", None)
@@ -169,17 +170,14 @@
                 logging.info("request case %s cost time: %s second" % (case_name, int(elapsed_time)))
                 logging.info("prompt tokens: %s" % prompt_tokens)
                 logging.info("completion tokens: %s" % completion_tokens)
                 logging.info("total tokens: %s" % total_tokens)
                 for openaiKey in self.usable_openai_keys:
                     if openaiKey.get("api_key", None) == open_ai_key:
                         openaiKey["token_limit"] += total_tokens
-                logging.info("active threads: %s" % self.get_active_thread_count())
-                if self.task_is_empty():
-                    logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
                 if call_back_func and self.call_back:
                     call_back_func = self.call_back.get(call_back_func, None)
                     if call_back_func:
                         call_back_func(call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name))
             except openai.error.RateLimitError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
                 self.__release_token(open_ai_key)
```

### Comparing `gpt4-api-0.1.6/setup.py` & `gpt4-api-0.1.7/setup.py`

 * *Files identical despite different names*

