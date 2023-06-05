# Comparing `tmp/python-pdfbox-v2-2.0.27.2.tar.gz` & `tmp/python-pdfbox-v2-2.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pdfbox-v2-2.0.27.2.tar", last modified: Tue Jan 24 15:45:13 2023, max compression
+gzip compressed data, was "python-pdfbox-v2-2.0.28.tar", last modified: Mon Jun  5 12:12:54 2023, max compression
```

## Comparing `python-pdfbox-v2-2.0.27.2.tar` & `python-pdfbox-v2-2.0.28.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/pdfbox/
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/pdfbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-01-24 15:45:13.000000 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-24 15:45:13.000000 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 15:45:13.000000 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-24 15:45:13.000000 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-24 15:45:13.000000 python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:45:13.191335 python-pdfbox-v2-2.0.27.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test space.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test.md
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    84980 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-01-24 15:44:54.000000 python-pdfbox-v2-2.0.27.2/tests/test_pdfbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.163332 python-pdfbox-v2-2.0.28/pdfbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/pdfbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 10085495 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/pdfbox/pdfbox-app-2.0.28.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 12:12:54.000000 python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:12:54.175332 python-pdfbox-v2-2.0.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test space.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    84980 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 12:12:45.000000 python-pdfbox-v2-2.0.28/tests/test_pdfbox.py
```

### Comparing `python-pdfbox-v2-2.0.27.2/LICENSE.rst` & `python-pdfbox-v2-2.0.28/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/PKG-INFO` & `python-pdfbox-v2-2.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.27.2
+Version: 2.0.28
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Lev E. Givon
 Author-email: lev@columbia.edu
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.27.2/README.rst` & `python-pdfbox-v2-2.0.28/README.rst`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/pdfbox/__init__.py` & `python-pdfbox-v2-2.0.28/pdfbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,61 +74,29 @@
         # Use PDFBOX environmental variable if it exists:
         if 'PDFBOX' in os.environ:
             pdfbox_path = pathlib.Path(os.environ['PDFBOX'])
             if not pdfbox_path.exists():
                 raise RuntimeError('pdfbox not found')
             return pdfbox_path
 
-        # Use platform-specific cache directory:
-        a = appdirs.AppDirs('python-pdfbox')
-        cache_dir = pathlib.Path(a.user_cache_dir)
-
-        # Try to find pdfbox-app-*.jar file with most recent version in cache directory:
-        file_list = list(cache_dir.glob('pdfbox-app-*.jar'))
-        if file_list:
-            def f(s):
-                v = re.search('pdfbox-app-([\w\.\-]+)\.jar', s.name).group(1)
-                return pkg_resources.parse_version(v)
-            return sorted(file_list, key=f)[-1]
-        else:
-            # If no jar files are cached, find the latest version jar, retrieve it,
-            # cache it, and verify its checksum:
-            pdfbox_url = self._get_compatible_pdfbox_url()
-            sha512_url = pdfbox_url + '.sha512'
-            r = urllib.request.urlopen(pdfbox_url)
-            try:
-                data = r.read()
-            except:
-                raise RuntimeError('error retrieving %s' % pdfbox_url)
-            else:
-                if not os.path.exists(cache_dir.as_posix()):
-                    cache_dir.mkdir(parents=True)
-                pdfbox_path = cache_dir.joinpath(pathlib.Path(pdfbox_url).name)
-                with open(pdfbox_path.as_posix(), 'wb') as f:
-                    f.write(data)
-
-            r = urllib.request.urlopen(sha512_url)
-            encoding = r.headers.get_content_charset('utf-8')
-            try:
-                sha512 = r.read().decode(encoding).strip()
-            except:
-                raise RuntimeError('error retrieving sha512sum')
-            else:
-                if not self._verify_sha512(data, sha512):
-                    raise RuntimeError('failed to verify sha512sum')
+        jar_path = os.path.dirname(os.path.abspath(__file__))
+        jar_file_path = os.path.join(jar_path, 'pdfbox-app-2.0.28.jar')
+
+        return jar_file_path
 
-            return pdfbox_path
 
     def __init__(self):
         self.pdfbox_path = self._get_pdfbox_path()
+        print(self.pdfbox_path)
         jpype.addClassPath(self.pdfbox_path)
         if not jpype.isJVMStarted():
             jpype.startJVM(convertStrings=False)
         import org.apache.pdfbox.tools as tools
         self.pdfbox_tools = tools
+        print("Here am i")
 
     def extract_text(self, input_path, output_path='',
                      password=None, encoding=None, html=False, sort=False,
                      ignore_beads=False, start_page=1, end_page=None, console=False):
         """
         Extract all text from PDF file.
```

### Comparing `python-pdfbox-v2-2.0.27.2/python_pdfbox_v2.egg-info/PKG-INFO` & `python-pdfbox-v2-2.0.28/python_pdfbox_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pdfbox-v2
-Version: 2.0.27.2
+Version: 2.0.28
 Summary: Python interface to Apache PDFBox command-line tools.
 Home-page: https://github.com/py-hacks/python-pdfbox
 Author: Lev E. Givon
 Author-email: lev@columbia.edu
 License: Apache
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `python-pdfbox-v2-2.0.27.2/setup.py` & `python-pdfbox-v2-2.0.28/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME =               'python-pdfbox-v2'
-VERSION =            '2.0.27.2'
+VERSION =            '2.0.28'
 AUTHOR =             'Lev E. Givon'
 AUTHOR_EMAIL =       'lev@columbia.edu'
 URL =                'https://github.com/py-hacks/python-pdfbox'
 DESCRIPTION =        'Python interface to Apache PDFBox command-line tools.'
 with open('README.rst', 'r') as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION = re.search('.*(^Package Description.*)', LONG_DESCRIPTION, re.MULTILINE|re.DOTALL).group(1)
```

### Comparing `python-pdfbox-v2-2.0.27.2/tests/test space.pdf` & `python-pdfbox-v2-2.0.28/tests/test space.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/tests/test.pdf` & `python-pdfbox-v2-2.0.28/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/tests/test2.pdf` & `python-pdfbox-v2-2.0.28/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/tests/test3.pdf` & `python-pdfbox-v2-2.0.28/tests/test3.pdf`

 * *Files identical despite different names*

### Comparing `python-pdfbox-v2-2.0.27.2/tests/test_pdfbox.py` & `python-pdfbox-v2-2.0.28/tests/test_pdfbox.py`

 * *Files identical despite different names*

