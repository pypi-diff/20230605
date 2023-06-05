# Comparing `tmp/qgate_perf-0.2.8-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17312 bytes, number of entries: 17
+Zip file size: 17311 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    13562 b- defN 23-May-30 17:30 qgate_perf/parallel_executor.py
--rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
+-rw-rw-rw-  2.0 fat    13564 b- defN 23-Jun-05 18:35 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat     5431 b- defN 23-Jun-05 18:34 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-30 17:39 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-05 18:36 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     4587 b- defN 23-May-26 18:34 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/RECORD
-17 files, 53959 bytes uncompressed, 15088 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-05 18:36 qgate_perf-0.2.9.dist-info/RECORD
+17 files, 53961 bytes uncompressed, 15087 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.8.dist-info/LICENSE
+Filename: qgate_perf-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.8.dist-info/METADATA
+Filename: qgate_perf-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.8.dist-info/WHEEL
+Filename: qgate_perf-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.8.dist-info/top_level.txt
+Filename: qgate_perf-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.8.dist-info/RECORD
+Filename: qgate_perf-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -163,17 +163,17 @@
             out = {
                 FileFormat.PRF_TYPE: FileFormat.PRF_CORE_TYPE,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR_ALL: processes * threads,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR: [processes, threads],
                 FileFormat.PRF_CORE_REAL_EXECUTOR: count,
                 FileFormat.PRF_CORE_GROUP: group,
                 FileFormat.PRF_CORE_TOTAL_CALL: sum_call,
+                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count) == 0 else (1 / (sum_time / count)) * count * run_setup._bulk_row,
                 FileFormat.PRF_CORE_AVRG_TIME: sum_time / count,
                 FileFormat.PRF_CORE_STD_DEVIATION: sum_deviation / count,
-                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count)==0 else (1 / (sum_time / count)) * count * run_setup._bulk_row,
                 FileFormat.PRF_CORE_TIME_END: datetime.datetime.utcnow().isoformat(' ')
             }
             self._print(file, f"  {json.dumps(out)}")
 
     def run_bulk_executor(self,
                               bulk_list= BundleHelper.ROW_1_COL_10_100,
                               executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
```

## qgate_perf/parallel_probe.py

 * *Ordering differences only*

```diff
@@ -97,19 +97,19 @@
     def ToString(self):
         """ Provider view to return value """
         if self.exception is None:
             out={
                 FileFormat.PRF_TYPE: FileFormat.PRF_DETAIL_TYPE,
                 FileFormat.PRF_DETAIL_PROCESSID: self.pid,
                 FileFormat.PRF_DETAIL_CALLS: self.counter,
-                FileFormat.PRF_DETAIL_TOTAL: self.total_duration,
                 FileFormat.PRF_DETAIL_AVRG: self.total_duration / self.counter,
                 FileFormat.PRF_DETAIL_MIN: self.min_duration,
                 FileFormat.PRF_DETAIL_MAX: self.max_duration,
                 FileFormat.PRF_DETAIL_STDEV: self.standard_deviation,
+                FileFormat.PRF_DETAIL_TOTAL: self.total_duration,
                 FileFormat.PRF_DETAIL_TIME_INIT: self.track_time[FileFormat.PRF_DETAIL_TIME_INIT].isoformat(' '),
                 FileFormat.PRF_DETAIL_TIME_START: self.track_time[FileFormat.PRF_DETAIL_TIME_START].isoformat(' '),
                 FileFormat.PRF_DETAIL_TIME_END: self.track_time[FileFormat.PRF_DETAIL_TIME_END].isoformat(' ')
             }
             return json.dumps(out)
         else:
             out={
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.8'
+__version__ = '0.2.9'
```

## Comparing `qgate_perf-0.2.8.dist-info/LICENSE` & `qgate_perf-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.8.dist-info/METADATA` & `qgate_perf-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.8
+Version: 0.2.9
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.2.8.dist-info/RECORD` & `qgate_perf-0.2.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=eCjSAFwP_SkXZ8LbSW4qW2hrYrPo77168kDW1mFhO10,13562
-qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
+qgate_perf/parallel_executor.py,sha256=-7Olurn3uN0urkPKtwnq4e8Vl6XQQTMBzGH_GUArl7U,13564
+qgate_perf/parallel_probe.py,sha256=D1TuHfYxoZxXa1xXhXk4uyRKmNOEoUtSc0dkZ6Yqe1U,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=hCpvZak-7VEyuDRgh_IqJx6VYcUDqTkXi1a27V8ddsI,1824
-qgate_perf/version.py,sha256=bBIENHlouRrMMv0LXT_sGmoD7UWHaQVBi8MmaJRsq6c,215
+qgate_perf/version.py,sha256=gt_GLa4bphFxrzuubUzK7feRw1do0IWOU3TwYMz1Kdc,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
 tests/test_run.py,sha256=TZzHiy02r0reYxB2bfoEKsDmtwAEBBXy9ZUy2UCK_9g,4587
-qgate_perf-0.2.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.2.8.dist-info/METADATA,sha256=9sBabIE1qd92hvKP6770-fp4TP832SsMw49lfoIahOs,6964
-qgate_perf-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.2.8.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.2.8.dist-info/RECORD,,
+qgate_perf-0.2.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.2.9.dist-info/METADATA,sha256=dlKzl98d6aPMYgA0ryZIQwJyQN80cJXaltjPcbFbp9s,6964
+qgate_perf-0.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.2.9.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.2.9.dist-info/RECORD,,
```

