# Comparing `tmp/google-csv-helper-1.0.2.tar.gz` & `tmp/google-csv-helper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.0.2.tar", last modified: Thu Jun  1 12:47:28 2023, max compression
+gzip compressed data, was "google-csv-helper-1.0.3.tar", last modified: Mon Jun  5 15:41:36 2023, max compression
```

## Comparing `google-csv-helper-1.0.2.tar` & `google-csv-helper-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-01 12:47:28.523179 google-csv-helper-1.0.2/
--rw-r--r--   0 changyy    (501) admin       (80)     1070 2023-05-31 17:26:00.000000 google-csv-helper-1.0.2/LICENSE
--rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-01 12:47:28.523026 google-csv-helper-1.0.2/PKG-INFO
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-01 12:47:28.522164 google-csv-helper-1.0.2/google_csv_helper/
--rw-r--r--   0 changyy    (501) admin       (80)       89 2023-06-01 12:14:19.000000 google-csv-helper-1.0.2/google_csv_helper/__init__.py
--rw-r--r--   0 changyy    (501) admin       (80)     6807 2023-06-01 12:14:19.000000 google-csv-helper-1.0.2/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 changyy    (501) admin       (80)     2583 2023-06-01 12:14:19.000000 google-csv-helper-1.0.2/google_csv_helper/csv_common.py
--rw-r--r--   0 changyy    (501) admin       (80)     9741 2023-06-01 12:14:19.000000 google-csv-helper-1.0.2/google_csv_helper/csv_helper.py
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-01 12:47:28.522842 google-csv-helper-1.0.2/google_csv_helper.egg-info/
--rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-01 12:47:28.000000 google-csv-helper-1.0.2/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 changyy    (501) admin       (80)      354 2023-06-01 12:47:28.000000 google-csv-helper-1.0.2/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 changyy    (501) admin       (80)        1 2023-06-01 12:47:28.000000 google-csv-helper-1.0.2/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-01 12:47:28.000000 google-csv-helper-1.0.2/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 changyy    (501) admin       (80)       18 2023-06-01 12:47:28.000000 google-csv-helper-1.0.2/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 changyy    (501) admin       (80)       38 2023-06-01 12:47:28.523219 google-csv-helper-1.0.2/setup.cfg
--rw-r--r--   0 changyy    (501) admin       (80)     1161 2023-06-01 12:47:22.000000 google-csv-helper-1.0.2/setup.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.795565 google-csv-helper-1.0.3/
+-rw-r--r--   0 changyy    (501) admin       (80)     3091 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/.gitignore
+-rw-r--r--   0 changyy    (501) admin       (80)     1070 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/LICENSE
+-rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-05 15:41:36.795416 google-csv-helper-1.0.3/PKG-INFO
+-rw-r--r--   0 changyy    (501) admin       (80)     3276 2023-06-05 14:36:39.000000 google-csv-helper-1.0.3/README.md
+-rw-r--r--   0 changyy    (501) admin       (80)      177 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/build.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.794352 google-csv-helper-1.0.3/google_csv_helper/
+-rw-r--r--   0 changyy    (501) admin       (80)      312 2023-06-05 14:08:43.000000 google-csv-helper-1.0.3/google_csv_helper/__init__.py
+-rw-r--r--   0 changyy    (501) admin       (80)     7389 2023-06-05 15:36:22.000000 google-csv-helper-1.0.3/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 changyy    (501) admin       (80)     2490 2023-06-05 14:13:19.000000 google-csv-helper-1.0.3/google_csv_helper/cmd.py
+-rw-r--r--   0 changyy    (501) admin       (80)     2778 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/google_csv_helper/csv_common.py
+-rw-r--r--   0 changyy    (501) admin       (80)     9958 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/google_csv_helper/csv_helper.py
+drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:41:36.795219 google-csv-helper-1.0.3/google_csv_helper.egg-info/
+-rw-r--r--   0 changyy    (501) admin       (80)      728 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 changyy    (501) admin       (80)      470 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 changyy    (501) admin       (80)        1 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       65 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       18 2023-06-05 15:41:36.000000 google-csv-helper-1.0.3/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/requirements.txt
+-rw-r--r--   0 changyy    (501) admin       (80)       38 2023-06-05 15:41:36.795604 google-csv-helper-1.0.3/setup.cfg
+-rw-r--r--   0 changyy    (501) admin       (80)     1735 2023-06-05 12:27:39.000000 google-csv-helper-1.0.3/setup.py
```

### Comparing `google-csv-helper-1.0.2/LICENSE` & `google-csv-helper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.2/PKG-INFO` & `google-csv-helper-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-csv-helper-1.0.2/google_csv_helper/adsense_csv_helper.py` & `google-csv-helper-1.0.3/google_csv_helper/adsense_csv_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # -*- encoding: utf-8 -*-
 
