# Comparing `tmp/pyiso8583-2.2.0.tar.gz` & `tmp/pyiso8583-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiso8583-2.2.0.tar", last modified: Sun Jan 30 08:13:50 2022, max compression
+gzip compressed data, was "pyiso8583-3.0.0.tar", last modified: Mon Jun  5 05:39:51 2023, max compression
```

## Comparing `pyiso8583-2.2.0.tar` & `pyiso8583-3.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-01-30 08:13:50.873211 pyiso8583-2.2.0/
--rw-rw-rw-   0        0        0     1072 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/LICENSE.md
--rw-rw-rw-   0        0        0      193 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1255 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/Makefile
--rw-rw-rw-   0        0        0     5540 2022-01-30 08:13:50.873211 pyiso8583-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4398 2022-01-30 08:00:39.000000 pyiso8583-2.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-01-30 08:13:50.848187 pyiso8583-2.2.0/docs/
--rw-rw-rw-   0        0        0      654 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/Makefile
--rw-rw-rw-   0        0        0      426 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/README.md
--rw-rw-rw-   0        0        0      159 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     2511 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/conf.py
--rw-rw-rw-   0        0        0      389 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/functions.rst
--rw-rw-rw-   0        0        0     9619 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/howto.rst
--rw-rw-rw-   0        0        0     1242 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/index.rst
--rw-rw-rw-   0        0        0      151 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/intro.rst
--rwxrwxrwx   0        0        0      795 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/make.bat
--rw-rw-rw-   0        0        0      163 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/docs/specifications.rst
-drwxrwxrwx   0        0        0        0 2022-01-30 08:13:50.852190 pyiso8583-2.2.0/iso8583/
--rw-rw-rw-   0        0        0     2754 2022-01-30 08:06:49.000000 pyiso8583-2.2.0/iso8583/__init__.py
--rw-rw-rw-   0        0        0    18935 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/iso8583/decoder.py
--rw-rw-rw-   0        0        0    17464 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/iso8583/encoder.py
--rw-rw-rw-   0        0        0        0 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/iso8583/py.typed
--rw-rw-rw-   0        0        0    83005 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/iso8583/specs.py
--rw-rw-rw-   0        0        0     5348 2022-01-30 08:13:10.000000 pyiso8583-2.2.0/iso8583/tools.py
-drwxrwxrwx   0        0        0        0 2022-01-30 08:13:50.869207 pyiso8583-2.2.0/pyiso8583.egg-info/
--rw-rw-rw-   0        0        0     5540 2022-01-30 08:13:50.000000 pyiso8583-2.2.0/pyiso8583.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2022-01-30 08:13:50.000000 pyiso8583-2.2.0/pyiso8583.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-30 08:13:50.000000 pyiso8583-2.2.0/pyiso8583.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-30 08:13:50.000000 pyiso8583-2.2.0/pyiso8583.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2022-01-30 08:13:50.000000 pyiso8583-2.2.0/pyiso8583.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      466 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      214 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       32 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/requirements.txt
--rw-rw-rw-   0        0        0      842 2022-01-30 08:13:50.877215 pyiso8583-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1544 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-30 08:13:50.872210 pyiso8583-2.2.0/tests/
--rw-rw-rw-   0        0        0        0 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0    59052 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/tests/test_decode.py
--rw-rw-rw-   0        0        0    74741 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/tests/test_encode.py
--rw-rw-rw-   0        0        0    18101 2022-01-30 07:59:52.000000 pyiso8583-2.2.0/tests/test_nibbles.py
--rw-rw-rw-   0        0        0    32905 2022-01-29 22:46:27.000000 pyiso8583-2.2.0/tests/test_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:39:51.270960 pyiso8583-3.0.0/
+-rw-rw-rw-   0        0        0     1072 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0      193 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1146 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/Makefile
+-rw-rw-rw-   0        0        0     5466 2023-06-05 05:39:51.270960 pyiso8583-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4398 2022-01-30 08:00:39.000000 pyiso8583-3.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 05:39:51.257459 pyiso8583-3.0.0/docs/
+-rw-rw-rw-   0        0        0      654 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0      426 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/README.md
+-rw-rw-rw-   0        0        0      159 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     2511 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0      389 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/functions.rst
+-rw-rw-rw-   0        0        0     9619 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/howto.rst
+-rw-rw-rw-   0        0        0     1242 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/index.rst
+-rw-rw-rw-   0        0        0      151 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/intro.rst
+-rwxrwxrwx   0        0        0      795 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0      163 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/docs/specifications.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 05:39:51.261961 pyiso8583-3.0.0/iso8583/
+-rw-rw-rw-   0        0        0     2754 2023-06-05 05:22:20.000000 pyiso8583-3.0.0/iso8583/__init__.py
+-rw-rw-rw-   0        0        0    18680 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/iso8583/decoder.py
+-rw-rw-rw-   0        0        0    18157 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/iso8583/encoder.py
+-rw-rw-rw-   0        0        0        0 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/iso8583/py.typed
+-rw-rw-rw-   0        0        0    83816 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/iso8583/specs.py
+-rw-rw-rw-   0        0        0     5323 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/iso8583/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:39:51.266460 pyiso8583-3.0.0/pyiso8583.egg-info/
+-rw-rw-rw-   0        0        0     5466 2023-06-05 05:39:51.000000 pyiso8583-3.0.0/pyiso8583.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-06-05 05:39:51.000000 pyiso8583-3.0.0/pyiso8583.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 05:39:51.000000 pyiso8583-3.0.0/pyiso8583.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-01-30 08:13:50.000000 pyiso8583-3.0.0/pyiso8583.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-05 05:39:51.000000 pyiso8583-3.0.0/pyiso8583.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      556 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      205 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       32 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/requirements.txt
+-rw-rw-rw-   0        0        0      217 2023-06-05 05:39:51.272459 pyiso8583-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-06-05 05:22:35.000000 pyiso8583-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:39:51.270460 pyiso8583-3.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-29 22:46:27.000000 pyiso8583-3.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    24525 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/tests/test_decode.py
+-rw-rw-rw-   0        0        0    25156 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/tests/test_encode.py
+-rw-rw-rw-   0        0        0    18101 2022-01-30 07:59:52.000000 pyiso8583-3.0.0/tests/test_nibbles.py
+-rw-rw-rw-   0        0        0    33563 2023-06-05 05:22:07.000000 pyiso8583-3.0.0/tests/test_tools.py
```

### Comparing `pyiso8583-2.2.0/LICENSE.md` & `pyiso8583-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/Makefile` & `pyiso8583-3.0.0/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -20,18 +20,14 @@
 	rm --force --recursive .coverage
 	rm --force --recursive ./htmlcov
 	rm --force --recursive coverage.xml
 
 coverage: coverage-clean
 	python -m pytest --cov=./iso8583
 	python -m coverage html --directory ./htmlcov
-	python -m coverage xml -o coverage.xml
-
-coverage-publish: coverage
-	codecov -f coverage.xml -t $(TOKEN)
 
 # Generate sphinx docs in docs/_build/html/index.html
 docs:
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 
 # Build and upload release to PyPI
```

### Comparing `pyiso8583-2.2.0/PKG-INFO` & `pyiso8583-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pyiso8583
-Version: 2.2.0
+Version: 3.0.0
 Summary: A serializer and deserializer of ISO8583 data.
 Home-page: https://github.com/knovichikhin/pyiso8583
 Author: Konstantin Novichikhin
 Author-email: konstantin.novichikhin@gmail.com
 License: MIT
 Keywords: iso8583 8583 banking protocol library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 
 iso8583 - a Python package for parsing ISO8583 data
 ===================================================
 
 |pypi| |docs| |coverage|
@@ -143,9 +141,7 @@
 .. |docs| image:: https://readthedocs.org/projects/pyiso8583/badge/?version=latest
     :alt: Documentation Status
     :target: https://pyiso8583.readthedocs.io/en/latest/?badge=latest
 
 .. |coverage| image:: https://codecov.io/gh/knovichikhin/pyiso8583/branch/master/graph/badge.svg
     :alt: Test coverage
     :target: https://codecov.io/gh/knovichikhin/pyiso8583
