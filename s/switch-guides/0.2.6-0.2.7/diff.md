# Comparing `tmp/switch_guides-0.2.6.tar.gz` & `tmp/switch_guides-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_guides-0.2.6.tar", last modified: Thu May  4 03:45:38 2023, max compression
+gzip compressed data, was "switch_guides-0.2.7.tar", last modified: Mon Jun  5 02:34:20 2023, max compression
```

## Comparing `switch_guides-0.2.6.tar` & `switch_guides-0.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.659229 switch_guides-0.2.6/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-05-04 03:45:16.000000 switch_guides-0.2.6/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)     4911 2023-05-04 03:45:16.000000 switch_guides-0.2.6/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-05-04 03:45:16.000000 switch_guides-0.2.6/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-05-04 03:45:16.000000 switch_guides-0.2.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     6205 2023-05-04 03:45:38.659229 switch_guides-0.2.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-05-04 03:45:16.000000 switch_guides-0.2.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-04 03:45:16.000000 switch_guides-0.2.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-05-04 03:45:38.659229 switch_guides-0.2.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1360 2023-05-04 03:45:16.000000 switch_guides-0.2.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.655229 switch_guides-0.2.6/switch_guides/
--rw-r--r--   0 vsts      (1001) docker     (122)    15127 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/SwitchGuideTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      714 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.655229 switch_guides-0.2.6/switch_guides/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.655229 switch_guides-0.2.6/switch_guides/extensions/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1444 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.655229 switch_guides-0.2.6/switch_guides/extensions/component/
--rw-r--r--   0 vsts      (1001) docker     (122)      365 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/component/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4558 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/component/form_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4576 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/extensions/component/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.659229 switch_guides-0.2.6/switch_guides/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      495 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3347 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/enums.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4739 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/guide.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/literals.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9589 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/models/step.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.659229 switch_guides-0.2.6/switch_guides/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)      766 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13031 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/pipeline/automation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.659229 switch_guides-0.2.6/switch_guides/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)     3163 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/tasks/GuideDefinitionTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)      605 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/tasks/GuideRetrySupportTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7701 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10606 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/tasks/GuideStepDefinitionTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1014 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.659229 switch_guides-0.2.6/switch_guides/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-05-04 03:45:16.000000 switch_guides-0.2.6/switch_guides/utils/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 03:45:38.655229 switch_guides-0.2.6/switch_guides.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     6205 2023-05-04 03:45:38.000000 switch_guides-0.2.6/switch_guides.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1156 2023-05-04 03:45:38.000000 switch_guides-0.2.6/switch_guides.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-04 03:45:38.000000 switch_guides-0.2.6/switch_guides.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-04 03:45:38.000000 switch_guides-0.2.6/switch_guides.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-05-04 03:45:38.000000 switch_guides-0.2.6/switch_guides.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-05 02:33:57.000000 switch_guides-0.2.7/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     4964 2023-06-05 02:33:57.000000 switch_guides-0.2.7/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-05 02:33:57.000000 switch_guides-0.2.7/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-06-05 02:33:57.000000 switch_guides-0.2.7/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6258 2023-06-05 02:34:20.079533 switch_guides-0.2.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-06-05 02:33:57.000000 switch_guides-0.2.7/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-06-05 02:33:57.000000 switch_guides-0.2.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-05 02:34:20.083533 switch_guides-0.2.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1367 2023-06-05 02:33:57.000000 switch_guides-0.2.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.075533 switch_guides-0.2.7/switch_guides/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15127 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/SwitchGuideTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      714 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/extensions/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1444 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/extensions/component/
+-rw-r--r--   0 vsts      (1001) docker     (122)      365 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/component/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4558 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/component/form_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4576 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/extensions/component/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      495 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3347 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4739 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/guide.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/literals.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9589 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/models/step.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)      766 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13031 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/pipeline/automation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3163 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/tasks/GuideDefinitionTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      605 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/tasks/GuideRetrySupportTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7701 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10606 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/tasks/GuideStepDefinitionTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1014 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-06-05 02:33:57.000000 switch_guides-0.2.7/switch_guides/utils/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 02:34:20.079533 switch_guides-0.2.7/switch_guides.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6258 2023-06-05 02:34:20.000000 switch_guides-0.2.7/switch_guides.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1156 2023-06-05 02:34:20.000000 switch_guides-0.2.7/switch_guides.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 02:34:20.000000 switch_guides-0.2.7/switch_guides.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-06-05 02:34:20.000000 switch_guides-0.2.7/switch_guides.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-06-05 02:34:20.000000 switch_guides-0.2.7/switch_guides.egg-info/top_level.txt
```

### Comparing `switch_guides-0.2.6/HISTORY.md` & `switch_guides-0.2.7/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 0.2.7
+Updated
+* pydantic version to latest 1.0.0
+
 ## 0.2.6
 
 Updated
 * journey_id is deprecated in favour of guide_id in SwitchGuideStepProcessInput
 * journey_id is also now optional
 
 ## 0.2.5
