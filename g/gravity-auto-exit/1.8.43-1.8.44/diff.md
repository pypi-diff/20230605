# Comparing `tmp/gravity_auto_exit-1.8.43-py3-none-any.whl.zip` & `tmp/gravity_auto_exit-1.8.44-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6205 bytes, number of entries: 11
+Zip file size: 6192 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-03 11:23 gravity_auto_exit/__init__.py
 -rw-rw-rw-  2.0 fat      978 b- defN 22-Nov-06 04:54 gravity_auto_exit/logger.py
--rw-rw-rw-  2.0 fat     7830 b- defN 23-Jun-05 11:55 gravity_auto_exit/main.py
--rw-rw-rw-  2.0 fat      654 b- defN 23-May-22 11:34 gravity_auto_exit/mixins.py
+-rw-rw-rw-  2.0 fat     7768 b- defN 23-Jun-05 12:04 gravity_auto_exit/main.py
+-rw-rw-rw-  2.0 fat      633 b- defN 23-Jun-05 12:04 gravity_auto_exit/mixins.py
 -rw-rw-rw-  2.0 fat      327 b- defN 22-Nov-06 04:14 gravity_auto_exit/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-06 04:12 gravity_auto_exit/logs/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 11:57 gravity_auto_exit-1.8.43.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      409 b- defN 23-Jun-05 11:57 gravity_auto_exit-1.8.43.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 11:57 gravity_auto_exit-1.8.43.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-05 11:57 gravity_auto_exit-1.8.43.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      944 b- defN 23-Jun-05 11:57 gravity_auto_exit-1.8.43.dist-info/RECORD
-11 files, 12343 bytes uncompressed, 4577 bytes compressed:  62.9%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 12:05 gravity_auto_exit-1.8.44.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      409 b- defN 23-Jun-05 12:05 gravity_auto_exit-1.8.44.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 12:05 gravity_auto_exit-1.8.44.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-05 12:05 gravity_auto_exit-1.8.44.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      944 b- defN 23-Jun-05 12:05 gravity_auto_exit-1.8.44.dist-info/RECORD
+11 files, 12260 bytes uncompressed, 4564 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gravity_auto_exit/settings.py
 Comment: 
 
 Filename: gravity_auto_exit/logs/__init__.py
 Comment: 
 
-Filename: gravity_auto_exit-1.8.43.dist-info/LICENSE
+Filename: gravity_auto_exit-1.8.44.dist-info/LICENSE
 Comment: 
 
-Filename: gravity_auto_exit-1.8.43.dist-info/METADATA
+Filename: gravity_auto_exit-1.8.44.dist-info/METADATA
 Comment: 
 
-Filename: gravity_auto_exit-1.8.43.dist-info/WHEEL
+Filename: gravity_auto_exit-1.8.44.dist-info/WHEEL
 Comment: 
 
-Filename: gravity_auto_exit-1.8.43.dist-info/top_level.txt
+Filename: gravity_auto_exit-1.8.44.dist-info/top_level.txt
 Comment: 
 
-Filename: gravity_auto_exit-1.8.43.dist-info/RECORD
+Filename: gravity_auto_exit-1.8.44.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gravity_auto_exit/main.py

```diff
@@ -139,16 +139,14 @@
     def try_recognise_plate(self):
         logger.debug(f'Taking photo...')
         photo = self.cam.take_shot()
         if not photo:
             return photo
         if self.size:
             photo = self.cut_photo(photo)
-        return
-        #result = self.get_car_number(photo)
         result = self._recognise(photo)
         return result
 
     def _recognise(self, photo):
         return self.neurocore_worker.get_car_number(photo)
 
     def get_car_number(self, photo):
```

## gravity_auto_exit/mixins.py

```diff
@@ -17,12 +17,11 @@
     def cut_photo(self, photo):
         if not self.size:
             return photo
         img = Image.open(io.BytesIO(photo))
         # left, upper, right, lower
         # 2592*1944
         im_r = img.crop(self.size)
-        im_r.show()
         img_byte_arr = io.BytesIO()
         im_r.save(img_byte_arr, format='PNG')
         img_byte_arr = img_byte_arr.getvalue()
         return img_byte_arr
```

## Comparing `gravity_auto_exit-1.8.43.dist-info/LICENSE` & `gravity_auto_exit-1.8.44.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gravity_auto_exit-1.8.43.dist-info/RECORD` & `gravity_auto_exit-1.8.44.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gravity_auto_exit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gravity_auto_exit/logger.py,sha256=fqAx0eDI7R3dEGnnkoIqaTbg2qrcVuRUGAeDFnMQktA,978
-gravity_auto_exit/main.py,sha256=cQzAs655YQTrRWSTil3VF1-XcZxRZNUgShnwsPZDMZU,7830
-gravity_auto_exit/mixins.py,sha256=o3GoP9Itk2-tlxkfcUHtme7s1DoY_tdB99S9TdIomRs,654
+gravity_auto_exit/main.py,sha256=xtVMyGbp9DkmfNtCfsEcwoWiSd2hRD8RwBHsB4wxvxg,7768
+gravity_auto_exit/mixins.py,sha256=w4tX3-c0wf_y6N8MQXN0Dw_OVh88TM_HzaJRdLz4hpk,633
 gravity_auto_exit/settings.py,sha256=W4ZrNBbyEsoDMvEAvRK5AH6Q2DLrK2tCzVX3i069rpE,327
 gravity_auto_exit/logs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gravity_auto_exit-1.8.43.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gravity_auto_exit-1.8.43.dist-info/METADATA,sha256=qBa7uDsausi-hGXQ8a56t5udo6HZvPU4679k7VV6qzU,409
-gravity_auto_exit-1.8.43.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gravity_auto_exit-1.8.43.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
-gravity_auto_exit-1.8.43.dist-info/RECORD,,
+gravity_auto_exit-1.8.44.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gravity_auto_exit-1.8.44.dist-info/METADATA,sha256=QB83bf_YG-zzjG6wuBUJWbL1Ih_xnoItzh_-hsIuKDs,409
+gravity_auto_exit-1.8.44.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gravity_auto_exit-1.8.44.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
+gravity_auto_exit-1.8.44.dist-info/RECORD,,
```

