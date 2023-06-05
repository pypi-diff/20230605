# Comparing `tmp/python-aresti-0.4.1.tar.gz` & `tmp/python-aresti-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aresti-0.4.1.tar", last modified: Thu Nov 24 12:04:55 2022, max compression
+gzip compressed data, was "python-aresti-0.4.3.tar", last modified: Mon Jun  5 07:40:21 2023, max compression
```

## Comparing `python-aresti-0.4.1.tar` & `python-aresti-0.4.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-11-24 12:04:55.092862 python-aresti-0.4.1/
--rw-r--r--   0 aha        (501) staff       (20)      247 2022-11-24 12:04:55.092735 python-aresti-0.4.1/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.4.1/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-11-24 12:04:55.090092 python-aresti-0.4.1/aresti/
--rw-r--r--   0 aha        (501) staff       (20)      141 2022-09-14 10:13:57.000000 python-aresti-0.4.1/aresti/__init__.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-11-24 12:04:55.091452 python-aresti-0.4.1/aresti/rajapinta/
--rw-r--r--   0 aha        (501) staff       (20)     1556 2022-08-30 07:23:25.000000 python-aresti-0.4.1/aresti/rajapinta/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      913 2022-08-29 18:10:37.000000 python-aresti-0.4.1/aresti/rajapinta/meta.py
--rw-r--r--   0 aha        (501) staff       (20)     3870 2022-08-30 07:23:19.000000 python-aresti-0.4.1/aresti/rajapinta/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)      729 2022-08-29 17:47:12.000000 python-aresti-0.4.1/aresti/rajapinta/vierasavain.py
--rw-r--r--   0 aha        (501) staff       (20)     3299 2022-09-14 10:13:57.000000 python-aresti-0.4.1/aresti/rest.py
--rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.4.1/aresti/sanoma.py
--rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.4.1/aresti/testi.py
--rw-r--r--   0 aha        (501) staff       (20)     2376 2022-11-23 08:08:10.000000 python-aresti-0.4.1/aresti/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     5238 2022-11-23 06:25:21.000000 python-aresti-0.4.1/aresti/yhteys.py
--rw-r--r--   0 aha        (501) staff       (20)       72 2021-03-18 13:07:55.000000 python-aresti-0.4.1/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2022-11-24 12:04:55.092553 python-aresti-0.4.1/python_aresti.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      247 2022-11-24 12:04:54.000000 python-aresti-0.4.1/python_aresti.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      470 2022-11-24 12:04:55.000000 python-aresti-0.4.1/python_aresti.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2022-11-24 12:04:54.000000 python-aresti-0.4.1/python_aresti.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     4769 2022-11-24 12:04:54.000000 python-aresti-0.4.1/python_aresti.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        8 2022-11-24 12:04:54.000000 python-aresti-0.4.1/python_aresti.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        7 2022-11-24 12:04:55.000000 python-aresti-0.4.1/python_aresti.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2022-11-24 12:04:55.092904 python-aresti-0.4.1/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      406 2022-09-14 10:13:57.000000 python-aresti-0.4.1/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.610128 python-aresti-0.4.3/
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 07:40:21.609952 python-aresti-0.4.3/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.4.3/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.607076 python-aresti-0.4.3/aresti/
+-rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.4.3/aresti/__init__.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.608865 python-aresti-0.4.3/aresti/rajapinta/
+-rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.4.3/aresti/rajapinta/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.4.3/aresti/rajapinta/meta.py
+-rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.4.3/aresti/rajapinta/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.4.3/aresti/rajapinta/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.4.3/aresti/rajapinta/vierasavain.py
+-rw-r--r--   0 aha        (501) staff       (20)     3299 2023-06-02 11:13:59.000000 python-aresti-0.4.3/aresti/rest.py
+-rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.4.3/aresti/sanoma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.4.3/aresti/testi.py
+-rw-r--r--   0 aha        (501) staff       (20)     2455 2023-06-02 11:37:47.000000 python-aresti-0.4.3/aresti/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.4.3/aresti/yhteys.py
+-rw-r--r--   0 aha        (501) staff       (20)       72 2021-03-18 13:07:55.000000 python-aresti-0.4.3/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-05 07:40:21.609788 python-aresti-0.4.3/python_aresti.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     3752 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-05 07:40:21.000000 python-aresti-0.4.3/python_aresti.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-05 07:40:21.610166 python-aresti-0.4.3/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.4.3/setup.py
```

### Comparing `python-aresti-0.4.1/aresti/rajapinta/meta.py` & `python-aresti-0.4.3/aresti/rajapinta/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # def __get__
 
   # class SisempiLuokka
 
 
 class RajapinnanTyyppi(type):
 
-  def __new__(mcs, name, bases, attrs, **kwargs):
+  def x___new__(mcs, name, bases, attrs, **kwargs):
     return super().__new__(
       mcs,
       name,
       bases,
       {
         avain: (
           SisempiLuokka(arvo)
```

### Comparing `python-aresti-0.4.1/aresti/rest.py` & `python-aresti-0.4.3/aresti/rest.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.1/aresti/sanoma.py` & `python-aresti-0.4.3/aresti/sanoma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.1/aresti/testi.py` & `python-aresti-0.4.3/aresti/testi.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.1/aresti/tyokalut.py` & `python-aresti-0.4.3/aresti/tyokalut.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 
 
 def mittaa(f):
   '''
   Mittaa ja raportoi asynkronisen metodin suoritukseen
   kulunut aika.
 
-  Ohitetaan, ellei `self.mittaa_pyynnot` ole tosi.
+  Ohitetaan, jos `self.mittaa_pyynnot` on tyhjä.
   '''
   # pylint: disable=invalid-name
   @functools.wraps(f)
   async def _f(self, *args, **kwargs):
-    if not getattr(self, 'mittaa_pyynnot', False):
+    if not (
+      mittaa_pyynnot := getattr(self, 'mittaa_pyynnot', False)
+    ):
       return await f(self, *args, **kwargs)
     alku = time()
     try:
       return await f(self, *args, **kwargs)
     finally:
-      kesto = f'{time() - alku:.1f}'.replace('.', ',')
-      print(f'{f.__name__} {args} kesti {kesto} s')
+      mittaa_pyynnot(f, args, time() - alku)
+      # kesto = f'{time() - alku:.1f}'.replace('.', ',')
+      #print(f'{f.__name__} {args} kesti {kesto} s')
     # async def _f
   return _f
   # def mittaa
 
 
 def kaanna_poikkeus(f):
   # pylint: disable=invalid-name
```

### Comparing `python-aresti-0.4.1/aresti/yhteys.py` & `python-aresti-0.4.3/aresti/yhteys.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,21 @@
     'https://testi.fi'
   ) as yhteys:
     data = await yhteys.nouda_data('/abc/def')
   ```
   '''
   palvelin = None
   debug = False
-  mittaa_pyynnot = False
+  mittaa_pyynnot = None
 
-  def __init__(self, palvelin=None, *, debug=None, mittaa_pyynnot=None):
+  def __init__(
+    self, palvelin=None, *,
+    debug=None,
+    mittaa_pyynnot=None
+  ):
     if palvelin is not None:
       self.palvelin = palvelin
     assert self.palvelin is not None
     if debug is not None:
       self.debug = debug
     if mittaa_pyynnot is not None:
       self.mittaa_pyynnot = mittaa_pyynnot
```

