# Comparing `tmp/pykeepass-4.0.4.tar.gz` & `tmp/pykeepass-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeepass-4.0.4.tar", last modified: Fri May 12 06:07:39 2023, max compression
+gzip compressed data, was "pykeepass-4.0.5.tar", last modified: Mon Jun  5 21:38:58 2023, max compression
```

## Comparing `pykeepass-4.0.4.tar` & `pykeepass-4.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.699094 pykeepass-4.0.4/
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.691094 pykeepass-4.0.4/.github/
--rw-r--r--   0 evan      (1000) evan      (1000)      180 2022-06-27 23:09:55.000000 pykeepass-4.0.4/.github/dependabot.yml
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.691094 pykeepass-4.0.4/.github/workflows/
--rw-r--r--   0 evan      (1000) evan      (1000)      725 2022-12-27 21:23:49.000000 pykeepass-4.0.4/.github/workflows/ci.yaml
--rw-r--r--   0 evan      (1000) evan      (1000)       82 2022-12-26 00:46:40.000000 pykeepass-4.0.4/.gitignore
--rw-r--r--   0 evan      (1000) evan      (1000)     2511 2023-05-12 06:00:00.000000 pykeepass-4.0.4/CHANGELOG.rst
--rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.4/LICENSE
--rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.4/MANIFEST.in
--rw-r--r--   0 evan      (1000) evan      (1000)      317 2022-07-20 18:02:33.000000 pykeepass-4.0.4/Makefile
--rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-05-12 06:07:39.699094 pykeepass-4.0.4/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)    14582 2023-05-12 06:07:16.000000 pykeepass-4.0.4/README.rst
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.695094 pykeepass-4.0.4/pykeepass/
--rw-r--r--   0 evan      (1000) evan      (1000)      132 2022-07-15 21:42:52.000000 pykeepass-4.0.4/pykeepass/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1657 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/attachment.py
--rw-r--r--   0 evan      (1000) evan      (1000)     5208 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/baseelement.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/blank_database.kdbx
--rw-r--r--   0 evan      (1000) evan      (1000)     3641 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/deprecated.py
--rw-r--r--   0 evan      (1000) evan      (1000)    12590 2023-05-12 05:57:00.000000 pykeepass-4.0.4/pykeepass/entry.py
--rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-06-27 23:09:55.000000 pykeepass-4.0.4/pykeepass/exceptions.py
--rw-r--r--   0 evan      (1000) evan      (1000)     3412 2022-12-26 00:46:40.000000 pykeepass-4.0.4/pykeepass/group.py
--rw-r--r--   0 evan      (1000) evan      (1000)     2403 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/icons.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.699094 pykeepass-4.0.4/pykeepass/kdbx_parsing/
--rw-r--r--   0 evan      (1000) evan      (1000)       23 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13134 2022-07-15 21:41:20.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/common.py
--rw-r--r--   0 evan      (1000) evan      (1000)      933 2022-11-14 23:31:17.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx.py
--rw-r--r--   0 evan      (1000) evan      (1000)     4922 2022-06-27 23:09:55.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx3.py
--rw-r--r--   0 evan      (1000) evan      (1000)     7954 2022-07-20 18:02:33.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx4.py
--rw-r--r--   0 evan      (1000) evan      (1000)    15444 2023-05-12 05:56:39.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/pytwofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.4/pykeepass/kdbx_parsing/twofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    29383 2022-12-26 00:46:40.000000 pykeepass-4.0.4/pykeepass/pykeepass.py
--rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.4/pykeepass/setters.py
--rw-r--r--   0 evan      (1000) evan      (1000)       48 2023-05-12 06:00:15.000000 pykeepass-4.0.4/pykeepass/version.py
--rw-r--r--   0 evan      (1000) evan      (1000)     2848 2022-12-26 00:46:38.000000 pykeepass-4.0.4/pykeepass/xpath.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-05-12 06:07:39.695094 pykeepass-4.0.4/pykeepass.egg-info/
--rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)      847 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/SOURCES.txt
--rw-r--r--   0 evan      (1000) evan      (1000)        1 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/dependency_links.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       80 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/requires.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       10 2023-05-12 06:07:39.000000 pykeepass-4.0.4/pykeepass.egg-info/top_level.txt
--rw-r--r--   0 evan      (1000) evan      (1000)      125 2022-07-20 18:02:33.000000 pykeepass-4.0.4/requirements-rtd.txt
--rw-r--r--   0 evan      (1000) evan      (1000)      111 2022-07-20 18:02:33.000000 pykeepass-4.0.4/requirements.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       38 2023-05-12 06:07:39.699094 pykeepass-4.0.4/setup.cfg
--rw-r--r--   0 evan      (1000) evan      (1000)      934 2023-05-12 06:02:15.000000 pykeepass-4.0.4/setup.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.186493 pykeepass-4.0.5/
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.178493 pykeepass-4.0.5/.github/
+-rw-r--r--   0 evan      (1000) evan      (1000)      180 2022-06-27 23:09:55.000000 pykeepass-4.0.5/.github/dependabot.yml
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.178493 pykeepass-4.0.5/.github/workflows/
+-rw-r--r--   0 evan      (1000) evan      (1000)      725 2022-12-27 21:23:49.000000 pykeepass-4.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0 evan      (1000) evan      (1000)       82 2022-12-26 00:46:40.000000 pykeepass-4.0.5/.gitignore
+-rw-r--r--   0 evan      (1000) evan      (1000)     2703 2023-06-05 21:37:45.000000 pykeepass-4.0.5/CHANGELOG.rst
+-rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.5/LICENSE
+-rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.5/MANIFEST.in
+-rw-r--r--   0 evan      (1000) evan      (1000)      317 2022-07-20 18:02:33.000000 pykeepass-4.0.5/Makefile
+-rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-06-05 21:38:58.182493 pykeepass-4.0.5/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)    14582 2023-05-22 00:01:13.000000 pykeepass-4.0.5/README.rst
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.182493 pykeepass-4.0.5/pykeepass/
+-rw-r--r--   0 evan      (1000) evan      (1000)      132 2022-07-15 21:42:52.000000 pykeepass-4.0.5/pykeepass/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1657 2022-07-20 18:02:33.000000 pykeepass-4.0.5/pykeepass/attachment.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     5294 2023-06-05 21:37:45.000000 pykeepass-4.0.5/pykeepass/baseelement.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.5/pykeepass/blank_database.kdbx
+-rw-r--r--   0 evan      (1000) evan      (1000)     3641 2022-07-20 18:02:33.000000 pykeepass-4.0.5/pykeepass/deprecated.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    12685 2023-06-05 21:37:45.000000 pykeepass-4.0.5/pykeepass/entry.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-06-27 23:09:55.000000 pykeepass-4.0.5/pykeepass/exceptions.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     3412 2022-12-26 00:46:40.000000 pykeepass-4.0.5/pykeepass/group.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2403 2022-07-20 18:02:33.000000 pykeepass-4.0.5/pykeepass/icons.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.182493 pykeepass-4.0.5/pykeepass/kdbx_parsing/
+-rw-r--r--   0 evan      (1000) evan      (1000)       23 2021-03-05 05:26:01.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13134 2022-07-15 21:41:20.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/common.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      933 2022-11-14 23:31:17.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     4922 2022-06-27 23:09:55.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx3.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     7954 2022-07-20 18:02:33.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx4.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13965 2023-05-22 00:01:13.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/pytwofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.5/pykeepass/kdbx_parsing/twofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    29383 2023-06-05 21:30:20.000000 pykeepass-4.0.5/pykeepass/pykeepass.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.5/pykeepass/setters.py
+-rw-r--r--   0 evan      (1000) evan      (1000)       48 2023-06-05 21:38:12.000000 pykeepass-4.0.5/pykeepass/version.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2848 2022-12-26 00:46:38.000000 pykeepass-4.0.5/pykeepass/xpath.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2023-06-05 21:38:58.182493 pykeepass-4.0.5/pykeepass.egg-info/
+-rw-r--r--   0 evan      (1000) evan      (1000)    14903 2023-06-05 21:38:58.000000 pykeepass-4.0.5/pykeepass.egg-info/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)      847 2023-06-05 21:38:58.000000 pykeepass-4.0.5/pykeepass.egg-info/SOURCES.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)        1 2023-06-05 21:38:58.000000 pykeepass-4.0.5/pykeepass.egg-info/dependency_links.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       80 2023-06-05 21:38:58.000000 pykeepass-4.0.5/pykeepass.egg-info/requires.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       10 2023-06-05 21:38:58.000000 pykeepass-4.0.5/pykeepass.egg-info/top_level.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)      125 2022-07-20 18:02:33.000000 pykeepass-4.0.5/requirements-rtd.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)      111 2022-07-20 18:02:33.000000 pykeepass-4.0.5/requirements.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       38 2023-06-05 21:38:58.186493 pykeepass-4.0.5/setup.cfg
+-rw-r--r--   0 evan      (1000) evan      (1000)      934 2023-05-22 00:01:13.000000 pykeepass-4.0.5/setup.py
```

### Comparing `pykeepass-4.0.4/.github/workflows/ci.yaml` & `pykeepass-4.0.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/CHANGELOG.rst` & `pykeepass-4.0.5/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-4.0.4 -
+4.0.5 -
+------------------
+- fixed #344 - AttributeError when accessing Times with None value
+- use __hash__ when evaluating equality
+- use mtime/uuid for HistoryEntry hashing
+
+4.0.4 - 2023-05-23
 ------------------
 - fixed #314 - correctly handle binaries with no data
 - fixed #265 - check for keepass signature
 - fixed #319 - support pathlib for filename/keyfile
 - fixed #194 - added 'protected' arg to _set_string_field
 - use official icon names from KeePass source and deprecate old icons
 - added Entry.is_custom_property_protected()
 - fixed #338 - allow comma entry tag separator
 
 4.0.3 - 2022-06-21
 ------------------
