# Comparing `tmp/auto_remote_sync-1.0.6.tar.gz` & `tmp/auto_remote_sync-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_remote_sync-1.0.6.tar", last modified: Tue Mar  7 00:40:18 2023, max compression
+gzip compressed data, was "auto_remote_sync-1.0.7.tar", last modified: Sun Jun  4 23:56:37 2023, max compression
```

## Comparing `auto_remote_sync-1.0.6.tar` & `auto_remote_sync-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    35148 2022-12-06 10:13:27.000000 auto_remote_sync-1.0.6/LICENSE
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4760 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)     3682 2022-12-06 10:06:22.000000 auto_remote_sync-1.0.6/README.md
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4760 2023-03-07 00:40:15.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)      265 2023-03-07 00:40:16.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/SOURCES.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2023-03-07 00:40:16.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/dependency_links.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2023-03-07 00:40:16.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/requires.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       10 2023-03-07 00:40:16.000000 auto_remote_sync-1.0.6/auto_remote_sync.egg-info/top_level.txt
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/autorsync/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     6305 2023-03-07 00:35:08.000000 auto_remote_sync-1.0.6/autorsync/__init__.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/scripts/
--rwxr-xr-x   0 aviram    (1000) aviram    (1000)     2389 2023-03-07 00:35:18.000000 auto_remote_sync-1.0.6/scripts/autorsync
--rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2023-03-07 00:40:18.000000 auto_remote_sync-1.0.6/setup.cfg
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1687 2022-12-06 10:00:40.000000 auto_remote_sync-1.0.6/setup.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    35148 2023-06-04 23:52:56.000000 auto_remote_sync-1.0.7/LICENSE
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     4897 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     3741 2023-06-04 23:52:56.000000 auto_remote_sync-1.0.7/README.md
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1380 2023-06-04 23:47:00.000000 auto_remote_sync-1.0.7/pyproject.toml
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/setup.cfg
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     4897 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      345 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       40 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/entry_points.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/requires.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       15 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/top_level.txt
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/autorsync/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     6385 2023-06-04 23:52:56.000000 auto_remote_sync-1.0.7/src/autorsync/__init__.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2023-06-04 23:56:37.000000 auto_remote_sync-1.0.7/src/tool/
+-rwxr-xr-x   0 aviram    (1000) aviram    (1000)     2389 2023-06-04 23:52:56.000000 auto_remote_sync-1.0.7/src/tool/__init__.py
```

### Comparing `auto_remote_sync-1.0.6/LICENSE` & `auto_remote_sync-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_remote_sync-1.0.6/PKG-INFO` & `auto_remote_sync-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: auto_remote_sync
-Version: 1.0.6
+Version: 1.0.7
 Summary: Automate execution of various rsync commands based on profiles defined on a YAML configuration file
-Home-page: https://github.com/avibrazil/autorsync
-Author: Avi Alkalay
-Author-email: avi@unix.sh
+Author-email: Avi Alkalay <avi@unix.sh>
+Project-URL: Homepage, https://github.com/avibrazil/autorsync
+Project-URL: Bug Tracker, https://github.com/avibrazil/autorsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Auto rsync
 
 Command to automate execution of various rsync commands based on profiles
 defined on a YAML configuration file.
@@ -99,14 +99,15 @@
 - `backup` and `backup_dir` makes rsync save backups on target of deleted or
 modified files on source. Value on `backup_dir` is a path relative to target
 folder
 - You can use Jinja logic in path parts, surrounded by `{{}}`. Currently these
 are the available variables:
     - `time`, a Python `datetime.datetime` object which includes local timezone
     - `hostname`, such as “rocket”
+    - `Hostname`, such as “rocket.mydomain.com” (FQDN)
     - `username`, UNIX user name as “joanbaez”
     - `home`, user’s home folder as “/home/joanbaez”
     - `userid`, user ID as “504”
     - `gecos`, user long name as “Joan Baez”
 
 ### Example usage
 - Show all profiles:
```

### Comparing `auto_remote_sync-1.0.6/README.md` & `auto_remote_sync-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 - `backup` and `backup_dir` makes rsync save backups on target of deleted or
 modified files on source. Value on `backup_dir` is a path relative to target
 folder
 - You can use Jinja logic in path parts, surrounded by `{{}}`. Currently these
 are the available variables:
     - `time`, a Python `datetime.datetime` object which includes local timezone
     - `hostname`, such as “rocket”
