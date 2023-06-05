# Comparing `tmp/inventree-wireviz-plugin-0.4.0.tar.gz` & `tmp/inventree-wireviz-plugin-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.4.0.tar", last modified: Thu Jun  1 13:59:14 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.4.1.tar", last modified: Mon Jun  5 03:41:08 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.4.0.tar` & `inventree-wireviz-plugin-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/setup.py
```

### Comparing `inventree-wireviz-plugin-0.4.0/LICENSE` & `inventree-wireviz-plugin-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.0/PKG-INFO` & `inventree-wireviz-plugin-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.4.0/README.md` & `inventree-wireviz-plugin-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.0/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.4.1/inventree_wireviz/wireviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,21 +426,23 @@
                 quantity = self.convert_quantity(quantity, unit, sub_part.units)
 
             if not description:
                 self.add_error(f"No description for line: {line}")
                 continue
 
             # Construct a new BomItem object
-            self.bom_items.append(BomItem(
-                part=self.part,
-                sub_part=sub_part,
-                quantity=quantity,
-                reference=' '.join(designators),
-                note="Wireviz BOM item"
-            ))
+            # Prevent zero-quantity BOM Items
+            if quantity > 0:
+                self.bom_items.append(BomItem(
+                    part=self.part,
+                    sub_part=sub_part,
+                    quantity=quantity,
+                    reference=' '.join(designators),
+                    note="Wireviz BOM item"
+                ))
         
         # Write BOM data to database
         self.save_bom_data()
 
     def save_bom_data(self):
         """Write the extracted BOM data to the database."""
```

### Comparing `inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.0/setup.py` & `inventree-wireviz-plugin-0.4.1/setup.py`

 * *Files identical despite different names*

