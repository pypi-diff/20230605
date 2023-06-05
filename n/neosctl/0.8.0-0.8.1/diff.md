# Comparing `tmp/neosctl-0.8.0.tar.gz` & `tmp/neosctl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.0.tar", max compression
+gzip compressed data, was "neosctl-0.8.1.tar", max compression
```

## Comparing `neosctl-0.8.0.tar` & `neosctl-0.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-05-31 10:11:42.836576 neosctl-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/constant.py
--rw-r--r--   0        0        0     4420 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    11574 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     4974 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     3842 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3331 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1157 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     3749 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3067 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8408 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12308 2023-05-31 10:11:42.839577 neosctl-0.8.0/neosctl/util.py
--rw-r--r--   0        0        0     3013 2023-05-31 10:11:42.839577 neosctl-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-06-05 09:49:22.667180 neosctl-0.8.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 09:49:22.667180 neosctl-0.8.1/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14159 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     4974 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     3842 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3331 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1157 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     3764 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3067 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8408 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12292 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-06-05 09:49:22.670180 neosctl-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.1/PKG-INFO
```

### Comparing `neosctl-0.8.0/README.md` & `neosctl-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.0
+# Core CLI v0.8.1
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.0/neosctl/auth.py` & `neosctl-0.8.1/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/cli.py` & `neosctl-0.8.1/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/profile.py` & `neosctl-0.8.1/neosctl/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,25 @@
     Create a profile that can be reused in later commands to define which
     services to interact with, and which user to interact as.
 
     Call `init` on an existing profile will update the existing profile.
     """
     typer.echo(f"Initialising [{ctx.obj.profile_name}] profile.")
     default_host = f"{hostname}/api/{{}}" if hostname else ""
+    bare_host = hostname.replace("http://", "").replace("https://", "") if hostname else ""
 
     if non_interactive and not (hostname and username):
         raise exit_with_output(
             msg="\nError: --hostname/-h and --username/-u required for non-interactive mode.",
             exit_code=1,
         )
 
     if non_interactive:
         gateway_api_url = gateway_api_url or f"{hostname}/api/gateway"
-        storage_api_url = storage_api_url or f"{hostname}/api/storage"
+        storage_api_url = storage_api_url or f"https://saas.{bare_host}"
         iam_api_url = iam_api_url or f"{hostname}/api/iam"
         registry_api_url = registry_api_url or f"{hostname}/api/registry"
 
     urls = {
         "gateway_api_url": gateway_api_url,
         "registry_api_url": registry_api_url,
         "iam_api_url": iam_api_url,
@@ -121,15 +122,15 @@
 @app.command()
 def view(
     ctx: typer.Context,
 ) -> None:
     """View configuration for a profile."""
     profile = get_user_profile_section(ctx.obj.config, ctx.obj.profile_name)
     raise exit_with_output(
-        msg=prettify_json({k: v for k, v in profile.items()}),
+        msg=prettify_json({k: v for k, v in profile.items()}),  # noqa: C416
     )
 
 
 @app.command(name="list")
 def list_profiles(
     ctx: typer.Context,
 ) -> None:
```

### Comparing `neosctl-0.8.0/neosctl/schema.py` & `neosctl-0.8.1/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/__init__.py` & `neosctl-0.8.1/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/data_product.py` & `neosctl-0.8.1/neosctl/services/gateway/data_product.py`

 * *Files 16% similar despite different names*

```diff
@@ -236,37 +236,104 @@
     """Get data product expectation rules."""
     util.get_and_process(
         ctx,
         f"{_data_product_url(ctx)}/expectation/rules",
     )
 
 
-@app.command(name="get-quality-expectation")
-def get_entity_quality_expectation(
+@app.command(name="get-expectation")
+def get_entity_expectation(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
+    *,
+    last_only: bool = typer.Option(
+        False,
+        "--last-only",
+        "-l",
+        help="Return only last settings.",
+        callback=util.sanitize,
+    ),
 ) -> None:
     """Get data product expectation settings."""
     util.get_and_process(
         ctx,
-        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation",
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation?last_only={last_only}",
     )
 
 
-@app.command(name="update-quality-expectation")
-def update_entity_quality_expectation(
+@app.command(name="create-expectation-custom")
+def create_expectation_custom(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
-    filepath: str = typer.Argument(..., help="Filepath to expectation description", callback=util.sanitize),
+    filepath: str = typer.Argument(..., help="Filepath to custom expectation description", callback=util.sanitize),
 ) -> None:
-    """Update data product expectation settings."""
-    data = util.load_object(schema.UpdateQualityExpectations, filepath, "expectation")
+    """Add data product custom expectation."""
+    data = util.load_object(schema.ExpectationItem, filepath, "custom expectation")
+    util.post_and_process(
+        ctx,
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation/custom",
+        json=data.dict(by_alias=True),
+    )
+
+
+@app.command(name="update-expectation-custom")
+def update_expectation_custom(
+    ctx: typer.Context,
+    identifier: str = arg_generator.identifier,
+    custom_identifier: str = typer.Argument(..., help="Custom expectation identifier", callback=util.sanitize),
+    filepath: str = typer.Argument(..., help="Filepath to custom expectation description", callback=util.sanitize),
+) -> None:
+    """Update data product custom expectation."""
+    data = util.load_object(schema.ExpectationItem, filepath, "custom expectation")
+    util.put_and_process(
+        ctx,
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation/custom/{custom_identifier}",
+        json=data.dict(by_alias=True),
+    )
+
+
+@app.command(name="delete-expectation-custom")
+def delete_expectation_custom(
+    ctx: typer.Context,
+    identifier: str = arg_generator.identifier,
+    custom_identifier: str = typer.Argument(..., help="Custom expectation identifier", callback=util.sanitize),
+) -> None:
+    """Delete data product custom expectation."""
+    util.delete_and_process(
+        ctx,
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation/custom/{custom_identifier}",
+    )
+
+
+@app.command(name="update-expectation-weights")
+def update_expectation_weights(
+    ctx: typer.Context,
+    identifier: str = arg_generator.identifier,
+    filepath: str = typer.Argument(..., help="Filepath to expectation weights description", callback=util.sanitize),
+) -> None:
+    """Update data product expectation weighgts."""
+    data = util.load_object(schema.ExpectationWeights, filepath, "expectation weights")
+    util.put_and_process(
+        ctx,
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation/weights",
+        json=data.dict(by_alias=True),
+    )
+
+
+@app.command(name="update-expectation-thresholds")
+def update_expectation_thresholds(
+    ctx: typer.Context,
+    identifier: str = arg_generator.identifier,
+    filepath: str = typer.Argument(..., help="Filepath to expectation thresholds description", callback=util.sanitize),
+) -> None:
+    """Update data product expectation thresholds."""
+    data = util.load_object(schema.ExpectationThresholds, filepath, "expectation thresholds")
     util.put_and_process(
         ctx,
-        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation",
+        f"{_identified_data_product_url(ctx, identifier)}/quality/expectation/thresholds",
         json=data.dict(by_alias=True),
     )
 
 
 @app.command(name="get-quality-profiling")
 def get_entity_quality_profiling(
     ctx: typer.Context,
```

### Comparing `neosctl-0.8.0/neosctl/services/gateway/data_source.py` & `neosctl-0.8.1/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/data_system.py` & `neosctl-0.8.1/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.1/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/entity.py` & `neosctl-0.8.1/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/link.py` & `neosctl-0.8.1/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/output.py` & `neosctl-0.8.1/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/schema.py` & `neosctl-0.8.1/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/secret.py` & `neosctl-0.8.1/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/spark.py` & `neosctl-0.8.1/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/gateway/tag.py` & `neosctl-0.8.1/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/iam/iam.py` & `neosctl-0.8.1/neosctl/services/iam/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     page_size: int = typer.Option(10, help="Page size number."),
     resource: typing.Optional[str] = typer.Option(None, help="Resource nrn.", callback=util.sanitize),
 ) -> None:
     """List existing policies."""
 
     @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
-        params: typing.Dict[str, typing.Union[int, str]] = {"page": page, "page_size": page_size}
+        params: typing.Dict[str, typing.Union[int, str]] = {"page": page, "page_size": page_size}  # noqa: FA100
         if resource:
             params["resource"] = resource
 
         return util.get(
             ctx,
             _iam_url(ctx.obj.get_iam_api_url(), "policy/users"),
             params=params,
```

### Comparing `neosctl-0.8.0/neosctl/services/iam/schema.py` & `neosctl-0.8.1/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/registry/registry.py` & `neosctl-0.8.1/neosctl/services/registry/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/services/storage/storage.py` & `neosctl-0.8.1/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.0/neosctl/util.py` & `neosctl-0.8.1/neosctl/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                 # Refresh the context
                 c = read_config_dotfile()
                 ctx.obj.config = c
                 ctx.obj.profile = get_user_profile(c, ctx.obj.profile_name)
 
                 r = method(*args, **kwargs)
 
-        return r  # noqa: RET504
+        return r
 
     return check_access_token
 
 
 def update_profile(
     ctx: click.Context,
     auth: schema.Auth = schema.Auth(),
```

### Comparing `neosctl-0.8.0/pyproject.toml` & `neosctl-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.0"
+version = "0.8.1"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
 
@@ -24,15 +24,15 @@
 # Tests
 freezegun = "^1.2.1"
 pretend = "^1.0.9"
 pytest = "~7.1.2"
 pytest-asyncio = "^0.18.3"
 pytest-benchmark = "^3.4.1"
 pytest-cov = "^3.0.0"
-pytest-env = "^0.6.2"
+pytest-env = "^0.8.1"
 pytest-random-order = "^1.0.4"
 requests = "^2.28.1"
 pytest-httpx = "^0.21.0"
 
 # Style
 ruff = {version="^0.0", source="pypi"}
 pre-commit = {version="^3.0.2", source="pypi"}
@@ -85,14 +85,15 @@
     "ANN101",  # type annotation on self
     "B008",  # typer involves a lot of function calls in function definitions
     "FBT003",  # boolean trap? no documentation
     "PLR0913",  # too many arguments to a function call
     "S",  # run full bandit as a commit-hook
     "TCH",  # typechecking blocks break tests
     "W291",  # Don't enforce whitespace, handled in pre-commit
+    "TD",  # TODO message formatting
 ]
 
 [tool.ruff.per-file-ignores]
 "neosctl/*"= [
     "D100", # Ignore module level docstrings, this project is never consumed
     "D104",  # Ignore public __init__ missing docstring.
 ]
```

### Comparing `neosctl-0.8.0/PKG-INFO` & `neosctl-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.0
+Version: 0.8.1
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.0
+# Core CLI v0.8.1
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

