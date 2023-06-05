# Comparing `tmp/dbt_core_interface-0.2.3.tar.gz` & `tmp/dbt_core_interface-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_core_interface-0.2.3.tar", max compression
+gzip compressed data, was "dbt_core_interface-0.2.4.tar", max compression
```

## Comparing `dbt_core_interface-0.2.3.tar` & `dbt_core_interface-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-04-02 03:00:55.882700 dbt_core_interface-0.2.3/LICENSE
--rw-r--r--   0        0        0     4400 2023-04-02 03:00:55.886700 dbt_core_interface-0.2.3/README.md
--rw-r--r--   0        0        0     2512 2023-04-02 03:01:09.638857 dbt_core_interface-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       87 2023-04-02 03:00:55.894700 dbt_core_interface-0.2.3/src/dbt_core_interface/__init__.py
--rw-r--r--   0        0        0   239099 2023-04-02 03:00:55.894700 dbt_core_interface-0.2.3/src/dbt_core_interface/project.py
--rw-r--r--   0        0        0     5202 1970-01-01 00:00:00.000000 dbt_core_interface-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:48:37.883155 dbt_core_interface-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4964 2023-06-05 06:48:37.883155 dbt_core_interface-0.2.4/README.md
+-rw-r--r--   0        0        0     2622 2023-06-05 06:48:52.743024 dbt_core_interface-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-05 06:48:37.895155 dbt_core_interface-0.2.4/src/dbt_core_interface/__init__.py
+-rw-r--r--   0        0        0     1214 2023-06-05 06:48:37.895155 dbt_core_interface-0.2.4/src/dbt_core_interface/dbt_templater/LICENSE.md
+-rw-r--r--   0        0        0      700 2023-06-05 06:48:37.895155 dbt_core_interface-0.2.4/src/dbt_core_interface/dbt_templater/__init__.py
+-rw-r--r--   0        0        0     9050 2023-06-05 06:48:37.895155 dbt_core_interface-0.2.4/src/dbt_core_interface/dbt_templater/templater.py
+-rw-r--r--   0        0        0   229322 2023-06-05 06:48:37.899155 dbt_core_interface-0.2.4/src/dbt_core_interface/project.py
+-rw-r--r--   0        0        0     4553 2023-06-05 06:48:37.899155 dbt_core_interface-0.2.4/src/dbt_core_interface/sqlfluff_util.py
+-rw-r--r--   0        0        0       29 2023-06-05 06:48:37.899155 dbt_core_interface-0.2.4/src/dbt_core_interface/state.py
+-rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 dbt_core_interface-0.2.4/PKG-INFO
```

### Comparing `dbt_core_interface-0.2.3/LICENSE` & `dbt_core_interface-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_core_interface-0.2.3/README.md` & `dbt_core_interface-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 - Run SQL and get results in python fully independent of the dbt adapter which automatically enables support for many databases
 
 - Run SQL with dbt SQL from a single method call
 
 - Load macros at runtime enabling custom functionality in third party extensions without requiring the dbt packaging system to be managed in userland
 
-- Compile dbt jinja extremely fast and efficiently, thread-safe and stress tested at load via a fastapi server which live compiles SQL
+- Compile dbt jinja extremely fast and efficiently, thread-safe and stress tested at load via a Bottle server which live compiles SQL
 
 - Manage multiple dbt projects in a single process using the DbtProjectContainer class
 
 `dbt-core-interface` is a wrapper that allows developers to rapidly develop features and integrations for dbt. This project aims to serve as a place for the community to aggregate the best ways to interface with dbt. It is afforded a much faster iteration cycle and much more freedom due to it's independence from the dbt codebase. It is intended to act as an common library to dbt's existing APIs for developers. Implementations can land here and prove themselves out before landing in the dbt-core codebase and benefit all developers involved. Sqlfluff dbt templater, dbt-osmosis, dbt-fastapi which I am ripping out of dbt-osmosis, an impending metadata manager, a testing framework will all leverage this library. As dbt core evolves and stabilizes its python API, this project will evolve with it. This may manifest in simplification of certain methods but our goal is to maintain the API and focus on driving efficient, innovative/creative, and agile community driven integration patterns.
 
 ## Requirements
 