-
-
```

### Comparing `pyiso8583-2.2.0/README.rst` & `pyiso8583-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/docs/Makefile` & `pyiso8583-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/docs/conf.py` & `pyiso8583-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/docs/howto.rst` & `pyiso8583-3.0.0/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/docs/index.rst` & `pyiso8583-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/docs/make.bat` & `pyiso8583-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/iso8583/__init__.py` & `pyiso8583-3.0.0/iso8583/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     2   Primary Account Number (PAN)  : '1234567890'
     >>> iso8583.pp(encoded, spec)
     t   Message Type                  : b'0200'
     p   Bitmap, Primary               : b'4000000000000000'
     2   Primary Account Number (PAN)  : b'10' b'1234567890'
 """
 
-__version__ = "2.2.0"
+__version__ = "3.0.0"
 __all__ = [
     "pp",
     "decode",
     "DecodeError",
     "encode",
     "EncodeError",
 ]
```

### Comparing `pyiso8583-2.2.0/iso8583/decoder.py` & `pyiso8583-3.0.0/iso8583/decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -107,40 +107,46 @@
     doc_dec: DecodedDict = {}
     doc_enc: EncodedDict = {}
     fields: Set[int] = set()
     idx = 0
 
     idx = _decode_header(s, doc_dec, doc_enc, idx, spec)
     idx = _decode_type(s, doc_dec, doc_enc, idx, spec)
-    idx = _decode_bitmaps(s, doc_dec, doc_enc, idx, spec, fields)
+    idx = _decode_bitmap(s, doc_dec, doc_enc, idx, "p", spec, fields)
+
+    # No need to produce secondary bitmap if it's not required
+    if 1 in fields:
+        idx = _decode_bitmap(s, doc_dec, doc_enc, idx, "1", spec, fields)
 
     # `field_key` can be used to throw an exception after the loop.
     # So, create it here in case the `fields` set is empty
     # and never enters the loop to create the variable.
     # Set `field_key` to the last mandatory one: primary bitmap.
     field_key = "p"
 
     for field_key in [str(i) for i in sorted(fields)]:
-        # Secondary bitmap is already decoded in _decode_bitmaps
+        # Secondary bitmap is already decoded
         if field_key == "1":
             continue
-        idx = _decode_field(s, doc_dec, doc_enc, idx, field_key, spec)
+        idx = _decode_field(s, doc_dec, doc_enc, idx, field_key, spec[field_key])
 
     if idx != len(s):
         raise DecodeError(
             "Extra data after last field", s, doc_dec, doc_enc, idx, field_key
         )
 
     return doc_dec, doc_enc
 
 
 #
 # Private interface
 #
 
+_FieldSpecDict = Mapping[str, Any]
+
 
 def _decode_header(
     s: Union[bytes, bytearray],
     doc_dec: DecodedDict,
     doc_enc: EncodedDict,
     idx: int,
     spec: SpecDict,
@@ -172,15 +178,15 @@
         An error decoding ISO8583 bytearray.
     """
 
     # Header is not expected according to specifications
     if spec["h"]["max_len"] <= 0:
         return idx
 