```

### Comparing `switch_guides-0.2.6/LICENCE` & `switch_guides-0.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/PKG-INFO` & `switch_guides-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_guides
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for building Platform Guides in Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,18 @@
 
 ```bash
 pip install switch-guides
 ```
 
 # History
 
+## 0.2.7
+Updated
+* pydantic version to latest 1.0.0
+
 ## 0.2.6
 
 Updated
 * journey_id is deprecated in favour of guide_id in SwitchGuideStepProcessInput
 * journey_id is also now optional
 
 ## 0.2.5
```

### Comparing `switch_guides-0.2.6/README.md` & `switch_guides-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/setup.py` & `switch_guides-0.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A package for building Platform Guides in Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_guides",
-    version="0.2.6",
+    version="0.2.7",
     packages=find_packages(
         include=["switch_guides", "switch_guides.*"],
         exclude=["switch_guides.tests", "switch_guides.tests.*"]
     ),
-    install_requires=['switch-api','pydantic==1.9.0'],
+    install_requires=['switch-api','pydantic>=1.0.0,<2.0.0'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Other Audience',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
```

### Comparing `switch_guides-0.2.6/switch_guides/SwitchGuideTask.py` & `switch_guides-0.2.7/switch_guides/SwitchGuideTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/__init__.py` & `switch_guides-0.2.7/switch_guides/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     'api',
     'step',
     'guide',
     'literals',
     'enums'
 ]
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
```

### Comparing `switch_guides-0.2.6/switch_guides/exceptions.py` & `switch_guides-0.2.7/switch_guides/exceptions.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/extensions/cache/cache.py` & `switch_guides-0.2.7/switch_guides/extensions/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/extensions/component/form_data.py` & `switch_guides-0.2.7/switch_guides/extensions/component/form_data.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/extensions/component/forms.py` & `switch_guides-0.2.7/switch_guides/extensions/component/forms.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/models/api.py` & `switch_guides-0.2.7/switch_guides/models/api.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/models/guide.py` & `switch_guides-0.2.7/switch_guides/models/guide.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/models/literals.py` & `switch_guides-0.2.7/switch_guides/models/literals.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/models/step.py` & `switch_guides-0.2.7/switch_guides/models/step.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/pipeline/__init__.py` & `switch_guides-0.2.7/switch_guides/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/pipeline/automation.py` & `switch_guides-0.2.7/switch_guides/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/tasks/GuideDefinitionTask.py` & `switch_guides-0.2.7/switch_guides/tasks/GuideDefinitionTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/tasks/GuideRetrySupportTask.py` & `switch_guides-0.2.7/switch_guides/tasks/GuideRetrySupportTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py` & `switch_guides-0.2.7/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/tasks/GuideStepDefinitionTask.py` & `switch_guides-0.2.7/switch_guides/tasks/GuideStepDefinitionTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/tasks/__init__.py` & `switch_guides-0.2.7/switch_guides/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides/utils/utils.py` & `switch_guides-0.2.7/switch_guides/utils/utils.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.6/switch_guides.egg-info/PKG-INFO` & `switch_guides-0.2.7/switch_guides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-guides
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for building Platform Guides in Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,18 @@
 
 ```bash
 pip install switch-guides
 ```
 
 # History
 
+## 0.2.7
+Updated
+* pydantic version to latest 1.0.0
+
 ## 0.2.6
 
 Updated
 * journey_id is deprecated in favour of guide_id in SwitchGuideStepProcessInput
 * journey_id is also now optional
 
 ## 0.2.5
```

### Comparing `switch_guides-0.2.6/switch_guides.egg-info/SOURCES.txt` & `switch_guides-0.2.7/switch_guides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

