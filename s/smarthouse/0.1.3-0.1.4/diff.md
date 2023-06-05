# Comparing `tmp/smarthouse-0.1.3.tar.gz` & `tmp/smarthouse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smarthouse-0.1.3.tar", last modified: Mon Jun  5 12:49:18 2023, max compression
+gzip compressed data, was "smarthouse-0.1.4.tar", last modified: Mon Jun  5 15:03:54 2023, max compression
```

## Comparing `smarthouse-0.1.3.tar` & `smarthouse-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.144427 smarthouse-0.1.3/
--rw-r--r--   0 ivan       (501) staff       (20)     4918 2023-06-05 12:49:18.143894 smarthouse-0.1.3/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     4379 2023-05-17 16:35:41.000000 smarthouse-0.1.3/README.md
--rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.3/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-06-05 12:49:18.144702 smarthouse-0.1.3/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1734 2023-06-05 12:48:54.000000 smarthouse-0.1.3/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.138275 smarthouse-0.1.3/smarthouse/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/action_decorators.py
--rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.3/smarthouse/app.py
--rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/device.py
--rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/device_generator.py
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/logger.py
--rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/storage.py
--rw-r--r--   0 ivan       (501) staff       (20)     8195 2023-06-05 12:47:44.000000 smarthouse-0.1.3/smarthouse/telegram_client.py
--rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.3/smarthouse/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 12:49:18.142514 smarthouse-0.1.3/smarthouse.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     4918 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      420 2023-06-05 12:49:18.000000 smarthouse-0.1.3/smarthouse.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      290 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       11 2023-06-05 12:49:17.000000 smarthouse-0.1.3/smarthouse.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.728768 smarthouse-0.1.4/
+-rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-06-05 15:03:54.728199 smarthouse-0.1.4/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     4537 2023-06-05 14:57:33.000000 smarthouse-0.1.4/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)     4925 2023-06-05 15:01:13.000000 smarthouse-0.1.4/README.rst
+-rw-r--r--   0 ivan       (501) staff       (20)     1015 2023-05-06 17:52:00.000000 smarthouse-0.1.4/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-06-05 15:03:54.729008 smarthouse-0.1.4/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1735 2023-06-05 14:55:41.000000 smarthouse-0.1.4/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.724013 smarthouse-0.1.4/smarthouse/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4079 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/action_decorators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2808 2023-05-17 15:01:34.000000 smarthouse-0.1.4/smarthouse/app.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11112 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/device.py
+-rw-r--r--   0 ivan       (501) staff       (20)      318 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/device_generator.py
+-rw-r--r--   0 ivan       (501) staff       (20)      420 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/logger.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2738 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/storage.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8195 2023-06-05 12:47:44.000000 smarthouse-0.1.4/smarthouse/telegram_client.py
+-rw-r--r--   0 ivan       (501) staff       (20)      968 2023-05-17 13:06:07.000000 smarthouse-0.1.4/smarthouse/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-05 15:03:54.727411 smarthouse-0.1.4/smarthouse.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     5106 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      431 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      290 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       11 2023-06-05 15:03:54.000000 smarthouse-0.1.4/smarthouse.egg-info/top_level.txt
```

### Comparing `smarthouse-0.1.3/PKG-INFO` & `smarthouse-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Smart House Scenarios
-Home-page: UNKNOWN
+Home-page: https://smarthouselib.readthedocs.io/
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # SmartHouse
 [![Coverage Status](https://coveralls.io/repos/github/vivenchik/smarthouse/badge.svg?branch=master)](https://coveralls.io/github/vivenchik/smarthouse?branch=master)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/smarthouselib/badge/?version=latest)](https://smarthouselib.readthedocs.io/en/latest/?badge=latest)
 
 SmartHouse - библиотека для управления умным домом. На текущий момент реализована интеграция с экосистемой [Яндекса](https://yandex.ru/dev/dialogs/smart-home/doc/concepts/platform-protocol.html).
 
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
```

### Comparing `smarthouse-0.1.3/README.md` & `smarthouse-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SmartHouse
 [![Coverage Status](https://coveralls.io/repos/github/vivenchik/smarthouse/badge.svg?branch=master)](https://coveralls.io/github/vivenchik/smarthouse?branch=master)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/smarthouselib/badge/?version=latest)](https://smarthouselib.readthedocs.io/en/latest/?badge=latest)
 
 SmartHouse - библиотека для управления умным домом. На текущий момент реализована интеграция с экосистемой [Яндекса](https://yandex.ru/dev/dialogs/smart-home/doc/concepts/platform-protocol.html).
 
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
```

### Comparing `smarthouse-0.1.3/pyproject.toml` & `smarthouse-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/setup.py` & `smarthouse-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         "python-dotenv",
     ]
 }
 
 
 setup(
     name="smarthouse",
-    version="0.1.3",
+    version="0.1.4",
     description="Smart House Scenarios",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    # url="https://smarthouse.readthedocs.io/",
+    url="https://smarthouselib.readthedocs.io/",
     author="Ivan Kriuchkov",
     author_email="vivenchik@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

### Comparing `smarthouse-0.1.3/smarthouse/action_decorators.py` & `smarthouse-0.1.4/smarthouse/action_decorators.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse/app.py` & `smarthouse-0.1.4/smarthouse/app.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse/device.py` & `smarthouse-0.1.4/smarthouse/device.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse/storage.py` & `smarthouse-0.1.4/smarthouse/storage.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse/telegram_client.py` & `smarthouse-0.1.4/smarthouse/telegram_client.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse/utils.py` & `smarthouse-0.1.4/smarthouse/utils.py`

 * *Files identical despite different names*

### Comparing `smarthouse-0.1.3/smarthouse.egg-info/PKG-INFO` & `smarthouse-0.1.4/smarthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smarthouse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Smart House Scenarios
-Home-page: UNKNOWN
+Home-page: https://smarthouselib.readthedocs.io/
 Author: Ivan Kriuchkov
 Author-email: vivenchik@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # SmartHouse
 [![Coverage Status](https://coveralls.io/repos/github/vivenchik/smarthouse/badge.svg?branch=master)](https://coveralls.io/github/vivenchik/smarthouse?branch=master)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/smarthouselib/badge/?version=latest)](https://smarthouselib.readthedocs.io/en/latest/?badge=latest)
 
 SmartHouse - библиотека для управления умным домом. На текущий момент реализована интеграция с экосистемой [Яндекса](https://yandex.ru/dev/dialogs/smart-home/doc/concepts/platform-protocol.html).
 
 Какие задачи решает
 -------------
 * Каркас для написания сценариев
 * Использование устройств как объектов или напрямую через клиента
```