-    return _decode_field(s, doc_dec, doc_enc, idx, "h", spec)
+    return _decode_field(s, doc_dec, doc_enc, idx, "h", spec["h"])
 
 
 def _decode_type(
     s: Union[bytes, bytearray],
     doc_dec: DecodedDict,
     doc_enc: EncodedDict,
     idx: int,
@@ -211,242 +217,153 @@
     ------
     DecodeError
         An error decoding ISO8583 bytearray.
     """
 
     # Message type is a set length in ISO8583
     if spec["t"]["data_enc"] == "b":
-        f_len = 2
+        expected_field_len = 2
     else:
-        f_len = 4
+        expected_field_len = 4
 
     doc_dec["t"] = ""
-    doc_enc["t"] = {"len": b"", "data": bytes(s[idx : idx + f_len])}
+    doc_enc["t"] = {"len": b"", "data": bytes(s[idx : idx + expected_field_len])}
 
-    if len(s[idx : idx + f_len]) != f_len:
+    if len(s[idx : idx + expected_field_len]) != expected_field_len:
         raise DecodeError(
-            f"Field data is {len(s[idx:idx + f_len])} bytes, expecting {f_len}",
+            f"Field data is {len(s[idx:idx + expected_field_len])} bytes, expecting {expected_field_len}",
             s,
             doc_dec,
             doc_enc,
             idx,
             "t",
         )
 
     if spec["t"]["data_enc"] == "b":
-        doc_dec["t"] = s[idx : idx + f_len].hex().upper()
+        doc_dec["t"] = s[idx : idx + expected_field_len].hex().upper()
     else:
-        try:
-            doc_dec["t"] = s[idx : idx + f_len].decode(spec["t"]["data_enc"])
-        except LookupError:
-            raise DecodeError(
-                "Failed to decode field, unknown encoding specified",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "t",
-            ) from None
-        except Exception:
-            raise DecodeError(
-                "Failed to decode field, invalid data",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "t",
-            ) from None
+        _decode_text_data(
+            s,
+            s[idx : idx + expected_field_len],
+            idx,
+            doc_dec,
+            doc_enc,
+            "t",
+            spec["t"],
+        )
 
-    return idx + f_len
+    return idx + expected_field_len
 
 
-def _decode_bitmaps(
+def _decode_bitmap(
     s: Union[bytes, bytearray],
     doc_dec: DecodedDict,
     doc_enc: EncodedDict,
     idx: int,
+    field_key: str,
     spec: SpecDict,
     fields: Set[int],
 ) -> int:
-    r"""Decode ISO8583 primary and secondary bitmaps.
+    r"""Decode ISO8583 a bitmap.
 
     Parameters
     ----------
     s : bytes or bytearray
         Encoded ISO8583 data
     doc_dec : dict
         Dict containing decoded ISO8583 data
     doc_enc : dict
         Dict containing encoded ISO8583 data
     idx : int
         Current index in ISO8583 byte array
     spec : dict
         A Python dict defining ISO8583 specification.
         See :mod:`iso8583.specs` module for examples.
+    field_key : str
+        Field ID to be decoded
     fields: set
         Will be populated with enabled field numbers
 
     Returns
     -------
     int
         Index in ISO8583 byte array where parsing of bitmaps ended
 
     Raises
     ------
     DecodeError
         An error decoding ISO8583 bytearray.
     """
 
-    # Primary bitmap is a set length in ISO8583
-    if spec["p"]["data_enc"] == "b":
-        f_len = 8
+    # Primary/Secondary bitmap is a set length in ISO8583
+    if spec[field_key]["data_enc"] == "b":
+        expected_field_len = 8
     else:
-        f_len = 16
+        expected_field_len = 16
 
-    doc_dec["p"] = ""
-    doc_enc["p"] = {"len": b"", "data": bytes(s[idx : idx + f_len])}
+    offset = 0 if field_key == "p" else 64
 
-    if len(s[idx : idx + f_len]) != f_len:
+    doc_dec[field_key] = ""
+    doc_enc[field_key] = {"len": b"", "data": bytes(s[idx : idx + expected_field_len])}
+
+    if len(s[idx : idx + expected_field_len]) != expected_field_len:
         raise DecodeError(
-            f"Field data is {len(s[idx:idx + f_len])} bytes, expecting {f_len}",
+            f"Field data is {len(s[idx:idx + expected_field_len])} bytes, expecting {expected_field_len}",
             s,
             doc_dec,
             doc_enc,
             idx,
-            "p",
+            field_key,
         )
 
-    if spec["p"]["data_enc"] == "b":
-        doc_dec["p"] = s[idx : idx + f_len].hex().upper()
-        bm = s[idx : idx + f_len]
-    else:
-        try:
-            doc_dec["p"] = s[idx : idx + f_len].decode(spec["p"]["data_enc"])
-        except LookupError:
-            raise DecodeError(
-                "Failed to decode field, unknown encoding specified",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "p",
-            ) from None
-        except Exception:
-            raise DecodeError(
-                "Failed to decode field, invalid data",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "p",
-            ) from None
-
-        try:
-            bm = bytes.fromhex(doc_dec["p"])
-        except Exception:
-            raise DecodeError(
-                "Failed to decode field, non-hex data",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "p",
-            ) from None
-
-    fields.update(
-        [
-            byte_idx * 8 + bit
-            for bit in range(1, 9)
-            for byte_idx, byte in enumerate(bm)
-            if byte >> (8 - bit) & 1
-        ]
-    )
-
-    idx += f_len
-
-    # No need to produce secondary bitmap if it's not required
-    if 1 not in fields:
-        return idx
-
-    # Decode secondary bitmap
-    # Secondary bitmap is a set length in ISO8583
-    if spec["1"]["data_enc"] == "b":
-        f_len = 8
+    if spec[field_key]["data_enc"] == "b":
+        doc_dec[field_key] = s[idx : idx + expected_field_len].hex().upper()
+        bitmap = s[idx : idx + expected_field_len]
     else:
-        f_len = 16
-
-    doc_dec["1"] = ""
-    doc_enc["1"] = {"len": b"", "data": bytes(s[idx : idx + f_len])}
-
-    if len(s[idx : idx + f_len]) != f_len:
-        raise DecodeError(
-            f"Field data is {len(s[idx:idx + f_len])} bytes, expecting {f_len}",
+        _decode_text_data(
             s,
+            s[idx : idx + expected_field_len],
+            idx,
             doc_dec,
             doc_enc,
-            idx,
-            "1",
+            field_key,
+            spec[field_key],
         )
 
-    if spec["1"]["data_enc"] == "b":
-        doc_dec["1"] = s[idx : idx + f_len].hex().upper()
-        bm = s[idx : idx + f_len]
-    else:
         try:
-            doc_dec["1"] = s[idx : idx + f_len].decode(spec["1"]["data_enc"])
-        except LookupError:
-            raise DecodeError(
-                "Failed to decode field, unknown encoding specified",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "1",
-            ) from None
-        except Exception:
-            raise DecodeError(
-                "Failed to decode field, invalid data",
-                s,
-                doc_dec,
-                doc_enc,
-                idx,
-                "1",
-            ) from None
-
-        try:
-            bm = bytes.fromhex(doc_dec["1"])
+            bitmap = bytes.fromhex(doc_dec[field_key])
         except Exception:
             raise DecodeError(
                 "Failed to decode field, non-hex data",
                 s,
                 doc_dec,
                 doc_enc,
                 idx,
-                "1",
+                field_key,
             ) from None
 
     fields.update(
         [
-            64 + byte_idx * 8 + bit
+            offset + byte_idx * 8 + bit
             for bit in range(1, 9)
-            for byte_idx, byte in enumerate(bm)
+            for byte_idx, byte in enumerate(bitmap)
             if byte >> (8 - bit) & 1
         ]
     )
 
-    return idx + f_len
+    return idx + expected_field_len
 
 
 def _decode_field(
     s: Union[bytes, bytearray],
     doc_dec: DecodedDict,
     doc_enc: EncodedDict,
     idx: int,
     field_key: str,
-    spec: SpecDict,
+    field_spec: _FieldSpecDict,
 ) -> int:
     r"""Decode ISO8583 individual fields.
 
     Parameters
     ----------
     s : bytes or bytearray
         Encoded ISO8583 data
@@ -454,32 +371,32 @@
         Dict containing decoded ISO8583 data
     doc_enc : dict
         Dict containing encoded ISO8583 data
     idx : int
         Current index in ISO8583 byte array
     field_key : str
         Field ID to be decoded
-    spec : dict
-        A Python dict defining ISO8583 specification.
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
         See :mod:`iso8583.specs` module for examples.
 
     Returns
     -------
     int
         Index in ISO8583 byte array where parsing of the field ended
 
     Raises
     ------
     DecodeError
         An error decoding ISO8583 bytearray.
     """
-    len_type = spec[field_key]["len_type"]
+    len_type = field_spec["len_type"]
 
     # Optional field added in v2.1. Prior specs do not have it.
-    len_count = spec[field_key].get("len_count", "bytes")
+    len_count = field_spec.get("len_count", "bytes")
 
     doc_dec[field_key] = ""
     doc_enc[field_key] = {"len": bytes(s[idx : idx + len_type]), "data": b""}
 
     if len(s[idx : idx + len_type]) != len_type:
         raise DecodeError(
             f"Field length is {len(s[idx:idx + len_type])} bytes wide, expecting {len_type}",
@@ -489,36 +406,52 @@
             idx,
             field_key,
         )
 
     # Parse field length if present.
     # For fixed-length fields max_len is the length.
     if len_type == 0:
-        enc_field_len: int = spec[field_key]["max_len"]
+        enc_field_len: int = field_spec["max_len"]
     # Variable field length
     else:
+        # Binary length
+        if field_spec["len_enc"] == "b":
+            try:
+                enc_field_len = int.from_bytes(
+                    s[idx : idx + len_type], "big", signed=False
+                )
+            # It does not seem to be possible to hit this unless
+            # it's a type or input parameter error.
+            # However, keeping this, because you just never know.
+            except Exception as e:  # pragma: no cover
+                raise DecodeError(
+                    f"Failed to decode field length, {e}",
+                    s,
+                    doc_dec,
+                    doc_enc,
+                    idx,
+                    field_key,
+                ) from None
         # BCD length
-        if spec[field_key]["len_enc"] in {"b", "bcd"}:
+        elif field_spec["len_enc"] == "bcd":
             try:
                 enc_field_len = int(s[idx : idx + len_type].hex(), 10)
             except Exception:
                 raise DecodeError(
                     "Failed to decode field length, invalid BCD data",
                     s,
                     doc_dec,
                     doc_enc,
                     idx,
                     field_key,
                 ) from None
         # Text length
         else:
             try:
-                decoded_length = s[idx : idx + len_type].decode(
-                    spec[field_key]["len_enc"]
-                )
+                decoded_length = s[idx : idx + len_type].decode(field_spec["len_enc"])
             except LookupError:
                 raise DecodeError(
                     "Failed to decode field length, unknown encoding specified",
                     s,
                     doc_dec,
                     doc_enc,
                     idx,
@@ -542,17 +475,17 @@
                     s,
                     doc_dec,
                     doc_enc,
                     idx,
                     field_key,
                 ) from None
 
-        if enc_field_len > spec[field_key]["max_len"]:
+        if enc_field_len > field_spec["max_len"]:
             raise DecodeError(
-                f"Field data is {enc_field_len} {len_count}, larger than maximum {spec[field_key]['max_len']}",
+                f"Field data is {enc_field_len} {len_count}, larger than maximum {field_spec['max_len']}",
                 s,
                 doc_dec,
                 doc_enc,
                 idx,
                 field_key,
             )
 
@@ -585,54 +518,47 @@
             s,
             doc_dec,
             doc_enc,
             idx,
             field_key,
         )
 
-    if spec[field_key]["data_enc"] == "b":
+    if field_spec["data_enc"] == "b":
         doc_dec[field_key] = doc_enc[field_key]["data"].hex().upper()
         if len_count == "nibbles" and enc_field_len & 1:
             doc_dec[field_key] = _remove_pad_field(
-                s, idx, doc_dec, doc_enc, field_key, spec, enc_field_len
-            )
-    else:
-        try:
-            doc_dec[field_key] = doc_enc[field_key]["data"].decode(
-                spec[field_key]["data_enc"]
-            )
-        except LookupError:
-            raise DecodeError(
-                "Failed to decode field, unknown encoding specified",
                 s,
-                doc_dec,
-                doc_enc,
                 idx,
-                field_key,
-            ) from None
-        except Exception:
-            raise DecodeError(
-                "Failed to decode field, invalid data",
-                s,
                 doc_dec,
                 doc_enc,
-                idx,
                 field_key,
-            ) from None
+                field_spec,
+                enc_field_len,
+            )
+    else:
+        _decode_text_data(
+            s,
+            doc_enc[field_key]["data"],
+            idx,
+            doc_dec,
+            doc_enc,
+            field_key,
+            field_spec,
+        )
 
     return idx + byte_field_len
 
 
 def _remove_pad_field(
     s: Union[bytes, bytearray],
     idx: int,
     doc_dec: DecodedDict,
     doc_enc: EncodedDict,
     field_key: str,
-    spec: SpecDict,
+    field_spec: _FieldSpecDict,
     enc_field_len: int,
 ) -> str:
     r"""Remove left or right pad from a BCD or hex field.
 
     Parameters
     ----------
     s : bytes or bytearray
@@ -641,39 +567,97 @@
         Current index in ISO8583 byte array
     doc_dec : dict
         Dict containing decoded ISO8583 data
     doc_enc : dict
         Dict containing encoded ISO8583 data
     field_key : str
         Field ID to remove pad from
-    spec : dict
-        A Python dict defining ISO8583 specification.
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
         See :mod:`iso8583.specs` module for examples.
     enc_field_len : int
         Number of nibbles expected in the field
 
     Returns
     -------
     str
         Field data without pad
 
     Raises
     ------
     DecodeError
         An error decoding ISO8583 bytearray.
     """
