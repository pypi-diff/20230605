# Comparing `tmp/cicc_excel-0.3.0.tar.gz` & `tmp/cicc_excel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicc_excel-0.3.0.tar", last modified: Sat Jun  3 01:26:21 2023, max compression
+gzip compressed data, was "cicc_excel-0.4.0.tar", last modified: Mon Jun  5 07:34:41 2023, max compression
```

## Comparing `cicc_excel-0.3.0.tar` & `cicc_excel-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.170000 cicc_excel-0.3.0/
--rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1837 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1274 2023-06-02 15:16:00.000000 cicc_excel-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.220000 cicc_excel-0.3.0/cicc_excel/
--rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.3.0/cicc_excel/__init__.py
--rw-rw-rw-   0        0        0    14346 2023-06-02 15:13:08.000000 cicc_excel-0.3.0/cicc_excel/excelwriter.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.250000 cicc_excel-0.3.0/cicc_excel.egg-info/
--rw-rw-rw-   0        0        0     1837 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-06-02 15:16:16.000000 cicc_excel-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1876 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1274 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.402358 cicc_excel-0.4.0/cicc_excel/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/cicc_excel/__init__.py
+-rw-rw-rw-   0        0        0    14325 2023-06-05 07:26:41.000000 cicc_excel-0.4.0/cicc_excel/excelwriter.py
+drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/cicc_excel.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-06-05 07:34:40.000000 cicc_excel-0.4.0/cicc_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 07:34:40.000000 cicc_excel-0.4.0/cicc_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-06-05 07:27:18.000000 cicc_excel-0.4.0/setup.py
```

### Comparing `cicc_excel-0.3.0/LICENSE` & `cicc_excel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.3.0/PKG-INFO` & `cicc_excel-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cicc_excel
-Version: 0.3.0
+Version: 0.4.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,7 +58,8 @@
 #another sheet
 wb.load_data(df3)
 wb.write_data('last_sheet_name')
 
 #save file
 wb.save()
 ```
+
```

### Comparing `cicc_excel-0.3.0/README.md` & `cicc_excel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.3.0/cicc_excel/excelwriter.py` & `cicc_excel-0.4.0/cicc_excel/excelwriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,16 @@
             elif column_name in text_columns:
                 ws.set_column(col_num, col_num, self.column_width['text'], None)
             else:
                 ws.set_column(col_num, col_num, self.column_width['default'], None)
             #write cells    
             for row_num, cell_value in enumerate(self.data[column_name]):
                 if pd.isnull(cell_value):
-                    ws.write(row_num + 1, col_num, '')
-                elif column_name in date_columns:
+                    cell_value = ''
+                if column_name in date_columns:
                     ws.write(row_num + 1, col_num, cell_value, style['date_format'])
                 elif column_name in sn_columns:
                     ws.write(row_num + 1, col_num, cell_value, style['sn_format'])
                 elif column_name in num_columns:
                     ws.write(row_num + 1, col_num, cell_value, style['number_format'])
                 elif column_name in percent_columns:
                     ws.write(row_num + 1, col_num, cell_value, style['percent_format'])
```

### Comparing `cicc_excel-0.3.0/cicc_excel.egg-info/PKG-INFO` & `cicc_excel-0.4.0/cicc_excel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cicc-excel
-Version: 0.3.0
+Version: 0.4.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,7 +58,8 @@
 #another sheet
 wb.load_data(df3)
 wb.write_data('last_sheet_name')
 
 #save file
 wb.save()
 ```
+
```

### Comparing `cicc_excel-0.3.0/setup.py` & `cicc_excel-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicc_excel",
-    version="0.3.0",
+    version="0.4.0",
     author="Pengcheng Song",
     author_email="smth_spc@hotmail.com",
     description="Library of export pandas into excel for CICCers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyuspc/cicc_excel",
     install_requires=[
```

