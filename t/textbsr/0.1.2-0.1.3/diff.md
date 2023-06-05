# Comparing `tmp/textbsr-0.1.2.tar.gz` & `tmp/textbsr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.1.2.tar", last modified: Mon Jun  5 12:14:39 2023, max compression
+gzip compressed data, was "textbsr-0.1.3.tar", last modified: Mon Jun  5 12:23:36 2023, max compression
```

## Comparing `textbsr-0.1.2.tar` & `textbsr-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:14:39.000000 textbsr-0.1.2/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     3225 2023-06-05 12:13:56.000000 textbsr-0.1.2/README.md
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-06-05 12:14:39.000000 textbsr-0.1.2/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1165 2023-06-05 12:14:01.000000 textbsr-0.1.2/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.2/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.2/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9774 2023-06-05 11:52:46.000000 textbsr-0.1.2/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.2/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6879 2023-06-05 11:52:47.000000 textbsr-0.1.2/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.2/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2636 2023-06-05 06:38:59.000000 textbsr-0.1.2/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/entry_points.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       47 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-06-05 12:14:39.000000 textbsr-0.1.2/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:23:36.000000 textbsr-0.1.3/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     3225 2023-06-05 12:13:56.000000 textbsr-0.1.3/README.md
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-06-05 12:23:36.000000 textbsr-0.1.3/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1165 2023-06-05 12:22:17.000000 textbsr-0.1.3/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.3/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.3/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9774 2023-06-05 11:52:46.000000 textbsr-0.1.3/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       15 2023-06-05 06:38:59.000000 textbsr-0.1.3/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6879 2023-06-05 12:19:06.000000 textbsr-0.1.3/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-06-05 06:38:59.000000 textbsr-0.1.3/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2636 2023-06-05 06:38:59.000000 textbsr-0.1.3/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     4433 2023-06-05 12:23:35.000000 textbsr-0.1.3/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      393 2023-06-05 12:23:36.000000 textbsr-0.1.3/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-06-05 12:23:35.000000 textbsr-0.1.3/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       53 2023-06-05 12:23:35.000000 textbsr-0.1.3/textbsr.egg-info/entry_points.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       47 2023-06-05 12:23:35.000000 textbsr-0.1.3/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-06-05 12:23:35.000000 textbsr-0.1.3/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.1.2/PKG-INFO` & `textbsr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.1.2
+Version: 0.1.3
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
 Description: 
         # Update v0.1.2
```

### Comparing `textbsr-0.1.2/README.md` & `textbsr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.2/setup.py` & `textbsr-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 def read(fname):
 	return codecs.open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name='textbsr',
-      version='0.1.2',
+      version='0.1.3',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       long_description=read("README.md"),
       long_description_content_type="text/markdown",
       packages=find_packages(),  #
       #
```

### Comparing `textbsr-0.1.2/textbsr/models/TextEnhancement.py` & `textbsr-0.1.3/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.2/textbsr/textbsr.py` & `textbsr-0.1.3/textbsr/textbsr.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.2/textbsr/utils/utils_image.py` & `textbsr-0.1.3/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.1.2/textbsr.egg-info/PKG-INFO` & `textbsr-0.1.3/textbsr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textbsr
-Version: 0.1.2
+Version: 0.1.3
 Summary: a simple version for blind text image super-resolution (current version is only for English and Chinese)
 Home-page: https://github.com/csxmli2016/MARCONet
 Author: Xiaoming Li
 Author-email: csxmli@gmail.com
 License: S-Lab License 1.0
 Description: 
         # Update v0.1.2
```

