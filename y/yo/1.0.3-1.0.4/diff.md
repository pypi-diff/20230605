# Comparing `tmp/yo-1.0.3.tar.gz` & `tmp/yo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.0.3.tar", last modified: Fri Jun  2 21:52:33 2023, max compression
+gzip compressed data, was "yo-1.0.4.tar", last modified: Mon Jun  5 17:03:17 2023, max compression
```

## Comparing `yo-1.0.3.tar` & `yo-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.761397 yo-1.0.3/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.3/LICENSE.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 21:52:33.761397 yo-1.0.3/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.3/README.md
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.3/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-06-02 21:52:33.761397 yo-1.0.3/setup.cfg
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-06-02 21:52:19.000000 yo-1.0.3/setup.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/tests/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.3/tests/test_api.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.3/tests/test_cmds.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.3/yo/__init__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.3/yo/__main__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67881 2023-06-02 18:54:59.000000 yo-1.0.3/yo/api.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo/data/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.3/yo/data/sample.yo.ini
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.761397 yo-1.0.3/yo/data/yo-tasks/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/drgn
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/ocid
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-deps
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.3/yo/data/yo-tasks/test-existing-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-run-many
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.3/yo/data/yo-tasks/test-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.3/yo/data/yo_tasklib.sh
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   109190 2023-06-02 21:52:19.000000 yo-1.0.3/yo/main.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.3/yo/oci.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.3/yo/util.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-02 21:52:33.757397 yo-1.0.3/yo.egg-info/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/SOURCES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/dependency_links.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/entry_points.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/requires.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-06-02 21:52:33.000000 yo-1.0.3/yo.egg-info/top_level.txt
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.125070 yo-1.0.4/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.4/LICENSE.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-05 17:03:17.125070 yo-1.0.4/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.4/README.md
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.4/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-06-05 17:03:17.125070 yo-1.0.4/setup.cfg
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-06-05 17:02:58.000000 yo-1.0.4/setup.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.121070 yo-1.0.4/tests/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.4/tests/test_api.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.4/tests/test_cmds.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.121070 yo-1.0.4/yo/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.4/yo/__init__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.4/yo/__main__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67881 2023-06-02 18:54:59.000000 yo-1.0.4/yo/api.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.121070 yo-1.0.4/yo/data/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.4/yo/data/sample.yo.ini
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.125070 yo-1.0.4/yo/data/yo-tasks/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.4/yo/data/yo-tasks/drgn
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.4/yo/data/yo-tasks/ocid
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.4/yo/data/yo-tasks/test-deps
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.4/yo/data/yo-tasks/test-existing-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.4/yo/data/yo-tasks/test-run-many
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.4/yo/data/yo-tasks/test-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.4/yo/data/yo_tasklib.sh
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   109434 2023-06-05 17:02:58.000000 yo-1.0.4/yo/main.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.4/yo/oci.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.4/yo/util.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-06-05 17:03:17.121070 yo-1.0.4/yo.egg-info/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/entry_points.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/requires.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-06-05 17:03:17.000000 yo-1.0.4/yo.egg-info/top_level.txt
```

### Comparing `yo-1.0.3/LICENSE.txt` & `yo-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/PKG-INFO` & `yo-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.3/README.md` & `yo-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/THIRD_PARTY_LICENSES.txt` & `yo-1.0.4/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/setup.py` & `yo-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `yo-1.0.3/tests/test_api.py` & `yo-1.0.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/tests/test_cmds.py` & `yo-1.0.4/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/__main__.py` & `yo-1.0.4/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/api.py` & `yo-1.0.4/yo/api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/sample.yo.ini` & `yo-1.0.4/yo/data/sample.yo.ini`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo-tasks/drgn` & `yo-1.0.4/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo-tasks/ocid` & `yo-1.0.4/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo-tasks/test-deps` & `yo-1.0.4/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo-tasks/test-run-many` & `yo-1.0.4/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo-tasks/test-task` & `yo-1.0.4/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/data/yo_tasklib.sh` & `yo-1.0.4/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/main.py` & `yo-1.0.4/yo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3131,22 +3131,25 @@
     """
     # The configuration "extension_modules" is still supported, but no longer
     # recommended. Entry points (below) are a better way that don't require the
     # user to manually configure things.
     for module in ctx.config.extension_modules:
         importlib.import_module(module)
 
-    # The importlib.metadata API is from Python 3.8+. So we can support the
-    # prior versions by falling back to pkg_resources.
-    try:
+    # The importlib.metadata API is included in Python 3.8+. Normally, one might
+    # simply try to import it, catching the ImportError and falling back to the
+    # older API. However, the API was _transitional_ in 3.8 and 3.9, and it is
+    # different enough to break callers compared to the non-transitional API. So
+    # here we are, using sys.version_info like heathens.
+    if sys.version_info >= (3, 10):
         from importlib.metadata import entry_points  # novermin
-    except ImportError:
+    else:
         import pkg_resources
 
-        def entry_points(group):  # type: ignore
+        def entry_points(group):
             return pkg_resources.iter_entry_points(group)
 
     for entry_point in entry_points(group="yo.extensions.v1"):
         entry_point.load()
 
 
 def main() -> None:
```

### Comparing `yo-1.0.3/yo/oci.py` & `yo-1.0.4/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo/util.py` & `yo-1.0.4/yo/util.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.3/yo.egg-info/PKG-INFO` & `yo-1.0.4/yo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yo-1.0.3/yo.egg-info/SOURCES.txt` & `yo-1.0.4/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

