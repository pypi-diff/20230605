# Comparing `tmp/datasette_dashboards-0.5.2.tar.gz` & `tmp/datasette_dashboards-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_dashboards-0.5.2.tar", max compression
+gzip compressed data, was "datasette_dashboards-0.5.3.tar", max compression
```

## Comparing `datasette_dashboards-0.5.2.tar` & `datasette_dashboards-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/LICENSE
--rw-r--r--   0        0        0    11777 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/README.md
--rw-r--r--   0        0        0     8184 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/datasette_dashboards/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/datasette_dashboards/py.typed
--rw-r--r--   0        0        0     1400 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/datasette_dashboards/static/dashboards.css
--rw-r--r--   0        0        0     6585 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/datasette_dashboards/static/dashboards.js
--rw-r--r--   0        0        0    64383 2023-05-02 20:15:51.935978 datasette_dashboards-0.5.2/datasette_dashboards/static/vega-embed.min.js
--rw-r--r--   0        0        0   244624 2023-05-02 20:15:51.939978 datasette_dashboards-0.5.2/datasette_dashboards/static/vega-lite.min.js
--rw-r--r--   0        0        0   510672 2023-05-02 20:15:51.943978 datasette_dashboards-0.5.2/datasette_dashboards/static/vega.min.js
--rw-r--r--   0        0        0     2292 2023-05-02 20:15:51.943978 datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_chart.html
--rw-r--r--   0        0        0      617 2023-05-02 20:15:51.943978 datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_list.html
--rw-r--r--   0        0        0     4999 2023-05-02 20:15:51.943978 datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_view.html
--rw-r--r--   0        0        0     1463 2023-05-02 20:15:51.955978 datasette_dashboards-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    12621 1970-01-01 00:00:00.000000 datasette_dashboards-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/LICENSE
+-rw-r--r--   0        0        0    11777 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/README.md
+-rw-r--r--   0        0        0     8275 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/datasette_dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/datasette_dashboards/py.typed
+-rw-r--r--   0        0        0     1400 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/datasette_dashboards/static/dashboards.css
+-rw-r--r--   0        0        0     6585 2023-06-05 07:20:35.354268 datasette_dashboards-0.5.3/datasette_dashboards/static/dashboards.js
+-rw-r--r--   0        0        0    64383 2023-06-05 07:20:35.358270 datasette_dashboards-0.5.3/datasette_dashboards/static/vega-embed.min.js
+-rw-r--r--   0        0        0   244624 2023-06-05 07:20:35.358270 datasette_dashboards-0.5.3/datasette_dashboards/static/vega-lite.min.js
+-rw-r--r--   0        0        0   510672 2023-06-05 07:20:35.362272 datasette_dashboards-0.5.3/datasette_dashboards/static/vega.min.js
+-rw-r--r--   0        0        0     2292 2023-06-05 07:20:35.362272 datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_chart.html
+-rw-r--r--   0        0        0      617 2023-06-05 07:20:35.362272 datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_list.html
+-rw-r--r--   0        0        0     4999 2023-06-05 07:20:35.362272 datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_view.html
+-rw-r--r--   0        0        0     1466 2023-06-05 07:20:35.374277 datasette_dashboards-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    12621 1970-01-01 00:00:00.000000 datasette_dashboards-0.5.3/PKG-INFO
```

### Comparing `datasette_dashboards-0.5.2/LICENSE` & `datasette_dashboards-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/README.md` & `datasette_dashboards-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/__init__.py` & `datasette_dashboards-0.5.3/datasette_dashboards/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,26 @@
     ) is False:
         raise Forbidden("execute-sql denied")
 
 
 async def fill_dynamic_filters(
     datasette: "Datasette", dashboard: t.Dict[str, t.Any]
 ) -> None:
