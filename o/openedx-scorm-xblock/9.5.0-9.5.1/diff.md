# Comparing `tmp/openedx-scorm-xblock-9.5.0.tar.gz` & `tmp/openedx-scorm-xblock-9.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openedx-scorm-xblock-9.5.0.tar", last modified: Wed Feb 17 14:29:24 2021, max compression
+gzip compressed data, was "dist/openedx-scorm-xblock-9.5.1.tar", last modified: Wed Feb 24 11:54:05 2021, max compression
```

## Comparing `openedx-scorm-xblock-9.5.0.tar` & `openedx-scorm-xblock-9.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/
--rw-rw-r--   0 regis     (1000) regis     (1000)     5589 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     4291 2021-02-17 14:29:19.000000 openedx-scorm-xblock-9.5.0/README.rst
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)     5589 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)      656 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       46 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       21 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       13 2021-02-17 14:29:24.000000 openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedxscorm/
--rw-rw-r--   0 regis     (1000) regis     (1000)       37 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedxscorm/locale/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/LC_MESSAGES/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1120 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/LC_MESSAGES/django.mo
--rw-rw-r--   0 regis     (1000) regis     (1000)     1503 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/LC_MESSAGES/django.po
--rw-rw-r--   0 regis     (1000) regis     (1000)    20847 2021-02-17 14:29:19.000000 openedx-scorm-xblock-9.5.0/openedxscorm/scormxblock.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedxscorm/static/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/openedxscorm/static/css/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1129 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/static/css/scormxblock.css
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/openedxscorm/static/html/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1016 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/static/html/scormxblock.html
--rw-rw-r--   0 regis     (1000) regis     (1000)     4328 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/static/html/studio.html
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.576094 openedx-scorm-xblock-9.5.0/openedxscorm/static/js/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/openedxscorm/static/js/src/
--rw-rw-r--   0 regis     (1000) regis     (1000)     5560 2021-02-17 14:28:44.000000 openedx-scorm-xblock-9.5.0/openedxscorm/static/js/src/scormxblock.js
--rw-rw-r--   0 regis     (1000) regis     (1000)     2185 2021-02-17 14:24:43.000000 openedx-scorm-xblock-9.5.0/openedxscorm/static/js/src/studio.js
--rw-rw-r--   0 regis     (1000) regis     (1000)     9335 2021-02-17 14:29:19.000000 openedx-scorm-xblock-9.5.0/openedxscorm/tests.py
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2021-02-17 14:29:24.580094 openedx-scorm-xblock-9.5.0/setup.cfg
--rw-rw-r--   0 regis     (1000) regis     (1000)     1561 2021-02-17 14:29:19.000000 openedx-scorm-xblock-9.5.0/setup.py
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.130519 openedx-scorm-xblock-9.5.1/
+-rw-r--r--   0 regis     (1000) regis     (1000)     5589 2021-02-24 11:54:05.130519 openedx-scorm-xblock-9.5.1/PKG-INFO
+-rw-r--r--   0 regis     (1000) regis     (1000)     4291 2021-02-24 11:53:12.000000 openedx-scorm-xblock-9.5.1/README.rst
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.126517 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/
+-rw-r--r--   0 regis     (1000) regis     (1000)     5589 2021-02-24 11:54:04.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 regis     (1000) regis     (1000)      656 2021-02-24 11:54:05.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)        1 2021-02-24 11:54:04.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       46 2021-02-24 11:54:04.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       21 2021-02-24 11:54:04.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/requires.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       13 2021-02-24 11:54:04.000000 openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.126517 openedx-scorm-xblock-9.5.1/openedxscorm/
+-rw-r--r--   0 regis     (1000) regis     (1000)       37 2020-04-25 11:25:31.000000 openedx-scorm-xblock-9.5.1/openedxscorm/__init__.py
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.122516 openedx-scorm-xblock-9.5.1/openedxscorm/locale/
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.122516 openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.126517 openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 regis     (1000) regis     (1000)     1120 2020-04-23 16:18:29.000000 openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 regis     (1000) regis     (1000)     1503 2020-04-25 11:25:50.000000 openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 regis     (1000) regis     (1000)    20944 2021-02-24 11:53:39.000000 openedx-scorm-xblock-9.5.1/openedxscorm/scormxblock.py
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.122516 openedx-scorm-xblock-9.5.1/openedxscorm/static/
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.126517 openedx-scorm-xblock-9.5.1/openedxscorm/static/css/
+-rw-r--r--   0 regis     (1000) regis     (1000)     1129 2020-04-25 11:23:44.000000 openedx-scorm-xblock-9.5.1/openedxscorm/static/css/scormxblock.css
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.130519 openedx-scorm-xblock-9.5.1/openedxscorm/static/html/
+-rw-r--r--   0 regis     (1000) regis     (1000)     1009 2021-02-24 11:53:39.000000 openedx-scorm-xblock-9.5.1/openedxscorm/static/html/scormxblock.html
+-rw-r--r--   0 regis     (1000) regis     (1000)     4328 2020-10-07 12:30:24.000000 openedx-scorm-xblock-9.5.1/openedxscorm/static/html/studio.html
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.122516 openedx-scorm-xblock-9.5.1/openedxscorm/static/js/
+drwxr-xr-x   0 regis     (1000) regis     (1000)        0 2021-02-24 11:54:05.130519 openedx-scorm-xblock-9.5.1/openedxscorm/static/js/src/
+-rw-r--r--   0 regis     (1000) regis     (1000)     5712 2021-02-24 11:53:39.000000 openedx-scorm-xblock-9.5.1/openedxscorm/static/js/src/scormxblock.js
+-rw-r--r--   0 regis     (1000) regis     (1000)     2185 2020-10-07 12:30:24.000000 openedx-scorm-xblock-9.5.1/openedxscorm/static/js/src/studio.js
+-rw-r--r--   0 regis     (1000) regis     (1000)     9335 2021-02-24 11:53:12.000000 openedx-scorm-xblock-9.5.1/openedxscorm/tests.py
+-rw-r--r--   0 regis     (1000) regis     (1000)       38 2021-02-24 11:54:05.130519 openedx-scorm-xblock-9.5.1/setup.cfg
+-rw-r--r--   0 regis     (1000) regis     (1000)     1561 2021-02-24 11:53:44.000000 openedx-scorm-xblock-9.5.1/setup.py
```

### Comparing `openedx-scorm-xblock-9.5.0/PKG-INFO` & `openedx-scorm-xblock-9.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-scorm-xblock
-Version: 9.5.0
+Version: 9.5.1
 Summary: Scorm XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://github.com/overhangio/openedx-scorm-xblock
 Project-URL: Code, https://github.com/overhangio/openedx-scorm-xblock
