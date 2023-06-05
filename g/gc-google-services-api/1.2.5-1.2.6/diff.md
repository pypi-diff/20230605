# Comparing `tmp/gc_google_services_api-1.2.5.tar.gz` & `tmp/gc_google_services_api-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc_google_services_api-1.2.5.tar", max compression
+gzip compressed data, was "gc_google_services_api-1.2.6.tar", max compression
```

## Comparing `gc_google_services_api-1.2.5.tar` & `gc_google_services_api-1.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35148 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/LICENSE
--rw-r--r--   0        0        0     4474 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/README.md
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/__init__.py
--rw-r--r--   0        0        0      799 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/auth/__tests__/__init__.py
--rw-r--r--   0        0        0     2114 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/auth/__tests__/test_auth.py
--rw-r--r--   0        0        0      276 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/bigquery/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/bigquery/__tests__/__init__.py
--rw-r--r--   0        0        0      921 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/bigquery/__tests__/test_bigquery.py
--rw-r--r--   0        0        0     3842 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/calendar_api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/calendar_api/__tests__/__init__.py
--rw-r--r--   0        0        0     7150 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/calendar_api/__tests__/test_calendar.py
--rw-r--r--   0        0        0     1681 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gmail/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gmail/__tests__/__init__.py
--rw-r--r--   0        0        0     2731 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gmail/__tests__/test_gmail.py
--rw-r--r--   0        0        0     1818 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gsheet/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gsheet/__tests__/__init__.py
--rw-r--r--   0        0        0     3605 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/gsheet/__tests__/test_gsheet.py
--rw-r--r--   0        0        0        0 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/permissions/__init__.py
--rw-r--r--   0        0        0     3023 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/permissions/drive.py
--rw-r--r--   0        0        0     3243 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/gc_google_services_api/permissions/workspace.py
--rw-r--r--   0        0        0      458 2023-03-10 11:20:11.565889 gc_google_services_api-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     5089 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/LICENSE
+-rw-r--r--   0        0        0     4790 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/__init__.py
+-rw-r--r--   0        0        0     2114 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/test_auth.py
+-rw-r--r--   0        0        0     1700 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0     3842 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/__init__.py
+-rw-r--r--   0        0        0     7150 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/test_calendar.py
+-rw-r--r--   0        0        0     1681 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/__init__.py
+-rw-r--r--   0        0        0     2731 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/test_gmail.py
+-rw-r--r--   0        0        0     1818 2023-06-05 07:09:37.693068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__tests__/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__tests__/test_gsheet.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/drive.py
+-rw-r--r--   0        0        0     3243 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/gc_google_services_api/permissions/workspace.py
+-rw-r--r--   0        0        0      458 2023-06-05 07:09:37.697068 gc_google_services_api-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.6/PKG-INFO
```

### Comparing `gc_google_services_api-1.2.5/LICENSE` & `gc_google_services_api-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/README.md` & `gc_google_services_api-1.2.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,28 @@
 ```
 
 ## 2.- Run test
 ```bash
 make test
 ```
 
+# Publish new version
+When your Pull Request is approved and merged with master, then to can generate new version running the next command:
+
+```bash
+make v=X.Y.Z release 
+```
+or you can execute
+```bash
+poetry version X.Y.Z <-- (New version)
+git commit -am "Release vX.Y.Z"
+git tag vX.Y.Z
+git push --follow-tags
+```
+
 Google services API
 =============================
 This repository is a suite that exposes Google services to easily integrate with our project (Big query, Google sheet, Gmail, etc...).
 
 Each api needs a different form of authentication, either because it requires the interaction of a person who approves the api to extract sensitive information or because we want to connect automatically without user intervention.
```

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/auth/__init__.py` & `gc_google_services_api-1.2.6/gc_google_services_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/auth/__tests__/test_auth.py` & `gc_google_services_api-1.2.6/gc_google_services_api/auth/__tests__/test_auth.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/bigquery/__tests__/test_bigquery.py` & `gc_google_services_api-1.2.6/gc_google_services_api/bigquery/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/calendar_api/__init__.py` & `gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/calendar_api/__tests__/test_calendar.py` & `gc_google_services_api-1.2.6/gc_google_services_api/calendar_api/__tests__/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/gmail/__init__.py` & `gc_google_services_api-1.2.6/gc_google_services_api/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/gmail/__tests__/test_gmail.py` & `gc_google_services_api-1.2.6/gc_google_services_api/gmail/__tests__/test_gmail.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/gsheet/__init__.py` & `gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/gsheet/__tests__/test_gsheet.py` & `gc_google_services_api-1.2.6/gc_google_services_api/gsheet/__tests__/test_gsheet.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/permissions/drive.py` & `gc_google_services_api-1.2.6/gc_google_services_api/permissions/drive.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/gc_google_services_api/permissions/workspace.py` & `gc_google_services_api-1.2.6/gc_google_services_api/permissions/workspace.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.5/PKG-INFO` & `gc_google_services_api-1.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gc-google-services-api
-Version: 1.2.5
+Version: 1.2.6
 Summary: 
 Author: Jonathan Rodríguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,14 +25,28 @@
 ```
 
 ## 2.- Run test
 ```bash
 make test
 ```
 
+# Publish new version
+When your Pull Request is approved and merged with master, then to can generate new version running the next command:
+
+```bash
+make v=X.Y.Z release 
+```
+or you can execute
+```bash
+poetry version X.Y.Z <-- (New version)
+git commit -am "Release vX.Y.Z"
+git tag vX.Y.Z
+git push --follow-tags
+```
+
 Google services API
 =============================
 This repository is a suite that exposes Google services to easily integrate with our project (Big query, Google sheet, Gmail, etc...).
 
 Each api needs a different form of authentication, either because it requires the interaction of a person who approves the api to extract sensitive information or because we want to connect automatically without user intervention.
```

