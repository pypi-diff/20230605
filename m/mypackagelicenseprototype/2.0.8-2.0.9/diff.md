# Comparing `tmp/mypackagelicenseprototype-2.0.8.tar.gz` & `tmp/mypackagelicenseprototype-2.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-2.0.8.tar", last modified: Mon Jun  5 12:18:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