@@ -52,14 +52,24 @@
 $ pip install dbt-core-interface
 ```
 
 ## Usage
 
 Please see the [Api Reference] for details.
 
+To launch the Bottle server for live compiling dbt jinja:
+
+    python -m dbt_core_interface.project
+
+This will launch the server on port 8581. You can then make requests to the server, e.g.:
+
+    curl -X POST -H "Content-Type: application/json" -H "X-dbt-Project: dbt_project" -d '{"project_dir":"/app/tests/sqlfluff_templater/fixtures/dbt/dbt_project/","profiles_dir":"/app/tests/sqlfluff_templater/fixtures/dbt/profiles_yml/","target":"dev"}' http://localhost:8581/register
+
+You can change the server hostname and port using the `--host` and `--port` arguments.
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `dbt_core_interface-0.2.3/pyproject.toml` & `dbt_core_interface-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-core-interface"
-version = "0.2.3"
+version = "0.2.4"
 description = "Dbt Core Interface"
 authors = ["Alex Butler <butler.alex2010@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/z3z1ma/dbt-core-interface"
 repository = "https://github.com/z3z1ma/dbt-core-interface"
 documentation = "https://dbt-core-interface.readthedocs.io"
@@ -68,14 +68,19 @@
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 disallow_untyped_calls = false
 exclude = ["noxfile.py", "dbt_core_interface.py"]
 
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."sqlfluff"]
+"dbt_templater" = "dbt_core_interface.dbt_templater"
+
 [tool.ruff]
 line-length = 100
 select = ["B", "B9", "C", "D", "E", "F", "N", "S", "W"]
 ignore = ["E501", "D203", "D213"]
 exclude = [
     ".bzr",
     ".direnv",
```

### Comparing `dbt_core_interface-0.2.3/src/dbt_core_interface/project.py` & `dbt_core_interface-0.2.4/src/dbt_core_interface/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import configparser
 import decimal
 import email.utils
 import functools
 import hashlib
 import hmac
 import http.client as httplib
+import importlib
 import itertools
 import json
 import logging
 import mimetypes
 import os
 import pickle
 import re
@@ -112,14 +113,21 @@
     from agate import Table  # type: ignore  # No stubs for agate
     from dbt.adapters.base import BaseAdapter, BaseRelation  # type: ignore
     from dbt.contracts.connection import AdapterResponse
     from dbt.contracts.results import ExecutionResult, RunExecutionResult
     from dbt.semver import VersionSpecifier
     from dbt.task.runnable import ManifestTask
 
+try:
+    import dbt_core_interface.state as dci_state
+    from dbt_core_interface.sqlfluff_util import lint_command
+except ImportError:
+    dci_state = None
+    lint_command = None
+
 # dbt-core-interface is designed for non-standard use. There is no
 # reason to track usage of this package.
 disable_tracking()
 
 urlunquote = functools.partial(urlunquote, encoding="latin1")
 
 # Version specific dbt constants and overrides
@@ -200,15 +208,14 @@
     "ServerCompileResult",
     "ServerResetResult",
     "ServerRegisterResult",
     "ServerUnregisterResult",
     "ServerErrorCode",
     "ServerError",
     "ServerErrorContainer",
-    "ServerPlugin",
     "run_server",
     "default_project_dir",
     "default_profiles_dir",
     "ColumnInfo",
     "ManifestNode",
 ]
 
