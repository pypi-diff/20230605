# Comparing `tmp/gpt4-api-0.1.5.tar.gz` & `tmp/gpt4-api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.5.tar", last modified: Fri Jun  2 05:45:24 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.1.6.tar", last modified: Mon Jun  5 02:38:41 2023, max compression
```

## Comparing `gpt4-api-0.1.5.tar` & `gpt4-api-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.5/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    16517 2023-06-02 05:45:06.000000 gpt4-api-0.1.5/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-02 05:45:24.000000 gpt4-api-0.1.5/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.5/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.6/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    16649 2023-06-05 02:35:42.000000 gpt4-api-0.1.6/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-05 02:38:41.000000 gpt4-api-0.1.6/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.6/setup.py
```

### Comparing `gpt4-api-0.1.5/api/gpt.py` & `gpt4-api-0.1.6/api/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 import threading
 import logging
 import time
 import openai
 import asyncio
 from pathlib import Path
 from multiprocessing import JoinableQueue
@@ -58,27 +56,31 @@
                 content = task.get("ask")
                 messages = task.get("messages")
                 if "retry" not in task:
                     task["retry"] = False
                 run_func(task, content, messages)
                 self.task_queue.task_done()
             except Empty:
+                logging.info("The queue has no content anymore")
+                break
+            except Exception as e:
+                logging.error(e)
                 break
 
     def __run_tasks(self, tasks, run_func):
         threads = []
         logging.info("Total threads: %s" % self.num_threads)
         for _ in range(self.num_threads):
             thread = threading.Thread(target=self.__worker, args=(run_func,))
             thread.start()
             threads.append(thread)
         logging.info("Total tasks: %s" % len(tasks))
         for task in tasks:
             self.task_queue.put(task)
-        self.task_queue.join()
+        # self.task_queue.join()
         for thread in threads:
             thread.join()
 
     @staticmethod
     def process_token(keys):
         usable_openai_keys = []
         for key in keys:
```

### Comparing `gpt4-api-0.1.5/setup.py` & `gpt4-api-0.1.6/setup.py`

 * *Files identical despite different names*

