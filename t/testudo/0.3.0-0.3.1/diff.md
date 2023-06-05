# Comparing `tmp/testudo-0.3.0.tar.gz` & `tmp/testudo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testudo-0.3.0.tar", last modified: Tue Apr 25 01:50:13 2023, max compression
+gzip compressed data, was "testudo-0.3.1.tar", last modified: Mon Jun  5 00:06:11 2023, max compression
```

## Comparing `testudo-0.3.0.tar` & `testudo-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34500 2023-03-25 23:45:23.607612 testudo-0.3.0/LICENSE
--rw-r--r--   0        0        0     2370 2023-03-25 23:45:23.607612 testudo-0.3.0/README.md
--rw-r--r--   0        0        0     1448 2023-04-25 01:04:47.119734 testudo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-25 01:04:47.119734 testudo-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2929 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/integration/test_reporter.py
--rw-r--r--   0        0        0     1589 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/integration/test_runner.py
--rw-r--r--   0        0        0        0 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/__init__.py
--rw-r--r--   0        0        0       35 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/resources/basic_config.yaml
--rw-r--r--   0        0        0     1118 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_cli.py
--rw-r--r--   0        0        0      788 2023-04-25 01:22:53.120640 testudo-0.3.0/tests/unit/test_config.py
--rw-r--r--   0        0        0     4569 2023-04-25 01:49:48.594171 testudo-0.3.0/tests/unit/test_reporter.py
--rw-r--r--   0        0        0     2550 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_runner.py
--rw-r--r--   0        0        0     3288 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/test_task_manager.py
--rw-r--r--   0        0        0      256 2023-03-25 23:45:23.607612 testudo-0.3.0/tests/unit/utils.py
--rw-r--r--   0        0        0        0 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/__init__.py
--rw-r--r--   0        0        0     1762 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/cli.py
--rw-r--r--   0        0        0      995 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/config.py
--rw-r--r--   0        0        0      246 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/log.py
--rw-r--r--   0        0        0     3837 2023-04-25 01:49:48.594171 testudo-0.3.0/testudo/reporter.py
--rw-r--r--   0        0        0     3857 2023-03-25 23:45:23.607612 testudo-0.3.0/testudo/runner.py
--rw-r--r--   0        0        0     5134 2023-04-25 01:36:29.661513 testudo-0.3.0/testudo/task_manager.py
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 testudo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-03-01 02:56:07.690971 testudo-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2370 2023-03-01 02:56:07.690971 testudo-0.3.1/README.md
+-rw-r--r--   0        0        0     1542 2023-06-05 00:03:26.345861 testudo-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-04 23:58:01.870951 testudo-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2929 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/integration/test_reporter.py
+-rw-r--r--   0        0        0     1589 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/integration/test_runner.py
+-rw-r--r--   0        0        0        0 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0       35 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/resources/basic_config.yaml
+-rw-r--r--   0        0        0     1118 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      788 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_config.py
+-rw-r--r--   0        0        0     4569 2023-06-04 23:58:01.870951 testudo-0.3.1/tests/unit/test_reporter.py
+-rw-r--r--   0        0        0     2550 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_runner.py
+-rw-r--r--   0        0        0     3288 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/test_task_manager.py
+-rw-r--r--   0        0        0      256 2023-03-01 02:56:07.690971 testudo-0.3.1/tests/unit/utils.py
+-rw-r--r--   0        0        0        0 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/__init__.py
+-rw-r--r--   0        0        0     1762 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/cli.py
+-rw-r--r--   0        0        0      995 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/config.py
+-rw-r--r--   0        0        0      246 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/log.py
+-rw-r--r--   0        0        0     3837 2023-06-04 23:58:01.870951 testudo-0.3.1/testudo/reporter.py
+-rw-r--r--   0        0        0     3857 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/runner.py
+-rw-r--r--   0        0        0     5134 2023-03-01 02:56:07.690971 testudo-0.3.1/testudo/task_manager.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 testudo-0.3.1/PKG-INFO
```

### Comparing `testudo-0.3.0/LICENSE` & `testudo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/README.md` & `testudo-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/pyproject.toml` & `testudo-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "testudo"
-version = "0.3.0"
+version = "0.3.1"
 description = "A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory."
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "click<9.0.0,>=8.0.3",
-    "legion-utils<1.0.0,>=0.3.0",
+    "legion-utils<1.0.0,>=0.3.2",
 ]
 requires-python = ">=3.8.3,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
@@ -26,16 +26,17 @@
     "pytest-cov>=3.0.0",
     "pytest-mock>=3.7.0",
     "pylint>=2.13.7",
     "mypy>=1.2.0",
     "flake8>=4.0.1",
     "bandit>=1.7.4",
     "black>=22.3.0",
-    "typeguard=4.0.0rc4",
     "pytest-xdist>=2.5.0",
+    "legion-utils @ file:///${PROJECT_ROOT}/../legion-utils",
+    "robotnikmq @ file:///${PROJECT_ROOT}/../robotnikmq",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
 [tool.pdm.scripts.publish-prod]
 cmd = "twine upload -r pypi dist/*"
```

### Comparing `testudo-0.3.0/tests/integration/test_reporter.py` & `testudo-0.3.1/tests/integration/test_reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/integration/test_runner.py` & `testudo-0.3.1/tests/integration/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/unit/test_cli.py` & `testudo-0.3.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/unit/test_config.py` & `testudo-0.3.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/unit/test_reporter.py` & `testudo-0.3.1/tests/unit/test_reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/unit/test_runner.py` & `testudo-0.3.1/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/tests/unit/test_task_manager.py` & `testudo-0.3.1/tests/unit/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/testudo/cli.py` & `testudo-0.3.1/testudo/cli.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/testudo/config.py` & `testudo-0.3.1/testudo/config.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/testudo/reporter.py` & `testudo-0.3.1/testudo/reporter.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/testudo/runner.py` & `testudo-0.3.1/testudo/runner.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/testudo/task_manager.py` & `testudo-0.3.1/testudo/task_manager.py`

 * *Files identical despite different names*

### Comparing `testudo-0.3.0/PKG-INFO` & `testudo-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testudo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A wrapper for commands to be run as periodic tasks while reporting on their results/errors to legiond. Intended to be integrated with supervisord, should work well with systemd in theory.
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Testudo
```