@@ -1022,14 +1029,17 @@
     dbt projects in a single process. It enables basic multitenant servers.
     """
 
     def __init__(self) -> None:
         """Initialize the container."""
         self._projects: Dict[str, DbtProject] = OrderedDict()
         self._default_project: Optional[str] = None
+        if dci_state is not None:
+            assert dci_state.dbt_project_container is None
+            dci_state.dbt_project_container = self
 
     def get_project(self, project_name: str) -> Optional[DbtProject]:
         """Primary interface to get a project and execute code."""
         return self._projects.get(project_name)
 
     def get_project_by_root_dir(self, root_dir: str) -> Optional[DbtProject]:
         """Get a project by its root directory."""
@@ -5710,14 +5720,15 @@
 
     FailedToReachServer = -1
     CompileSqlFailure = 1
     ExecuteSqlFailure = 2
     ProjectParseFailure = 3
     ProjectNotRegistered = 4
     ProjectHeaderNotSupplied = 5
+    MissingRequiredParams = 6
 
 
 @dataclass
 class ServerError:
     """An error that can be serialized to JSON."""
 
     code: ServerErrorCode
@@ -6024,24 +6035,38 @@
             )
         )
     if project in runners:
         # Idempotent
         return asdict(ServerRegisterResult(added=project, projects=runners.registered_projects()))
 
     # Inputs
-    project_dir = request.json["project_dir"]
-    profiles_dir = request.json["profiles_dir"]
-    target = request.json.get("target")
+    kwargs = {}
+    params = {}
+    if request.query:
+        params.update(dict(request.query.decode()))
+    if request.json:
+        params.update(dict(request.json))
+    kwargs.setdefault("project_dir", params.get("project-dir") or params.get("project_dir"))
+    kwargs.setdefault("profiles_dir", params.get("profiles-dir") or params.get("profiles_dir"))
+    kwargs.setdefault("target", params.get("target"))
+    for k in ("project_dir",):
+        if kwargs.get(k) is None:
+            response.status = 400
+            return asdict(
+                ServerErrorContainer(
+                    error=ServerError(
+                        code=ServerErrorCode.MissingRequiredParams,
+                        message=f"Missing required parameter {k}",
+                        data=dict(request.headers),
+                    )
+                )
+            )
 
     try:
-        new_runner = DbtProject(
-            project_dir=project_dir,
-            profiles_dir=profiles_dir,
-            target=target,
-        )
+        new_runner = DbtProject(**kwargs)
     except Exception as init_err:
         return asdict(
             ServerErrorContainer(
                 error=ServerError(
                     code=ServerErrorCode.ProjectParseFailure,
                     message=str(init_err),
                     data=init_err.__dict__,
@@ -6087,177 +6112,14 @@
                 )
             )
         )
     runners.drop_project(project)
     return asdict(ServerUnregisterResult(removed=project, projects=runners.registered_projects()))
 
 
-@route("/v1/info", methods="GET")
-def trino_info(runners: DbtProjectContainer):
-    """Trino info endpoint."""
-    return {
-        "coordinator": {},
-        "workers": [],
-        "memory": {},
-        "jvm": {},
-        "system": {},
-    }
-
-
-# TODO: These are here while we map agate types to trino types.
-# public final class ClientStandardTypes
-# {
-#     public static final String BIGINT = "bigint";
-#     public static final String INTEGER = "integer";
-#     public static final String SMALLINT = "smallint";
-#     public static final String TINYINT = "tinyint";
-#     public static final String BOOLEAN = "boolean";
-#     public static final String DATE = "date";
-#     public static final String DECIMAL = "decimal";
-#     public static final String REAL = "real";
-#     public static final String DOUBLE = "double";
-#     public static final String HYPER_LOG_LOG = "HyperLogLog";
-#     public static final String QDIGEST = "qdigest";
-#     public static final String P4_HYPER_LOG_LOG = "P4HyperLogLog";
-#     public static final String INTERVAL_DAY_TO_SECOND = "interval day to second";
-#     public static final String INTERVAL_YEAR_TO_MONTH = "interval year to month";
-#     public static final String TIMESTAMP = "timestamp";
-#     public static final String TIMESTAMP_WITH_TIME_ZONE = "timestamp with time zone";
-#     public static final String TIME = "time";
-#     public static final String TIME_WITH_TIME_ZONE = "time with time zone";
-#     public static final String VARBINARY = "varbinary";
-#     public static final String VARCHAR = "varchar";
-#     public static final String CHAR = "char";
-#     public static final String ROW = "row";
-#     public static final String ARRAY = "array";
-#     public static final String MAP = "map";
-#     public static final String JSON = "json";
-#     public static final String IPADDRESS = "ipaddress";
-#     public static final String UUID = "uuid";
-#     public static final String GEOMETRY = "Geometry";
-#     public static final String SPHERICAL_GEOGRAPHY = "SphericalGeography";
-#     public static final String BING_TILE = "BingTile";
-#     private ClientStandardTypes() {}
-# }
-
-# TODO: This is just a note to acknowledge that we cannot use the default trino catalog
-# yet some integrations may expect this type of query to succeed.
-# select schema_name AS label,
-# schema_name AS schema,
-# 'connection.schema' as type,
-# 'group-by-ref-type' as iconId,
-# '<catalog>' as database
-# from <catalog>.information_schema.schemata
-
-
-@route("/v1/statement", method="POST")
-def trino_statement(runners: DbtProjectContainer):
-    """Trino statement endpoint.
-
-    This endpoint is used to execute queries and return the results.
-    It is very minimal right now. The only purpose is to proxy SELECT queries
-    to dbt from a JDBC and return the results to the JDBC.
-    """
-    from agate import data_types
-
-    # User Support
-    _user = request.headers.get("X-Presto-User", "default")
-    # Project Support
-    project_runner = (
-        runners.get_project(request.get_header("X-dbt-Project")) or runners.get_default_project()
-    )
-    if not project_runner:
-        return {
-            "errorName": "ProjectNotRegistered",
-            "errorType": "USER_ERROR",
-            "errorLocation": {"lineNumber": 1, "columnNumber": 1},
-            "error": "Project is not registered. Make a POST request to the /register endpoint",
-        }
-    query = request.body.read().decode("utf-8")
-    res = project_runner.execute_code(query)
-    columns = []
-    for column in res.table.columns:
-        if isinstance(column.data_type, data_types.Text):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "varchar",
-                    "typeSignature": {
-                        "rawType": "varchar",
-                        "arguments": [{"kind": "LONG_LITERAL", "value": 255}],
-                    },
-                }
-            ]
-        elif isinstance(column.data_type, data_types.Number):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "bigint",
-                    "typeSignature": {"rawType": "bigint", "arguments": []},
-                }
-            ]
-        elif isinstance(column.data_type, data_types.Boolean):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "boolean",
-                    "typeSignature": {"rawType": "boolean", "arguments": []},
-                }
-            ]
-        elif isinstance(column.data_type, data_types.Date):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "date",
-                    "typeSignature": {"rawType": "date", "arguments": []},
-                }
-            ]
-        elif isinstance(column.data_type, data_types.DateTime):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "timestamp",
-                    "typeSignature": {"rawType": "timestamp", "arguments": []},
-                }
-            ]
-        elif isinstance(column.data_type, data_types.TimeDelta):
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "interval day to second",
-                    "typeSignature": {
-                        "rawType": "interval day to second",
-                        "arguments": [],
-                    },
-                }
-            ]
-        else:
-            columns += [
-                {
-                    "name": column.name,
-                    "type": "varchar",
-                    "typeSignature": {
-                        "rawType": "varchar",
-                        "arguments": [{"kind": "LONG_LITERAL", "value": 255}],
-                    },
-                }
-            ]
-    return {
-        "id": "someId",
-        # TODO: this should not be static
-        "infoUri": "http://localhost:8581/v1/info",
-        "columns": columns,
-        "data": [list(row) for row in res.table.rows],
-        "stats": {
-            "state": "FINISHED",
-            "nodes": 1,
-        },
-    }
-
-
 @route(["/health", "/api/health"], methods="GET")
 def health_check(runners: DbtProjectContainer) -> dict:
     """Health check endpoint."""
     # Project Support
     project_runner = (
         runners.get_project(request.get_header("X-dbt-Project")) or runners.get_default_project()
     )
@@ -6286,17 +6148,79 @@
             "error": None,
         },
         "id": str(uuid.uuid4()),
         "dbt-interface-server": __name__,
     }
 
 
-ServerPlugin = DbtInterfaceServerPlugin()
-install(ServerPlugin)
-install(JSONPlugin(json_dumps=lambda body: json.dumps(body, default=server_serializer)))
+if lint_command:
+    @route('/lint', method='POST')
+    def lint_sql(
+        runners: DbtProjectContainer,
+    ):
+        LOGGER.info(f"lint_sql()")
+        # Project Support
+        project_runner = (
+            runners.get_project(request.get_header("X-dbt-Project")) or runners.get_default_project()
+        )
+        LOGGER.info(f"got project: {project_runner}")
+        if not project_runner:
+            response.status = 400
+            return asdict(
+                ServerErrorContainer(
+                    error=ServerError(
+                        code=ServerErrorCode.ProjectNotRegistered,
+                        message=(
+                            "Project is not registered. Make a POST request to the /register endpoint"
+                            " first to register a runner"
+                        ),
+                        data={"registered_projects": runners.registered_projects()},
+                    )
+                )
+            )
+
+        sql_path = request.query.get("sql_path")
+        LOGGER.info(f"sql_path: {sql_path}")
+        if sql_path:
+            # Lint a file
+            LOGGER.info(f"linting file: {sql_path}")
+            sql = Path(sql_path)
+        else:
+            # Lint a string
+            LOGGER.info(f"linting string")
+            sql = request.body.getvalue().decode('utf-8')
+        if not sql:
+            response.status = 400
+            return {
+                "error": {
+                    "data": {},
+                    "message": "No SQL provided. Either provide a SQL file path or a SQL string to lint.",
+                }
+            }
+        try:
+            LOGGER.info(f"Calling lint_command()")
+            temp_result = lint_command(
+                Path(project_runner.config.project_root),
+                sql=sql,
+                extra_config_path=Path(request.query.get("extra_config_path")) if request.query.get("extra_config_path") else None,
+            )
+            result = temp_result["violations"] if temp_result is not None else []
+        except Exception as lint_err:
+            logging.exception("Linting failed")
+            response.status = 500
+            return {
+                "error": {
+                    "data": {},
+                    "message": str(lint_err),
+                }
+            }
+        else:
+            LOGGER.info(f"Linting succeeded")
+            lint_result = {"result": [error for error in result]}
+        return lint_result
 
 
 def run_server(runner: Optional[DbtProject] = None, host="localhost", port=8581):
     """Run the dbt core interface server.
 
     See supported servers below. By default, the server will run with the
     `WSGIRefServer` which is a pure Python server. If you want to use a different server,