-- add otp support
-- add debug_setup() function
+- added otp support
+- added debug_setup() function
 
 4.0.2 - 2022-05-21
 ------------------
 - added support for argon2id key derivation function
 - added credential expiry functions
 - fixes #223 - safe saving
```

### Comparing `pykeepass-4.0.4/LICENSE` & `pykeepass-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/PKG-INFO` & `pykeepass-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.4
+Version: 4.0.5
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Home-page: https://github.com/libkeepass/pykeepass
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 License: GPL3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `pykeepass-4.0.4/README.rst` & `pykeepass-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/attachment.py` & `pykeepass-4.0.5/pykeepass/attachment.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/baseelement.py` & `pykeepass-4.0.5/pykeepass/baseelement.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def _path(self):
         return self._element.getroottree().getpath(self._element)
 
     def _get_times_property(self, prop):
         times = self._element.find('Times')
         if times is not None:
             prop = times.find(prop)
-            if prop is not None:
+            if prop is not None and prop.text is not None:
                 return self._kp._decode_time(prop.text)
 
     def _set_times_property(self, prop, value):
         times = self._element.find('Times')
         if times is not None:
             prop = times.find(prop)
             if prop is not None:
@@ -162,19 +162,21 @@
 
     def __unicode__(self):
         return self.__str__()
 
     def __repr__(self):
         return self.__str__()
 
+    def __hash__(self):
+        return hash((self.uuid,))
+
     def __eq__(self, other):
-        if hasattr(other, 'uuid'):
-            return self.uuid == other.uuid
-        else:
-            return False
+        if isinstance(other, BaseElement):
+            return hash(self) == hash(other)
+        return NotImplemented
 
     def touch(self, modify=False):
         """
         Update last access time of an entry/group
 
         Args:
             modify (bool): update access time as well a modification time
```

