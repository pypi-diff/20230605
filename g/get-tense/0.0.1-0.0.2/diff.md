# Comparing `tmp/get_tense-0.0.1.tar.gz` & `tmp/get_tense-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_tense-0.0.1.tar", last modified: Mon Jun  5 10:55:21 2023, max compression
+gzip compressed data, was "get_tense-0.0.2.tar", last modified: Mon Jun  5 12:23:12 2023, max compression
```

## Comparing `get_tense-0.0.1.tar` & `get_tense-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 10:55:21.074935 get_tense-0.0.1/
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      362 2023-06-05 10:55:21.074935 get_tense-0.0.1/PKG-INFO
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       27 2023-06-05 10:47:46.000000 get_tense-0.0.1/README.md
-drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 10:55:21.074935 get_tense-0.0.1/get_tense/
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      154 2023-06-05 10:52:18.000000 get_tense-0.0.1/get_tense/__init__.py
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)     3641 2023-06-05 10:52:19.000000 get_tense-0.0.1/get_tense/get_tense.py
-drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 10:55:21.074935 get_tense-0.0.1/get_tense.egg-info/
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      362 2023-06-05 10:55:21.000000 get_tense-0.0.1/get_tense.egg-info/PKG-INFO
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      227 2023-06-05 10:55:21.000000 get_tense-0.0.1/get_tense.egg-info/SOURCES.txt
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)        1 2023-06-05 10:55:21.000000 get_tense-0.0.1/get_tense.egg-info/dependency_links.txt
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       26 2023-06-05 10:55:21.000000 get_tense-0.0.1/get_tense.egg-info/requires.txt
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       10 2023-06-05 10:55:21.000000 get_tense-0.0.1/get_tense.egg-info/top_level.txt
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       38 2023-06-05 10:55:21.074935 get_tense-0.0.1/setup.cfg
--rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)     1051 2023-06-05 10:54:57.000000 get_tense-0.0.1/setup.py
+drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 12:23:12.062728 get_tense-0.0.2/
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      362 2023-06-05 12:23:12.062728 get_tense-0.0.2/PKG-INFO
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       27 2023-06-05 10:47:46.000000 get_tense-0.0.2/README.md
+drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 12:23:12.062728 get_tense-0.0.2/get_tense/
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      154 2023-06-05 12:22:32.000000 get_tense-0.0.2/get_tense/__init__.py
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)     3641 2023-06-05 10:52:19.000000 get_tense-0.0.2/get_tense/get_tense.py
+drwxrwxr-x   0 ujjwal    (1000) ujjwal    (1000)        0 2023-06-05 12:23:12.062728 get_tense-0.0.2/get_tense.egg-info/
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      362 2023-06-05 12:23:11.000000 get_tense-0.0.2/get_tense.egg-info/PKG-INFO
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)      227 2023-06-05 12:23:12.000000 get_tense-0.0.2/get_tense.egg-info/SOURCES.txt
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)        1 2023-06-05 12:23:11.000000 get_tense-0.0.2/get_tense.egg-info/dependency_links.txt
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       19 2023-06-05 12:23:11.000000 get_tense-0.0.2/get_tense.egg-info/requires.txt
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       10 2023-06-05 12:23:11.000000 get_tense-0.0.2/get_tense.egg-info/top_level.txt
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)       38 2023-06-05 12:23:12.062728 get_tense-0.0.2/setup.cfg
+-rw-rw-r--   0 ujjwal    (1000) ujjwal    (1000)     1042 2023-06-05 12:22:36.000000 get_tense-0.0.2/setup.py
```

### Comparing `get_tense-0.0.1/get_tense/get_tense.py` & `get_tense-0.0.2/get_tense/get_tense.py`

 * *Files identical despite different names*

### Comparing `get_tense-0.0.1/setup.py` & `get_tense-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import codecs
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (HERE / 'README.md').read_text(encoding='utf-8')
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 __maintainer__ = 'Ujjwal Chowdhury'
 
 
 # Setting up
 setup(
     name='get_tense',
     version=__version__,
@@ -20,15 +20,15 @@
     author=__maintainer__,
     author_email='<u77w41@gmail.com>',
     url='https://github.com/U77w41/',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=['nltk','regex','pickle','pathlib'],
+    install_requires=['nltk','regex','pathlib'],
     tests_require=['pytest'],
     keywords= ['python','text','regex', 'tense classification','grammer']
 )
 
 #################################################################################################################
 # python3 setup.py sdist bdist_wheel
 # twine upload dist/*
```