@@ -6311,229 +6235,36 @@
     if runner:
         ServerPlugin.runners.add_parsed_project(runner)
     run(host=host, port=port)
 
 
 # endregion
 
-# region: dbt-core-interface data diffs
-
-try:
-    # TODO: we can drop this and use subprocesses to run git commands
-    from git import Repo
-except ImportError:
-    pass
-else:
-    from pathlib import Path
-
-    def build_diff_queries(model: str, runner: DbtProject) -> Tuple[str, str]:
-        """Leverage git to build two temporary tables for diffing the results of a query throughout a change."""
-        # Resolve git node
-        node = runner.get_ref_node(model)
-        dbt_path = Path(node.root_path)
-        repo = Repo(dbt_path, search_parent_directories=True)
-        t = next(Path(repo.working_dir).rglob(node.original_file_path)).relative_to(
-            repo.working_dir
-        )
-        sha = repo.head.object.hexsha
-        target = repo.head.object.tree[str(t)]
-
-        # Create original node
-        git_node_name = "z_" + sha[-7:]
-        original_node = runner.get_server_node(
-            target.data_stream.read().decode("utf-8"), git_node_name
-        )
-
-        # Alias changed node
-        changed_node = node
-
-        # Compile models
-        original_node = runner.compile_node(original_node)
-        changed_node = runner.compile_node(changed_node)
-
-        return original_node.compiled_sql, changed_node.compiled_sql
-
-    def build_diff_tables(model: str, runner: DbtProject) -> Tuple["BaseRelation", "BaseRelation"]:
-        """Leverage git to build two temporary tables for diffing the results of a query throughout a change."""
-        # Resolve git node
-        node = runner.get_ref_node(model)
-        dbt_path = Path(node.root_path)
-        repo = Repo(dbt_path, search_parent_directories=True)
-        t = next(Path(repo.working_dir).rglob(node.original_file_path)).relative_to(
-            repo.working_dir
-        )
-        sha = repo.head.object.hexsha
-        target = repo.head.object.tree[str(t)]
-
-        # Create original node
-        git_node_name = "z_" + sha[-7:]
-        original_node = runner.get_server_node(
-            target.data_stream.read().decode("utf-8"), git_node_name
-        )
-
-        # Alias changed node
-        changed_node = node
-
-        # Compile models
-        original_node = runner.compile_node(original_node).node
-        changed_node = runner.compile_node(changed_node).node
-
-        # Lookup and resolve original ref based on git sha
-        git_node_parts = original_node.database, "dbt_diff", git_node_name
-        ref_a, did_exist = runner.get_or_create_relation(*git_node_parts)
-        if not did_exist:
-            LOGGER.info("Creating new relation for %s", ref_a)
-            with runner.adapter.connection_named("dbt-osmosis"):
-                runner.execute_macro(
-                    "create_schema",
-                    kwargs={"relation": ref_a},
-                )
-                runner.execute_macro(
-                    "create_table_as",
-                    kwargs={
-                        "sql": original_node.compiled_sql,
-                        "relation": ref_a,
-                        "temporary": True,
-                    },
-                    run_compiled_sql=True,
-                )
-
-        # Resolve modified fake ref based on hash of it compiled SQL
-        temp_node_name = (
-            "z_"
-            + hashlib.md5(
-                changed_node.compiled_sql.encode("utf-8"),
-                usedforsecurity=False,
-            ).hexdigest()[-7:]
-        )
-        git_node_parts = original_node.database, "dbt_diff", temp_node_name
-        ref_b, did_exist = runner.get_or_create_relation(*git_node_parts)
-        if not did_exist:
-            ref_b = runner.adapter.Relation.create(*git_node_parts)
-            LOGGER.info("Creating new relation for %s", ref_b)
-            with runner.adapter.connection_named("dbt-osmosis"):
-                runner.execute_macro(
-                    "create_schema",
-                    kwargs={"relation": ref_b},
-                )
-                runner.execute_macro(
-                    "create_table_as",
-                    kwargs={
-                        "sql": original_node.compiled_sql,
-                        "relation": ref_b,
-                        "temporary": True,
-                    },
-                    run_compiled_sql=True,
-                )
-
-        return ref_a, ref_b
-
-    def diff_tables(
-        ref_a: "BaseRelation",
-        ref_b: "BaseRelation",
-        pk: str,
-        runner: DbtProject,
-        aggregate: bool = True,
-    ) -> "Table":
-        """Given two relations, compare the results and return a table of the differences."""
-        LOGGER.info("Running diff")
-        _, table = runner.adapter_execute(
-            runner.execute_macro(
-                (
-                    "_dbt_osmosis_compare_relations_agg"
-                    if aggregate
-                    else "_dbt_osmosis_compare_relations"
-                ),
-                kwargs={
-                    "a_relation": ref_a,
-                    "b_relation": ref_b,
-                    "primary_key": pk,
-                },
-            ),
-            auto_begin=True,
-            fetch=True,
-        )
-        return table
-
-    def diff_queries(
-        sql_a: str, sql_b: str, pk: str, runner: DbtProject, aggregate: bool = True
-    ) -> "Table":
-        """Given two queries, compare the results and return a table of the differences."""
-        LOGGER.info("Running diff")
-        _, table = runner.adapter_execute(
-            runner.execute_macro(
-                "_dbt_osmosis_compare_queries_agg" if aggregate else "_dbt_osmosis_compare_queries",
-                kwargs={
-                    "a_query": sql_a,
-                    "b_query": sql_b,
-                    "primary_key": pk,
-                },
-            ),
-            auto_begin=True,
-            fetch=True,
-        )
-        return table
-
-    def diff_and_print_to_console(
-        model: str,
-        pk: str,
-        runner: DbtProject,
-        make_temp_tables: bool = False,
-        agg: bool = True,
-        output: str = "table",
-    ) -> None:
-        """Compare two tables and print the results to the console."""
-        import agate
-
-        if make_temp_tables:
-            table = diff_tables(*build_diff_tables(model, runner), pk, runner, agg)
-        else:
-            table = diff_queries(*build_diff_queries(model, runner), pk, runner, agg)
-        print("")
-        output = output.lower()
-        if output == "table":
-            table.print_table()
-        elif output in ("chart", "bar"):
-            if not agg:
-                LOGGER.warn(
-                    "Cannot render output format chart with --no-agg option, defaulting to table"
-                )
-                table.print_table()
-            else:
-                _table = table.compute(
-                    [
-                        (
-                            "in_original, in_changed",
-                            agate.Formula(agate.Text(), lambda r: "%(in_a)s, %(in_b)s" % r),
-                        )
-                    ]
-                )
-                _table.print_bars(
-                    label_column_name="in_original, in_changed", value_column_name="count"
-                )
-        elif output == "csv":
-            table.to_csv("dbt-osmosis-diff.csv")
-        else:
-            LOGGER.warn("No such output format %s, defaulting to table", output)
-            table.print_table()
-
-
-# endregion
 
 if __name__ == "__main__":
     import argparse
 