```

### Comparing `openedx-scorm-xblock-9.5.0/README.rst` & `openedx-scorm-xblock-9.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/PKG-INFO` & `openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-scorm-xblock
-Version: 9.5.0
+Version: 9.5.1
 Summary: Scorm XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://github.com/overhangio/openedx-scorm-xblock
 Project-URL: Code, https://github.com/overhangio/openedx-scorm-xblock
```

### Comparing `openedx-scorm-xblock-9.5.0/openedx_scorm_xblock.egg-info/SOURCES.txt` & `openedx-scorm-xblock-9.5.1/openedx_scorm_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/LC_MESSAGES/django.mo` & `openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/locale/es_419/LC_MESSAGES/django.po` & `openedx-scorm-xblock-9.5.1/openedxscorm/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/scormxblock.py` & `openedx-scorm-xblock-9.5.1/openedxscorm/scormxblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,37 +334,40 @@
         return self.set_value(data)
 
     def set_value(self, data):
         name = data.get("name")
         completion_percent = None
         success_status = None
         completion_status = None
-        context = {"result": "success"}
+        lesson_score = None
 
         if name == "cmi.core.lesson_status":
             lesson_status = data.get("value")
             if lesson_status in ["passed", "failed"]:
                 success_status = lesson_status
             elif lesson_status in ["completed", "incomplete"]:
                 completion_status = lesson_status
         elif name == "cmi.success_status":
             success_status = data.get("value")
         elif name == "cmi.completion_status":
             completion_status = data.get("value")
         elif name in ["cmi.core.score.raw", "cmi.score.raw"] and self.has_score:
