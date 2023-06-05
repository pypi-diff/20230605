# Comparing `tmp/cads_sdk-0.0.23-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 56028 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-19 04:21 cads_sdk/__init__.py
+Zip file size: 56496 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-05 06:39 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    19283 b- defN 23-May-19 04:21 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    20636 b- defN 23-Jun-05 03:48 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx     1291 b- defN 23-May-19 02:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1480 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/RECORD
-18 files, 278644 bytes uncompressed, 53622 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7111 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-05 06:39 cads_sdk-0.0.24.dist-info/RECORD
+18 files, 279982 bytes uncompressed, 54090 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.23.dist-info/METADATA
+Filename: cads_sdk-0.0.24.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.23.dist-info/WHEEL
+Filename: cads_sdk-0.0.24.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.23.dist-info/top_level.txt
+Filename: cads_sdk-0.0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.23.dist-info/RECORD
+Filename: cads_sdk-0.0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.23'
+__version__ = '0.0.24'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/display.py

```diff
@@ -32,14 +32,15 @@
     Type,
     Union,
     cast,
     overload,
     TYPE_CHECKING,
 )
 from pyspark.sql.column import Column
+from pyspark.sql.functions import input_file_name
 
 import pandas as pd
 pd.options.display.width = 200
 
 
 def cvtColor(binary):
     b,g,r = Image.open(io.BytesIO(binary)).split()
@@ -273,16 +274,16 @@
 
 
 from spark_sdk.utils import import_or_install
 import_or_install("ipywidgets")
 try:
     os.system("jupyter nbextension enable --py --sys-prefix widgetsnbextension")
 except:
-    os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 ipywidgets")
-    os.system("jupyter nbextension enable --py --sys-prefix widgetsnbextension")
+    os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 ipywidgets --prefix /opt/conda/lib/python3.8/")
+    os.system("/opt/conda/bin/jupyter nbextension enable --py --sys-prefix widgetsnbextension")
     
 from ipywidgets.widgets import Box
 from ipywidgets import widgets
 from traitlets import traitlets
 
 from spark_sdk import PySpark
 import numpy as np
@@ -497,44 +498,71 @@
         return df
     
     
     def write_to_folder(self, row):
         if '.pcm' in row.path:
             data = np.frombuffer(row.audio, dtype = 'float64')
             from IPython.display import Audio, display
-            self.output.append_display_data(Audio(data, rate=int(row['samplerate'])))
+            self.output.append_display_data(Audio(data, rate=int(row.samplerate)))
             
         elif '.wav' in row.path:
             from scipy.io import wavfile
             samplerate, data = wavfile.read(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
             
         elif '.mp3' in row.path:
             samplerate, data = read_mp3(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
+        print("DEBUG display succeed")
+    
+    def read_audio_pq(self, parquet_file, path):
+        import os
+        import subprocess
+        from pyarrow import fs
+        import pyarrow.parquet as pq
+        import pyarrow as pa
+
+        os.environ['HADOOP_CONF_DIR'] = "/etc/hadoop/conf/"
+        os.environ['JAVA_HOME'] = "/usr/jdk64/jdk1.8.0_112"
+        os.environ['HADOOP_HOME'] = "/usr/hdp/3.1.0.0-78/hadoop"
+        os.environ['ARROW_LIBHDFS_DIR'] = "/usr/hdp/3.1.0.0-78/usr/lib/"
+        os.environ['CLASSPATH'] = subprocess.check_output("$HADOOP_HOME/bin/hadoop classpath --glob", shell=True).decode('utf-8')
+
+        hdfs = fs.HadoopFileSystem(host="hdfs://hdfs-cluster.datalake.bigdata.local", port=8020)
+
+        df_pq = pq.read_table(parquet_file)
+        pdf = df_pq.to_pandas()
+        pdf = pdf[pdf['path']==path].iloc[0]
+        self.write_to_folder(pdf)
+        
             
     def displayAudio(self, ex):
         get_value = ex.description
         
-        df = self.generate_sql("*")
+        if isinstance(self.input_path, str):
+            df = self.generate_sql("*")
+        elif isinstance(self.input_path, SparkDataFrame):
+            df = self.input_path
         
         if 'rel_path' in df.schema.names:
-            print("DEUBG filter", f"rel_path like '%{os.path.basename(get_value)}'")
             df.createOrReplaceTempView("tmp_df")
-            df = ss.sql(f"""SELECT * FROM tmp_df where rel_path like '%{os.path.basename(get_value)}'""")
+            df = df.filter(f"rel_path like '%{os.path.basename(get_value)}'").withColumn("parquet_file", input_file_name()).select('parquet_file')
+            # df = ss.sql(f"""SELECT path FROM tmp_df where rel_path like '%{os.path.basename(get_value)}' limit 1""").withColumn("parquet_file", input_file_name())
         else:
             df = df.filter(f"path = '{get_value}'").limit(1)
         
         if df.count() == 0:
             df = self.generate_sql("*")
             df = df.filter(f"path = '{get_value}'").limit(1)
             
-        _ = [self.write_to_folder(row) for row in df.collect()]
+        self.read_audio_pq(df.select('parquet_file').collect()[0].parquet_file, get_value)
+
+        # _ = [self.write_to_folder(row) for row in df.collect()]
         # df.foreach(self.write_to_folder)
         
         
     def _repr_html_(self):
         width = height = ''
         if self.width:
             width = ' width="%d"' % self.width
@@ -543,15 +571,15 @@
             
         if isinstance(self.input_path, str):
             df_path = self.generate_sql("path")
         
             if isinstance(self.from_idx, int):
                 df_path = df_path[self.from_idx:self.to_idx]
         elif isinstance(self.input_path, SparkDataFrame):
-            df_path = self.input_path[self.from_idx:self.to_idx]
+            df_path = self.input_path.select("path")[self.from_idx:self.to_idx]
         
         else:
             raise ValueError("Check your input_path, it not string or can not be found")
             
         
         selection_box = widgets.VBox()
         selection_toggles = []
```

