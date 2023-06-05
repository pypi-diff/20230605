# Comparing `tmp/gensp-1.0.1.tar.gz` & `tmp/gensp-1.0.2-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensp-1.0.1.tar", last modified: Mon Jun  5 03:36:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