+    - `Hostname`, such as “rocket.mydomain.com” (FQDN)
     - `username`, UNIX user name as “joanbaez”
     - `home`, user’s home folder as “/home/joanbaez”
     - `userid`, user ID as “504”
     - `gecos`, user long name as “Joan Baez”
 
 ### Example usage
 - Show all profiles:
```

### Comparing `auto_remote_sync-1.0.6/auto_remote_sync.egg-info/PKG-INFO` & `auto_remote_sync-1.0.7/src/auto_remote_sync.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: auto-remote-sync
-Version: 1.0.6
+Version: 1.0.7
 Summary: Automate execution of various rsync commands based on profiles defined on a YAML configuration file
-Home-page: https://github.com/avibrazil/autorsync
-Author: Avi Alkalay
-Author-email: avi@unix.sh
+Author-email: Avi Alkalay <avi@unix.sh>
+Project-URL: Homepage, https://github.com/avibrazil/autorsync
+Project-URL: Bug Tracker, https://github.com/avibrazil/autorsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Recovery Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Auto rsync
 
 Command to automate execution of various rsync commands based on profiles
 defined on a YAML configuration file.
@@ -99,14 +99,15 @@
 - `backup` and `backup_dir` makes rsync save backups on target of deleted or
 modified files on source. Value on `backup_dir` is a path relative to target
 folder
 - You can use Jinja logic in path parts, surrounded by `{{}}`. Currently these
 are the available variables:
     - `time`, a Python `datetime.datetime` object which includes local timezone
     - `hostname`, such as “rocket”
+    - `Hostname`, such as “rocket.mydomain.com” (FQDN)
     - `username`, UNIX user name as “joanbaez”
     - `home`, user’s home folder as “/home/joanbaez”
     - `userid`, user ID as “504”
     - `gecos`, user long name as “Joan Baez”
 
 ### Example usage
 - Show all profiles:
```

### Comparing `auto_remote_sync-1.0.6/autorsync/__init__.py` & `auto_remote_sync-1.0.7/src/autorsync/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 import subprocess
 import logging
 import yaml
 import jinja2
 
 
-__version__="1.0.6"
+__version__="1.0.7"
 
 
 __all__=['RSyncProfile', 'RSyncProfiles']
 
 
 class RSyncProfile():
     # The barebone defaults
@@ -28,15 +28,16 @@
         time            = datetime.datetime.now(
                             tz=(
                                 datetime.datetime.now(tz=datetime.timezone.utc)
                                 .astimezone()
                                 .tzinfo
                             )
         ),
-        hostname        = platform.uname().node,
+        hostname        = platform.node().split('.',1)[0],
+        Hostname        = platform.node(),
         username        = pwd.getpwuid(os.getuid()).pw_name,
         userid          = pwd.getpwuid(os.getuid()).pw_uid,
         gecos           = pwd.getpwuid(os.getuid()).pw_gecos,
         home            = pwd.getpwuid(os.getuid()).pw_dir,
     )
 
     as_str_template=(
@@ -98,28 +99,26 @@
             target=self.get_target(),
             command=self.make_command()
         )
 
 
 
     def render(self,text):
-#         datapool=dict(
-#             time=self.current_time,
-#             hostname=self.hostname,
-#         )
-
         return jinja2.Template(text).render(self.datapool)
 
 
 
     def make_command(self,simulate=False):
         command=[
-            'rsync','--fuzzy','--sparse','--human-readable','--hard-links',
-            '--perms','--recursive','--times','--atimes','--open-noatime',
-            '--devices','--specials','--links','--mkpath','--verbose'
+            'rsync',
+            '--human-readable', '--fuzzy',   '--sparse',   '--hard-links',
+            '--recursive',      '--perms',   '--owner',    '--group',
+            '--executability',  '--times',   '--atimes',   '--acls',
+            '--open-noatime',   '--devices', '--specials', '--links',
+            '--mkpath',         '--verbose', '--xattrs',
         ]
 
         if self.simulate or simulate:
             command.append("--dry-run")
 
         if self.delete:
             command.append("--delete")
```

### Comparing `auto_remote_sync-1.0.6/scripts/autorsync` & `auto_remote_sync-1.0.7/src/tool/__init__.py`

 * *Files identical despite different names*

