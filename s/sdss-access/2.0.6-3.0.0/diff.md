# Comparing `tmp/sdss-access-2.0.6.tar.gz` & `tmp/sdss-access-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-access-2.0.6.tar", last modified: Fri Jun  2 14:11:18 2023, max compression
+gzip compressed data, was "dist/sdss-access-3.0.0.tar", last modified: Mon Jun  5 18:55:13 2023, max compression
```

## Comparing `sdss-access-2.0.6.tar` & `sdss-access-3.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-02 14:11:05.000000 sdss-access-2.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 14:11:05.000000 sdss-access-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-02 14:11:18.000000 sdss-access-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-02 14:11:05.000000 sdss-access-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/etc/sdss_access.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/misc/docupaths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/path/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/baseaccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/system_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 14:11:18.000000 sdss-access-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 14:11:05.000000 sdss-access-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-05 18:55:00.000000 sdss-access-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 18:55:00.000000 sdss-access-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-05 18:55:13.000000 sdss-access-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-05 18:55:00.000000 sdss-access-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/etc/sdss_access.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/misc/docupaths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access/path/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/path/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49658 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/path/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/baseaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-06-05 18:55:00.000000 sdss-access-3.0.0/python/sdss_access/sync/system_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-05 18:55:12.000000 sdss-access-3.0.0/python/sdss_access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-05 18:55:13.000000 sdss-access-3.0.0/python/sdss_access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:55:12.000000 sdss-access-3.0.0/python/sdss_access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:55:12.000000 sdss-access-3.0.0/python/sdss_access.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 18:55:12.000000 sdss-access-3.0.0/python/sdss_access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 18:55:12.000000 sdss-access-3.0.0/python/sdss_access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-05 18:55:13.000000 sdss-access-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 18:55:00.000000 sdss-access-3.0.0/setup.py
```

### Comparing `sdss-access-2.0.6/LICENSE.md` & `sdss-access-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/__init__.py` & `sdss-access-3.0.0/python/sdss_access/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,13 +22,12 @@
 log.debug("SDSS_ACCESS> Using {0}".format(tree))
 
 
 # Loads config
 config = get_config(NAME)
 
 
-#__version__ = '1.0.0dev'
 __version__ = get_package_version(path=__file__, package_name=NAME)
 
 
-from .path import Path as SDSSPath, AccessError
+from .path import Path, AccessError
 from .sync import HttpAccess, Access, BaseAccess, RsyncAccess, CurlAccess
```

### Comparing `sdss-access-2.0.6/python/sdss_access/misc/docupaths.py` & `sdss-access-3.0.0/python/sdss_access/misc/docupaths.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/path/changelog.py` & `sdss-access-3.0.0/python/sdss_access/path/changelog.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         to_list (bool):
             If True, returns a list of strings formatted for printing. Default is False.
 
     Returns:
         A dictionary of relevant changes between the two releases
     '''
 
-    diffs = compute_path_changes(new, old, pprint=pprint, paths_only=True, to_list=to_list)
-
-    return diffs
+    return compute_path_changes(new, old, pprint=pprint, paths_only=True, to_list=to_list)
 
 
 def get_path_templates(name, public=None):
     ''' Return the path templates for all releases
 
     Produces a dictionary of path templates for a given
     path name for all releases.  Set public keyword to toggle only
@@ -62,15 +60,15 @@
     Returns:
         A dictionary of the path template per release
     '''
     releases = Tree.get_available_releases(public=public)
     versions = {}
     for release in reversed(releases):
         release = 'sdsswork' if 'WORK' in release else release
-        tree = Tree(config=release)
+        tree = Tree(config=release.lower())
         versions[release] = tree.paths.get(name, None)
     return versions
 
 
 def get_available_releases(public=None):
     ''' Get the available releases
