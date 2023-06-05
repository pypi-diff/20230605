# Comparing `tmp/lib-dzne-filedata-0.4.3.tar.gz` & `tmp/lib-dzne-filedata-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.4.3.tar", last modified: Mon Jun  5 06:10:34 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.4.4.tar", last modified: Mon Jun  5 21:19:43 2023, max compression
```

## Comparing `lib-dzne-filedata-0.4.3.tar` & `lib-dzne-filedata-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.4.3/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.4.3/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      556 2023-06-04 22:32:33.000000 lib-dzne-filedata-0.4.3/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)     7505 2023-06-04 22:33:39.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 06:10:34.026910 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-05 06:10:34.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-06-05 06:10:34.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-05 06:10:34.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       36 2023-06-05 06:10:34.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-06-05 06:10:34.000000 lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 21:19:43.890044 lib-dzne-filedata-0.4.4/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.4.4/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-05 21:19:43.890044 lib-dzne-filedata-0.4.4/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.4.4/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      556 2023-06-05 21:18:47.000000 lib-dzne-filedata-0.4.4/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-05 21:19:43.890044 lib-dzne-filedata-0.4.4/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 21:19:43.886044 lib-dzne-filedata-0.4.4/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 21:19:43.890044 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     7508 2023-06-05 21:18:00.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-05 21:19:43.890044 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-05 21:19:43.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-06-05 21:19:43.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-05 21:19:43.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       36 2023-06-05 21:19:43.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-06-05 21:19:43.000000 lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.4.3/LICENSE` & `lib-dzne-filedata-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.4.3/PKG-INFO` & `lib-dzne-filedata-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.4.3
+Version: 0.4.4
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.4.3/pyproject.toml` & `lib-dzne-filedata-0.4.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.4.3"
+version = "0.4.4"
 description = "Libary for filedata handling. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-filedata-0.4.3/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.4.4/src/lib_dzne_filedata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         else:
             cls.check_ext(file)
             ans = self._save(file=file, **kwargs)
         if ans is not None:
             raise TypeError()
     @classmethod
     def from_file(cls, file, /, *types):
-        ext = _os.path.splitext(file)
+        ext = _os.path.splitext(file)[1]
         for t in types:
             if not issubclass(t, cls):
                 raise ValueError()
             if t._ext == ext:
                 return t.load(file)
         raise ValueError()
     @classmethod
```

### Comparing `lib-dzne-filedata-0.4.3/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.4.4/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.4.3
+Version: 0.4.4
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

