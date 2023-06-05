# Comparing `tmp/dartrig-0.1.5.tar.gz` & `tmp/dartrig-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.5.tar", last modified: Sun Jun  4 14:34:56 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.6.tar", last modified: Mon Jun  5 04:08:34 2023, max compression
```

## Comparing `dartrig-0.1.5.tar` & `dartrig-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:34:56.000000 dartrig-0.1.5/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.5/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.5/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-04 14:34:55.000000 dartrig-0.1.5/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    15543 2023-06-04 14:34:55.000000 dartrig-0.1.5/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.5/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-04 14:34:56.000000 dartrig-0.1.5/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:08:34.000000 dartrig-0.1.6/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.6/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.6/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:08:33.000000 dartrig-0.1.6/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15549 2023-06-05 04:07:43.000000 dartrig-0.1.6/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.6/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:08:34.000000 dartrig-0.1.6/setup.cfg
```

### Comparing `dartrig-0.1.5/PKG-INFO` & `dartrig-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.5
+Version: 0.1.6
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.5/LICENSE` & `dartrig-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.5/README.md` & `dartrig-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.5/setup.py` & `dartrig-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.5",
+    version="0.1.6",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.11'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.5/dartrig/__init__.py` & `dartrig-0.1.6/dartrig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return self.request_detail_with_dcm(rcp_no, dtd, dcm_no, ele_id, offset, length)
 
     def request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0, length=0):
         dtd_split = dtd.split(".")[0]
         file_cache_key = f"{rcp_no}_{dcm_no}_{dtd_split}_{ele_id}_{offset}"
 
         url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length={length}&dtd={dtd}"
-        self.logger.info(f"request_detail_with_dcm url : {url}")
+        self.logger.debug(f"request_detail_with_dcm url : {url}")
         return self._try_file_cache_request(url, "viewer", file_cache_key, ext="html" if dtd.lower() == "html" else "xml")
 
     def _try_file_cache_request(self, url, prefix, file_cache_key, ext="html"):
         if self.file_cache is not None:
             cached = self.file_cache.get_file(prefix=prefix, key=file_cache_key, ext=ext)
             if cached is not None:
                 self.logger.debug(f"file cache hit for key {file_cache_key}")
@@ -114,20 +114,20 @@
         except Exception as ex:
             logger.exception(ex)
             raise ValueError(f"dcm number fetch failed for rcp_no : [{rcp_no}]")
 
         return dcm_no
 
     def get_dsaf_meta(self, rcp_no, keyword="연결재무") -> Dict[str, any]:
-        cache_key = f"dcm_no_meta_{rcp_no}"
+        cache_key = f"dcm_meta_{rcp_no}"
         try:
             if self.cache is not None:
                 cached = self.cache.hget(cache_key)
                 if cached is not None:
-                    logger.debug(f"dsaf001_report cache hit for rcp_no {rcp_no}")
+                    logger.debug(f"dsaf001_meta cache hit for rcp_no {rcp_no} => {cached}")
                     return cached
 
             html_text = self._try_file_cache_request(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", "dsaf", rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
             find1_num = html_text.index(keyword)  # 여기 viewDoc에서 필요한 정보가 다 들어있음
             res_text = remove_strs_list(html_text[find1_num:find1_num + 250],
@@ -137,15 +137,15 @@
             ele_id = find1_list[3]
             offset = find1_list[4]
             length = find1_list[5]
 
             meta = { "dcm_no" : dcm_no, "ele_id" : ele_id, "offset" : offset, "length" : length }
             if self.cache is not None:
                 self.cache.hset(cache_key, meta)
-                logger.debug(f"dsaf001_report cache set for rcp_no {rcp_no}")
+                logger.debug(f"dsaf001_meta cache set for rcp_no {rcp_no}")
 
             return meta
         except Exception as ex:
             logger.exception(ex)
             raise ValueError(f"dsaf meta fetch failed for rcp_no : [{rcp_no}]")
 
     def _deprecated_get_dsaf_html(self, rcp_no):
```

### Comparing `dartrig-0.1.5/dartrig/annotations.py` & `dartrig-0.1.6/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.5/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.6/dartrig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.5
+Version: 0.1.6
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

