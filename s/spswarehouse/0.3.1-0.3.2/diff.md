# Comparing `tmp/spswarehouse-0.3.1.tar.gz` & `tmp/spswarehouse-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.3.1.tar", last modified: Thu May 25 16:20:38 2023, max compression
+gzip compressed data, was "spswarehouse-0.3.2.tar", last modified: Mon Jun  5 20:48:24 2023, max compression
```

## Comparing `spswarehouse-0.3.1.tar` & `spswarehouse-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.537935 spswarehouse-0.3.1/
--rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2023-05-25 16:20:38.534528 spswarehouse-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 16:20:38.537935 spswarehouse-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-25 16:20:09.000000 spswarehouse-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.498908 spswarehouse-0.3.1/spswarehouse/
--rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.3.1/spswarehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.521589 spswarehouse-0.3.1/spswarehouse/calpads/
--rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.3.1/spswarehouse/calpads/__init__.py
--rw-rw-rw-   0        0        0    40625 2023-05-25 16:11:09.000000 spswarehouse-0.3.1/spswarehouse/calpads/calpads.py
--rw-rw-rw-   0        0        0     6136 2023-05-25 16:11:09.000000 spswarehouse-0.3.1/spswarehouse/calpads/calpads_config.py
--rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.3.1/spswarehouse/credentials.py.template
--rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.3.1/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.3.1/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.3.1/spswarehouse/googleslides.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.530139 spswarehouse-0.3.1/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.3.1/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    21618 2023-05-25 16:20:04.000000 spswarehouse-0.3.1/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.3.1/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.3.1/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.3.1/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.3.1/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.3.1/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:20:38.511771 spswarehouse-0.3.1/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 16:20:38.000000 spswarehouse-0.3.1/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 20:48:24.832456 spswarehouse-0.3.2/
+-rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2023-06-05 20:48:24.831456 spswarehouse-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 20:48:24.833456 spswarehouse-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-06-05 20:44:26.000000 spswarehouse-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:48:24.808862 spswarehouse-0.3.2/spswarehouse/
+-rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.3.2/spswarehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:48:24.822456 spswarehouse-0.3.2/spswarehouse/calpads/
+-rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.3.2/spswarehouse/calpads/__init__.py
+-rw-rw-rw-   0        0        0    40625 2023-05-25 16:11:09.000000 spswarehouse-0.3.2/spswarehouse/calpads/calpads.py
+-rw-rw-rw-   0        0        0     6136 2023-05-25 16:11:09.000000 spswarehouse-0.3.2/spswarehouse/calpads/calpads_config.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.3.2/spswarehouse/credentials.py.template
+-rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.3.2/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.3.2/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.3.2/spswarehouse/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:48:24.828456 spswarehouse-0.3.2/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.3.2/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    21618 2023-06-05 20:44:03.000000 spswarehouse-0.3.2/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.3.2/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.3.2/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.3.2/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.3.2/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.3.2/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-06-05 20:48:24.815862 spswarehouse-0.3.2/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2023-06-05 20:48:24.000000 spswarehouse-0.3.2/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-06-05 20:48:24.000000 spswarehouse-0.3.2/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 20:48:24.000000 spswarehouse-0.3.2/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 20:48:24.000000 spswarehouse-0.3.2/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.3.1/LICENSE` & `spswarehouse-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/PKG-INFO` & `spswarehouse-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.3.1
+Version: 0.3.2
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.3.1/README.md` & `spswarehouse-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/setup.py` & `spswarehouse-0.3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse",
-    version="0.3.1",
+    version="0.3.2",
     author="Summit Public Schools; Harry Li Consulting, LLC",
     author_email="warehouse@summitps.org",
     description="Summit Public Schools Snowflake warehouse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse",
     packages=setuptools.find_packages(),
```

### Comparing `spswarehouse-0.3.1/spswarehouse/__init__.py` & `spswarehouse-0.3.2/spswarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/calpads/calpads.py` & `spswarehouse-0.3.2/spswarehouse/calpads/calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/calpads/calpads_config.py` & `spswarehouse-0.3.2/spswarehouse/calpads/calpads_config.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/credentials.py.template` & `spswarehouse-0.3.2/spswarehouse/credentials.py.template`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/googledrive.py` & `spswarehouse-0.3.2/spswarehouse/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/googlesheets.py` & `spswarehouse-0.3.2/spswarehouse/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/googleslides.py` & `spswarehouse-0.3.2/spswarehouse/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.3.2/spswarehouse/powerschool/powerschool.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                 elem = WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.ID, 'prReloadButton')))
                 elem.click()
                 logging.info('PowerSchool report is not ready, refreshing and waiting.')
                 time.sleep(3)
             else:
                 # Download the first report in table
                 queued_reports = WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((
-                    By.XPATH, '//*[@id="queuecontent"]/table/tbody/tr[2]/td[7]/a')))
+                    By.XPATH, '//*[@id="queuecontent"]/table/tbody/tr[2]/td[8]/a')))
                 download_link = queued_reports.get_attribute('href')
                 original_files_list = os.listdir(destination_directory_path)
                 self.driver.get(download_link) #downloads the file
                 logging.info('PowerSchool report downloaded.')
                 break
 
         self._wait_for_new_file_in_folder(destination_directory_path, original_files_list)
```

### Comparing `spswarehouse-0.3.1/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.3.2/spswarehouse/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/table_names.py` & `spswarehouse-0.3.2/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/table_utils.py` & `spswarehouse-0.3.2/spswarehouse/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse/warehouse.py` & `spswarehouse-0.3.2/spswarehouse/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.3.1/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.3.2/spswarehouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.3.1
+Version: 0.3.2
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.3.1/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.3.2/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