-import csv_common as csvCommonInfo
-import csv_helper as csvHelper
+from google_csv_helper import csv_common
+from google_csv_helper import csv_helper
 
 import pandas
 import datetime
 
-class AdsenseCSVHelper(csvHelper.CSVHelper):
+class AdsenseCSVHelper(csv_helper.CSVHelper):
     def getDateRangeReport(self, dataframe: pandas.DataFrame, keyFieldName:str, valueFilterBegin:str, valueFilterEnd:str, minmaxDateInputFormat:str, minmaxDateOutputFormat:str ):
         output = {}
+        if len(dataframe.index) == 0:
+            if self.debugMode:
+                print(f"[WARNING] dataframe is empty.")
+            return output
 
         pickedData = dataframe[ (dataframe[keyFieldName] >= valueFilterBegin) & (dataframe[keyFieldName] <= valueFilterEnd) ]
+        if len(pickedData.index) == 0:
+            if self.debugMode:
+                print(f"[WARNING] dataframe is empty, too")
+            return output
 
         maxRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].max() ]
         minRow = pickedData[ pickedData['Estimated earnings (USD)'] == pickedData['Estimated earnings (USD)'].min() ]
 
         maxRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(maxRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
         minRowDateInfo = datetime.datetime.strftime(datetime.datetime.strptime(minRow.iloc[0][keyFieldName], minmaxDateInputFormat), minmaxDateOutputFormat)
 
@@ -75,44 +83,50 @@
         #print(f"Filter: {prevDateFilterBegin} ~ {prevDateFilterEnd}")
 
         output["output"]["date"]["duration"]["begin"] = DateFilterBegin
         output["output"]["date"]["duration"]["end"] = DateFilterEnd
         output["output"]["date"]["previous"]["begin"] = prevDateFilterBegin
         output["output"]["date"]["previous"]["end"] = prevDateFilterEnd
 
+
         for k, v in self.getAllResult().items():
             target = k
             if k.find("adsense") > 0:
                 target = "Adsense China" if k.find("cn") > 0 or k.find("china") > 0 else "Adsense Global"
             elif k.find("admob") > 0:
                 target = "Admob China" if k.find("cn") > 0 or k.find("china") > 0 else "Admob Global"
     
             prevItemInfo = self.getDateRangeReport(v["Date"], 'Date', prevDateFilterBegin, prevDateFilterEnd, '%Y-%m-%d', '%m/%d %a')
             item = self.getDateRangeReport(v["Date"], 'Date', DateFilterBegin, DateFilterEnd, '%Y-%m-%d', '%m/%d %a')
     
             compareInfo = {}
-            for lookup in csvCommonInfo.CSV_OUTPUT_REPORT_COMPARISON_INFO:
+            for lookup in csv_common.CSV_OUTPUT_REPORT_COMPARISON_INFO:
+                if lookup not in item or lookup not in prevItemInfo:
+                    compareInfo[lookup] = 0
+                    continue
                 compareInfo[lookup] = (item[lookup] - prevItemInfo[lookup]) * 100 / prevItemInfo[lookup]
 
             output["output"]["csv"]["data"].append([
                 f"{target}",
-                item['Estimated earnings (USD)'],
+                item['Estimated earnings (USD)'] if 'Estimated earnings (USD)' in item else 0.0,
                 compareInfo['Estimated earnings (USD)'],
-                item['Average earnings (USD)'],
+                item['Average earnings (USD)'] if 'Average earnings (USD)' in item else 0.0,
                 compareInfo['Average earnings (USD)'],
-                item['Average CPC'],
+                item['Average CPC'] if 'Average CPC' in item else 0.0,
                 compareInfo['Average CPC'],
-                item['Lowest earnings'],
-                item['Lowest earnings info'],
-                item['Highest earnings'],
-                item['Highest earnings info'],
+                item['Lowest earnings'] if 'Lowest earnings' in item else 0.0,
+                item['Lowest earnings info'] if 'Lowest earnings info' in item else None,
+                item['Highest earnings'] if 'Highest earnings' in item else 0.0,
+                item['Highest earnings info'] if 'Highest earnings info' in item else None,
             ])
 
-            output["output"]["csv"]["total"]["Cumulative Revenue"] += item['Estimated earnings (USD)']
-            output["output"]["csv"]["total"]["Average Daily Revenue"] += item['Average earnings (USD)']
+            if 'Estimated earnings (USD)' in item:
+                output["output"]["csv"]["total"]["Cumulative Revenue"] += item['Estimated earnings (USD)']
+            if 'Average earnings (USD)' in item:
+                output["output"]["csv"]["total"]["Average Daily Revenue"] += item['Average earnings (USD)']
 
         return output
 
     def getDailyMarkDownReport(self, pickedDate: datetime.date, pickedReportKeyword: list[str]) -> str:
         data = self.getDailySummaryReport(pickedDate, pickedReportKeyword)
 
         output = [ 
@@ -125,14 +139,7 @@
         for item in data["output"]["csv"]["data"]:
             output.append( f"| {item[0]} | {item[1]:,.2f} | {item[3]:,.2f} ({item[4]:.2f}%) | {item[5]:.4f} ({item[6]:.2f}%) | {item[7]:,.2f} [{item[8]}] | {item[9]:,.2f} [{item[10]}] " )
 
         output.append( f"| Total | {data['output']['csv']['total']['Cumulative Revenue']:,.2f} | {data['output']['csv']['total']['Average Daily Revenue']:,.2f} | | | ")
 
         return "\n".join(output)
 
-if __name__ == '__main__':
-    import sys
-    obj = AdsenseCSVHelper(sys.argv[1:] if len(sys.argv) >= 2 else '')
-    #obj.enableDebug()
-    obj.readAllCSVRawFile()
-    #print(obj.getAllJSONResult())
-    print(obj.getDailyMarkDownReport(datetime.date.today(), ["adsense", "admob"]))
```

### Comparing `google-csv-helper-1.0.2/google_csv_helper/csv_common.py` & `google-csv-helper-1.0.3/google_csv_helper/csv_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,20 @@
         "handler": lambda x: str(float(x.replace('%',''))*0.01),
         "newFieldName": "CTR",
     },
     "Clicks": {
         "handlerType": "calc",
         "handler": lambda row: (row['Estimated earnings (USD)'] / row["Clicks"]) if row["Clicks"] != 0 else 0,
         "newFieldName": "CPC (USD)",
-    }
+    },
+    "Impressions": {
+        "handlerType": "calc",
+        "handler": lambda row: (row['Clicks'] / row["Impressions"]) if row["Impressions"] != 0 else 0,
+        "newFieldName": "CTR",
+    },
 }
 
 CSV_FIELD_NAME_DATA_TYPE = {
     #"Date": str,
     #"Month": str,
     #"Week": str,
     "Estimated earnings (USD)": 1.0,
@@ -74,15 +79,15 @@
     'Date', 'Week', 'Month',
 ]
 
 CSV_OUTPUT_REPORT_COMPARISON_INFO = [
 	'Estimated earnings (USD)', 'Average earnings (USD)' , 'Average CPC',
 ]
 