-            self.lesson_score = float(data.get("value", 0)) / 100.0
-            context.update({"lesson_score": self.lesson_score})
+            lesson_score = float(data.get("value", 0)) / 100.0
         elif name == "cmi.progress_measure":
             try:
                 completion_percent = float(data.get("value"))
             except (ValueError, TypeError):
                 pass
         else:
             self.scorm_data[name] = data.get("value", "")
 
+        context = {"result": "success"}
+        if lesson_score is not None:
+            self.lesson_score = lesson_score
+            context.update({"grade": self.get_grade()})
         if completion_percent is not None:
             self.emit_completion(completion_percent)
         if completion_status:
             self.lesson_status = completion_status
             context.update({"completion_status": completion_status})
         if success_status:
             self.success_status = success_status
```

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/static/css/scormxblock.css` & `openedx-scorm-xblock-9.5.1/openedxscorm/static/css/scormxblock.css`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/static/html/scormxblock.html` & `openedx-scorm-xblock-9.5.1/openedxscorm/static/html/scormxblock.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load i18n %}
 
 <div class="openedxscorm_block">
     {% if index_page_url %}
 
     {% if scorm_xblock.has_score %}
     <p>
-        (<span class="lesson_score">{{ grade|floatformat }}</span>/{{ scorm_xblock.weight|floatformat }} {% trans "points" %})
+        (<span class="grade">{{ grade|floatformat }}</span>/{{ scorm_xblock.weight|floatformat }} {% trans "points" %})
         <span class="completion_status">{% trans completion_status %}</span>
     </p>
     {% endif %}
 
     <div class="js-scorm-block">
         <div class="scorm_button">
             <button class="js-button-full-screen full-screen-on">
```

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/static/html/studio.html` & `openedx-scorm-xblock-9.5.1/openedxscorm/static/html/studio.html`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/static/js/src/scormxblock.js` & `openedx-scorm-xblock-9.5.1/openedxscorm/static/js/src/scormxblock.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -153,16 +153,18 @@
         $.ajax({
             type: "POST",
             url: setValuesUrl,
             data: JSON.stringify(data),
             success: function(results) {
                 for (var i = 0; i < results.length; i += 1) {
                     var result = results[i];
-                    if (typeof result.lesson_score != "undefined") {
-                        $(element).find(".lesson_score").html(result.lesson_score);
+                    if (typeof result.grade != "undefined") {
+                        // Properly display at most two decimals
+                        console.log(result.grade, Math.round(result.grade * 100) / 100)
+                        $(element).find(".grade").html(Math.round(result.grade * 100) / 100);
                     }
                     $(element).find(".completion_status").html(result.completion_status);
                 }
             },
             complete: function() {
                 // Recursive call to itself
                 processSetValueQueueItems();
```

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/static/js/src/studio.js` & `openedx-scorm-xblock-9.5.1/openedxscorm/static/js/src/studio.js`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/openedxscorm/tests.py` & `openedx-scorm-xblock-9.5.1/openedxscorm/tests.py`

 * *Files identical despite different names*

### Comparing `openedx-scorm-xblock-9.5.0/setup.py` & `openedx-scorm-xblock-9.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.rst"), "rt", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name="openedx-scorm-xblock",
-    version="9.5.0",
+    version="9.5.1",
     description="Scorm XBlock for Open edX",
     long_description=readme,
     long_description_content_type="text/x-rst",
     author="Overhang.io",
     author_email="contact@overhang.io",
     project_urls={
         "Documentation": "https://github.com/overhangio/openedx-scorm-xblock",
```

