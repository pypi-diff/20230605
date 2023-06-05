# Comparing `tmp/s3manifestcollectstatic-0.1.0.tar.gz` & `tmp/s3manifestcollectstatic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3manifestcollectstatic-0.1.0.tar", max compression
+gzip compressed data, was "s3manifestcollectstatic-0.2.0.tar", max compression
```

## Comparing `s3manifestcollectstatic-0.1.0.tar` & `s3manifestcollectstatic-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2021-04-12 01:21:45.288248 s3manifestcollectstatic-0.1.0/LICENSE
--rw-r--r--   0        0        0      373 2021-04-12 01:27:22.125283 s3manifestcollectstatic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-12 01:28:45.037531 s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/__init__.py
--rw-r--r--   0        0        0      178 2021-04-12 01:28:45.037531 s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/apps.py
--rw-r--r--   0        0        0        0 2021-04-12 01:28:45.037531 s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/management/__init__.py
--rw-r--r--   0        0        0        0 2021-04-12 01:28:45.037531 s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/management/commands/__init__.py
--rw-r--r--   0        0        0     2655 2021-04-12 01:28:45.037531 s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py
--rw-r--r--   0        0        0      671 2021-04-12 01:31:47.085111 s3manifestcollectstatic-0.1.0/setup.py
--rw-r--r--   0        0        0      530 2021-04-12 01:31:47.085287 s3manifestcollectstatic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 17:27:56.865881 s3manifestcollectstatic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1323 2023-06-05 17:27:56.865964 s3manifestcollectstatic-0.2.0/README.md
+-rw-r--r--   0        0        0     1068 2023-06-05 19:48:56.575384 s3manifestcollectstatic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866271 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-05 17:27:56.866362 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/apps.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866439 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:56.866532 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/__init__.py
+-rw-r--r--   0        0        0     3430 2023-06-05 19:43:47.495074 s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 s3manifestcollectstatic-0.2.0/PKG-INFO
```

### Comparing `s3manifestcollectstatic-0.1.0/LICENSE` & `s3manifestcollectstatic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s3manifestcollectstatic-0.1.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py` & `s3manifestcollectstatic-0.2.0/s3manifestcollectstatic/management/commands/s3manifestcollectstatic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,95 @@
-from django.core.management.base import BaseCommand
-from django.core.management import call_command
-from django.conf import settings
-from django.utils.module_loading import import_string
-from tempfile import TemporaryDirectory
+import json
 from concurrent.futures import ThreadPoolExecutor
+from contextlib import contextmanager
 from pathlib import Path
-import json
+from tempfile import TemporaryDirectory
+
+from django import VERSION
+from django.conf import settings
+from django.contrib.staticfiles.storage import staticfiles_storage
+from django.core.management import call_command
+from django.core.management.base import BaseCommand
 
 MANIFEST_PATH = "staticfiles.json"
 
 
 class Command(BaseCommand):
     def log(self, msg, level=2):
         """
         Small log helper
         """
         if self.verbosity >= level:
             self.stdout.write(msg)
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '-f', '--force', action='store_true',
+            "-f",
+            "--force",
+            action="store_true",
             help="Force the reupload of files",
         )
 
-    def handle(self, *args, **options):
-        self.verbosity = options["verbosity"]
+    @staticmethod
+    @contextmanager
+    def override_storage_settings(static_root, staticfiles_storage):
+        saved_static_root = settings.STATIC_ROOT
+        settings.STATIC_ROOT = static_root
 
-        with TemporaryDirectory() as tmpdirname:
-            saved_static_root = settings.STATIC_ROOT
+        if VERSION < (4, 2) or settings.is_overridden("STATICFILES_STORAGE"):
             saved_storage = settings.STATICFILES_STORAGE
+            settings.STATICFILES_STORAGE = staticfiles_storage
+            yield
+            settings.STATICFILES_STORAGE = saved_storage
+        else:
+            saved_storage = settings.STORAGES
+            settings.STORAGES = {
+                **saved_storage,
+                "staticfiles": {
+                    "BACKEND": staticfiles_storage,
+                },
+            }
+            yield
+            settings.STORAGES = saved_storage
 
-            settings.STATIC_ROOT = tmpdirname
-            settings.STATICFILES_STORAGE = 'django.contrib.staticfiles.storage.ManifestStaticFilesStorage'
-
-            call_command("collectstatic")
+        settings.STATIC_ROOT = saved_static_root
 
-            settings.STATIC_ROOT = saved_static_root
-            settings.STATICFILES_STORAGE = saved_storage
+    def handle(self, *args, **options):
+        self.force = options["force"]
+        self.verbosity = options["verbosity"]
 
-            storage = import_string(saved_storage)()
+        with TemporaryDirectory() as tmpdirname:
+            with self.override_storage_settings(
+                tmpdirname,
+                staticfiles_storage="django.contrib.staticfiles.storage.ManifestStaticFilesStorage",
+            ):
+                call_command("collectstatic")
 
             manifest = Path(tmpdirname) / MANIFEST_PATH
-            with manifest.open('rb') as f:
+            with manifest.open("rb") as f:
                 to_upload = set(json.load(f)["paths"].values())
 
-            if storage.exists(MANIFEST_PATH):
-                with storage.open(MANIFEST_PATH) as f:
+            if staticfiles_storage.exists(MANIFEST_PATH):
+                with staticfiles_storage.open(MANIFEST_PATH) as f:
                     already_uploaded = set(json.load(f)["paths"].values())
                     intersection = to_upload.intersection(already_uploaded)
-                    self.log(f'{len(intersection)} files were already uploaded', level=1)
+                    self.log(f"{len(intersection)} files were already uploaded", level=1)
 
-                    if options["force"]:
+                    if self.force:
                         self.log("Forcing the reupload of files", level=1)
                     else:
                         to_upload.difference_update(already_uploaded)
 
             def _save_asset(path):
                 path_obj = Path(tmpdirname) / path
-                with path_obj.open('rb') as f:
-                    storage.save(path, f)
+                with path_obj.open("rb") as f:
+                    staticfiles_storage.save(path, f)
                 return path
 
-            self.log(f"Start upload of {len(to_upload)} files", level=1)
+            self.log(f"Start the upload of {len(to_upload)} files", level=1)
             with ThreadPoolExecutor() as executor:
                 for path in executor.map(_save_asset, to_upload):
-                    self.log(f'{path} was uploaded', level=2)
+                    self.log(f"{path} was uploaded", level=2)
 
             # Save manifest in the end when everything succeeded
             self.log("Uploading the manifest", level=1)
             _save_asset(MANIFEST_PATH)
```