-CSV_OUTPUT_FIELD_NAME_DATA_TYP = {
+CSV_OUTPUT_FIELD_NAME_DATA_TYPE = {
     #"Date": str,
     #"Month": str,
     #"Week": str,
     "Estimated earnings (USD)": 1.0,
     "Page views": 1,
     "Page RPM (USD)": 1.0,
     "Impressions": 1,
```

### Comparing `google-csv-helper-1.0.2/google_csv_helper/csv_helper.py` & `google-csv-helper-1.0.3/google_csv_helper/csv_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- encoding: utf-8 -*-
 
-import csv_common as csvCommonInfo
+from google_csv_helper import csv_common
 
 import os
 import io
 import json
+import csv
 import pandas
 import datetime
 
 class CSVHelper:
     raw_csv_files_output = {}
     pandas_dataframe_output = {}
     debugMode = False
@@ -47,23 +48,26 @@
                         lookup[full_path] = dirpath
         self.raw_csv_files_output = output
 
     def readAllCSVRawFile(self):
         output = {}
         for key, values in self.raw_csv_files_output.items():
             for item in values:
-                #print(item)
+                if self.debugMode:
+                    print(f"readAllCSVRawFile: {item}")
                 df = None
                 for try_encodeing in ['utf-8', 'utf-16le']:
                     try:
                         df = pandas.read_csv(item, sep='[,\\t]', engine='python', encoding=try_encodeing)
                         if len(df.index) > 1:
                             break
                     except Exception as e:
                         pass
+                if self.debugMode:
+                    print(df)
                 self.handlePandasDataFrame(key, item, df)
         return output
 
     def getAllJSONResult(self) -> dict[str, pandas.DataFrame]:
         output = {'key':[], 'data':{} }
         for key in self.getAllKey():
             output['key'].append(key)
@@ -92,80 +96,81 @@
                     for row in csvparser:
                         if csvheader == None:
                             csvheader = row
                         else:
                             #print(row)
                             #print(csvheader)
                             for index, header in enumerate(csvheader):
-                                if header in csvCommonInfo.CSV_OUTPUT_FIELD_NAME_DATA_TYPE:
-                                    if isinstance(csvCommonInfo.CSV_OUTPUT_FIELD_NAME_DATA_TYPE[header], int):
+                                if header in csv_common.CSV_OUTPUT_FIELD_NAME_DATA_TYPE:
+                                    if isinstance(csv_common.CSV_OUTPUT_FIELD_NAME_DATA_TYPE[header], int):
                                         try:
                                             row[index] = int(row[index])
                                         except Exception as e:
                                             row[index] = 0
-                                    elif isinstance(csvCommonInfo.CSV_OUTPUT_FIELD_NAME_DATA_TYPE[header], float):
+                                    elif isinstance(csv_common.CSV_OUTPUT_FIELD_NAME_DATA_TYPE[header], float):
                                         try:
                                             row[index] = float(row[index])
                                         except Exception as e:
                                             row[index] = 0.0
                             #print(row)
                             #sys.exit(0)
                         output[k].append(row)
             return output
         return None
 
     def handlePandasDataFrame(self, key:str, filename:str , dataFrame: pandas.DataFrame):
         if isinstance(dataFrame, pandas.DataFrame) == False:
             return
-        #print(f"{key}: {filename}")
+        if self.debugMode:
+            print(f"handlePandasDataFrame: {key}: {filename}")
 
         fieldRename = {}
         # field name transform
         for field in dataFrame.columns:
-            if field in csvCommonInfo.CSV_FIELD_NAME_TRANSFORM:
-                fieldRename[field] = csvCommonInfo.CSV_FIELD_NAME_TRANSFORM[field]
+            if field in csv_common.CSV_FIELD_NAME_TRANSFORM:
+                fieldRename[field] = csv_common.CSV_FIELD_NAME_TRANSFORM[field]
         if len(fieldRename) > 0:
             dataFrame.rename(columns=fieldRename, inplace = True)
 
         if key not in self.pandas_dataframe_output:
             self.pandas_dataframe_output[key] = {}
 
         #keyField = dataFrame.columns[0]
         keyField = None
         for field in dataFrame.columns:
-            if field in csvCommonInfo.CSV_INPUT_CHECK_MAIN_FIELD:
+            if field in csv_common.CSV_INPUT_CHECK_MAIN_FIELD:
                 keyField = field
                 break
 
         # Skip
         if keyField == None:
             if self.debugMode:
-                 print(f"[WARNING] keyField({csvCommonInfo.CSV_INPUT_CHECK_MAIN_FIELD}) not found, skip this data: {filename}")
+                print(f"[WARNING] keyField({csv_common.CSV_INPUT_CHECK_MAIN_FIELD}) not found, skip this data: {filename}, fields: {dataFrame.columns}")
             return
 
-        for field, info in csvCommonInfo.CSV_FIELD_VALUE_TRANSFORM.items():
+        for field, info in csv_common.CSV_FIELD_VALUE_TRANSFORM.items():
             if field in dataFrame.columns and info['newFieldName'] not in dataFrame.columns:
                 #print(dataFrame.columns)
                 if self.debugMode:
                     print(f"[INFO] create '{info['newFieldName']}' field from '{field}' dataframe via '{info['handlerType']}'")
                 if info['handlerType'] == 'function':
                     dataFrame[info['newFieldName']] = dataFrame[field].apply(info['handler'])
                 elif info['handlerType'] == 'calc':
                     dataFrame[info['newFieldName']] = dataFrame.apply(info['handler'], axis=1)
                 #print(dataFrame[[field, info['newFieldName']]])
 
-        for field in csvCommonInfo.CSV_OUTPUT_ADSENSE_FIELDS:
+        for field in csv_common.CSV_OUTPUT_ADSENSE_FIELDS:
             if field not in dataFrame.columns:
                 if self.debugMode:
-                    print(f"[WARNING] dataField({csvCommonInfo.CSV_OUTPUT_ADSENSE_FIELDS}) not found, skip this data: {filename}")
+                    print(f"[WARNING] dataField({csv_common.CSV_OUTPUT_ADSENSE_FIELDS}) not found, skip this data: {filename}, field: {dataFrame.columns}")
                 return
             
         if self.debugMode:
             print(f"[INFO] import file: {filename}")
-        currentData = dataFrame[ [keyField] + csvCommonInfo.CSV_OUTPUT_ADSENSE_FIELDS ]
+        currentData = dataFrame[ [keyField] + csv_common.CSV_OUTPUT_ADSENSE_FIELDS ]
         currentDataLength = len(currentData)
         currentDateBegin = currentData[keyField][0] if currentDataLength > 0 else None
         currentDateEnd = currentData[keyField][currentDataLength - 1] if currentDataLength > 0 else None
 
         # set output
         if keyField not in self.pandas_dataframe_output[key]:
             self.pandas_dataframe_output[key][keyField] = currentData
@@ -174,15 +179,15 @@
         # update data
         keyFieldOldData = self.pandas_dataframe_output[key][keyField][keyField]
         oldDataLength = len(keyFieldOldData)
         oldDateBegin = keyFieldOldData[0] if oldDataLength > 0 else None
         oldDateEnd = keyFieldOldData[oldDataLength-1] if oldDataLength > 0 else None
 
         if oldDateBegin >= currentDateBegin or oldDateEnd <= currentDateEnd:
-            self.pandas_dataframe_output[key][keyField] = self.handleDataFrameMerge(self.pandas_dataframe_output[key][keyField], currentData, keyField, csvCommonInfo.CSV_OUTPUT_ADSENSE_FIELDS[0])
+            self.pandas_dataframe_output[key][keyField] = self.handleDataFrameMerge(self.pandas_dataframe_output[key][keyField], currentData, keyField, csv_common.CSV_OUTPUT_ADSENSE_FIELDS[0])
         return
 
     def handleDataFrameMerge(self, oldDataFrame: pandas.DataFrame, newDataFrame: pandas.DataFrame, keyField:str, valueField:str) -> pandas.DataFrame:
         #print("in handleDataFrameMerge")
         # https://pandas.pydata.org/docs/reference/api/pandas.concat.html?highlight=concat#pandas.concat
         # https://pandas.pydata.org/docs/reference/api/pandas.merge_ordered.html
         output = pandas.merge_ordered(oldDataFrame, newDataFrame)
```

### Comparing `google-csv-helper-1.0.2/google_csv_helper.egg-info/PKG-INFO` & `google-csv-helper-1.0.3/google_csv_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-csv-helper-1.0.2/setup.py` & `google-csv-helper-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 from setuptools import setup, find_packages
 import os
+import re
 import pathlib
 
 CWD = pathlib.Path(__file__).parent.resolve()
 
-VERSION = '1.0.2' 
+VERSION = '1.0.0' 
+with open(os.path.join(CWD, 'google_csv_helper', '__init__.py'), 'r') as f:
+    re_version_pattern = re.compile(r"=[\s]*['\"]([0-9\.]+)['\"]")
+    for line in f:
+        line = line.strip()
+        if line.find('version') >= 0:
+            extractVersionInfo = re_version_pattern.search(line)
+            if extractVersionInfo:
+                VERSION = extractVersionInfo.group(1)
+
 PYTHON_REQUIRES = ">=3.10"
 URL = "https://github.com/changyy/google-csv-helper"
 DOWNLOAD_URL = "https://pypi.org/project/google-csv-helper/"
 DESCRIPTION = 'A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.'
 LONG_DESCRIPTION = DESCRIPTION
-INSTALL_REQUIRES = []
-with open(os.path.join(CWD, "requirements.txt"), 'r') as f:
-    INSTALL_REQUIRES = [s.strip() for s in f.read().split("\n")]
+INSTALL_REQUIRES = ['pandas']
+try:
+    with open(os.path.join(CWD, "requirements.txt"), 'r') as f:
+        INSTALL_REQUIRES = [s.strip() for s in f.read().split("\n")]
+except Exception as e:
+    pass
 
 setup(
     name="google-csv-helper", 
     version=VERSION,
     author="Yuan-Yi Chang",
     author_email="<changyy.csie@gmail.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
     keywords=['python', 'google', 'csv', 'adsense', 'admob', 'report'],
     python_requires=PYTHON_REQUIRES,
     url=URL,
     download_url=DOWNLOAD_URL,
+    entry_points={
+        'console_scripts': [
+            'google-csv-helper = google_csv_helper.cmd:main',
+        ],
+    },
     classifiers= [
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
     ]
 )
```

