# Comparing `tmp/dartrig-0.1.6.tar.gz` & `tmp/dartrig-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.6.tar", last modified: Mon Jun  5 04:08:34 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.7.tar", last modified: Mon Jun  5 04:12:35 2023, max compression
```

## Comparing `dartrig-0.1.6.tar` & `dartrig-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:08:34.000000 dartrig-0.1.6/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.6/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.6/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:08:33.000000 dartrig-0.1.6/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    15549 2023-06-05 04:07:43.000000 dartrig-0.1.6/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.6/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:08:34.000000 dartrig-0.1.6/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:08:34.000000 dartrig-0.1.6/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:12:35.000000 dartrig-0.1.7/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.7/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.7/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:12:34.000000 dartrig-0.1.7/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15575 2023-06-05 04:12:34.000000 dartrig-0.1.7/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.7/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:12:35.000000 dartrig-0.1.7/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:12:35.000000 dartrig-0.1.7/setup.cfg
```

### Comparing `dartrig-0.1.6/PKG-INFO` & `dartrig-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.6
+Version: 0.1.7
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.6/LICENSE` & `dartrig-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.6/README.md` & `dartrig-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.6/setup.py` & `dartrig-0.1.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.6",
+    version="0.1.7",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.11'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.6/dartrig/__init__.py` & `dartrig-0.1.7/dartrig/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
 
         return dcm_no
 
     def get_dsaf_meta(self, rcp_no, keyword="연결재무") -> Dict[str, any]:
         cache_key = f"dcm_meta_{rcp_no}"
         try:
             if self.cache is not None:
-                cached = self.cache.hget(cache_key)
-                if cached is not None:
+                cached: Dict = self.cache.hget(cache_key)
+                if cached is not None and len(cached) > 0:
                     logger.debug(f"dsaf001_meta cache hit for rcp_no {rcp_no} => {cached}")
                     return cached
 
             html_text = self._try_file_cache_request(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", "dsaf", rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
             find1_num = html_text.index(keyword)  # 여기 viewDoc에서 필요한 정보가 다 들어있음
```

### Comparing `dartrig-0.1.6/dartrig/annotations.py` & `dartrig-0.1.7/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.6/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.7/dartrig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.6
+Version: 0.1.7
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