+    #logging.basicConfig(level=logging.INFO)
     parser = argparse.ArgumentParser(
         description="Run the dbt interface server. Defaults to the WSGIRefServer"
     )
     parser.add_argument(
         "--host",
         default="localhost",
         help="The host to run the server on. Defaults to localhost",
     )
     parser.add_argument(
         "--port",
         default=8581,
         help="The port to run the server on. Defaults to 8581",
     )
     args = parser.parse_args()
+    ServerPlugin = DbtInterfaceServerPlugin()
+    install(ServerPlugin)
+    install(JSONPlugin(json_dumps=lambda body: json.dumps(body, default=server_serializer)))
+
+    if lint_command and importlib.util.find_spec('sqlfluff_templater_dbt'):
+        LOGGER.error("sqlfluff-templater-dbt is not compatible with dbt-core-interface server. "
+                       "Please uninstall it to continue.")
+        sys.exit(1)
+
     run_server(host=args.host, port=args.port)
```

### Comparing `dbt_core_interface-0.2.3/PKG-INFO` & `dbt_core_interface-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core-interface
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dbt Core Interface
 Home-page: https://github.com/z3z1ma/dbt-core-interface
 License: MIT
 Author: Alex Butler
 Author-email: butler.alex2010@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 3 - Alpha
