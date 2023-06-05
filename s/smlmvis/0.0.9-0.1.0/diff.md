# Comparing `tmp/smlmvis-0.0.9.tar.gz` & `tmp/smlmvis-0.1.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smlmvis-0.0.9.tar", last modified: Thu Nov 28 21:42:52 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

