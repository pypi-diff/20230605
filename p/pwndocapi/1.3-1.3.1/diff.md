# Comparing `tmp/pwndocapi-1.3.tar.gz` & `tmp/pwndocapi-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwndocapi-1.3.tar", last modified: Mon Apr 17 14:54:01 2023, max compression
+gzip compressed data, was "pwndocapi-1.3.1.tar", last modified: Mon Jun  5 09:06:29 2023, max compression
```

## Comparing `pwndocapi-1.3.tar` & `pwndocapi-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:54:01.152783 pwndocapi-1.3/
--rwxrwxr-x   0 root         (0) root         (0)    35149 2023-04-17 14:44:54.000000 pwndocapi-1.3/LICENSE
--rwxrwxr-x   0 root         (0) root         (0)       53 2023-04-17 14:44:54.000000 pwndocapi-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      544 2023-04-17 14:54:01.152783 pwndocapi-1.3/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)       35 2023-04-17 14:44:54.000000 pwndocapi-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:54:01.148783 pwndocapi-1.3/pwndocapi/
--rwxrwxr-x   0 root         (0) root         (0)     8188 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/API.py
--rwxrwxr-x   0 root         (0) root         (0)      215 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:54:01.148783 pwndocapi-1.3/pwndocapi/api/
--rwxrwxr-x   0 root         (0) root         (0)      305 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      744 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/audits.py
--rwxrwxr-x   0 root         (0) root         (0)      344 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/clients.py
--rwxrwxr-x   0 root         (0) root         (0)      352 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/companies.py
--rwxrwxr-x   0 root         (0) root         (0)     1081 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/data.py
--rwxrwxr-x   0 root         (0) root         (0)      747 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/api/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:54:01.152783 pwndocapi-1.3/pwndocapi/models/
--rwxrwxr-x   0 root         (0) root         (0)     4191 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/Audit.py
--rwxrwxr-x   0 root         (0) root         (0)      208 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/AuditError.py
--rwxrwxr-x   0 root         (0) root         (0)     2146 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/Finding.py
--rwxrwxr-x   0 root         (0) root         (0)      269 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/Priority.py
--rwxrwxr-x   0 root         (0) root         (0)      284 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/RemediationComplexity.py
--rwxrwxr-x   0 root         (0) root         (0)     2962 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/User.py
--rwxrwxr-x   0 root         (0) root         (0)      367 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/models/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      816 2023-04-17 14:45:51.000000 pwndocapi-1.3/pwndocapi/pwndoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:54:01.148783 pwndocapi-1.3/pwndocapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      544 2023-04-17 14:54:01.000000 pwndocapi-1.3/pwndocapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-17 14:54:01.000000 pwndocapi-1.3/pwndocapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:54:01.000000 pwndocapi-1.3/pwndocapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 14:54:01.000000 pwndocapi-1.3/pwndocapi.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        8 2023-04-17 14:44:54.000000 pwndocapi-1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 14:54:01.152783 pwndocapi-1.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      857 2023-04-17 14:44:54.000000 pwndocapi-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/
+-rwxrwxr-x   0 root         (0) root         (0)    35149 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/LICENSE
+-rwxrwxr-x   0 root         (0) root         (0)       53 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)       35 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/pwndocapi/
+-rwxrwxr-x   0 root         (0) root         (0)     8362 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/API.py
+-rwxrwxr-x   0 root         (0) root         (0)      215 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/pwndocapi/api/
+-rwxrwxr-x   0 root         (0) root         (0)      349 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)      744 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/audits.py
+-rwxrwxr-x   0 root         (0) root         (0)      344 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/clients.py
+-rwxrwxr-x   0 root         (0) root         (0)      352 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/companies.py
+-rwxrwxr-x   0 root         (0) root         (0)     1081 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/data.py
+-rwxrwxr-x   0 root         (0) root         (0)      747 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/users.py
+-rw-rw-r--   0 root         (0) root         (0)      362 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/api/vulnerabilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/pwndocapi/models/
+-rwxrwxr-x   0 root         (0) root         (0)     4170 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/Audit.py
+-rwxrwxr-x   0 root         (0) root         (0)      208 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/AuditError.py
+-rwxrwxr-x   0 root         (0) root         (0)     2146 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/Finding.py
+-rwxrwxr-x   0 root         (0) root         (0)      269 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/Priority.py
+-rwxrwxr-x   0 root         (0) root         (0)      284 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/RemediationComplexity.py
+-rwxrwxr-x   0 root         (0) root         (0)     2962 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/User.py
+-rwxrwxr-x   0 root         (0) root         (0)      367 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/models/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)      873 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/pwndocapi/pwndoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/pwndocapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-05 09:06:29.000000 pwndocapi-1.3.1/pwndocapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-05 09:06:29.000000 pwndocapi-1.3.1/pwndocapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 09:06:29.000000 pwndocapi-1.3.1/pwndocapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-05 09:06:29.000000 pwndocapi-1.3.1/pwndocapi.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)       16 2023-06-05 09:05:05.000000 pwndocapi-1.3.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 09:06:29.408012 pwndocapi-1.3.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      859 2023-06-05 09:05:20.000000 pwndocapi-1.3.1/setup.py
```

### Comparing `pwndocapi-1.3/LICENSE` & `pwndocapi-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/PKG-INFO` & `pwndocapi-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwndocapi
-Version: 1.3
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: https://github.com/p0dalirius/pwndocapi
 Author: Podalirius
 Author-email: podalirius@protonmail.com
 License: GPL2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pwndocapi-1.3/pwndocapi/API.py` & `pwndocapi-1.3.1/pwndocapi/API.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,30 +98,30 @@
 
     def audits_list(self):  # ok
         return self.__api_get("/api/audits")
 
     def audits_get_by_id(self, _audit_id):  # ok
         return self.__api_get("/api/audits/%s" % _audit_id)
 
