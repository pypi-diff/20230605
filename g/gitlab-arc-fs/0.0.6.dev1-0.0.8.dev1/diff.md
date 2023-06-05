# Comparing `tmp/gitlab_arc_fs-0.0.6.dev1.tar.gz` & `tmp/gitlab_arc_fs-0.0.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_arc_fs-0.0.6.dev1.tar", last modified: Wed May 31 07:45:17 2023, max compression
+gzip compressed data, was "gitlab_arc_fs-0.0.8.dev1.tar", last modified: Mon Jun  5 08:34:51 2023, max compression
```

## Comparing `gitlab_arc_fs-0.0.6.dev1.tar` & `gitlab_arc_fs-0.0.8.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-02-27 10:58:22.000000 gitlab_arc_fs-0.0.6.dev1/README.md
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      424 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/entry_points.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/requires.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/top_level.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/setup.cfg
--rw-rw-r--   0 julian    (1000) julian    (1000)      768 2023-05-31 07:00:27.000000 gitlab_arc_fs-0.0.6.dev1/setup.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.780414 gitlab_arc_fs-0.0.6.dev1/src/
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/
--rw-rw-r--   0 julian    (1000) julian    (1000)       72 2023-05-31 06:59:25.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/__init__.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     8611 2023-05-31 06:59:34.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_filestream.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    28273 2023-05-31 06:59:29.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_fs.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    11153 2023-05-31 07:05:11.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/lfs_file.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     1046 2023-05-31 07:00:16.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/opener.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/tests/
--rw-rw-r--   0 julian    (1000) julian    (1000)    10257 2023-05-30 12:58:02.000000 gitlab_arc_fs-0.0.6.dev1/tests/test_gitlab_fs.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-02-27 10:58:22.000000 gitlab_arc_fs-0.0.8.dev1/README.md
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      424 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/entry_points.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/requires.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-06-05 08:34:51.000000 gitlab_arc_fs-0.0.8.dev1/gitlab_arc_fs.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/setup.cfg
+-rw-rw-r--   0 julian    (1000) julian    (1000)      768 2023-06-05 08:29:53.000000 gitlab_arc_fs-0.0.8.dev1/setup.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/src/
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/
+-rw-rw-r--   0 julian    (1000) julian    (1000)       72 2023-05-31 06:59:25.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/__init__.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     8611 2023-06-01 11:10:56.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_filestream.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    28274 2023-06-05 08:10:53.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_fs.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    11337 2023-06-05 08:08:08.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/lfs_file.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     1046 2023-05-31 07:00:16.000000 gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/opener.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-06-05 08:34:51.879120 gitlab_arc_fs-0.0.8.dev1/tests/
+-rw-rw-r--   0 julian    (1000) julian    (1000)    10257 2023-05-30 12:58:02.000000 gitlab_arc_fs-0.0.8.dev1/tests/test_gitlab_fs.py
```

### Comparing `gitlab_arc_fs-0.0.6.dev1/setup.py` & `gitlab_arc_fs-0.0.8.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
         'fs.opener': [
             'gitlab = gitlab_fs.opener:GitlabFSOpener',
         ]
     },
     license="MY LICENSE",
     packages=['gitlab_arc_fs'],
     package_dir={'gitlab_arc_fs': 'src/gitlab_arc_fs'},
-    version="0.0.6.dev1",
+    version="0.0.8.dev1",
     url="https://git.bwcloud.uni-freiburg.de/julian.weidhase/GitlabFS",
     python_requires='>=3.8'
 )
```

### Comparing `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_filestream.py` & `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_filestream.py`

 * *Files identical despite different names*

### Comparing `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_fs.py` & `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/gitlab_fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         try:
             with requests.Session() as session:
                 r = session.get(download_url,
                                 headers={"PRIVATE-TOKEN": self.token},
                                 data={"simple": True,
                                       "pagination": "keyset",
                                       "order_by": "id",
-                                      "sort": "asc"})
+                                      "sort": "desc"})
                 r.raise_for_status()
         except requests.HTTPError as e:
             print("Bad status code:", r.status_code)
             print("Exiting program")
             raise SystemExit(e)
         except requests.exceptions.Timeout:
             print("Timout error")
```

### Comparing `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/lfs_file.py` & `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/lfs_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,34 +292,41 @@
         download_url = (f"https://git.nfdi4plants.org/api/v4/projects/"
                         f"{self.repo_id}"
                         f"/repository/files/"
                         f"{file_path_gitattributes}"
                         f"/raw?ref="
                         f"{self.ref}")
 
+        action = "update"
         response = requests.get(download_url, headers=headers)
 
         new_line = f"{self.path} filter=lfs diff=lfs merge=lfs -text\n"
 
-        content = response.text + "\n" + new_line
+        try:
+            response.raise_for_status()
+            content = response.text + "\n" + new_line
+        except requests.HTTPError:
+            action = "create"
+            content = new_line
+
         data = [
             ('branch', f'{ref}'),
             ('commit_message', 'Modify .gitattributes'),
-            ('actions[][action]', 'update'),
+            ('actions[][action]', f'{action}'),
             ('actions[][file_path]', ".gitattributes"),
             ('actions[][content]', f"{content}")]
         url = (f'https://git.nfdi4plants.org/api/v4/projects/{self.repo_id}'
                f'/repository/commits')
         response = requests.post(url,
                                  headers=headers,
                                  data=data)
 
     def read(self):
         """
-        This file type only supports read access.
+        This file type only supports write access.
 
         """
         raise NotImplementedError
 
     def flush(self) -> None:
         self.tempfile.flush()
         return super().flush()
```

### Comparing `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/opener.py` & `gitlab_arc_fs-0.0.8.dev1/src/gitlab_arc_fs/opener.py`

 * *Files identical despite different names*

### Comparing `gitlab_arc_fs-0.0.6.dev1/tests/test_gitlab_fs.py` & `gitlab_arc_fs-0.0.8.dev1/tests/test_gitlab_fs.py`

 * *Files identical despite different names*