-    pad: str = spec[field_key].get("left_pad", "")[:1]
+    pad: str = field_spec.get("left_pad", "")[:1]
     if len(pad) > 0 and doc_dec[field_key][:1] == pad:
         return doc_dec[field_key][1:]
 
-    pad = spec[field_key].get("right_pad", "")[:1]
+    pad = field_spec.get("right_pad", "")[:1]
     if len(pad) > 0 and doc_dec[field_key][-1:] == pad:
         return doc_dec[field_key][:-1]
 
     raise DecodeError(
         f"Field data is {len(doc_dec[field_key])} nibbles, expecting {enc_field_len}",
         s,
         doc_dec,
         doc_enc,
         idx,
         field_key,
     )
+
+
+def _decode_text_data(
+    s: Union[bytes, bytearray],
+    data: Union[bytes, bytearray],
+    idx: int,
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    field_key: str,
+    field_spec: _FieldSpecDict,
+) -> None:
+    r"""Decode non-binary field and handle errors if any
+
+    Parameters
+    ----------
+    s : bytes or bytearray
+        Encoded ISO8583 data
+    data : bytes or bytearray
+        Encoded ISO8583 data to decode
+    idx : int
+        Current index in ISO8583 byte array
+    doc_dec : dict
+        Dict containing decoded ISO8583 data
+    doc_enc : dict
+        Dict containing encoded ISO8583 data
+    field_key : str
+        Field ID to remove pad from
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
+        See :mod:`iso8583.specs` module for examples.
+    enc_field_len : int
+        Number of nibbles expected in the field
+
+    Raises
+    ------
+    DecodeError
+        An error decoding ISO8583 bytearray.
+    """
+    try:
+        doc_dec[field_key] = data.decode(field_spec["data_enc"])
+    except LookupError:
+        raise DecodeError(
+            "Failed to decode field, unknown encoding specified",
+            s,
+            doc_dec,
+            doc_enc,
+            idx,
+            field_key,
+        ) from None
+    except Exception:
+        raise DecodeError(
+            "Failed to decode field, invalid data",
+            s,
+            doc_dec,
+            doc_enc,
+            idx,
+            field_key,
+        ) from None
```

### Comparing `pyiso8583-2.2.0/iso8583/encoder.py` & `pyiso8583-3.0.0/iso8583/encoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, Mapping, MutableMapping, Set, Tuple, Type
+import binascii
 
 __all__ = ["encode", "EncodeError"]
 
 DecodedDict = MutableMapping[str, str]
 EncodedDict = Dict[str, Dict[str, bytes]]
 SpecDict = Mapping[str, Mapping[str, Any]]
 
@@ -88,25 +89,31 @@
     s += _encode_type(doc_dec, doc_enc, spec)
     s += _encode_bitmaps(doc_dec, doc_enc, spec, fields)
 
     for field_key in [str(i) for i in sorted(fields)]:
         # Secondary bitmap is already encoded in _encode_bitmaps
         if field_key == "1":
             continue
-        s += _encode_field(doc_dec, doc_enc, field_key, spec)
+        s += _encode_field(doc_dec, doc_enc, field_key, spec[field_key])
 
     return s, doc_enc
 
 
 #
 # Private interface
 #
 
+_FieldSpecDict = Mapping[str, Any]
 
-def _encode_header(doc_dec: DecodedDict, doc_enc: EncodedDict, spec: SpecDict) -> bytes:
+
+def _encode_header(
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    spec: SpecDict,
+) -> bytes:
     r"""Encode ISO8583 header data if present from `d["h"]`.
 
     Parameters
     ----------
     doc_dec : dict
         Dict containing decoded ISO8583 data
     doc_enc : dict
@@ -132,18 +139,22 @@
 
     # Header data is a required field.
     if "h" not in doc_dec:
         raise EncodeError(
             "Field data is required according to specifications", doc_dec, doc_enc, "h"
         )
 
-    return _encode_field(doc_dec, doc_enc, "h", spec)
+    return _encode_field(doc_dec, doc_enc, "h", spec["h"])
 
 
-def _encode_type(doc_dec: DecodedDict, doc_enc: EncodedDict, spec: SpecDict) -> bytes:
+def _encode_type(
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    spec: SpecDict,
+) -> bytes:
     r"""Encode ISO8583 message type from `d["t"]`.
 
     Parameters
     ----------
     doc_dec : dict
         Dict containing decoded ISO8583 data
     doc_enc : dict
@@ -165,68 +176,41 @@
 
     # Message type is a required field.
     if "t" not in doc_dec:
         raise EncodeError("Field data is required", doc_dec, doc_enc, "t")
 
     # Message type is a set length in ISO8583
     if spec["t"]["data_enc"] == "b":
-        f_len = 2
+        expected_field_len = 2
     else:
-        f_len = 4
+        expected_field_len = 4
 
     doc_enc["t"] = {"len": b"", "data": b""}
 
     if spec["t"]["data_enc"] == "b":
-        try:
-            doc_enc["t"]["data"] = bytes.fromhex(doc_dec["t"])
-        except Exception:
-            if len(doc_dec["t"]) % 2 == 1:
-                raise EncodeError(
-                    "Failed to encode field, odd-length hex data",
-                    doc_dec,
-                    doc_enc,
-                    "t",
-                ) from None
-            raise EncodeError(
-                "Failed to encode field, non-hex data",
-                doc_dec,
-                doc_enc,
-                "t",
-            ) from None
+        enc_field_len = _encode_bindary_field(doc_dec, doc_enc, "t", spec["t"], "bytes")
     else:
-        try:
-            doc_enc["t"]["data"] = doc_dec["t"].encode(spec["t"]["data_enc"])
-        except LookupError:
-            raise EncodeError(
-                "Failed to encode field, unknown encoding specified",
-                doc_dec,
-                doc_enc,
-                "t",
-            ) from None
-        except Exception:
-            raise EncodeError(
-                "Failed to encode field, invalid data",
-                doc_dec,
-                doc_enc,
-                "t",
-            ) from None
+        enc_field_len = _encode_text_field(doc_dec, doc_enc, "t", spec["t"], "bytes")
 
