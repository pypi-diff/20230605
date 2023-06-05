# Comparing `tmp/python-aresti-0.4.3.tar.gz` & `tmp/python-aresti-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aresti-0.4.3.tar", last modified: Mon Jun  5 07:40:21 2023, max compression
+gzip compressed data, was "python-aresti-0.4.4.tar", last modified: Mon Jun  5 11:18:55 2023, max compression
```

## Comparing `python-aresti-0.4.3.tar` & `python-aresti-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.610128 python-aresti-0.4.3/
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 07:40:21.609952 python-aresti-0.4.3/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.4.3/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.607076 python-aresti-0.4.3/aresti/
--rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.4.3/aresti/__init__.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.608865 python-aresti-0.4.3/aresti/rajapinta/
--rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.4.3/aresti/rajapinta/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.4.3/aresti/rajapinta/meta.py
--rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.4.3/aresti/rajapinta/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.4.3/aresti/rajapinta/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.4.3/aresti/rajapinta/vierasavain.py
--rw-r--r--   0 aha        (501) staff       (20)     3299 2023-06-02 11:13:59.000000 python-aresti-0.4.3/aresti/rest.py
--rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.4.3/aresti/sanoma.py
--rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.4.3/aresti/testi.py
--rw-r--r--   0 aha        (501) staff       (20)     2455 2023-06-02 11:37:47.000000 python-aresti-0.4.3/aresti/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.4.3/aresti/yhteys.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-03-18 13:07:55.000000 python-aresti-0.4.3/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.609788 python-aresti-0.4.3/python_aresti.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     3752 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 07:40:21.610166 python-aresti-0.4.3/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.4.3/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:55.871923 python-aresti-0.4.4/
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 11:18:55.871786 python-aresti-0.4.4/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.4.4/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:55.869186 python-aresti-0.4.4/aresti/
+-rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.4.4/aresti/__init__.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:55.870652 python-aresti-0.4.4/aresti/rajapinta/
+-rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.4.4/aresti/rajapinta/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.4.4/aresti/rajapinta/meta.py
+-rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.4.4/aresti/rajapinta/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.4.4/aresti/rajapinta/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.4.4/aresti/rajapinta/vierasavain.py
+-rw-r--r--   0 aha        (501) staff       (20)     3299 2023-06-02 11:13:59.000000 python-aresti-0.4.4/aresti/rest.py
+-rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.4.4/aresti/sanoma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.4.4/aresti/testi.py
+-rw-r--r--   0 aha        (501) staff       (20)     2345 2023-06-05 08:50:11.000000 python-aresti-0.4.4/aresti/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.4.4/aresti/yhteys.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:17:11.000000 python-aresti-0.4.4/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 11:18:55.871619 python-aresti-0.4.4/python_aresti.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     3883 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-05 11:18:55.000000 python-aresti-0.4.4/python_aresti.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 11:18:55.871960 python-aresti-0.4.4/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.4.4/setup.py
```

### Comparing `python-aresti-0.4.3/aresti/rajapinta/__init__.py` & `python-aresti-0.4.4/aresti/rajapinta/__init__.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/rajapinta/meta.py` & `python-aresti-0.4.4/aresti/rajapinta/meta.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/rajapinta/nakyma.py` & `python-aresti-0.4.4/aresti/rajapinta/nakyma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/rajapinta/tyokalut.py` & `python-aresti-0.4.4/aresti/rajapinta/tyokalut.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/rajapinta/vierasavain.py` & `python-aresti-0.4.4/aresti/rajapinta/vierasavain.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/rest.py` & `python-aresti-0.4.4/aresti/rest.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/sanoma.py` & `python-aresti-0.4.4/aresti/sanoma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/testi.py` & `python-aresti-0.4.4/aresti/testi.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/aresti/tyokalut.py` & `python-aresti-0.4.4/aresti/tyokalut.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     ):
       return await f(self, *args, **kwargs)
     alku = time()
     try:
       return await f(self, *args, **kwargs)
     finally:
       mittaa_pyynnot(f, args, time() - alku)
-      # kesto = f'{time() - alku:.1f}'.replace('.', ',')
-      #print(f'{f.__name__} {args} kesti {kesto} s')
     # async def _f
   return _f
   # def mittaa
 
 
 def kaanna_poikkeus(f):
   # pylint: disable=invalid-name
```

### Comparing `python-aresti-0.4.3/aresti/yhteys.py` & `python-aresti-0.4.4/aresti/yhteys.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.3/python_aresti.egg-info/historia.json` & `python-aresti-0.4.4/python_aresti.egg-info/historia.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '4b7cbfd6b7bfe7efe2ff036abe2569aea0f2d281'), ('versio', "*

 * *           "'0.4.4'), ('kuvaus', 'PEP 517 -yhteensopivuus')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "PEP 517 -yhteensopivuus",
+        "revisio": "4b7cbfd6b7bfe7efe2ff036abe2569aea0f2d281",
+        "versio": "0.4.4"
+    },
+    {
         "kuvaus": "P\u00e4ivitetty versiointij\u00e4rjestelm\u00e4",
         "revisio": "6519c9634b687651f1c7d2d66b8ffe552416f92a",
         "versio": "0.4.3"
     },
     {
         "kuvaus": "Suoritetaan `AsynkroninenYhteys.mittaa_pyynnot` silloin, kun se on asetettu",
         "revisio": "4ebef1c521b9c496de9621058f99a34114711eae",
```

