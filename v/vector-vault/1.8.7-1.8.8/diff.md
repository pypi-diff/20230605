# Comparing `tmp/vector_vault-1.8.7.tar.gz` & `tmp/vector_vault-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.7.tar", last modified: Sun Jun  4 23:35:41 2023, max compression
+gzip compressed data, was "vector_vault-1.8.8.tar", last modified: Mon Jun  5 02:11:12 2023, max compression
```

## Comparing `vector_vault-1.8.7.tar` & `vector_vault-1.8.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.067160 vector_vault-1.8.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:35:41.066989 vector_vault-1.8.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 23:35:41.067198 vector_vault-1.8.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 23:35:34.000000 vector_vault-1.8.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.063967 vector_vault-1.8.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 23:35:41.000000 vector_vault-1.8.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 23:35:41.066665 vector_vault-1.8.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    10755 2023-06-04 18:24:37.000000 vector_vault-1.8.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-04 22:09:16.000000 vector_vault-1.8.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.7/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    28069 2023-06-04 23:35:21.000000 vector_vault-1.8.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-1.8.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.628578 vector_vault-1.8.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-05 02:11:12.628430 vector_vault-1.8.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-05 02:11:12.628620 vector_vault-1.8.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-05 02:10:45.000000 vector_vault-1.8.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.626680 vector_vault-1.8.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.628230 vector_vault-1.8.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13363 2023-06-05 02:09:13.000000 vector_vault-1.8.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-05 02:10:12.000000 vector_vault-1.8.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-05 02:10:06.000000 vector_vault-1.8.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.8/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    27815 2023-06-05 02:10:21.000000 vector_vault-1.8.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-1.8.8/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.8/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.7/LICENSE` & `vector_vault-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/PKG-INFO` & `vector_vault-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.7
+Version: 1.8.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.7/README.md` & `vector_vault-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/setup.py` & `vector_vault-1.8.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.7",
+    version="1.8.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.8/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.7
+Version: 1.8.8
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.7/vectorvault/__init__.py` & `vector_vault-1.8.8/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/cloudmanager.py` & `vector_vault-1.8.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/creds.py` & `vector_vault-1.8.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/download.py` & `vector_vault-1.8.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/itemize.py` & `vector_vault-1.8.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/signup.py` & `vector_vault-1.8.8/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/vault.py` & `vector_vault-1.8.8/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,35 +431,33 @@
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
-                        if self.ai.get_tokens(user_input) > 4000:
-                            user_input = user_input[-13000:]
                         if include_context_meta:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                             for text in context:
                                 input_ += text['data']
                         response = self.ai.llm_w_context(segment, input_, history, model=model)
                     else:
                         response = self.ai.llm(segment, history, model=model)
                     break
                 except Exception as e:
                     exception += 1
+                    print(traceback.format_exc())
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     if exceptions >= 5:
                         print(f"API Failed too many times, exiting loop: {e}.")
                         break
-                    print(traceback.format_exc())
                     time.sleep(5)
                     
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
@@ -552,16 +550,14 @@
                         user_input = segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
-                        if self.ai.get_tokens(user_input) > 4000:
-                            user_input = user_input[-13000:]
                         if include_context_meta:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
```

### Comparing `vector_vault-1.8.7/vectorvault/vecreq.py` & `vector_vault-1.8.8/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.7/vectorvault/wrap.py` & `vector_vault-1.8.8/vectorvault/wrap.py`

 * *Files identical despite different names*