@@ -50,15 +50,15 @@
 
 - Run SQL and get results in python fully independent of the dbt adapter which automatically enables support for many databases
 
 - Run SQL with dbt SQL from a single method call
 
 - Load macros at runtime enabling custom functionality in third party extensions without requiring the dbt packaging system to be managed in userland
 
-- Compile dbt jinja extremely fast and efficiently, thread-safe and stress tested at load via a fastapi server which live compiles SQL
+- Compile dbt jinja extremely fast and efficiently, thread-safe and stress tested at load via a Bottle server which live compiles SQL
 
 - Manage multiple dbt projects in a single process using the DbtProjectContainer class
 
 `dbt-core-interface` is a wrapper that allows developers to rapidly develop features and integrations for dbt. This project aims to serve as a place for the community to aggregate the best ways to interface with dbt. It is afforded a much faster iteration cycle and much more freedom due to it's independence from the dbt codebase. It is intended to act as an common library to dbt's existing APIs for developers. Implementations can land here and prove themselves out before landing in the dbt-core codebase and benefit all developers involved. Sqlfluff dbt templater, dbt-osmosis, dbt-fastapi which I am ripping out of dbt-osmosis, an impending metadata manager, a testing framework will all leverage this library. As dbt core evolves and stabilizes its python API, this project will evolve with it. This may manifest in simplification of certain methods but our goal is to maintain the API and focus on driving efficient, innovative/creative, and agile community driven integration patterns.
 
 ## Requirements
 
@@ -72,14 +72,24 @@
 $ pip install dbt-core-interface
 ```
 
 ## Usage
 
 Please see the [Api Reference] for details.
 
+To launch the Bottle server for live compiling dbt jinja:
+
+    python -m dbt_core_interface.project
+
+This will launch the server on port 8581. You can then make requests to the server, e.g.:
+
+    curl -X POST -H "Content-Type: application/json" -H "X-dbt-Project: dbt_project" -d '{"project_dir":"/app/tests/sqlfluff_templater/fixtures/dbt/dbt_project/","profiles_dir":"/app/tests/sqlfluff_templater/fixtures/dbt/profiles_yml/","target":"dev"}' http://localhost:8581/register
+
+You can change the server hostname and port using the `--host` and `--port` arguments.
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

