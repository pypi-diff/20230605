# Comparing `tmp/cleepcli-1.8.1.tar.gz` & `tmp/cleepcli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleepcli-1.8.1.tar", last modified: Thu Oct  3 18:08:16 2019, max compression
+gzip compressed data, was "dist/cleepcli-1.9.0.tar", last modified: Sun Oct  6 11:03:00 2019, max compression
```

## Comparing `cleepcli-1.8.1.tar` & `cleepcli-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-03 18:08:16.000000 cleepcli-1.8.1/
--rw-r--r--   0 root         (0) root         (0)     3077 2019-04-12 21:12:45.000000 cleepcli-1.8.1/README.md
--rw-r--r--   0 root         (0) root         (0)      379 2019-10-03 18:08:16.000000 cleepcli-1.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       79 2019-10-03 18:08:16.000000 cleepcli-1.8.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-03 18:08:16.000000 cleepcli-1.8.1/cleepcli/
--rw-r--r--   0 root         (0) root         (0)     6129 2019-04-19 10:24:41.000000 cleepcli-1.8.1/cleepcli/docs.py
--rw-r--r--   0 root         (0) root         (0)     3594 2019-04-14 09:51:10.000000 cleepcli-1.8.1/cleepcli/file.py
--rw-r--r--   0 root         (0) root         (0)    10805 2019-04-18 21:52:53.000000 cleepcli-1.8.1/cleepcli/watch.py
--rwxr-xr-x   0 root         (0) root         (0)       32 2019-10-03 17:54:42.000000 cleepcli-1.8.1/cleepcli/git_password.sh
--rw-r--r--   0 root         (0) root         (0)    10466 2019-06-27 13:47:10.000000 cleepcli-1.8.1/cleepcli/module.py
--rw-r--r--   0 root         (0) root         (0)    12089 2019-04-15 19:03:02.000000 cleepcli-1.8.1/cleepcli/console.py
--rw-r--r--   0 root         (0) root         (0)     3794 2019-07-10 09:47:20.000000 cleepcli-1.8.1/cleepcli/git.py
--rw-r--r--   0 root         (0) root         (0)     6619 2019-05-03 22:09:14.000000 cleepcli-1.8.1/cleepcli/distrib.py
--rw-r--r--   0 root         (0) root         (0)     1120 2019-10-03 18:07:39.000000 cleepcli-1.8.1/cleepcli/config.py
--rw-r--r--   0 root         (0) root         (0)     2217 2019-06-13 10:17:57.000000 cleepcli-1.8.1/cleepcli/cleepapi.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-04-05 12:50:03.000000 cleepcli-1.8.1/cleepcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5164 2019-04-16 13:23:44.000000 cleepcli-1.8.1/cleepcli/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-03 18:08:16.000000 cleepcli-1.8.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)     8752 2019-10-03 18:06:13.000000 cleepcli-1.8.1/bin/cleep-cli
--rw-r--r--   0 root         (0) root         (0)      886 2019-05-13 19:32:24.000000 cleepcli-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-03 18:08:16.000000 cleepcli-1.8.1/cleepcli.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2019-10-03 18:08:15.000000 cleepcli-1.8.1/cleepcli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      379 2019-10-03 18:08:15.000000 cleepcli-1.8.1/cleepcli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      168 2019-10-03 18:08:15.000000 cleepcli-1.8.1/cleepcli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      443 2019-10-03 18:08:16.000000 cleepcli-1.8.1/cleepcli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-10-03 18:08:15.000000 cleepcli-1.8.1/cleepcli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2019-04-09 08:29:51.000000 cleepcli-1.8.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-06 11:03:00.000000 cleepcli-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     3639 2019-10-06 11:01:55.000000 cleepcli-1.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      379 2019-10-06 11:03:00.000000 cleepcli-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       79 2019-10-06 11:03:00.000000 cleepcli-1.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli/
+-rw-r--r--   0 root         (0) root         (0)     6129 2019-04-19 10:24:41.000000 cleepcli-1.9.0/cleepcli/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2019-04-14 09:51:10.000000 cleepcli-1.9.0/cleepcli/file.py
+-rw-r--r--   0 root         (0) root         (0)    10805 2019-04-18 21:52:53.000000 cleepcli-1.9.0/cleepcli/watch.py
+-rwxr-xr-x   0 root         (0) root         (0)       32 2019-10-03 17:54:42.000000 cleepcli-1.9.0/cleepcli/git_password.sh
+-rw-r--r--   0 root         (0) root         (0)    11304 2019-10-06 11:01:28.000000 cleepcli-1.9.0/cleepcli/module.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2019-04-15 19:03:02.000000 cleepcli-1.9.0/cleepcli/console.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2019-07-10 09:47:20.000000 cleepcli-1.9.0/cleepcli/git.py
+-rw-r--r--   0 root         (0) root         (0)     6619 2019-05-03 22:09:14.000000 cleepcli-1.9.0/cleepcli/distrib.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2019-10-06 11:01:28.000000 cleepcli-1.9.0/cleepcli/config.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2019-06-13 10:17:57.000000 cleepcli-1.9.0/cleepcli/cleepapi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-04-05 12:50:03.000000 cleepcli-1.9.0/cleepcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5164 2019-04-16 13:23:44.000000 cleepcli-1.9.0/cleepcli/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-06 11:03:00.000000 cleepcli-1.9.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     9122 2019-10-06 11:01:28.000000 cleepcli-1.9.0/bin/cleep-cli
+-rw-r--r--   0 root         (0) root         (0)      886 2019-05-13 19:32:24.000000 cleepcli-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        9 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      379 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      168 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      443 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-10-06 11:03:00.000000 cleepcli-1.9.0/cleepcli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2019-04-09 08:29:51.000000 cleepcli-1.9.0/MANIFEST.in
```

### Comparing `cleepcli-1.8.1/README.md` & `cleepcli-1.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 # Cleep-cli
 
 This utility helps developers to build Cleep applications providing some useful commands:
-* `coreget` to clone or pull official Cleep repository.
-* `coresync` to synchronize sources from repository to execution folders.
-* `modcreate` to create module (aka application) skeleton.
-* `modsync` to synchronize sources from module folder to execution folders.
-* `watch` to watch for repository filesystem changes and automatically update files on execution folders. It also restart backend or/and frontend according to changes.
+* Core commands:
+    * `coreget` to clone or pull official Cleep repository.
+    * `coresync` to synchronize sources from repository to execution folders.
+    * `cpuprof` to run CPU profiler on application execution instance.
+    * `memprof` to run memory profiler on application execution instance.
+    * `reset` clear existing installed Cleep files and install it again.
+* Module commands:
+    * `modsync` to synchronize sources from module folder to execution folders.
+    * `modcreate` to create module (aka application) skeleton.
+    * `moddelete` to delete installed files of a module
+    * `modtests` to execute module unit tests
+    * `modtestscov` to display last execution tests coverage
+    * `moddocs` to generate module documentation
+* Watch commands:
+    * `watch` to watch for repository filesystem changes and automatically update files on execution folders. It also restart backend or/and frontend according to changes.
+* Misc commands:
+    * `version` to get cleep-cli version
 
 ## Installation
 Cleep-cli is automatically installed and managed by [Cleep developer](https://github.com/tangb/cleepmod-developer) application.
 
 If you want to install it manually, execute following command:
 > pip install cleepcli
```

### Comparing `cleepcli-1.8.1/cleepcli/docs.py` & `cleepcli-1.9.0/cleepcli/docs.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/file.py` & `cleepcli-1.9.0/cleepcli/file.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/watch.py` & `cleepcli-1.9.0/cleepcli/watch.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/module.py` & `cleepcli-1.9.0/cleepcli/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -327,7 +327,34 @@
             self.logger.error('Error occured while pulling repository: %s' % ('killed' if resp['killed'] else resp['stderr']))
             shutil.rmtree(path)
             return False
         
         self.logger.info('Done')
         return True
 
+    def delete(self, module_name):
+        """
+        Delete installed files for specified  module
+
+        Args:
+            module_name (string): module name
+        """
+        #build all module paths
+        paths = [
+            os.path.join(config.MODULES_DST, module_name),
+            os.path.join(config.MODULES_HTML_DST, module_name),
+            os.path.join(config.MODULES_SCRIPTS_DST, module_name),
+        ]
+        self.logger.info('Deleting module "%s" in "%s"' % (module_name, paths))
+        
+        deleted = False
+        for path in paths:
+            if os.path.exists(path):
+                shutil.rmtree(path)
+                self.logger.debug('Directory "%s" deleted' % path)
+                deleted = True
+
+        if not deleted:
+            self.logger.info('Nothing has been deleted')
+
+        return True
+
```

### Comparing `cleepcli-1.8.1/cleepcli/console.py` & `cleepcli-1.9.0/cleepcli/console.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/git.py` & `cleepcli-1.9.0/cleepcli/git.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/distrib.py` & `cleepcli-1.9.0/cleepcli/distrib.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/config.py` & `cleepcli-1.9.0/cleepcli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-VERSION = '1.8.1'
+VERSION = '1.9.0'
 
 DEFAULT_MODULES = ['system', 'parameters', 'cleepbus', 'audio', 'network']
 MODULES_REPO_URL = {
     'system': 'https://github.com/tangb/cleepmod-system.git',
     'parameters': 'https://github.com/tangb/cleepmod-parameters.git',
     'cleepbus': 'https://github.com/tangb/cleepmod-cleepbus.git',
     'audio': 'https://github.com/tangb/cleepmod-audio.git',
```

### Comparing `cleepcli-1.8.1/cleepcli/cleepapi.py` & `cleepcli-1.9.0/cleepcli/cleepapi.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/cleepcli/test.py` & `cleepcli-1.9.0/cleepcli/test.py`

 * *Files identical despite different names*

### Comparing `cleepcli-1.8.1/bin/cleep-cli` & `cleepcli-1.9.0/bin/cleep-cli`

 * *Files 5% similar despite different names*

```diff
@@ -193,14 +193,27 @@
     """
     m = Module()
     res = m.create(module)
 
     if not res:
         sys.exit(1)
 
+@mod.command()
+@click.option('--module', prompt='Module name', help='Module name.')
+def moddelete(module):
+    """
+    Delete all installed files for specified module
+    """
+    if click.confirm('All installed files for module "%s" will be deleted. Confirm ?' % module):
+        m = Module()
+        res = m.delete(module)
+
+        if not res:
+            sys.exit(1)
+
 @click.group()
 def watchdog():
     pass
 
 @watchdog.command()
 @click.option('--quiet', is_flag=True, help='Disable logging.')
 @click.option('--loglevel', default=logging.INFO, help='Logging level (10=DEBUG, 20=INFO, 30=WARN, 40=ERROR).')
```

### Comparing `cleepcli-1.8.1/setup.py` & `cleepcli-1.9.0/setup.py`

 * *Files identical despite different names*