```

### Comparing `sdss-access-2.0.6/python/sdss_access/path/path.py` & `sdss-access-3.0.0/python/sdss_access/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     ----------
     templates : dict
         The set of templates read from the configuration file.
     """
 
     _netloc = {"dtn": "dtn.sdss.org", "sdss": "data.sdss.org", "sdss5": "data.sdss5.org",
                "mirror": "data.mirror.sdss.org", "svn": "svn.sdss.org"}
-    _s5cfgs = ['sdss5', 'ipl1']  # list of collab-only SDSS-V releases/configs
+    _s5cfgs = ['sdsswork', 'sdss5', 'ipl1']  # list of collab-only SDSS-V releases/configs
 
     def __init__(self, release=None, public=False, mirror=False, verbose=False,
                  force_modules=None, preserve_envvars=None):
         # set release
         self.release = release or os.getenv('TREE_VER', 'sdsswork')
         self.verbose = verbose
         self.force_modules = force_modules or config.get('force_modules')
@@ -203,18 +203,24 @@
             return keys
 
         # loop over special method names and extract keywords
         for function in functions:
             method = getattr(self, function[1:-1])
             # get source code of special method
             source = self._find_source(method)
-            fkeys = re.findall(r'kwargs\[(.*?)\]', source)
+
+            # matches on kwargs.get("xxx"), kwargs.get("xxx", None), or kwargs["xxx"]
+            # on either single or double quoted string, with or without a default value
+            patt = r"kwargs.get\(\W(\w+)\W,*\s*.*\)|kwargs\[\W(\w+)\W\]"
+            fkeys = re.findall(patt, source)
+
             if fkeys:
-                # evaluate to proper string
-                fkeys = [ast.literal_eval(k) for k in fkeys]
+                # condense gorups down to proper string list
+                fkeys = [str(i) for k in fkeys for i in k if i]
+
                 keys.extend(fkeys)
         return keys
 
     @staticmethod
     def _find_source(method):
         ''' find source code of a given method
 
@@ -1238,15 +1244,17 @@
             A set of folders.
         '''
         # with k = 100 then even with 10 M sources, each folder will have ~1,000 files
         k = 100
         if 'cat_id' in kwargs:
             cat_id = int(kwargs['cat_id'])
         elif 'catid' in kwargs:
-            cat_id = int(kwargs['catid'])
+            # removing the undesired version as this messes up the lookup_keys method
+            kwargs['cat_id'] = kwargs.pop('catid')
+            cat_id = int(kwargs['cat_id'])
         return f"{(cat_id // k) % k:0>2.0f}/{cat_id % k:0>2.0f}"
 
     def component_default(self, filetype, **kwargs):
         ''' Return the component name, if given.
 
         The component designates a stellar or planetary body following the
         Washington Multiplicity Catalog, which was adopted by the XXIV meeting
@@ -1295,22 +1303,27 @@
         Returns
         -------
         prefix : str
             The APOGEE prefix (ap/as).
 
         '''
 
-        telescope = kwargs.get('telescope', None)
+        # since telescope or instrument already defined in the main
+        # template for all paths, we rename the kwargs dict so these keywords
+        # do not get picked up by the lookup_keys method.
+        newkw = kwargs.copy()
+
+        telescope = newkw.get('telescope', None)
         if telescope is not None:
             prefix = {'apo25m': 'ap', 'apo1m': 'ap', 'lco25m': 'as'}
             if telescope not in prefix:
                 raise ValueError(f'{telescope} not in allowed list of prefixes')
             return prefix[telescope]
 
-        instrument = kwargs.get('instrument', None)
+        instrument = newkw.get('instrument', None)
         if instrument is not None:
             prefix = {'apogee-n': 'ap', 'apogee-s': 'as'}
             if instrument not in prefix:
                 raise ValueError(f'{instrument} not in allowed list of prefixes')
             return prefix[instrument]
 
         return ''
```

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/access.py` & `sdss-access-3.0.0/python/sdss_access/sync/access.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/auth.py` & `sdss-access-3.0.0/python/sdss_access/sync/auth.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/baseaccess.py` & `sdss-access-3.0.0/python/sdss_access/sync/baseaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 # The line above will help with 2to3 support.
 
 import abc
 import six
 from os.path import join, sep
-from sdss_access import SDSSPath
+from sdss_access import Path
 from sdss_access.sync.auth import Auth, AuthMixin
 from sdss_access.sync.stream import Stream
 from sdss_access import is_posix, AccessError
 
 
-class BaseAccess(six.with_metaclass(abc.ABCMeta, AuthMixin, SDSSPath)):
+class BaseAccess(six.with_metaclass(abc.ABCMeta, AuthMixin, Path)):
     """Class for providing Rsync or Curl access to SDSS SAS Paths
     """
     remote_scheme = None
     access_mode = 'rsync' if is_posix else 'curl'
 
     def __init__(self, label=None, stream_count=5, mirror=False, public=False, release=None,
                  verbose=False, force_modules=None, preserve_envvars=None):
```

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/cli.py` & `sdss-access-3.0.0/python/sdss_access/sync/cli.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/curl.py` & `sdss-access-3.0.0/python/sdss_access/sync/curl.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/http.py` & `sdss-access-3.0.0/python/sdss_access/sync/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     from urllib2 import HTTPError
 except:
     from urllib.request import HTTPPasswordMgrWithDefaultRealm, HTTPBasicAuthHandler, build_opener, install_opener, urlopen
     from urllib.error import HTTPError
 
 from os import makedirs
 from os.path import isfile, exists, dirname
-from sdss_access import SDSSPath
+from sdss_access import Path
 from sdss_access.sync.auth import Auth, AuthMixin
 from tqdm import tqdm
 
 
-class HttpAccess(AuthMixin, SDSSPath):
+class HttpAccess(AuthMixin, Path):
     """Class for providing HTTP access via urllib.request (python3) or urllib2 (python2) to SDSS SAS Paths
     """
 
     def __init__(self, verbose=None, public=None, release=None, label='sdss_http'):
         super(HttpAccess, self).__init__(public=public, release=release, verbose=verbose)
         self.verbose = verbose
         self.label = label
```

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/rsync.py` & `sdss-access-3.0.0/python/sdss_access/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/stream.py` & `sdss-access-3.0.0/python/sdss_access/sync/stream.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access/sync/system_call.py` & `sdss-access-3.0.0/python/sdss_access/sync/system_call.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access.egg-info/SOURCES.txt` & `sdss-access-3.0.0/python/sdss_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.6/python/sdss_access.egg-info/requires.txt` & `sdss-access-3.0.0/python/sdss_access.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 six>=1.11
 requests>=2.10.0
-sdss-tree<4.0.0,>=3.1.2
+sdss-tree>=4.0.0
 sdsstools>=0.4.5
 tqdm>=4.46.0
 
 [dev]
 Sphinx>=2.1.0
 sphinx_bootstrap_theme>=0.4.12
 recommonmark>=0.6
```

### Comparing `sdss-access-2.0.6/setup.cfg` & `sdss-access-3.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-access
-version = 2.0.6
+version = 3.0.0
 author = Brian Cherinka
 author_email = bcherinka@stsci.edu
 description = Package to dynamically build filepaths and access all SDSS SAS products
 url = https://github.com/sdss/sdss_access
 project_urls = 
 	Repository = https://github.com/sdss/sdss_access
 	Documentation = https://sdss-access.readthedocs.org
@@ -30,15 +30,15 @@
 python_requires = >=3.6
 packages = find:
 package_dir = 
 	= python
 install_requires = 
 	six>=1.11
 	requests>=2.10.0
-	sdss-tree>=3.1.2,<4.0.0
+	sdss-tree>=4.0.0
 	sdsstools>=0.4.5
 	tqdm>=4.46.0
 scripts = 
 
 [options.packages.find]
 where = 
 	python
@@ -97,23 +97,24 @@
 	W504
 	W505
 per-file-ignores = 
 	*/__init__.py:E,W
 max-line-length = 99
 
 [tool:pytest]
-addopts = --cov sdss_access --cov-report html -W ignore
+addopts = --cov sdss_access --cov-report xml --cov-report html --cov-report term -W ignore
 
 [coverage:run]
 branch = true
 include = 
 	python/sdss_access/*
 omit = 
 	*/utils/*.py
 	*/__init__.py
+	*/sync/system_call.py
 
 [coverage:report]
 exclude_lines = 
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