## Comparing `cads_sdk-0.0.23.dist-info/METADATA` & `cads_sdk-0.0.24.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.23
+Version: 0.0.24
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -168,15 +168,15 @@
 ### Suport pcm, mp3, wav format
 ### Convert a folder audio to parquet
 ```python
 from cads_sdk.nosql.converter import ConvertFromFolderImage
 
 converter = ConvertFromFolderAudio(
               input_path='/path/to/audio_wav/*.wav', #(1)
-              input_type = 'wav' # 'wav'| 'mp3' | 'pcm' ('wav', 'mp3')
+              input_type = 'wav' # 'wav'| 'mp3' | 'pcm'
               input_recursive = False,
               output_path = f"file:/output/path/audio_wav.parquet",
              )
 
 converter.execute()
 ```
 ### Convert a parquet to folder audio
```

## Comparing `cads_sdk-0.0.23.dist-info/RECORD` & `cads_sdk-0.0.24.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=zwcmYI4WuxBuYAxJZ-A11xdLaQVP-lzvOTXYMMUCSJs,1265
+cads_sdk/__init__.py,sha256=DVBD1xBwRvzE4TUxF8sD7DrB423KMIaWfTInn2Jvv6c,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
 cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
-cads_sdk/nosql/display.py,sha256=xoPolRkz6LUhCAKOVZWrgKdFzoj91Gfte3hO7iJ1ADY,19283
+cads_sdk/nosql/display.py,sha256=rylK42WnTnUNzsoLO-ZL4nQnVQNmwKqlb3GMyHxKoEs,20636
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=nQVGBLBx7mhIgLulY1_bUefBEOqHhZbht4jI9E9azuY,1291
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.23.dist-info/METADATA,sha256=sGgeOoM69xQF9TQNJpFnSbtPJdPxGIp_XnLWEWsqiKE,7126
-cads_sdk-0.0.23.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.23.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.23.dist-info/RECORD,,
+cads_sdk-0.0.24.dist-info/METADATA,sha256=1m9WfBIYRLRQeQ5FwlB1YzyVqrCy4j7XS4x84g-v2ps,7111
+cads_sdk-0.0.24.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.24.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.24.dist-info/RECORD,,
```

