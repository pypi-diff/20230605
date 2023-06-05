# Comparing `tmp/fsspec_dnanexus-0.0.2-py3-none-any.whl.zip` & `tmp/fsspec_dnanexus-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14174 bytes, number of entries: 10
+Zip file size: 14326 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       70 b- defN 23-May-01 15:26 dxfsspec/__init__.py
 -rw-r--r--  2.0 unx    16792 b- defN 23-May-15 08:23 dxfsspec/core.py
--rw-r--r--  2.0 unx       70 b- defN 23-May-15 11:44 fsspec_dnanexus/__init__.py
--rw-r--r--  2.0 unx    20669 b- defN 23-May-29 13:24 fsspec_dnanexus/core.py
--rw-r--r--  2.0 unx     1064 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5334 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-May-29 14:20 fsspec_dnanexus-0.0.2.dist-info/RECORD
-10 files, 45007 bytes uncompressed, 12718 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 08:22 fsspec_dnanexus/__init__.py
+-rw-r--r--  2.0 unx    20706 b- defN 23-Jun-05 08:22 fsspec_dnanexus/core.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5598 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jun-05 10:14 fsspec_dnanexus-0.0.3.dist-info/RECORD
+10 files, 45332 bytes uncompressed, 12870 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fsspec_dnanexus/__init__.py
 Comment: 
 
 Filename: fsspec_dnanexus/core.py
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/LICENSE.txt
+Filename: fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/METADATA
+Filename: fsspec_dnanexus-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/WHEEL
+Filename: fsspec_dnanexus-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/entry_points.txt
+Filename: fsspec_dnanexus-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/top_level.txt
+Filename: fsspec_dnanexus-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.0.2.dist-info/RECORD
+Filename: fsspec_dnanexus-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fsspec_dnanexus/__init__.py

```diff
@@ -1 +1,3 @@
-from .core import DXFileSystem, DXFileSystemException, DXPathExtractor
+from .core import DXFileSystem, DXFileSystemException, DXPathExtractor
+
+__version__ = "0.0.3"
```

## fsspec_dnanexus/core.py

```diff
@@ -108,16 +108,17 @@
         project_id, file_id, _ = self.dx_path_extractor.extract_path(path)
 
         if not project_id or not file_id:
             raise DXFileSystemException(f"ValueError: Unsupported format of this path {path}")
 
         logger.debug(f"Get info of '{file_id}' in '{project_id}'")
         try:
-            dxfile = DXFile(file_id, project=project_id)
-            return dxfile.describe()
+            desc = DXFile(file_id, project=project_id).describe()
+            desc["type"] = desc["class"]
+            return desc
         except ResourceNotFound as e:
             raise DXFileSystemException(f"FileNotFound: {e}")
 
     def exists(self, path, **kwargs):
         logger.debug(f"Check if {path} exists")
         describe = self._file_describe(path, **kwargs)
         return describe is not None
```

## Comparing `fsspec_dnanexus-0.0.2.dist-info/LICENSE.txt` & `fsspec_dnanexus-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fsspec_dnanexus-0.0.2.dist-info/METADATA` & `fsspec_dnanexus-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec-dnanexus
-Version: 0.0.2
+Version: 0.0.3
 Summary: fsspec backend for the DNAnexus platform
 Maintainer: DNAnexus-xVantage
 Maintainer-email: tphan@dnanexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,18 +14,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: dxpy (==0.345.0)
 Requires-Dist: fsspec (==2023.4.0)
 
 # fsspec_dnanexus
