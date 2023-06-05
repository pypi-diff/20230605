# Comparing `tmp/cads_sdk-0.0.24-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 56496 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-05 06:39 cads_sdk/__init__.py
+Zip file size: 56553 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-05 09:30 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    20636 b- defN 23-Jun-05 03:48 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    20911 b- defN 23-Jun-05 09:30 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx     1291 b- defN 23-May-19 02:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7111 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/RECORD
-18 files, 279982 bytes uncompressed, 54090 bytes compressed:  80.7%
+-rw-rw-r--  2.0 unx     7111 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/RECORD
+18 files, 280257 bytes uncompressed, 54147 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.24.dist-info/METADATA
+Filename: cads_sdk-0.0.25.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.24.dist-info/WHEEL
+Filename: cads_sdk-0.0.25.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.24.dist-info/top_level.txt
+Filename: cads_sdk-0.0.25.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.24.dist-info/RECORD
+Filename: cads_sdk-0.0.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.24'
+__version__ = '0.0.25'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/display.py

```diff
@@ -512,14 +512,15 @@
             
         elif '.mp3' in row.path:
             samplerate, data = read_mp3(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
         print("DEBUG display succeed")
     
+    
     def read_audio_pq(self, parquet_file, path):
         import os
         import subprocess
         from pyarrow import fs
         import pyarrow.parquet as pq
         import pyarrow as pa
 
@@ -534,36 +535,36 @@
         df_pq = pq.read_table(parquet_file)
         pdf = df_pq.to_pandas()
         pdf = pdf[pdf['path']==path].iloc[0]
         self.write_to_folder(pdf)
         
             
     def displayAudio(self, ex):
-        get_value = ex.description
+        get_value = ex.value
+        get_des = ex.description
         
         if isinstance(self.input_path, str):
             df = self.generate_sql("*")
         elif isinstance(self.input_path, SparkDataFrame):
             df = self.input_path
         
         if 'rel_path' in df.schema.names:
             df.createOrReplaceTempView("tmp_df")
-            df = df.filter(f"rel_path like '%{os.path.basename(get_value)}'").withColumn("parquet_file", input_file_name()).select('parquet_file')
+            df = df.filter(f"rel_path = '{get_value}'").withColumn("parquet_file", input_file_name()).select('parquet_file')
             # df = ss.sql(f"""SELECT path FROM tmp_df where rel_path like '%{os.path.basename(get_value)}' limit 1""").withColumn("parquet_file", input_file_name())
         else:
             df = df.filter(f"path = '{get_value}'").limit(1)
         
         if df.count() == 0:
             df = self.generate_sql("*")
             df = df.filter(f"path = '{get_value}'").limit(1)
             
-        self.read_audio_pq(df.select('parquet_file').collect()[0].parquet_file, get_value)
+        self.read_audio_pq(df.select('parquet_file').collect()[0].parquet_file, get_des)
 
         # _ = [self.write_to_folder(row) for row in df.collect()]
-        # df.foreach(self.write_to_folder)
         
         
     def _repr_html_(self):
         width = height = ''
         if self.width:
             width = ' width="%d"' % self.width
         if self.height:
@@ -571,28 +572,39 @@
             
         if isinstance(self.input_path, str):
             df_path = self.generate_sql("path")
         
             if isinstance(self.from_idx, int):
                 df_path = df_path[self.from_idx:self.to_idx]
         elif isinstance(self.input_path, SparkDataFrame):
-            df_path = self.input_path.select("path")[self.from_idx:self.to_idx]
+            if isinstance(self.from_idx, int):
+                df_path = self.input_path[self.from_idx:self.to_idx]
+            else:
+                df_path = self.input_path.limit(self.limit)
         
         else:
             raise ValueError("Check your input_path, it not string or can not be found")
             
         
         selection_box = widgets.VBox()
         selection_toggles = []
         selected_labels = {}
         
         layout = widgets.Layout(width=str(pd.options.display.width*5)+'px', height='40px')
         
-        for row in df_path.orderBy('path').collect():
-            o = LoadedButton(description=row.path, value=row.path,layout=layout)
+        if 'rel_path' in df_path.schema.names:
+            df_path = df_path.select("path", "rel_path")
+        else:
+            df_path = df_path.selct("path")
+            
+        for row in sorted(df_path.collect()):
+            if 'rel_path' in df_path.schema.names:
+                o = LoadedButton(description=row.path, value=row.rel_path,layout=layout)
+            else:
+                o = LoadedButton(description=row.path, value=row.path,layout=layout)
             o.on_click(self.displayAudio)
             selection_toggles.append(o)
 
         selection_box.children = selection_toggles
         self.output = widgets.Output()
         return display(selection_box, self.output)
     
@@ -602,17 +614,14 @@
             "point is EXCLUDED), listlike of integers, boolean array"
         )
         
         from pandas.core.indexers import (check_array_indexer, is_list_like_indexer)
         
         if not isinstance(key, slice):
             raise ValueError("Invalid call for scalar access (getting)!")
-        # if not is_list_like_indexer(key):
-        #     raise ValueError(f"Can only index by location with a {key}]")
-            
         
         self.from_idx = key.start
         self.to_idx = key.stop
         return self._repr_html_()
     
     def __repr__(self):
         return ""
```

## Comparing `cads_sdk-0.0.24.dist-info/METADATA` & `cads_sdk-0.0.25.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.24
+Version: 0.0.25
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

## Comparing `cads_sdk-0.0.24.dist-info/RECORD` & `cads_sdk-0.0.25.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=DVBD1xBwRvzE4TUxF8sD7DrB423KMIaWfTInn2Jvv6c,1265
+cads_sdk/__init__.py,sha256=eyC0S1MrgjKdxxp0dvuaG_BNw7s7IE4mOzhIsa6FOVw,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
 cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
-cads_sdk/nosql/display.py,sha256=rylK42WnTnUNzsoLO-ZL4nQnVQNmwKqlb3GMyHxKoEs,20636
+cads_sdk/nosql/display.py,sha256=5GlofvnWxw4nzz9hOeee3v_UpAYpRmdI59WNmkLIbgA,20911
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=nQVGBLBx7mhIgLulY1_bUefBEOqHhZbht4jI9E9azuY,1291
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.24.dist-info/METADATA,sha256=1m9WfBIYRLRQeQ5FwlB1YzyVqrCy4j7XS4x84g-v2ps,7111
-cads_sdk-0.0.24.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.24.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.24.dist-info/RECORD,,
+cads_sdk-0.0.25.dist-info/METADATA,sha256=oOe24RoJjXMbuR2dg3QyND59ZY1qoPXVNts9Y8vagT4,7111
+cads_sdk-0.0.25.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.25.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.25.dist-info/RECORD,,
```

