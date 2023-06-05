# Comparing `tmp/hansken-2023.5.1.tar.gz` & `tmp/hansken-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hansken-2023.5.1.tar", last modified: Mon May  1 09:18:09 2023, max compression
+gzip compressed data, was "hansken-2023.6.5.tar", last modified: Mon Jun  5 14:12:38 2023, max compression
```

## Comparing `hansken-2023.5.1.tar` & `hansken-2023.6.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.341517 hansken-2023.5.1/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-05-01 09:18:00.000000 hansken-2023.5.1/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-05-01 09:18:00.000000 hansken-2023.5.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-01 09:18:09.341517 hansken-2023.5.1/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-05-01 09:18:00.000000 hansken-2023.5.1/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-05-01 09:18:05.000000 hansken-2023.5.1/hansken/VERSION
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2358 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/abstract_trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/admin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    31922 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/auth.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/connect.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26374 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/query.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/export.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/report/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.333517 hansken-2023.5.1/hansken/recipes/report/templates/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken/recipes/report/templates/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/base.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/default.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/macros.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/print.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/recipes/report/templates/hansken/table.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   134425 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/remote.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.341517 hansken-2023.5.1/hansken/tool/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/_webhdfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_backup.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_extract.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_grant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_mount.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11094 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_quickstart.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_shell.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_stats.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_tasks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_tools.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_upload.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/tool/command_versions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59342 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-05-01 09:18:00.000000 hansken-2023.5.1/hansken/util.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-01 09:18:09.337517 hansken-2023.5.1/hansken.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      247 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-05-01 09:18:09.000000 hansken-2023.5.1/hansken.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-01 09:18:09.341517 hansken-2023.5.1/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1809 2023-05-01 09:18:00.000000 hansken-2023.5.1/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.562204 hansken-2023.6.5/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-06-05 14:12:29.000000 hansken-2023.6.5/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-06-05 14:12:29.000000 hansken-2023.6.5/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-06-05 14:12:38.558204 hansken-2023.6.5/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-06-05 14:12:29.000000 hansken-2023.6.5/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.554203 hansken-2023.6.5/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-06-05 14:12:34.000000 hansken-2023.6.5/hansken/VERSION
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2483 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/abstract_trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/admin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32028 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/auth.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/connect.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26374 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/query.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.558204 hansken-2023.6.5/hansken/recipes/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/export.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.558204 hansken-2023.6.5/hansken/recipes/report/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.550203 hansken-2023.6.5/hansken/recipes/report/templates/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.558204 hansken-2023.6.5/hansken/recipes/report/templates/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/templates/hansken/base.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/templates/hansken/default.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/templates/hansken/macros.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/templates/hansken/print.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/recipes/report/templates/hansken/table.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   134425 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/remote.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.558204 hansken-2023.6.5/hansken/tool/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/_webhdfs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_backup.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_extract.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_grant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_mount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11147 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_quickstart.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_shell.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_stats.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_tasks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_tools.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_upload.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/tool/command_versions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59342 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-06-05 14:12:29.000000 hansken-2023.6.5/hansken/util.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-05 14:12:38.554203 hansken-2023.6.5/hansken.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      299 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-06-05 14:12:38.000000 hansken-2023.6.5/hansken.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-05 14:12:38.562204 hansken-2023.6.5/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1876 2023-06-05 14:12:29.000000 hansken-2023.6.5/setup.py
```

### Comparing `hansken-2023.5.1/LICENSE` & `hansken-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/PKG-INFO` & `hansken-2023.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.5.1
+Version: 2023.6.5
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hansken-2023.5.1/README.md` & `hansken-2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/__init__.py` & `hansken-2023.6.5/hansken/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from pkg_resources import resource_string
+try:
+    from importlib.resources import files
+except ImportError:
+    # TODO: remove when hansken.py targets python >= 3.9
+    from importlib_resources import files
 
 
 try:
-    # read the resource VERSION as binary data to determine value for __version__
-    __version__ = resource_string(__name__, 'VERSION').decode('utf-8').strip()
+    # read installed package version from the package resource file "VERSION"
+    __version__ = (files(__name__) / 'VERSION').read_text(encoding='utf-8').strip()
 except Exception:
     __version__ = '0.0+unknown'
 
 
 class envvars:  # noqa: N801
     """
     `hansken.envvars` contains the names of all :ref:`environment variables
```

### Comparing `hansken-2023.5.1/hansken/abstract_trace.py` & `hansken-2023.6.5/hansken/abstract_trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/admin.py` & `hansken-2023.6.5/hansken/admin.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/auth.py` & `hansken-2023.6.5/hansken/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     Request the list of IDPs from remote, at ``base_url/saml/idps``.
 
     :param base_url: full url for the Hansken REST API
     :return: `dict` mapping IDP entity ids to the full IDP entry
     """
     idps = requests.get(glue_url(base_url, '/saml', '/idps'),
                         headers={'Accept': 'application/json'},
-                        verify=verify)
+                        verify=verify)  # nosec: B113 (currently not dealing with timeouts)
 
     if idps.status_code == codes.ok:
         return {idp.get('entityID'): idp for idp in idps.json()}
     elif idps.status_code == codes.not_found:
         # an allinone will simply not know about SAML, responding with a 404
         log.warn('remote does not understand SAML: {}: {}', idps.status_code, idps.reason)
         return {}
