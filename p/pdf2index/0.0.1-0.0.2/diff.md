# Comparing `tmp/pdf2index-0.0.1-py3-none-any.whl.zip` & `tmp/pdf2index-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5003 bytes, number of entries: 10
+Zip file size: 5172 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 pdf2index/__about__.py
 -rw-r--r--  2.0 unx       26 b- defN 20-Feb-02 00:00 pdf2index/__init__.py
 -rw-r--r--  2.0 unx     2169 b- defN 20-Feb-02 00:00 pdf2index/__main__.py
 -rw-r--r--  2.0 unx     2292 b- defN 20-Feb-02 00:00 pdf2index/keywords.py
 -rw-r--r--  2.0 unx      852 b- defN 20-Feb-02 00:00 pdf2index/pdf.py
-?rw-r--r--  2.0 unx     1529 b- defN 20-Feb-02 00:00 pdf2index-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pdf2index-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       44 b- defN 20-Feb-02 00:00 pdf2index-0.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1036 b- defN 20-Feb-02 00:00 pdf2index-0.0.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      793 b- defN 20-Feb-02 00:00 pdf2index-0.0.1.dist-info/RECORD
-10 files, 8850 bytes uncompressed, 3649 bytes compressed:  58.8%
+?rw-r--r--  2.0 unx     1857 b- defN 20-Feb-02 00:00 pdf2index-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pdf2index-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       44 b- defN 20-Feb-02 00:00 pdf2index-0.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1036 b- defN 20-Feb-02 00:00 pdf2index-0.0.2.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx      793 b- defN 20-Feb-02 00:00 pdf2index-0.0.2.dist-info/RECORD
+10 files, 9178 bytes uncompressed, 3818 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pdf2index/keywords.py
 Comment: 
 
 Filename: pdf2index/pdf.py
 Comment: 
 
-Filename: pdf2index-0.0.1.dist-info/METADATA
+Filename: pdf2index-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pdf2index-0.0.1.dist-info/WHEEL
+Filename: pdf2index-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pdf2index-0.0.1.dist-info/entry_points.txt
+Filename: pdf2index-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pdf2index-0.0.1.dist-info/licenses/LICENSE.txt
+Filename: pdf2index-0.0.2.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: pdf2index-0.0.1.dist-info/RECORD
+Filename: pdf2index-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdf2index/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `pdf2index-0.0.1.dist-info/METADATA` & `pdf2index-0.0.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf2index
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://gitlab.com/philipp.herkert/pdf2index
 Project-URL: Issues, https://gitlab.com/philipp.herkert/pdf2index/-/issues
 Project-URL: Source, https://gitlab.com/philipp.herkert/pdf2index
 Author: Philipp Herkert
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -36,16 +36,28 @@
 
 ## Installation
 
 ```console
 pip install pdf2index
 ```
 
+Consider installing in a `venv` or using `pipx`
+
+Warning: This package has large dependencies. You will be downloading ~2 GB.
+
+## Usage
+
+```console
+pdf2index book1.pdf book2.pdf book3.pdf --password $(<password_file.txt) --out index.txt
+```
+
+Note: The order of the pdfs matters as the books will be referenced in that order.
+
 ## Dev
 
 ```console
- hatch run pdf2index data/book* -p $(<data/passwd/pass.txt)
+ hatch run pdf2index data/Book* -p $(<data/passwd/passwd.txt)
 ```
 
 ## License
 
 `pdf2index` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

## Comparing `pdf2index-0.0.1.dist-info/licenses/LICENSE.txt` & `pdf2index-0.0.2.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pdf2index-0.0.1.dist-info/RECORD` & `pdf2index-0.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-pdf2index/__about__.py,sha256=sXLh7g3KC4QCFxcZGBTpG2scR7hmmBsMjq6LqRptkRg,22
+pdf2index/__about__.py,sha256=QvlVh4JTl3JL7jQAja76yKtT-IvF4631ASjWY1wS6AQ,22
 pdf2index/__init__.py,sha256=48zRUzNIJ42exCaQuXx6XHkpYN_07u4hqTNqRX8VLqw,26
 pdf2index/__main__.py,sha256=b6nG7QjmsKy2oM9lUUaxW5006XRZyHOUUTrMBqQjiTE,2169
 pdf2index/keywords.py,sha256=z8DYi9GN4q0k5SRMHLIbbfP4aWZ2WeaRHWYm-VJuF9g,2292
 pdf2index/pdf.py,sha256=IDf6iwg-T9X-YLVCDQiyQtyLj4aO7WWvM-Q6YUYH4JA,852
-pdf2index-0.0.1.dist-info/METADATA,sha256=f3h3G-HMYdM86aNatEYfyXXsZlBdFZgUqDX-awWrdZ4,1529
-pdf2index-0.0.1.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
-pdf2index-0.0.1.dist-info/entry_points.txt,sha256=XNVXXP4-NV25f48G3zubo2DcJ25PKKM5kW6qEdFIDN4,44
-pdf2index-0.0.1.dist-info/licenses/LICENSE.txt,sha256=WvwiBQtt_VVnf6szbVDxrAuRc6U6TLa7mbnvJSWzMGw,1036
-pdf2index-0.0.1.dist-info/RECORD,,
+pdf2index-0.0.2.dist-info/METADATA,sha256=aRpJEUh52u18p8HdGRTLOyGJdj7Be6tbtOF3jkHy4ic,1857
+pdf2index-0.0.2.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
+pdf2index-0.0.2.dist-info/entry_points.txt,sha256=XNVXXP4-NV25f48G3zubo2DcJ25PKKM5kW6qEdFIDN4,44
+pdf2index-0.0.2.dist-info/licenses/LICENSE.txt,sha256=WvwiBQtt_VVnf6szbVDxrAuRc6U6TLa7mbnvJSWzMGw,1036
+pdf2index-0.0.2.dist-info/RECORD,,
```