-
-fsspec backend for DNAnexus
-
-    https://filesystem-spec.readthedocs.io/en/latest/
+[fsspec backend](https://filesystem-spec.readthedocs.io/en/latest/) for [DNAnexus](https://dnanexus.com)
 
 
 ## Installation
 
     pip install fsspec-dnanexus
 
 ## Usage
@@ -53,18 +50,18 @@
     dxfs.ls("dnanexus://my-dx-project:/my/folder", detail=True)
 
 DNAnexus entities are represented when listing a directory, but currently manipulation can only be done on files and folders
 
 Libraries such as pandas and modin have fsspec support built-in, and you can use the dnanexus URL once fsspec_dnanexus is installed
 
 ## Examples
+Reading a CSV or parquet in pandas using project name
 
-Reading a file in pandas using project name
-
-    df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv")
+    df = pd.read_csv("dnanexus://my-dx-project:/folder/data.csv")
+    df = pd.read_parquet("dnanexus://my-dx-project:/folder/data.parquet")
 
 Writing a pandas dataframe using project ID
 
     df.to_csv("dnanexus://project-XXXX:/folder/filename2.csv")
 
 Reading using fsspec.open
 
@@ -80,15 +77,14 @@
         url = f"dnanexus://{f['project']}:{f['name']}"
         df = pd.read_csv(url)
         print(df.iloc[:10])
 
 When writing files by default it will create any intermediate directories if they do not exist.
 
 ## Handling of duplicate file paths
-
 DNAnexus platform allows for duplicate filenames (but not folders)
 
 When reading files, a file URL resolves only to the file with the latest creation date and ignore the rest.
 
 When writing files, the default behaviour is to mimic POSIX file system such that there are no surprises from
 users coming from other fsspec backends, but this can easily be overrided in storage_options:
 
@@ -96,20 +92,22 @@
 * allow_duplicate_filenames: True - writes the file at specified path disregarding existing files
 
 If the user's token allows for file writing but does not allow for the removal of the file (e.g. protected projects), the behaviour falls
 back to allow_duplicate_filenames: True to ensure no data loss.
 
 
 ## Credentials
-
 The credentials used by fsspec_dnanexus to access DNAnexus is resolved in the following order:
 
-1. The token parameter passed into DXFileSystem's constructor or when making pandas calls
+1. The token parameter passed in using storage_options
+
+        # Option 1a
+        dxfs = fsspec.filesystem("dnanexus", storage_options = {"token": "YOUR_DNANEXUS_TOKEN"})
 
-        dxfs = DXFileSystem(storge_options = {"token": "YOUR_DNANEXUS_TOKEN"})
+        # Option 1b
         df = pd.read_csv("dnanexus://my-dx-project:/folder/filename1.csv", storage_options={
             "token": "YOUR_DNANEXUS_TOKEN",
         })
 
 2. The FSSPEC_DNANEXUS_TOKEN environment variable
 
         os.environ['FSSPEC_DNANEXUS_TOKEN'] = "YOUR_DNANEXUS_TOKEN"
@@ -124,33 +122,31 @@
 
 1. The following commands are currently unsupported:
     * dxfs.touch
     * dxfs.cat
     * dxfs.copy
     * dxfs.rm
 
-2. Parquet support has not beem tested
-3. No caching, which means repeated reads of a file will be inefficient
-4. fsspec transactions (e.g. `with fs.transaction:`) are not supported.
-5. Files not in 'closed' state on DNAnexus are not listed by ls() currently.
+2. No local caching, which means repeated reads of a file will incur repeated downloads
+3. fsspec transactions (e.g. `with fs.transaction:`) are not supported.
+4. Files not in 'closed' state on DNAnexus are not listed by ls() currently.
 
 
 ## Logging
 
 You can override the logging level by setting the following environment variable
-
     os.environ["FSSPEC_DNANEXUS_LOGGING_LEVEL"] = "DEBUG"
 
 Valid logging levels are listed here: https://docs.python.org/3/library/logging.html#levels
 
 
-# Changelog
-
-## [0.0.2] - 2023-05-29
+## Changelog
 
-### Fixed
-* Project description in PyPi, corrected import statement in README
+#### 0.0.3 (2023-06-05)
+* Fixed: When using PyArrow to read parquet, `pd.read_parquet` can be invoked directly, no longer requiring
+  passing in file handler from `fsspec.open()`.
 
-## [0.0.1] - 2023-05-29
+#### 0.0.2 (2023-05-29)
+* Fixed: Project description in PyPi, corrected import statement in README
 
-### Added
+#### 0.0.1 (2023-05-29)
 * Initial release
```