@@ -112,15 +112,15 @@
     idp_realm = idp_realm.group('realm') if idp_realm else None
 
     # probe the 'regular' login page to see whether we should be using Kerberos
     probe = glue_url(idp_url[:idp_url.index('/SSOSoap/')], '/UI', '/Login')
     log.info('probing OpenAM login URL {} (realm {})', probe, idp_realm)
     probe = requests.get(probe, params=omit_empty({
         'realm': idp_realm
-    }), allow_redirects=False, verify=verify)
+    }), allow_redirects=False, verify=verify)  # nosec: B113 (currently not dealing with timeouts)
 
     if probe.headers.get('WWW-Authenticate') == 'Negotiate':
         # idp wants us to use Kerberos, construct the info we need
         params = omit_empty({
             'realm': idp_realm,
             'module': 'WindowsDesktopSSO'
         })
```

### Comparing `hansken-2023.5.1/hansken/connect.py` & `hansken-2023.6.5/hansken/connect.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/query.py` & `hansken-2023.6.5/hansken/query.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/recipes/export.py` & `hansken-2023.6.5/hansken/recipes/export.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/recipes/report/__init__.py` & `hansken-2023.6.5/hansken/recipes/report/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/recipes/report/templates/hansken/base.html` & `hansken-2023.6.5/hansken/recipes/report/templates/hansken/base.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/recipes/report/templates/hansken/macros.html` & `hansken-2023.6.5/hansken/recipes/report/templates/hansken/macros.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/remote.py` & `hansken-2023.6.5/hansken/remote.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/__init__.py` & `hansken-2023.6.5/hansken/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/_webhdfs.py` & `hansken-2023.6.5/hansken/tool/_webhdfs.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_backup.py` & `hansken-2023.6.5/hansken/tool/command_backup.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_extract.py` & `hansken-2023.6.5/hansken/tool/command_extract.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_grant.py` & `hansken-2023.6.5/hansken/tool/command_grant.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_mount.py` & `hansken-2023.6.5/hansken/tool/command_mount.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_quickstart.py` & `hansken-2023.6.5/hansken/tool/command_quickstart.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
               '(this typically ends with "/gatekeeper")')
         args.endpoint = prompt('Hansken REST API endpoint')
 
     log.info('endpoint to be used: {}', args.endpoint)
 
     if args.endpoint.startswith('https'):
         try:
-            requests.get(args.endpoint, verify=True)
+            requests.get(args.endpoint, verify=True)  # nosec: B113 (currently not dealing with timeouts)
             # no error from requests, verify can be left/set at True
             args.verify = True
         except SSLError:
             print('it seems the REST API endpoint at {} uses an invalid certificate'.format(args.endpoint))
             args.verify = confirm('certificate verification', value=False, fallback=True)
 
     print()
```

### Comparing `hansken-2023.5.1/hansken/tool/command_shell.py` & `hansken-2023.6.5/hansken/tool/command_shell.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_stats.py` & `hansken-2023.6.5/hansken/tool/command_stats.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_tasks.py` & `hansken-2023.6.5/hansken/tool/command_tasks.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_tools.py` & `hansken-2023.6.5/hansken/tool/command_tools.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_upload.py` & `hansken-2023.6.5/hansken/tool/command_upload.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/tool/command_versions.py` & `hansken-2023.6.5/hansken/tool/command_versions.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/trace.py` & `hansken-2023.6.5/hansken/trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken/util.py` & `hansken-2023.6.5/hansken/util.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/hansken.egg-info/PKG-INFO` & `hansken-2023.6.5/hansken.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.5.1
+Version: 2023.6.5
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hansken-2023.5.1/hansken.egg-info/SOURCES.txt` & `hansken-2023.6.5/hansken.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hansken-2023.5.1/setup.py` & `hansken-2023.6.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     version_string = version.read().strip()
 
 with open(path.join(here, 'README.md')) as readme:
     long_description = readme.read()
 
 dependencies = ['decorator',
                 'ijson>=3.1',
+                'importlib-resources>=1.3 ; python_version<"3.9"',
                 'iso8601',
                 'logbook>=1.0',
                 'more-itertools',
                 'python-dateutil',
                 'requests>=2.7.0',
                 'tabulate']
```

