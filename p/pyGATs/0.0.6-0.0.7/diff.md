# Comparing `tmp/pyGATs-0.0.6.tar.gz` & `tmp/pyGATs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGATs-0.0.6.tar", last modified: Fri Jun  2 11:50:58 2023, max compression
+gzip compressed data, was "pyGATs-0.0.7.tar", last modified: Mon Jun  5 10:00:39 2023, max compression
```

## Comparing `pyGATs-0.0.6.tar` & `pyGATs-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 11:50:46.000000 pyGATs-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:50:58.540125 pyGATs-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-02 11:50:46.000000 pyGATs-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-02 11:50:46.000000 pyGATs-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:50:58.540125 pyGATs-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.536125 pyGATs-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/src/pyGATs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 11:50:58.000000 pyGATs-0.0.6/src/pyGATs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/src/pygats/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/pygats.py
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-02 11:50:46.000000 pyGATs-0.0.6/src/pygats/recog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:50:58.540125 pyGATs-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 11:50:46.000000 pyGATs-0.0.6/tests/test_pygats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:00:39.389751 pyGATs-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 10:00:24.000000 pyGATs-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-05 10:00:39.389751 pyGATs-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-05 10:00:24.000000 pyGATs-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-05 10:00:24.000000 pyGATs-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:00:39.389751 pyGATs-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:00:39.385751 pyGATs-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:00:39.385751 pyGATs-0.0.7/src/pyGATs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-05 10:00:39.000000 pyGATs-0.0.7/src/pyGATs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 10:00:39.000000 pyGATs-0.0.7/src/pyGATs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:00:39.000000 pyGATs-0.0.7/src/pyGATs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 10:00:39.000000 pyGATs-0.0.7/src/pyGATs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 10:00:39.000000 pyGATs-0.0.7/src/pyGATs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:00:39.389751 pyGATs-0.0.7/src/pygats/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 10:00:24.000000 pyGATs-0.0.7/src/pygats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-05 10:00:24.000000 pyGATs-0.0.7/src/pygats/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-05 10:00:24.000000 pyGATs-0.0.7/src/pygats/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-06-05 10:00:24.000000 pyGATs-0.0.7/src/pygats/pygats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-06-05 10:00:24.000000 pyGATs-0.0.7/src/pygats/recog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:00:39.389751 pyGATs-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 10:00:24.000000 pyGATs-0.0.7/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-05 10:00:24.000000 pyGATs-0.0.7/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 10:00:24.000000 pyGATs-0.0.7/tests/test_pygats.py
```

### Comparing `pyGATs-0.0.6/LICENSE` & `pyGATs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/PKG-INFO` & `pyGATs-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyGATs-0.0.6/README.md` & `pyGATs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/pyproject.toml` & `pyGATs-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyGATs"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="vsysoev" },
 ]
 description = "Automate end-to-end and exploratory testing"
 keywords = ["gui", "testing", "automatic"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyGATs-0.0.6/src/pyGATs.egg-info/PKG-INFO` & `pyGATs-0.0.7/src/pyGATs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGATs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automate end-to-end and exploratory testing
 Author: vsysoev
 License: MIT License
         
         Copyright (c) 2022 IntegraSDL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyGATs-0.0.6/src/pygats/formatters.py` & `pyGATs-0.0.7/src/pygats/formatters.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/src/pygats/misc.py` & `pyGATs-0.0.7/src/pygats/misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/src/pygats/pygats.py` & `pyGATs-0.0.7/src/pygats/pygats.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/src/pygats/recog.py` & `pyGATs-0.0.7/src/pygats/recog.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,16 +242,14 @@
         width (int, optional): The multiplier to determine the beginning of the crop area by width.
         height (int, optional): The multiplier to determine the beginning of the crop area by height
         extend (bool, optional): Whether to extend the crop area by a factor of 2.
 
     Returns:
         Image: The cropped image area.
     """
-    if width == 0 and height == 0:
-        return img
     img_width, img_height = img.size
     factor = 1
     if extend:
         crop_width = img_width // 4
         crop_height = img_height // 4
         factor = 2
     else:
@@ -276,26 +274,25 @@
         extend (bool, optional): Whether to extend the crop area by a factor of 2.
         Defaults to False.
 
     Returns:
         Image: The cropped image area.
     """
     crop_area_params = {
-        'all': img,
         'center': (img, 1, 1, extend),
-        'top-left': (img, 1, 1, extend),
+        'top-left': (img, 0, 0, extend),
         'left': (img, 0, 1, extend),
         'bottom-left': (img, 0, 2, extend),
         'top': (img, 1, 0, extend),
         'bottom': (img, 1, 2, extend),
         'top-right': (img, 2, 0, extend),
         'right': (img, 2, 1, extend),
         'bottom-right': (img, 2, 2, extend)
     }
-    return crop_image(**crop_area_params.get(crop_area)) if crop_area_params.get(crop_area) else img
+    return crop_image(*crop_area_params.get(crop_area)) if crop_area_params.get(crop_area) else img
 
 
 def find_text(img: Image, txt, skip=0, extend=False, one_word=False):
     """Function finds text in image with Tesseract
 
     Args:
         img (Image): image where text will be recognized
@@ -311,31 +308,43 @@
             w (int), h (int): width and height of rectangle where text resides
             found (bool): whether the text is found in the image
     """
     img = find_crop_image(img, txt.area, extend=extend)
     recognized = pytesseract.image_to_data(img, txt.lang).split('\n')
     if not one_word:
         combine_words_in_lines(recognized)
-    x, y, w, h, found = -1, -1, -1, -1, False
+    ret_tuple = (-1, -1, -1, -1, False)
     for line in recognized[1:]:
-        if txt.text in line.split('\t')[11]:
-            print("Найден текст " + line.split('\t')[11])
-            x, y, w, h = map(int, line.split('\t')[6:10])
-            if skip <= 0:
-                break
-            skip -= 1
-            return x, y, w, h, True
-        if int(line.split('\t')[6] + line.split('\t')[7]) != 0:
-            x, y, w, h = map(int, line.split('\t')[6:10])
-            cropped_img = img.crop(x, y, x + w, y + h)
-            x, y, w, h, found = find_cropped_text(
-                cropped_img, txt, skip=skip, one_word=one_word)
-            if found:
-                return x, y, w, h, True
-    return x, y, w, h, found
+        splitted = line.split('\t')
+        if len(splitted) == 12:
+            if splitted[11].find(txt.text) != -1:
+                print("Найден текст " + splitted[11])
+                ret_tuple = (int(splitted[6]),
+                             int(splitted[7]),
+                             int(splitted[8]),
+                             int(splitted[9]),
+                             True)
+                if skip <= 0:
+                    break
+                skip -= 1
+            else:
+                if int(splitted[6]) + int(splitted[7]) != 0:
+                    cropped = img.crop(
+                        (int(splitted[6]), int(splitted[7]),
+                            int(splitted[6]) + int(splitted[8]),
+                            int(splitted[7]) + int(splitted[9])))
+                    cropped_tuple = find_cropped_text(
+                        cropped, txt, 0, one_word)
+                    if cropped_tuple[4]:
+                        return (cropped_tuple[0] + int(splitted[6]),
+                                cropped_tuple[1] + int(splitted[7]),
+                                cropped_tuple[2],
+                                cropped_tuple[3],
+                                cropped_tuple[4])
+    return ret_tuple
 
 
 def recognize_text(img, lang):
     """Function recognizes text in image with Tesseract and combine
     lines to tuple and return lists
 
     Args:
```

### Comparing `pyGATs-0.0.6/tests/test_formatters.py` & `pyGATs-0.0.7/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/tests/test_misc.py` & `pyGATs-0.0.7/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyGATs-0.0.6/tests/test_pygats.py` & `pyGATs-0.0.7/tests/test_pygats.py`

 * *Files identical despite different names*