### Comparing `pykeepass-4.0.4/pykeepass/blank_database.kdbx` & `pykeepass-4.0.5/pykeepass/blank_database.kdbx`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/deprecated.py` & `pykeepass-4.0.5/pykeepass/deprecated.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/entry.py` & `pykeepass-4.0.5/pykeepass/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
                 E.String(E.Key('Password'), E.Value(password, Protected="True"))
             )
             if url:
                 self._element.append(E.String(E.Key('URL'), E.Value(url)))
             if notes:
                 self._element.append(E.String(E.Key('Notes'), E.Value(notes)))
             if otp:
-                self._element.append(E.String(E.Key('otp'), E.Value(otp)))
+                self._element.append(
+                    E.String(E.Key('otp'), E.Value(otp, Protected="True"))
+                )
             if tags:
                 self._element.append(
                     E.Tags(';'.join(tags) if type(tags) is list else tags)
                 )
             self._element.append(
                 E.AutoType(
                     E.Enabled(str(autotype_enabled)),
@@ -379,10 +381,11 @@
 
 class HistoryEntry(Entry):
 
     def __str__(self):
         pathstr = super().__str__()
         return 'HistoryEntry: {}'.format(pathstr)
 
-    def __eq__(self, other):
-        # all history items share the same uuid, so examine xml directly
-        return self._element == other._element
+    def __hash__(self):
+        # All history items share the same UUID with themselves and their
+        # parent, so consider the mtime also
+        return hash((self.uuid, self.mtime))
```

### Comparing `pykeepass-4.0.4/pykeepass/group.py` & `pykeepass-4.0.5/pykeepass/group.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/icons.py` & `pykeepass-4.0.5/pykeepass/icons.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/common.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/common.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx3.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx3.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/kdbx4.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/kdbx4.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/pytwofish.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/pytwofish.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,30 +133,21 @@
 
 
 #
 # Private.
 #
 
 import struct
-import sys
-
-WORD_BIGENDIAN = 0
-if sys.byteorder == 'big':
-    WORD_BIGENDIAN = 1
 
 def rotr32(x, n):
     return (x >> n) | ((x << (32 - n)) & 0xFFFFFFFF)
 
 def rotl32(x, n):
     return ((x << n) & 0xFFFFFFFF) | (x >> (32 - n))
 
-def byteswap32(x):
-    return ((x & 0xff) << 24) | (((x >> 8) & 0xff) << 16) | \
-           (((x >> 16) & 0xff) << 8) | ((x >> 24) & 0xff)
-
 class TWI:
     def __init__(self):
         self.k_len = 0 # word32
         self.l_key = [0]*40 # word32
         self.s_key = [0]*4 # word32
         self.qt_gen = 0 # word32
         self.q_tab = [[0]*256, [0]*256] # byte
@@ -288,110 +279,82 @@
     pkey.k_len = int((key_len * 8) / 64)
 
     a = 0
     b = 0
     me_key = [0,0,0,0]
     mo_key = [0,0,0,0]
     for i in range(pkey.k_len):
-        if WORD_BIGENDIAN:
-            a = byteswap32(in_key[i + 1])
-            me_key[i] = a
-            b = byteswap32(in_key[i + i + 1])
-        else:
-            a = in_key[i + i]
-            me_key[i] = a
-            b = in_key[i + i + 1]
+        a = in_key[i + i]
+        me_key[i] = a
+        b = in_key[i + i + 1]
         mo_key[i] = b
         pkey.s_key[pkey.k_len - i - 1] = mds_rem(a, b);
     for i in range(0, 40, 2):
         a = (0x01010101 * i) % 0x100000000;
         b = (a + 0x01010101) % 0x100000000;
         a = h_fun(pkey, a, me_key);
         b = rotl32(h_fun(pkey, b, mo_key), 8);
         pkey.l_key[i] = (a + b) % 0x100000000;
         pkey.l_key[i + 1] = rotl32((a + 2 * b) % 0x100000000, 9);
     gen_mk_tab(pkey, pkey.s_key)
 
 def encrypt(pkey, in_blk):
     blk = [0, 0, 0, 0]
 
-    if WORD_BIGENDIAN:
-        blk[0] = byteswap32(in_blk[0]) ^ pkey.l_key[0];
-        blk[1] = byteswap32(in_blk[1]) ^ pkey.l_key[1];
-        blk[2] = byteswap32(in_blk[2]) ^ pkey.l_key[2];
-        blk[3] = byteswap32(in_blk[3]) ^ pkey.l_key[3];
-    else:
-        blk[0] = in_blk[0] ^ pkey.l_key[0];
-        blk[1] = in_blk[1] ^ pkey.l_key[1];
-        blk[2] = in_blk[2] ^ pkey.l_key[2];
-        blk[3] = in_blk[3] ^ pkey.l_key[3];
+    blk[0] = in_blk[0] ^ pkey.l_key[0];
+    blk[1] = in_blk[1] ^ pkey.l_key[1];
+    blk[2] = in_blk[2] ^ pkey.l_key[2];
+    blk[3] = in_blk[3] ^ pkey.l_key[3];
 
     for i in range(8):
         t1 = ( pkey.mk_tab[0][byte(blk[1],3)] ^ pkey.mk_tab[1][byte(blk[1],0)] ^ pkey.mk_tab[2][byte(blk[1],1)] ^ pkey.mk_tab[3][byte(blk[1],2)] );
         t0 = ( pkey.mk_tab[0][byte(blk[0],0)] ^ pkey.mk_tab[1][byte(blk[0],1)] ^ pkey.mk_tab[2][byte(blk[0],2)] ^ pkey.mk_tab[3][byte(blk[0],3)] );
 
         blk[2] = rotr32(blk[2] ^ ((t0 + t1 + pkey.l_key[4 * (i) + 8]) % 0x100000000), 1);
         blk[3] = rotl32(blk[3], 1) ^ ((t0 + 2 * t1 + pkey.l_key[4 * (i) + 9]) % 0x100000000);
 
         t1 = ( pkey.mk_tab[0][byte(blk[3],3)] ^ pkey.mk_tab[1][byte(blk[3],0)] ^ pkey.mk_tab[2][byte(blk[3],1)] ^ pkey.mk_tab[3][byte(blk[3],2)] );
         t0 = ( pkey.mk_tab[0][byte(blk[2],0)] ^ pkey.mk_tab[1][byte(blk[2],1)] ^ pkey.mk_tab[2][byte(blk[2],2)] ^ pkey.mk_tab[3][byte(blk[2],3)] );
 
         blk[0] = rotr32(blk[0] ^ ((t0 + t1 + pkey.l_key[4 * (i) + 10]) % 0x100000000), 1);
         blk[1] = rotl32(blk[1], 1) ^ ((t0 + 2 * t1 + pkey.l_key[4 * (i) + 11]) % 0x100000000);
 
-    if WORD_BIGENDIAN:
-        in_blk[0] = byteswap32(blk[2] ^ pkey.l_key[4]);
-        in_blk[1] = byteswap32(blk[3] ^ pkey.l_key[5]);
-        in_blk[2] = byteswap32(blk[0] ^ pkey.l_key[6]);
-        in_blk[3] = byteswap32(blk[1] ^ pkey.l_key[7]);
-    else:
-        in_blk[0] = blk[2] ^ pkey.l_key[4];
-        in_blk[1] = blk[3] ^ pkey.l_key[5];
-        in_blk[2] = blk[0] ^ pkey.l_key[6];
-        in_blk[3] = blk[1] ^ pkey.l_key[7];
+    in_blk[0] = blk[2] ^ pkey.l_key[4];
+    in_blk[1] = blk[3] ^ pkey.l_key[5];
+    in_blk[2] = blk[0] ^ pkey.l_key[6];
+    in_blk[3] = blk[1] ^ pkey.l_key[7];
 
     return
 
 def decrypt(pkey, in_blk):
     blk = [0, 0, 0, 0]
 
-    if WORD_BIGENDIAN:
-        blk[0] = byteswap32(in_blk[0]) ^ pkey.l_key[4];
-        blk[1] = byteswap32(in_blk[1]) ^ pkey.l_key[5];
-        blk[2] = byteswap32(in_blk[2]) ^ pkey.l_key[6];
-        blk[3] = byteswap32(in_blk[3]) ^ pkey.l_key[7];
-    else:
-        blk[0] = in_blk[0] ^ pkey.l_key[4];
-        blk[1] = in_blk[1] ^ pkey.l_key[5];
-        blk[2] = in_blk[2] ^ pkey.l_key[6];
-        blk[3] = in_blk[3] ^ pkey.l_key[7];
+    blk[0] = in_blk[0] ^ pkey.l_key[4];
+    blk[1] = in_blk[1] ^ pkey.l_key[5];
+    blk[2] = in_blk[2] ^ pkey.l_key[6];
+    blk[3] = in_blk[3] ^ pkey.l_key[7];
 
     for i in range(7, -1, -1):
         t1 = ( pkey.mk_tab[0][byte(blk[1],3)] ^ pkey.mk_tab[1][byte(blk[1],0)] ^ pkey.mk_tab[2][byte(blk[1],1)] ^ pkey.mk_tab[3][byte(blk[1],2)] )
         t0 = ( pkey.mk_tab[0][byte(blk[0],0)] ^ pkey.mk_tab[1][byte(blk[0],1)] ^ pkey.mk_tab[2][byte(blk[0],2)] ^ pkey.mk_tab[3][byte(blk[0],3)] )
 
         blk[2] = rotl32(blk[2], 1) ^ ((t0 + t1 + pkey.l_key[4 * (i) + 10]) % 0x100000000)
         blk[3] = rotr32(blk[3] ^ ((t0 + 2 * t1 + pkey.l_key[4 * (i) + 11]) % 0x100000000), 1)
 
         t1 = ( pkey.mk_tab[0][byte(blk[3],3)] ^ pkey.mk_tab[1][byte(blk[3],0)] ^ pkey.mk_tab[2][byte(blk[3],1)] ^ pkey.mk_tab[3][byte(blk[3],2)] )
         t0 = ( pkey.mk_tab[0][byte(blk[2],0)] ^ pkey.mk_tab[1][byte(blk[2],1)] ^ pkey.mk_tab[2][byte(blk[2],2)] ^ pkey.mk_tab[3][byte(blk[2],3)] )
 
         blk[0] = rotl32(blk[0], 1) ^ ((t0 + t1 + pkey.l_key[4 * (i) + 8]) % 0x100000000)
         blk[1] = rotr32(blk[1] ^ ((t0 + 2 * t1 + pkey.l_key[4 * (i) + 9]) % 0x100000000), 1)
 
-    if WORD_BIGENDIAN:
-        in_blk[0] = byteswap32(blk[2] ^ pkey.l_key[0]);
-        in_blk[1] = byteswap32(blk[3] ^ pkey.l_key[1]);
-        in_blk[2] = byteswap32(blk[0] ^ pkey.l_key[2]);
-        in_blk[3] = byteswap32(blk[1] ^ pkey.l_key[3]);
-    else:
-        in_blk[0] = blk[2] ^ pkey.l_key[0];
-        in_blk[1] = blk[3] ^ pkey.l_key[1];
-        in_blk[2] = blk[0] ^ pkey.l_key[2];
-        in_blk[3] = blk[1] ^ pkey.l_key[3];
+    in_blk[0] = blk[2] ^ pkey.l_key[0];
+    in_blk[1] = blk[3] ^ pkey.l_key[1];
+    in_blk[2] = blk[0] ^ pkey.l_key[2];
+    in_blk[3] = blk[1] ^ pkey.l_key[3];
+
     return
 
 __testkey = b'\xD4\x3B\xB7\x55\x6E\xA3\x2E\x46\xF2\xA2\x82\xB7\xD4\x5B\x4E\x0D\x57\xFF\x73\x9D\x4D\xC9\x2C\x1B\xD7\xFC\x01\x70\x0C\xC8\x21\x6F'
 __testdat = b'\x90\xAF\xE9\x1B\xB2\x88\x54\x4F\x2C\x32\xDC\x23\x9B\x26\x35\xE6'
 assert b'l\xb4V\x1c@\xbf\n\x97\x05\x93\x1c\xb6\xd4\x08\xe7\xfa' == Twofish(__testkey).encrypt(__testdat)
 assert __testdat == Twofish(__testkey).decrypt(b'l\xb4V\x1c@\xbf\n\x97\x05\x93\x1c\xb6\xd4\x08\xe7\xfa')
```

### Comparing `pykeepass-4.0.4/pykeepass/kdbx_parsing/twofish.py` & `pykeepass-4.0.5/pykeepass/kdbx_parsing/twofish.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/pykeepass.py` & `pykeepass-4.0.5/pykeepass/pykeepass.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/setters.py` & `pykeepass-4.0.5/pykeepass/setters.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass/xpath.py` & `pykeepass-4.0.5/pykeepass/xpath.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/pykeepass.egg-info/PKG-INFO` & `pykeepass-4.0.5/pykeepass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.4
+Version: 4.0.5
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Home-page: https://github.com/libkeepass/pykeepass
 Author: Philipp Schmitt
 Author-email: philipp@schmitt.co
 License: GPL3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `pykeepass-4.0.4/pykeepass.egg-info/SOURCES.txt` & `pykeepass-4.0.5/pykeepass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.4/setup.py` & `pykeepass-4.0.5/setup.py`

 * *Files identical despite different names*

