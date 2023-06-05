# Comparing `tmp/mdapackmol-fmt-0.1.0.tar.gz` & `tmp/mdapackmol_fmt-0.1.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdapackmol-fmt-0.1.0.tar", last modified: Fri Jun  2 19:48:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

