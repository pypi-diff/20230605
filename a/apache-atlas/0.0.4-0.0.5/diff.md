# Comparing `tmp/apache-atlas-0.0.4.tar.gz` & `tmp/apache_atlas-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-atlas-0.0.4.tar", last modified: Mon Jan 18 21:30:20 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