-    for flt in dashboard.get("filters", {}).values():
+    for flt in dashboard["filters"].values():
         if flt["type"] == "select" and {"db", "query"} & flt.keys():
             values = [
                 row[0] for row in await datasette.execute(flt["db"], flt["query"])
             ]
             flt["options"] = values
 
 
 def get_dashboard_filters_keys(
     request: Request, dashboard: t.Dict[str, t.Any]
 ) -> t.Set[str]:
-    filters_keys = (dashboard.get("filters") or {}).keys()
+    filters_keys = dashboard["filters"].keys()
     return set(filters_keys) & set(request.args.keys())
 
 
 def get_dashboard_filters(request: Request, opts_keys: t.Set[str]) -> t.Dict[str, str]:
     return {key: request.args[key] for key in opts_keys}
 
 
@@ -111,14 +111,17 @@
     config = datasette.plugin_config("datasette-dashboards") or {}
     slug = urllib.parse.unquote(request.url_vars["slug"])
     try:
         dashboard = config[slug]
     except KeyError:
         raise NotFound(f"Dashboard not found: {slug}")
 
+    dashboard["filters"] = dashboard.get("filters", {})
+    dashboard["charts"] = dashboard.get("charts", {})
+
     settings = dashboard.get("settings", {})
     dbs = set([chart["db"] for chart in dashboard["charts"].values() if "db" in chart])
     for db in dbs:
         try:
             database = datasette.get_database(db)
         except KeyError:
             raise NotFound(f"Database does not exist: {db}")
```

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/static/dashboards.css` & `datasette_dashboards-0.5.3/datasette_dashboards/static/dashboards.css`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/static/dashboards.js` & `datasette_dashboards-0.5.3/datasette_dashboards/static/dashboards.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/static/vega-embed.min.js` & `datasette_dashboards-0.5.3/datasette_dashboards/static/vega-embed.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/static/vega-lite.min.js` & `datasette_dashboards-0.5.3/datasette_dashboards/static/vega-lite.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/static/vega.min.js` & `datasette_dashboards-0.5.3/datasette_dashboards/static/vega.min.js`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_chart.html` & `datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_chart.html`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_list.html` & `datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_list.html`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/datasette_dashboards/templates/dashboard_view.html` & `datasette_dashboards-0.5.3/datasette_dashboards/templates/dashboard_view.html`

 * *Files identical despite different names*

### Comparing `datasette_dashboards-0.5.2/pyproject.toml` & `datasette_dashboards-0.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasette-dashboards"
-version = "0.5.2"
+version = "0.5.3"
 description = "Datasette plugin providing data dashboards from metadata"
 repository = "https://github.com/rclement/datasette-dashboards"
 authors = ["Romain Clement"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "datasette_dashboards"}]
 
@@ -20,21 +20,21 @@
 [tool.poetry.group.dev.dependencies]
 black = "==23.3.0"
 datasette-block-robots = "==1.1"
 datasette-cluster-map = "==0.17.2"
 datasette-publish-vercel = "==0.14.2"
 datasette-sqlite-http = "==0.1.0a2"
 datasette-vega = "==0.6.2"
-faker = "==18.6.1"
+faker = "==18.10.1"
 flake8 = "==6.0.0"
-mypy = "==1.2.0"
+mypy = "==1.3.0"
 pytest = "==7.3.1"
 pytest-asyncio = "==0.21.0"
-pytest-cov = "==4.0.0"
-sqlite-utils = "==3.30"
+pytest-cov = "==4.1.0"
+sqlite-utils = "==3.32.1"
 
 [tool.poetry.plugins."datasette"]
 "dashboards" = "datasette_dashboards"
 
 [tool.mypy]
 show_error_codes = "True"
 pretty = "True"
```

### Comparing `datasette_dashboards-0.5.2/PKG-INFO` & `datasette_dashboards-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-dashboards
-Version: 0.5.2
+Version: 0.5.3
 Summary: Datasette plugin providing data dashboards from metadata
 Home-page: https://github.com/rclement/datasette-dashboards
 License: Apache License, Version 2.0
 Author: Romain Clement
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