-    if len(doc_enc["t"]["data"]) != f_len:
+    if enc_field_len != expected_field_len:
         raise EncodeError(
-            f"Field data is {len(doc_enc['t']['data'])} bytes, expecting {f_len}",
+            f"Field data is {enc_field_len} bytes, expecting {expected_field_len}",
             doc_dec,
             doc_enc,
             "t",
         )
 
     return doc_enc["t"]["data"]
 
 
 def _encode_bitmaps(
-    doc_dec: DecodedDict, doc_enc: EncodedDict, spec: SpecDict, fields: Set[int]
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    spec: SpecDict,
+    fields: Set[int],
 ) -> bytes:
     r"""Encode ISO8583 primary and secondary bitmap from dictionary keys.
 
     Parameters
     ----------
     doc_dec : dict
         Dict containing decoded ISO8583 data
@@ -297,83 +281,50 @@
     # Encode primary bitmap
     doc_dec["p"] = s[0:8].hex().upper()
     doc_enc["p"] = {"len": b"", "data": b""}
 
     if spec["p"]["data_enc"] == "b":
         doc_enc["p"]["data"] = bytes(s[0:8])
     else:
-        try:
-            doc_enc["p"]["data"] = doc_dec["p"].encode(spec["p"]["data_enc"])
-        except LookupError:
-            raise EncodeError(
-                "Failed to encode field, unknown encoding specified",
-                doc_dec,
-                doc_enc,
-                "p",
-            ) from None
-        # It does not seem to be possible to hit this because standard
-        # encodings are able to encode ASCII A-F characters.
-        # However, keeping this, because you just never know.
-        except Exception as e:  # pragma: no cover
-            raise EncodeError(
-                f"Failed to encode field, {e}",
-                doc_dec,
-                doc_enc,
-                "p",
-            ) from None
+        _encode_text_field(doc_dec, doc_enc, "p", spec["p"], "bytes")
 
     # No need to produce secondary bitmap if it's not required
     if 1 not in fields:
         return doc_enc["p"]["data"]
 
     # Encode secondary bitmap
     doc_dec["1"] = s[8:16].hex().upper()
     doc_enc["1"] = {"len": b"", "data": b""}
 
     if spec["1"]["data_enc"] == "b":
         doc_enc["1"]["data"] = bytes(s[8:16])
     else:
-        try:
-            doc_enc["1"]["data"] = doc_dec["1"].encode(spec["1"]["data_enc"])
-        except LookupError:
-            raise EncodeError(
-                "Failed to encode field, unknown encoding specified",
-                doc_dec,
-                doc_enc,
-                "1",
-            ) from None
-        # It does not seem to be possible to hit this because standard
-        # encodings are able to encode ASCII A-F characters.
-        # However, keeping this, because you just never know.
-        except Exception as e:  # pragma: no cover
-            raise EncodeError(
-                f"Failed to encode field, {e}",
-                doc_dec,
-                doc_enc,
-                "1",
-            ) from None
+        _encode_text_field(doc_dec, doc_enc, "1", spec["1"], "bytes")
 
     return doc_enc["p"]["data"] + doc_enc["1"]["data"]
 
 
 def _encode_field(
-    doc_dec: DecodedDict, doc_enc: EncodedDict, field_key: str, spec: SpecDict
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    field_key: str,
+    field_spec: _FieldSpecDict,
 ) -> bytes:
     r"""Encode ISO8583 individual field from `doc_dec[field_key]`.
 
     Parameters
     ----------
     doc_dec : dict
         Dict containing decoded ISO8583 data
     doc_enc : dict
         Dict containing encoded ISO8583 data
     field_key : str
         Field ID to be encoded
-    spec : dict
-        A Python dict defining ISO8583 specification.
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
         See :mod:`iso8583.specs` module for examples.
 
     Returns
     -------
     bytes
         Encoded ISO8583 field data
 
