# Comparing `tmp/custom_secrets_manager-1.0.2.tar.gz` & `tmp/custom_secrets_manager-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_secrets_manager-1.0.2.tar", last modified: Sat Jun  3 22:04:37 2023, max compression
+gzip compressed data, was "custom_secrets_manager-1.0.3a0.tar", last modified: Mon Jun  5 17:03:42 2023, max compression
```

## Comparing `custom_secrets_manager-1.0.2.tar` & `custom_secrets_manager-1.0.3a0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.368783 custom_secrets_manager-1.0.2/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 22:04:37.368066 custom_secrets_manager-1.0.2/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      943 2023-06-03 21:05:39.000000 custom_secrets_manager-1.0.2/README.md
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.357760 custom_secrets_manager-1.0.2/custom_secrets_manager/
--rw-r--r--   0 vashishtha   (501) staff       (20)       22 2023-06-03 22:03:21.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/__init__.py
--rw-r--r--   0 vashishtha   (501) staff       (20)      638 2023-06-03 21:56:56.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/secrets_loader.py
--rw-r--r--   0 vashishtha   (501) staff       (20)     2422 2023-06-03 19:50:25.000000 custom_secrets_manager-1.0.2/custom_secrets_manager/starter_process.py
-drwxr-xr-x   0 vashishtha   (501) staff       (20)        0 2023-06-03 22:04:37.367324 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/
--rw-r--r--   0 vashishtha   (501) staff       (20)     1696 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/PKG-INFO
--rw-r--r--   0 vashishtha   (501) staff       (20)      414 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/SOURCES.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)        1 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/dependency_links.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       87 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/entry_points.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       10 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/requires.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       23 2023-06-03 22:04:36.000000 custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/top_level.txt
--rw-r--r--   0 vashishtha   (501) staff       (20)       38 2023-06-03 22:04:37.368935 custom_secrets_manager-1.0.2/setup.cfg
--rw-r--r--   0 vashishtha   (501) staff       (20)     1411 2023-06-03 20:39:12.000000 custom_secrets_manager-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.730187 custom_secrets_manager-1.0.3a0/custom_secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager/starter_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 17:03:42.000000 custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:03:42.734187 custom_secrets_manager-1.0.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-05 17:03:27.000000 custom_secrets_manager-1.0.3a0/setup.py
```

### Comparing `custom_secrets_manager-1.0.2/PKG-INFO` & `custom_secrets_manager-1.0.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: custom_secrets_manager
-Version: 1.0.2
+Version: 1.0.3a0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This starter_process script performs the following tasks:
   - Creates a `secrets_registry.log` file as a database for secrets, API keys, or passwords found in the parent directory of the script.
   - Scans the parent directory for suggestive file names like secrets or keys with file extensions **`.yaml`**, **`.json`**, or **`.ini`**. If there is a mention of a key name without a value, it checks the corresponding value in `os.environ` and updates the registry accordingly.
   - Makes available a `secrets_loader.py` module to load secrets from the secrets_registry.log file.
   - Generates meaningful logs in the standard output and saves logs in the `load_config_process.log` file in the same directory.
   - Checks if a `.gitignore` file exists in the directory and ensures that entries are made for secrets files.
```

### Comparing `custom_secrets_manager-1.0.2/README.md` & `custom_secrets_manager-1.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.2/custom_secrets_manager/secrets_loader.py` & `custom_secrets_manager-1.0.3a0/custom_secrets_manager/secrets_loader.py`

 * *Files identical despite different names*

### Comparing `custom_secrets_manager-1.0.2/custom_secrets_manager.egg-info/PKG-INFO` & `custom_secrets_manager-1.0.3a0/custom_secrets_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: custom-secrets-manager
-Version: 1.0.2
+Version: 1.0.3a0
 Summary: A utility for managing secrets and API keys
 Home-page: https://github.com/vvid643/custom_secrets_manager
 Author: Vashishtha Vidyarthi
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This starter_process script performs the following tasks:
   - Creates a `secrets_registry.log` file as a database for secrets, API keys, or passwords found in the parent directory of the script.
   - Scans the parent directory for suggestive file names like secrets or keys with file extensions **`.yaml`**, **`.json`**, or **`.ini`**. If there is a mention of a key name without a value, it checks the corresponding value in `os.environ` and updates the registry accordingly.
   - Makes available a `secrets_loader.py` module to load secrets from the secrets_registry.log file.
   - Generates meaningful logs in the standard output and saves logs in the `load_config_process.log` file in the same directory.
   - Checks if a `.gitignore` file exists in the directory and ensures that entries are made for secrets files.
```

### Comparing `custom_secrets_manager-1.0.2/setup.py` & `custom_secrets_manager-1.0.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     license=LICENSE,
     url=URL,
     packages=find_packages(),
     install_requires=REQUIRES,
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

