# Comparing `tmp/intelicity-0.0.7-py3-none-any.whl.zip` & `tmp/intelicity-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 19226 bytes, number of entries: 23
+Zip file size: 19280 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      198 b- defN 23-Jun-02 15:43 intelicity/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 intelicity/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 intelicity/bound_box.py
--rw-rw-r--  2.0 unx     3342 b- defN 23-Jun-02 15:43 intelicity/containers.py
+-rw-rw-r--  2.0 unx     3387 b- defN 23-Jun-05 21:47 intelicity/containers.py
 -rw-rw-r--  2.0 unx     6812 b- defN 23-Jun-05 21:26 intelicity/contents.py
--rw-rw-r--  2.0 unx     1181 b- defN 23-Jun-02 15:45 intelicity/file_header.py
+-rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-05 21:47 intelicity/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 intelicity/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 intelicity/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 intelicity/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-02 13:45 src/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 src/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 src/bound_box.py
 -rw-rw-r--  2.0 unx     3335 b- defN 23-Jun-02 13:23 src/containers.py
 -rw-rw-r--  2.0 unx     6699 b- defN 23-Jun-02 13:23 src/contents.py
 -rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-02 13:24 src/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 src/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 src/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 src/main.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-05 21:27 intelicity-0.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-05 21:27 intelicity-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 21:27 intelicity-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 21:27 intelicity-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-05 21:27 intelicity-0.0.7.dist-info/RECORD
-23 files, 60891 bytes uncompressed, 16426 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/RECORD
+23 files, 60982 bytes uncompressed, 16480 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: src/image.py
 Comment: 
 
 Filename: src/main.py
 Comment: 
 
-Filename: intelicity-0.0.7.dist-info/LICENSE
+Filename: intelicity-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: intelicity-0.0.7.dist-info/METADATA
+Filename: intelicity-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: intelicity-0.0.7.dist-info/WHEEL
+Filename: intelicity-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: intelicity-0.0.7.dist-info/top_level.txt
+Filename: intelicity-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: intelicity-0.0.7.dist-info/RECORD
+Filename: intelicity-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intelicity/containers.py

```diff
@@ -12,16 +12,16 @@
         with open(path, 'w') as file:
             for file_content in self.contents:
                 file.write(str(file_content)+"\n")
 
 
 class NetworkOutputContainer(Container):
     @classmethod
-    def create_from_line_list(cls, lines: list[str]) -> "NetworkOutputContainer":
-        contents = [NetworkOutputContent.create_from_line(line) for line in lines]
+    def create_from_line_list(cls, lines: list[str], local_root_object_id=0) -> "NetworkOutputContainer":
+        contents = [NetworkOutputContent.create_from_line(line,local_root_object_id) for line in lines]
         return NetworkOutputContainer(contents)
 
     def __init__(self, contents: list[NetworkOutputContent]):
         super().__init__(contents)
 
     def concatenate(self, network_output_container: "NetworkOutputContainer") -> None:
         """
```

## intelicity/file_header.py

```diff
@@ -15,19 +15,19 @@
         self.driver_id = file_name_info[0]
         self.date = file_name_info[1]
         self.time = file_name_info[2]
 
     def get_neighbor_image(self) -> Image:
         return Image(self.path.with_suffix(".jpg"))
 
-    def open_as_network_output_container(self) -> NetworkOutputContainer:
+    def open_as_network_output_container(self, local_root_object_id=0) -> NetworkOutputContainer:
         lines: list[str]
         with open(self.path, 'r') as file:
             lines = file.read().splitlines()
-        network_output_container = NetworkOutputContainer.create_from_line_list(lines)
+        network_output_container = NetworkOutputContainer.create_from_line_list(lines, local_root_object_id)
         return network_output_container
 
     def open_as_database_container(self) -> DatabaseContainer:
         lines: list[str]
         with open(self.path, 'r') as file:
             lines = file.readlines()
         database_container = DatabaseContainer.create_from_line_list(lines)
```

## Comparing `intelicity-0.0.7.dist-info/LICENSE` & `intelicity-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intelicity-0.0.7.dist-info/METADATA` & `intelicity-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelicity
-Version: 0.0.7
+Version: 0.0.8
 Summary: a library for reading and managing data from the Intelicity server
 Author: Me
 Author-email: Felipe Rodrigues Peixoto da Silva <frps2003@gmail.com>
 License: MIT
 Project-URL: Homepage, https://inteli.city/
 Project-URL: project, https://github.com/Comunalti/Intelicity_Library
 Classifier: Programming Language :: Python :: 3
```

## Comparing `intelicity-0.0.7.dist-info/RECORD` & `intelicity-0.0.8.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 intelicity/__init__.py,sha256=9altPjTiEzAuopDxqZp8lxcRVVQy6ljkePJykZhhKGs,198
 intelicity/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
 intelicity/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
-intelicity/containers.py,sha256=ueAGxShYGzMZT-fQGxkRpQslLP5jmVLKC09ZnVM4PC0,3342
+intelicity/containers.py,sha256=tah1soBkAWdcFNY6TU7Zu1WYeFKflawQ7DrIQ_binrI,3387
 intelicity/contents.py,sha256=HZLC6swlVvt8b50JUkSMPpsNhq1iU2fBdMdI__9y66o,6812
-intelicity/file_header.py,sha256=sAFSRT63Jzf-mB40F1qZsEgs7Pb-N-_IWve7OySHnpg,1181
+intelicity/file_header.py,sha256=buYfFX4j_FEYda4RaKUC2lceVWZG7fyuUDYp8W13aLY,1227
 intelicity/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 intelicity/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 intelicity/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
 src/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
 src/containers.py,sha256=lmFi2ycZdA2iwqrY0vWsZG89QY81kEdsoVlP0IWJwRY,3335
 src/contents.py,sha256=8OQTCisgAt7W8kV0Kbz5Qeo7PhtwobRM4Ssmw1vFAY0,6699
 src/file_header.py,sha256=PpvZii5xMJhZMlVOlg2vmKHApM8kQvFB-ck-dV3j-bk,1171
 src/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 src/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 src/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
-intelicity-0.0.7.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-intelicity-0.0.7.dist-info/METADATA,sha256=GMBAlkw7Z1nBV8VQzkqh3mNcxBpyPOIztCqOAvBlVuE,643
-intelicity-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-intelicity-0.0.7.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
-intelicity-0.0.7.dist-info/RECORD,,
+intelicity-0.0.8.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+intelicity-0.0.8.dist-info/METADATA,sha256=MlLRKuxkHD4pM0o1u31QsyKhybmxfQ77WifV84L0Hk0,643
+intelicity-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+intelicity-0.0.8.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
+intelicity-0.0.8.dist-info/RECORD,,
```