-    def audit_add_finding(self, _audit_id, title, vulnType, category, description, observation, remediation, references, remediationComplexity, priority, poc, scope, cvssv3, cvssScore, cvssSeverity, customFields=[]):
+    def audit_add_finding(self, _audit_id, title, vulnType, category, description, observation, remediation, references, remediationComplexity, priority, poc, scope, cvssv3, customFields=[]):
         return self.__api_post(
             "/api/audits/%s/findings" % _audit_id,
             jsondata={
                 "title": title,
                 "vulnType": vulnType,
                 "category": category,
                 "description": description,
                 "observation": observation,
                 "remediation": remediation,
                 "references": references,
                 "remediationComplexity": remediationComplexity,
                 "priority": priority,
                 "cvssv3": cvssv3,
-                "cvssScore": cvssScore,
-                "cvssSeverity": cvssSeverity,
+                # "cvssScore": cvssScore,
+                # "cvssSeverity": cvssSeverity,
                 "poc": poc,
                 "scope": scope,
                 "customFields": customFields
             }
         )
 
     def audit_list_findings(self, _audit_id):
@@ -168,14 +168,18 @@
 
     def findings_get_by_id(self, _audit_id, _finding_id):  # ok
         return self.__api_get("/api/audits/%s/findings/%s" % (_audit_id, _finding_id))
 
     def findings_delete_by_id(self, _audit_id, _finding_id):  # ok
         return self.__api_delete("/api/audits/%s/findings/%s" % (_audit_id, _finding_id))
 
+    # Vulnerabilities =================================================================
+    def vulnerabilities_list(self, lang):
+        return self.__api_get("/api/vulnerabilities/%s" % lang)
+
     # Internal Methods =========================================================
 
     def __api_get(self, endpoint):
         r = self.session.get(self.target + endpoint, verify=False)
         if DEBUG == True:
             print("[debug] GET %s" % endpoint)
             print(json.dumps(r.json(), indent=4))
```

### Comparing `pwndocapi-1.3/pwndocapi/api/audits.py` & `pwndocapi-1.3.1/pwndocapi/api/audits.py`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/pwndocapi/api/data.py` & `pwndocapi-1.3.1/pwndocapi/api/data.py`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/pwndocapi/api/users.py` & `pwndocapi-1.3.1/pwndocapi/api/users.py`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/pwndocapi/models/Audit.py` & `pwndocapi-1.3.1/pwndocapi/models/Audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.api = api
         self._id = _id
         self.__load()
 
     def delete(self):
         self.api.audits_delete(self._id)
 
-    def add_finding(self, title, vulnType, category, description, observation, remediation, references, remediationComplexity, priority, poc, scope, cvssv3, cvssScore, cvssSeverity, customFields=[]):
+    def add_finding(self, title, vulnType, category, description, observation, remediation, references, remediationComplexity, priority, poc, scope, cvssv3, customFields=[]):
         scope = "<ul>" + "".join(["<li><p>%s</p></li>" % vt for vt in scope]) + "</ul>"
 
         self.api.audit_add_finding(
             self._id,
             title=title,
             vulnType=vulnType,
             category=category,
@@ -38,16 +38,16 @@
             remediation=remediation,
             references=references,
             remediationComplexity=remediationComplexity,
             priority=priority,
             poc=poc,
             scope=scope,
             cvssv3=cvssv3,
-            cvssScore=cvssScore,
-            cvssSeverity=cvssSeverity,
+            # cvssScore=cvssScore,
+            # cvssSeverity=cvssSeverity,
             customFields=customFields
         )
 
     def delete_all_findings(self):
         self.api.audit_delete_all_findings(self._id)
 
     ## Data =========================================================
```

### Comparing `pwndocapi-1.3/pwndocapi/models/Finding.py` & `pwndocapi-1.3.1/pwndocapi/models/Finding.py`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/pwndocapi/models/User.py` & `pwndocapi-1.3.1/pwndocapi/models/User.py`

 * *Files identical despite different names*

### Comparing `pwndocapi-1.3/pwndocapi.egg-info/PKG-INFO` & `pwndocapi-1.3.1/pwndocapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwndocapi
-Version: 1.3
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: https://github.com/p0dalirius/pwndocapi
 Author: Podalirius
 Author-email: podalirius@protonmail.com
 License: GPL2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pwndocapi-1.3/pwndocapi.egg-info/SOURCES.txt` & `pwndocapi-1.3.1/pwndocapi.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pwndocapi.egg-info/top_level.txt
 pwndocapi/api/__init__.py
 pwndocapi/api/audits.py
 pwndocapi/api/clients.py
 pwndocapi/api/companies.py
 pwndocapi/api/data.py
 pwndocapi/api/users.py
+pwndocapi/api/vulnerabilities.py
 pwndocapi/models/Audit.py
 pwndocapi/models/AuditError.py
 pwndocapi/models/Finding.py
 pwndocapi/models/Priority.py
 pwndocapi/models/RemediationComplexity.py
 pwndocapi/models/User.py
 pwndocapi/models/__init__.py
```

### Comparing `pwndocapi-1.3/setup.py` & `pwndocapi-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import setuptools
 
 long_description = "A Python native library to automate reporting vulnerabilities into pwndoc."
 
 setuptools.setup(
     name="pwndocapi",
-    version="1.3",
+    version="1.3.1",
     description="",
     url="https://github.com/p0dalirius/pwndocapi",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=setuptools.find_packages(),
```