@@ -383,127 +334,96 @@
         An error encoding ISO8583 bytearray.
     """
 
     # Encode field data
     doc_enc[field_key] = {"len": b"", "data": b""}
 
     # Optional field added in v2.1. Prior specs do not have it.
-    len_count = spec[field_key].get("len_count", "bytes")
+    len_count = field_spec.get("len_count", "bytes")
 
     # Binary data: either hex or BCD
-    if spec[field_key]["data_enc"] == "b":
-        if len_count == "nibbles" and len(doc_dec[field_key]) & 1:
-            try:
-                nibble_data = _add_pad_field(doc_dec, field_key, spec)
-                doc_enc[field_key]["data"] = bytes.fromhex(nibble_data)
-            except Exception:
-                if len(nibble_data) % 2 == 1:
-                    raise EncodeError(
-                        "Failed to encode field, odd-length nibble data, specify pad",
-                        doc_dec,
-                        doc_enc,
-                        field_key,
-                    ) from None
-                raise EncodeError(
-                    "Failed to encode field, non-hex data",
-                    doc_dec,
-                    doc_enc,
-                    field_key,
-                ) from None
-        else:
-            try:
-                doc_enc[field_key]["data"] = bytes.fromhex(doc_dec[field_key])
-            except Exception:
-                if len(doc_dec[field_key]) % 2 == 1:
-                    raise EncodeError(
-                        "Failed to encode field, odd-length hex data",
-                        doc_dec,
-                        doc_enc,
-                        field_key,
-                    ) from None
-                raise EncodeError(
-                    "Failed to encode field, non-hex data",
-                    doc_dec,
-                    doc_enc,
-                    field_key,
-                ) from None
-
-        # Encoded field length can be in bytes or half bytes (nibbles)
-        if len_count == "nibbles":
-            enc_field_len = len(doc_dec[field_key])
-        else:
-            enc_field_len = len(doc_enc[field_key]["data"])
+    if field_spec["data_enc"] == "b":
+        enc_field_len = _encode_bindary_field(
+            doc_dec,
+            doc_enc,
+            field_key,
+            field_spec,
+            len_count,
+        )
     # Text data
     else:
-        try:
-            doc_enc[field_key]["data"] = doc_dec[field_key].encode(
-                spec[field_key]["data_enc"]
-            )
-        except LookupError:
-            raise EncodeError(
-                "Failed to encode field, unknown encoding specified",
-                doc_dec,
-                doc_enc,
-                field_key,
-            ) from None
-        except Exception:
-            raise EncodeError(
-                "Failed to encode field, invalid data",
-                doc_dec,
-                doc_enc,
-                field_key,
-            ) from None
-
-        # Encoded field length can be in bytes or half bytes (nibbles)
-        if len_count == "nibbles":
-            enc_field_len = len(doc_enc[field_key]["data"]) * 2
-        else:
-            enc_field_len = len(doc_enc[field_key]["data"])
+        enc_field_len = _encode_text_field(
+            doc_dec,
+            doc_enc,
+            field_key,
+            field_spec,
+            len_count,
+        )
 
-    len_type = spec[field_key]["len_type"]
+    len_type = field_spec["len_type"]
 
     # Handle fixed length field. No need to calculate length.
     if len_type == 0:
-        if enc_field_len != spec[field_key]["max_len"]:
+        if enc_field_len != field_spec["max_len"]:
             raise EncodeError(
-                f"Field data is {enc_field_len} {len_count}, expecting {spec[field_key]['max_len']}",
+                f"Field data is {enc_field_len} {len_count}, expecting {field_spec['max_len']}",
                 doc_dec,
                 doc_enc,
                 field_key,
             )
 
         doc_enc[field_key]["len"] = b""
         return doc_enc[field_key]["data"]
 
     # Continue with variable length field.
 
-    if enc_field_len > spec[field_key]["max_len"]:
+    if enc_field_len > field_spec["max_len"]:
         raise EncodeError(
-            f"Field data is {enc_field_len} {len_count}, larger than maximum {spec[field_key]['max_len']}",
+            f"Field data is {enc_field_len} {len_count}, larger than maximum {field_spec['max_len']}",
             doc_dec,
             doc_enc,
             field_key,
         )
 
-    # Encode field length
-    if spec[field_key]["len_enc"] in {"b", "bcd"}:
-        # Odd field length type is not allowed for purpose of string
-        # to BCD translation. Double it, e.g.:
+    # Encode binary field length
+    if field_spec["len_enc"] == "b":
+        try:
+            doc_enc[field_key]["len"] = (enc_field_len).to_bytes(
+                len_type, "big", signed=False
+            )
+        except OverflowError:
+            raise EncodeError(
+                "Failed to encode field length, field length does not fit into configured field size",
+                doc_dec,
+                doc_enc,
+                field_key,
+            ) from None
+    # Encode BCD field length
+    elif field_spec["len_enc"] == "bcd":
+        # Odd field length type is not allowed when translating string BCD. Pad it, e.g.:
         # BCD LVAR length \x09 must be string "09"
         # BCD LLVAR length \x99 must be string "99"
         # BCD LLLVAR length \x09\x99 must be string "0999"
         # BCD LLLLVAR length \x99\x99 must be string "9999"
-        doc_enc[field_key]["len"] = bytes.fromhex(
-            "{:0{len_type}d}".format(enc_field_len, len_type=len_type * 2)
-        )
+        bcd_field_len = "{:0{len_type}d}".format(enc_field_len, len_type=len_type * 2)
+
+        if len(bcd_field_len) > (len_type * 2):
+            raise EncodeError(
+                "Failed to encode field length, field length does not fit into configured field size",
+                doc_dec,
+                doc_enc,
+                field_key,
+            ) from None
+
+        doc_enc[field_key]["len"] = binascii.a2b_hex(bcd_field_len)
     else:
         try:
             doc_enc[field_key]["len"] = bytes(
                 "{:0{len_type}d}".format(enc_field_len, len_type=len_type),
-                spec[field_key]["len_enc"],
+                field_spec["len_enc"],
             )
         except LookupError:
             raise EncodeError(
                 "Failed to encode field length, unknown encoding specified",
                 doc_dec,
                 doc_enc,
                 field_key,
@@ -515,37 +435,173 @@
             raise EncodeError(
                 f"Failed to encode field length, {e}",
                 doc_dec,
                 doc_enc,
                 field_key,
             ) from None
 
+        if len(doc_enc[field_key]["len"]) > len_type:
+            raise EncodeError(
+                "Failed to encode field length, field length does not fit into configured field size",
+                doc_dec,
+                doc_enc,
+                field_key,
+            ) from None
+
     return doc_enc[field_key]["len"] + doc_enc[field_key]["data"]
 
 
-def _add_pad_field(doc_dec: DecodedDict, field_key: str, spec: SpecDict) -> str:
+def _encode_bindary_field(
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    field_key: str,
+    field_spec: _FieldSpecDict,
+    len_count: str,
+) -> int:
+    r"""Encode ISO8583 individual field from `doc_dec[field_key]` to its binary representation.
+
+    Parameters
+    ----------
+    doc_dec : dict
+        Dict containing decoded ISO8583 data
+    doc_enc : dict
+        Dict containing encoded ISO8583 data
+    field_key : str
+        Field ID to be encoded
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
+        See :mod:`iso8583.specs` module for examples.
+
+    Returns
+    -------
+    int
+        Length of the encoded ISO8583 field data. The length is either nibbles or bytes.
+
+    Raises
+    ------
+    EncodeError
+        An error encoding ISO8583 bytearray.
+    """
+    try:
+        # Odd length nibbles need to be padded because it's not possible to send half a byte
+        if len_count == "nibbles" and len(doc_dec[field_key]) & 1:
+            data_to_encode = _add_pad_field(doc_dec, field_key, field_spec)
+        else:
+            data_to_encode = doc_dec[field_key]
+        doc_enc[field_key]["data"] = binascii.a2b_hex(data_to_encode)
+    except Exception:
+        if len_count == "nibbles" and len(data_to_encode) % 2 == 1:
+            raise EncodeError(
+                "Failed to encode field, odd-length nibble data, specify pad",
+                doc_dec,
+                doc_enc,
+                field_key,
+            ) from None
+        if len(data_to_encode) % 2 == 1:
+            raise EncodeError(
+                "Failed to encode field, odd-length hex data",
+                doc_dec,
+                doc_enc,
+                field_key,
+            ) from None
+        raise EncodeError(
+            "Failed to encode field, non-hex data",
+            doc_dec,
+            doc_enc,
+            field_key,
+        ) from None
+
+    # Encoded field length can be in bytes or half bytes (nibbles).
+    # Encoded nibble length directly corresponds to the count of received nibbles.
+    if len_count == "nibbles":
+        return len(doc_dec[field_key])
+    else:
+        return len(doc_enc[field_key]["data"])
+
+
+def _add_pad_field(
+    doc_dec: DecodedDict,
+    field_key: str,
+    field_spec: _FieldSpecDict,
+) -> str:
     r"""Pad a BCD or hex field from the left or right.
 
     Parameters
     ----------
     doc_dec : dict
         Dict containing decoded ISO8583 data
     field_key : str
         Field ID to pad
