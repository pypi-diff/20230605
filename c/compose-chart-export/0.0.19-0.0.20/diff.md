# Comparing `tmp/compose_chart_export-0.0.19-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13357 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-30 12:37 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-May-30 12:37 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14564 b- defN 23-May-30 12:37 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4974 b- defN 23-May-30 12:37 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2285 b- defN 23-May-30 12:37 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9604 b- defN 23-May-30 12:37 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2365 b- defN 23-May-30 12:37 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-30 12:37 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      626 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/RECORD
-13 files, 38370 bytes uncompressed, 11301 bytes compressed:  70.5%
+Zip file size: 13386 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 06:58 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-05 06:58 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14564 b- defN 23-Jun-05 06:58 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4974 b- defN 23-Jun-05 06:58 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jun-05 06:58 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9602 b- defN 23-Jun-05 06:58 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Jun-05 06:58 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 06:58 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      626 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-Jun-05 06:58 compose_chart_export-0.0.20.dist-info/RECORD
+13 files, 38437 bytes uncompressed, 11330 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.19.dist-info/METADATA
+Filename: compose_chart_export-0.0.20.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.19.dist-info/WHEEL
+Filename: compose_chart_export-0.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.19.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.20.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.19.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.19.dist-info/RECORD
+Filename: compose_chart_export-0.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/chart_export.py

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from pathlib import Path
 from typing import Callable, Dict, List, Optional
 
 from compose_chart_export.chart_file_templates import (
     ChartTemplateSpec,
     chart_yaml,
     daemonset_yaml,
@@ -41,15 +42,16 @@
 
 
 def _export_chart(
     spec: ChartTemplateSpec,
     chart_path: Path,
     skip_generators: Optional[List[str]] = None,
 ) -> Path:
-    clean_dir(chart_path)
+    if chart_path.is_dir() and os.listdir(chart_path):
+        clean_dir(chart_path)
     skip_generators = skip_generators or []
     for rel_path, content_generator in PATH_TO_GENERATORS.items():
         if rel_path in skip_generators:
             continue
         dest = chart_path / rel_path
         if content := content_generator(spec):
             ensure_parents_write_text(dest, content)
```

## compose_chart_export/compose_export.py

```diff
@@ -122,22 +122,22 @@
     >>> ensure_chart_version_valid("v0.0.1")
     'v0.0.1'
     >>> ensure_chart_version_valid("latest-amd")
     '0.0.1-latest-amd'
     """
     check_version = chart_version if chart_version[0].isdigit() else chart_version[1:]
     try:
-        semver.parse_version_info(check_version)
+        semver.VersionInfo.parse(check_version)
         return chart_version
     except ValueError:
         updated_version = f"0.0.1-{chart_version}"
         logger.warning(
             f"not a valid semver: {chart_version}, will try: {updated_version}"
         )
-    semver.parse_version_info(updated_version)
+    semver.VersionInfo.parse(updated_version)
     return updated_version
 
 
 def export_from_compose(
     compose_path: PathLike,
     chart_version: str,
     chart_name: str = "",
```

## Comparing `compose_chart_export-0.0.19.dist-info/METADATA` & `compose_chart_export-0.0.20.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.19
+Version: 0.0.20
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.18)
-Requires-Dist: model-lib (==0.0.18)
+Requires-Dist: docker-compose-parser (==0.0.20)
+Requires-Dist: model-lib (==0.0.20)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: semver (==2.13.0)
 Requires-Dist: typing-extensions (>=4.3.0)
-Requires-Dist: zero-3rdparty (==0.0.18)
+Requires-Dist: zero-3rdparty (==0.0.20)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.19.dist-info/RECORD` & `compose_chart_export-0.0.20.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-compose_chart_export/chart_export.py,sha256=tg2QiDVn29_Uic_3WPKWkaAhMMN3HQ6jALSG8-Lfv-s,2448
+compose_chart_export/chart_export.py,sha256=lRtxzU3Ac2SfOAxZmSv9ml0KsDM4tHx5ois0BOFF9dc,2517
 compose_chart_export/chart_file_templates.py,sha256=sQMgnbhaCgppTOO5XZD72YbshNJS90INvCENukeNY3w,14564
 compose_chart_export/chart_mods.py,sha256=6eaO7tuccQWcZDc_yoi3p7aIOO2YQ4vAb2aqKZ5qBzc,4974
 compose_chart_export/chart_read.py,sha256=5A7mcFdq1lnD7fitj5-evHE9A0zJ6aAlY0KEYPmeRZo,2285
-compose_chart_export/compose_export.py,sha256=zCMO0r4-9ZwaVPNmcadu6F5lvzF0wMP7Hb_7PZ8tLZI,9604
+compose_chart_export/compose_export.py,sha256=9CLgDO88kYyR55TcHxhGsgaA4xbyj2f-mSXINYRP55w,9602
 compose_chart_export/ports.py,sha256=ubPaqe31gwDqPj8s4Bd6pZf8qB02hylpoQpYpbFkYwc,2365
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.19.dist-info/METADATA,sha256=OcL4cu7dYQGY2yhneG4qyYKdARwVZzRqJpD7OnrINuc,626
-compose_chart_export-0.0.19.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.19.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.19.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.19.dist-info/RECORD,,
+compose_chart_export-0.0.20.dist-info/METADATA,sha256=nuys7GXtj31MjHpzgOic_SVIOhYUMSPmEkV1NNUQfL0,626
+compose_chart_export-0.0.20.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.20.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.20.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.20.dist-info/RECORD,,
```