-    spec : dict
-        A Python dict defining ISO8583 specification.
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
         See :mod:`iso8583.specs` module for examples.
 
     Returns
     -------
     str
         Padded field data
     """
-    pad: str = spec[field_key].get("left_pad", "")[:1]
+    pad: str = field_spec.get("left_pad", "")[:1]
     if len(pad) > 0:
         return pad + doc_dec[field_key]
 
-    pad = spec[field_key].get("right_pad", "")[:1]
+    pad = field_spec.get("right_pad", "")[:1]
     if len(pad) > 0:
         return doc_dec[field_key] + pad
 
     return doc_dec[field_key]
+
+
+def _encode_text_field(
+    doc_dec: DecodedDict,
+    doc_enc: EncodedDict,
+    field_key: str,
+    field_spec: _FieldSpecDict,
+    len_count: str,
+) -> int:
+    r"""Encode ISO8583 individual field from `doc_dec[field_key]` to its text representation.
+
+    Parameters
+    ----------
+    doc_dec : dict
+        Dict containing decoded ISO8583 data
+    doc_enc : dict
+        Dict containing encoded ISO8583 data
+    field_key : str
+        Field ID to be encoded
+    field_spec : dict
+        A Python dict defining ISO8583 specification for this field.
+        See :mod:`iso8583.specs` module for examples.
+
+    Returns
+    -------
+    int
+        Length of the encoded ISO8583 field data. The length is either nibbles or bytes.
+
+    Raises
+    ------
+    EncodeError
+        An error encoding ISO8583 bytearray.
+    """
+    try:
+        doc_enc[field_key]["data"] = doc_dec[field_key].encode(field_spec["data_enc"])
+    except LookupError:
+        raise EncodeError(
+            "Failed to encode field, unknown encoding specified",
+            doc_dec,
+            doc_enc,
+            field_key,
+        ) from None
+    except Exception:
+        raise EncodeError(
+            "Failed to encode field, invalid data",
+            doc_dec,
+            doc_enc,
+            field_key,
+        ) from None
+
+    # Encoded field length can be in bytes or half bytes (nibbles)
+    # Encoded nibble length directly corresponds to the count of received nibbles.
+    if len_count == "nibbles":
+        return len(doc_enc[field_key]["data"]) * 2
+    else:
+        return len(doc_enc[field_key]["data"])
```

### Comparing `pyiso8583-2.2.0/iso8583/specs.py` & `pyiso8583-3.0.0/iso8583/specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,55 +14,59 @@
 
 Mandatory Field Properties
 --------------------------
 Each field defines these properties:
 
 - **data_enc** - field data encoding type. Set to:
 
-  - ``b`` for binary or Binary-Coded Decimal (BCD) data. For example,
-    ``ABCD`` hex string is encoded as ``\xAB\xCD`` 2-byte value. Or ``1234``
-    numeric string is encoded as ``\x12\x34`` 2-byte BCD value.
+  - ``b`` for binary data. For example, ``ABCD`` hex string is encoded as
+    ``\xAB\xCD`` 2-byte value. This encoding type is also used for Binary-Coded
+    Decimal (BCD) because BCD encoding is a subset of hex encoding. For example,
+    ``1234`` numeric string is encoded as ``\x12\x34`` 2-byte BCD value.
   - Or any valid Python encoding. For example, ``ascii`` or
     ``latin-1`` for ASCII data and ``cp500`` or similar for EBCDIC data.
     For a list of built-in encodings, see Python standard encodings:
     https://docs.python.org/3/library/codecs.html#standard-encodings
 
 - **len_enc** - field length encoding type. This is needed for some fields,
   such as ICC data, that could have binary data but ASCII length.
   This parameter does not affect fixed-length fields. Set to:
 
-  - ``bcd`` for Binary-Coded Decimal (BCD) length. For example,
-    ``1234`` field length is encoded as ``\x12\x34`` 2-byte BCD value.
+  - ``b`` for binary length. For example, 16 byte long field will have length
+    encoded as ``\x10``.
+  - ``bcd`` for Binary-Coded Decimal (BCD) length. For example, 16 byte long
+    field will have length encoded as ``\x16``.
   - Or any valid Python encoding. For example, ``ascii`` or
     ``latin-1`` for ASCII length and ``cp500`` or similar for EBCDIC length.
     For a list of built-in encodings, see Python standard encodings:
     https://docs.python.org/3/library/codecs.html#standard-encodings
 
 - **len_type** - field length type: fixed, LVAR, LLVAR, etc.
   Expressed as a number of bytes in field length. For example,
   ASCII LLVAR length takes up 2 bytes (``b'00' - b'99'``).
   BCD LLVAR length can take up only 1 byte (``b'\x00' - b'\x99'``).
+  For binary lengths lenght type specifies the width of an unsigned integer.
   Therefore, **len_type** depends on the type of **len_enc** being used.
-  BCD **len_enc** can fit higher length ranges in fewer bytes.
+  BCD and binary **len_enc** can fit higher length ranges in fewer bytes.
 
-  +--------------+---------------------------------------+
-  |              |              **len_enc**              |
-  |              +----------------+----------------------+
-  | **len_type** | ASCII / EBCDIC | Binary-Coded Decimal |
-  +--------------+----------------+----------------------+
-  |  Fixed       |          ``0`` |                ``0`` |
-  +--------------+----------------+----------------------+
-  |  LVAR        |          ``1`` |                ``1`` |
-  +--------------+----------------+----------------------+
-  |  LLVAR       |          ``2`` |                ``1`` |
-  +--------------+----------------+----------------------+
-  |  LLLVAR      |          ``3`` |                ``2`` |
-  +--------------+----------------+----------------------+
-  |  LLLLVAR     |          ``4`` |                ``2`` |
-  +--------------+----------------+----------------------+
+  +--------------+--------------------------------------------------------+
+  |              |                      **len_enc**                       |
+  |              +----------------+----------------------+----------------+
+  | **len_type** | ASCII / EBCDIC | Binary-Coded Decimal |     Binary     |
+  +--------------+----------------+----------------------+----------------+
+  |  Fixed       |          ``0`` |                ``0`` |          ``0`` |
+  +--------------+----------------+----------------------+----------------+
+  |  LVAR        |          ``1`` |                ``1`` |  ``1`` (uint8) |
+  +--------------+----------------+----------------------+----------------+
+  |  LLVAR       |          ``2`` |                ``1`` |  ``1`` (uint8) |
+  +--------------+----------------+----------------------+----------------+
+  |  LLLVAR      |          ``3`` |                ``2`` | ``2`` (uint16) |
+  +--------------+----------------+----------------------+----------------+
+  |  LLLLVAR     |          ``4`` |                ``2`` | ``2`` (uint16) |
+  +--------------+----------------+----------------------+----------------+
 
 - **max_len** - field maximum length in bytes or nibbles. For fixed fields
   **max_len** defines the length of the field.
 
 - **desc** - field description that's printed in a pretty format.
   **desc** plays no role in encoding or decoding data. It's safe to omit it
   from the specifications. However, if omitted :func:`iso8583.pp` may or may
@@ -160,22 +164,32 @@
     }
 
 Field 6, a 3-nibble binary or BCD fixed field right-padded with 0.
 Length encoding makes no difference, since the field has no length::
 
     specification["6"] = {
         "data_enc": "b",
-        "len_enc": "bcd",
+        "len_enc": "ascii",
         "len_type": 0,
         "len_count": "nibbles",
         "right_pad": "0",
         "max_len": 3,
         "desc": "Binary or BCD fixed field measured in nibbles, e.g. \x11\x10"
     }
 
+Field 7, a 16-byte ascii field with binary length::
+
+    specification["2"] = {
+        "data_enc": "ascii",
+        "len_enc": "b",
+        "len_type": 1,
+        "max_len": 16,
+        "desc": "ASCII field with binary length, e.g. \x101234567890123456"
+    }
+
 Sample Message Specifications
 -----------------------------
 
 ASCII/Binary
 ~~~~~~~~~~~~
 
 Bitmaps, MACs, PIN, and ICC data are in binary::
```

### Comparing `pyiso8583-2.2.0/iso8583/tools.py` & `pyiso8583-3.0.0/iso8583/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys as _sys
-from typing import (Any, Callable, Dict, Generator, Mapping, Optional, TextIO,
-                    Union)
+from typing import Any, Callable, Dict, Generator, Mapping, Optional, TextIO, Union
 
 __all__ = ["pp"]
 
 DecodedDict = Mapping[str, str]
 EncodedDict = Mapping[str, Mapping[str, bytes]]
 SpecDict = Mapping[str, Mapping[str, Any]]
 
@@ -81,15 +80,14 @@
     doc: Union[DecodedDict, EncodedDict],
     spec: SpecDict,
     desc_width: int,
     stream: TextIO,
     line_width: int,
     field_key: str,
 ) -> None:
-
     indent = 5
     stream.write("{index:3s}".format(index=str(field_key)))
 
     if desc_width > 0:
         stream.write(
             " {desc: <{desc_width}}".format(
                 desc=spec[field_key]["desc"][:desc_width],
```

### Comparing `pyiso8583-2.2.0/pyiso8583.egg-info/PKG-INFO` & `pyiso8583-3.0.0/pyiso8583.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pyiso8583
-Version: 2.2.0
+Version: 3.0.0
 Summary: A serializer and deserializer of ISO8583 data.
 Home-page: https://github.com/knovichikhin/pyiso8583
 Author: Konstantin Novichikhin
 Author-email: konstantin.novichikhin@gmail.com
 License: MIT
 Keywords: iso8583 8583 banking protocol library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 
 iso8583 - a Python package for parsing ISO8583 data
 ===================================================
 
 |pypi| |docs| |coverage|
@@ -143,9 +141,7 @@
 .. |docs| image:: https://readthedocs.org/projects/pyiso8583/badge/?version=latest
     :alt: Documentation Status
     :target: https://pyiso8583.readthedocs.io/en/latest/?badge=latest
 
 .. |coverage| image:: https://codecov.io/gh/knovichikhin/pyiso8583/branch/master/graph/badge.svg
     :alt: Test coverage
     :target: https://codecov.io/gh/knovichikhin/pyiso8583
-
-
```

### Comparing `pyiso8583-2.2.0/pyiso8583.egg-info/SOURCES.txt` & `pyiso8583-3.0.0/pyiso8583.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/setup.py` & `pyiso8583-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from setuptools import find_packages, setup
 
-from iso8583 import __version__
-
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -21,22 +18,22 @@
 if __name__ == "__main__":
 
     with open("README.rst", "r", encoding="utf-8") as f:
         readme = f.read()
 
     setup(
         name="pyiso8583",
-        version=__version__,
+        version="3.0.0",
         author="Konstantin Novichikhin",
         author_email="konstantin.novichikhin@gmail.com",
         description="A serializer and deserializer of ISO8583 data.",
         long_description=readme,
         long_description_content_type="text/x-rst",
         license="MIT",
         url="https://github.com/knovichikhin/pyiso8583",
         packages=find_packages(exclude=["tests"]),
         package_data={"iso8583": ["py.typed"]},
         zip_safe=False,
         classifiers=classifiers,
-        python_requires=">=3.6",
+        python_requires=">=3.7",
         keywords="iso8583 8583 banking protocol library",
     )
```

### Comparing `pyiso8583-2.2.0/tests/test_nibbles.py` & `pyiso8583-3.0.0/tests/test_nibbles.py`

 * *Files identical despite different names*

### Comparing `pyiso8583-2.2.0/tests/test_tools.py` & `pyiso8583-3.0.0/tests/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import copy
 from io import StringIO
 
 import iso8583
 import iso8583.specs
-import pytest
+import typing
 from iso8583.tools import _wrap_bytes_repr, _wrap_str_repr
 
-spec = copy.deepcopy(iso8583.specs.default)
 
-
-def test_pp(capsys):
+def test_pp(capsys: typing.Any) -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 6
     spec["h"]["len_type"] = 0
-    doc_dec = {}
+    doc_dec: typing.Dict[str, str] = {}
     iso8583.pp(doc_dec, spec)
 
     captured = capsys.readouterr()
 
     r = captured.out.split("\n")
 
     assert r[0] == ""
@@ -54,16 +53,17 @@
     assert r[5] == "44  Additional Response Data      : b'03' b'123'"
     assert r[6] == "123 Reserved for Private Use      : b'003' b'123'"
     assert r[7] == ""
     assert len(r) == 8
     # fmt: on
 
 
-def test_pp_variable_header(capsys):
+def test_pp_variable_header(capsys: typing.Any) -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 6
     spec["h"]["len_type"] = 2
     doc_dec = {}
     doc_dec["h"] = "header"
     doc_dec["t"] = "0200"
     doc_dec["2"] = "12345678"
     doc_dec["44"] = "123"
@@ -123,16 +123,17 @@
     assert r[5] == "44  Additional Response Data      : b'03' b'123'"
     assert r[6] == "123 Reserved for Private Use      : b'003' b'123'"
     assert r[7] == ""
     assert len(r) == 8
     # fmt: on
 
 
-def test_pp_stream():
+def test_pp_stream() -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 6
     spec["h"]["len_type"] = 0
     doc_dec = {}
     doc_dec["h"] = "header"
     doc_dec["t"] = "0200"
     doc_dec["2"] = "12345678"
     doc_dec["44"] = "123"
@@ -163,21 +164,22 @@
     assert r[5] == "44  Additional Response Data      : b'03' b'123'"
     assert r[6] == "123 Reserved for Private Use      : b'003' b'123'"
     assert r[7] == ""
     assert len(r) == 8
     # fmt: on
 
 
-def test_pp_optional_fields():
+def test_pp_optional_fields() -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 6
     spec["h"]["len_type"] = 0
 
     # Empty
-    doc_dec = {}
+    doc_dec: typing.Dict[str, str] = {}
 
     sio = StringIO()
     iso8583.pp(doc_dec, spec, stream=sio)
     r = sio.getvalue().split("\n")
     assert r[0] == ""
     assert len(r) == 1
 
@@ -247,21 +249,22 @@
     assert r[3] == "1   Bitmap, Secondary             : b'\\x00\\x00\\x00\\x00\\x00\\x00\\x00 '"
     assert r[4] == "123 Reserved for Private Use      : b'003' b'123'"
     assert r[5] == ""
     assert len(r) == 6
     # fmt: on
 
 
-def test_pp_header_present_but_not_in_spec():
+def test_pp_header_present_but_not_in_spec() -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 0
     spec["h"]["len_type"] = 0
 
     # Empty
-    doc_dec = {}
+    doc_dec: typing.Dict[str, str] = {}
 
     sio = StringIO()
     iso8583.pp(doc_dec, spec, stream=sio)
     r = sio.getvalue().split("\n")
     assert r[0] == ""
     assert len(r) == 1
 
@@ -285,16 +288,17 @@
     r = sio.getvalue().split("\n")
     assert r[0] == "t   Message Type                  : '0200'"
     assert r[1] == ""
     assert len(r) == 2
     # fmt: on
 
 
-def test_pp_no_desc():
+def test_pp_no_desc() -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 0
     spec["h"]["len_type"] = 0
 
     doc_dec = {}
     doc_dec["t"] = "0200"
     doc_dec["2"] = "12345678"
     doc_dec["44"] = "123"
@@ -323,16 +327,17 @@
     assert r[4] == "44 : b'03' b'123'"
     assert r[5] == "123: b'003' b'123'"
     assert r[6] == ""
     assert len(r) == 7
     # fmt: on
 
 
-def test_pp_folding():
+def test_pp_folding() -> None:
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 0
     spec["h"]["len_type"] = 0
 
     doc_dec = {}
     doc_dec["t"] = "0200"
     doc_dec["123"] = "123456789012345678901234567890123456789012345678901234567890"
     _, doc_enc = iso8583.encode(doc_dec, spec)
@@ -712,26 +717,27 @@
     assert r[35] == "     '0'"
     assert r[36] == "123: '1'"
     assert r[37] == ""
     assert len(r) == 38
     # fmt: on
 
 
-def test_pp_invalid_types():
+def test_pp_invalid_types() -> None:
     """Invalid types should simply be printed as repr()
     If encoded dictionary does not have required 'len' and 'data'
     keys then no data should be printed.
     """
     # fmt: off
+    spec = copy.deepcopy(iso8583.specs.default)
     spec["h"]["max_len"] = 0
     spec["h"]["len_type"] = 0
 
-    doc_dec = {}
-    doc_dec["t"] = [1, 2, 3, 4]
-    doc_dec["123"] = set([1, 2, 3])
+    doc_dec: typing.Dict[str, str] = {}
+    doc_dec["t"] = [1, 2, 3, 4] # type: ignore
+    doc_dec["123"] = set([1, 2, 3]) # type: ignore
 
     # standard width = 80
     sio = StringIO()
     iso8583.pp(doc_dec, spec, stream=sio, line_width=80)
     r = sio.getvalue().split("\n")
     assert r[0] == "t   Message Type                  : [1, 2, 3, 4]"
     assert r[1] == "123 Reserved for Private Use      : {1, 2, 3}"
@@ -744,33 +750,33 @@
     r = sio.getvalue().split("\n")
     assert r[0] == "t   Message Type                  : [1, 2, 3, 4]"
     assert r[1] == "123 Reserved for Private Use      : {1, 2, 3}"
     assert r[2] == ""
     assert len(r) == 3
 
     # invalid encoded data
-    doc_enc = {}
-    doc_enc["t"] = {}
-    doc_enc["1"] = {'len': b'len'}
-    doc_enc["2"] = {'data': b'data'}
-    doc_enc["3"] = {'spam': b'eggs'}
+    doc_enc: typing.Dict[str, str] = {}
+    doc_enc["t"] = {} # type: ignore
+    doc_enc["1"] = {"len": b"len"} # type: ignore
+    doc_enc["2"] = {"data": b"data"} # type: ignore
+    doc_enc["3"] = {"spam": b"eggs"} # type: ignore
 
     sio = StringIO()
     iso8583.pp(doc_enc, spec, stream=sio, line_width=80)
     r = sio.getvalue().split("\n")
     assert r[0] == "t   Message Type                  : b''"
     assert r[1] == "1   Bitmap, Secondary             : b'len' b''"
     assert r[2] == "2   Primary Account Number (PAN)  : b'data'"
     assert r[3] == "3   Processing Code               : b''"
     assert r[4] == ""
     assert len(r) == 5
     # fmt: on
 
 
-def test_pp_no_yield_on_empty_string(capsys):
+def test_pp_no_yield_on_empty_string(capsys: typing.Any) -> None:
     for _ in _wrap_bytes_repr(b"", 10):
         print("spam")
 
     for _ in _wrap_str_repr("", 10):
         print("eggs")
 
     captured = capsys.readouterr()
```

