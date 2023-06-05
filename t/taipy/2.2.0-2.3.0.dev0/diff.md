# Comparing `tmp/taipy-2.2.0.tar.gz` & `tmp/taipy-2.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-2.2.0.tar", last modified: Thu Apr 13 18:52:50 2023, max compression
+gzip compressed data, was "taipy-2.3.0.dev0.tar", last modified: Mon Jun  5 16:13:40 2023, max compression
```

## Comparing `taipy-2.2.0.tar` & `taipy-2.3.0.dev0.tar`

### file list

```diff
@@ -1,22 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.221018 taipy-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-13 18:52:40.000000 taipy-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 18:52:40.000000 taipy-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 18:52:50.217018 taipy-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-13 18:52:40.000000 taipy-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:52:50.221018 taipy-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-13 18:52:40.000000 taipy-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 18:52:40.000000 taipy-2.2.0/src/taipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/src/taipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:52:43.000000 taipy-2.2.0/src/taipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 18:52:50.000000 taipy-2.2.0/src/taipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:52:50.217018 taipy-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-13 18:52:40.000000 taipy-2.2.0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 16:13:06.000000 taipy-2.3.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.515587 taipy-2.3.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/_help_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_cli/_scaffold_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/gui_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/gui_core/GuiCoreLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/gui_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.515587 taipy-2.3.0.dev0/src/taipy/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/src/taipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.519587 taipy-2.3.0.dev0/src/taipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:13:33.000000 taipy-2.3.0.dev0/src/taipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:13:40.000000 taipy-2.3.0.dev0/src/taipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:13:40.523587 taipy-2.3.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-05 16:13:07.000000 taipy-2.3.0.dev0/tests/test_run.py
```

### Comparing `taipy-2.2.0/LICENSE` & `taipy-2.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-2.2.0/setup.py` & `taipy-2.3.0.dev0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 # Copyright 2023 Avaiga Private Limited
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with
 # the License. You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,63 +9,89 @@
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 """The setup script."""
 
 import json
 import os
-from setuptools import find_packages, find_namespace_packages, setup
+from pathlib import Path
+
+from setuptools import find_namespace_packages, find_packages, setup
+from setuptools.command.build_py import build_py
 
-with open("README.md") as readme_file:
-    readme = readme_file.read()
+with open("README.md", "rb") as readme_file:
+    readme = readme_file.read().decode("UTF-8")
 
 with open(f"src{os.sep}taipy{os.sep}version.json") as version_file:
     version = json.load(version_file)
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
-    "taipy-gui>=2.2,<2.3",
-    "taipy-rest>=2.2,<2.3",
+    "cookiecutter>=2.1.1,<2.2",
+    "taipy-gui>=2.3.0.dev0,<3.0",
+    "taipy-rest>=2.3.0.dev0,<3.0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
-    "ngrok": ["pyngrok>=5"],
-    "image": ["python-magic;platform_system!='Windows'", "python-magic-bin;platform_system=='Windows'"],
+    "ngrok": ["pyngrok>=5.1,<6.0"],
+    "image": [
+        "python-magic>=0.4.24,<0.5;platform_system!='Windows'",
+        "python-magic-bin>=0.4.14,<0.5;platform_system=='Windows'",
+    ],
     "rdp": ["rdp>=0.8"],
-    "arrow": ["pyarrow>=7.0"],
+    "arrow": ["pyarrow>=10.0.1,<11.0"],
     "mssql": ["pyodbc>=4"],
 }
 
+
+def _build_webapp():
+    already_exists = Path("./src/taipy/gui_core/lib/taipy-gui-core.js").exists()
+    if not already_exists:
+        os.system("cd gui && npm ci && npm run build")
+
+
+class NPMInstall(build_py):
+    def run(self):
+        _build_webapp()
+        build_py.run(self)
+
+
 setup(
     author="Avaiga",
     author_email="dev@taipy.io",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    description="The Python application builder. Turns Data and AI algorithms into full web apps in no time.",
+    description="A 360° open-source platform from Python pilots to production-ready web apps.",
     install_requires=requirements,
+    entry_points={
+        "console_scripts": [
+            "taipy = taipy._entrypoint:_entrypoint",
+        ]
+    },
     license="Apache License 2.0",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="taipy",
     name="taipy",
     package_dir={"": "src"},
     packages=find_namespace_packages(where="src") + find_packages(include=["taipy"]),
     include_package_data=True,
     test_suite="tests",
     url="https://github.com/avaiga/taipy",
     version=version_string,
     zip_safe=False,
     extras_require=extras_require,
+    cmdclass={"build_py": NPMInstall},
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `taipy-2.2.0/src/taipy/__init__.py` & `taipy-2.3.0.dev0/src/taipy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,38 +6,46 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from importlib.util import find_spec
-from .version import _get_version
 
-__version__ = _get_version()
-
-if find_spec('taipy'):
+if find_spec("taipy"):
     if find_spec("taipy.config"):
-        from taipy.config import Config
-        from taipy.config import Scope
-        from taipy.config import Frequency
+        from taipy.config import Config, Frequency, Scope
 
     if find_spec("taipy.core"):
+        from taipy.core._core import Core
+        from taipy.core.cycle.cycle import Cycle
+        from taipy.core.cycle.cycle_id import CycleId
+        from taipy.core.data.data_node import DataNode
+        from taipy.core.data.data_node_id import DataNodeId
+        from taipy.core.job.job import Job
+        from taipy.core.job.job_id import JobId
+        from taipy.core.job.status import Status
+        from taipy.core.pipeline.pipeline import Pipeline
+        from taipy.core.pipeline.pipeline_id import PipelineId
+        from taipy.core.scenario.scenario import Scenario
+        from taipy.core.scenario.scenario_id import ScenarioId
         from taipy.core.taipy import (
             cancel_job,
             clean_all_entities,
             clean_all_entities_by_version,
             compare_scenarios,
             create_pipeline,
             create_scenario,
             delete,
             delete_job,
             delete_jobs,
             export_scenario,
             get,
             get_cycles,
+            get_cycles_scenarios,
             get_data_nodes,
             get_jobs,
             get_latest_job,
             get_parents,
             get_pipelines,
             get_primary,
             get_primary_scenarios,
@@ -49,30 +57,27 @@
             subscribe_pipeline,
             subscribe_scenario,
             tag,
             unsubscribe_pipeline,
             unsubscribe_scenario,
             untag,
         )
-        from taipy.core._core import Core
-        from taipy.core.common.alias import CycleId, DataNodeId, JobId, PipelineId, ScenarioId, TaskId
-        from taipy.core.cycle.cycle import Cycle
-        from taipy.core.data.data_node import DataNode
-        from taipy.core.job.job import Job
-        from taipy.core.job.status import Status
-        from taipy.core.pipeline.pipeline import Pipeline
-        from taipy.core.scenario.scenario import Scenario
         from taipy.core.task.task import Task
+        from taipy.core.task.task_id import TaskId
 
-    if find_spec('taipy.gui'):
+    if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
-        if find_spec('taipy.enterprise') and find_spec('taipy.enterprise.gui'):
+        from .gui_core.GuiCoreLib import GuiCore
+
+        Gui.add_library(GuiCore())
+
+        if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
-    if find_spec('taipy.rest'):
+    if find_spec("taipy.rest"):
         from taipy.rest import Rest
 
-    if find_spec('taipy._run'):
+    if find_spec("taipy._run"):
         from taipy._run import _run as run
```

### Comparing `taipy-2.2.0/src/taipy/_run.py` & `taipy-2.3.0.dev0/src/taipy/_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,52 +5,75 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
+import sys
 import typing as t
 
+from flask import Flask
+
+from taipy.core import Core
 from taipy.gui import Gui
 from taipy.rest import Rest
-from taipy.core import Core
 
+if sys.version_info >= (3, 10):
+    from typing import TypeGuard
 
-def _run(*apps: t.List[t.Union[Gui, Rest, Core]], **kwargs) -> t.Optional[t.Union[Gui, Rest, Core]]:
+_AppType = t.Union[Gui, Rest, Core]
+_AppTypeT = t.TypeVar("_AppTypeT", Gui, Rest, Core)
+
+
+def _run(*services: _AppType, **kwargs) -> t.Optional[Flask]:
     """Run one or multiple Taipy services.
 
     A Taipy service is an instance of a class that runs code as a Web application.
 
     Parameters:
-        *args (List[Union[`Gui^`, `Rest^`, `Core^`]]): Services to run. If several services are provided, all the services run simultaneously. If this is empty or set to None, this method does nothing.
+        *services (Union[`Gui^`, `Rest^`, `Core^`]): Services to run, as separate arguments.<br/>
+            If several services are provided, all the services run simultaneously.<br/>
+            If this is empty or set to None, this method does nothing.
         **kwargs: Other parameters to provide to the services.
     """
-    gui = __typing_get(apps, Gui)
-    rest = __typing_get(apps, Rest)
-    core = __typing_get(apps, Core)
+
+    gui = __get_app(services, Gui)
+    rest = __get_app(services, Rest)
+    core = __get_app(services, Core)
 
     if gui and core:
-        from taipy.core._version._version_cli import _VersioningCLI
+        from taipy.core._version._cli._core_cli import _CoreCLI
         from taipy.gui._gui_cli import _GuiCLI
 
-        _VersioningCLI._create_parser()
-        _GuiCLI._create_parser()
+        _CoreCLI.create_parser()
+        _GuiCLI.create_parser()
 
     if rest or core:
         if not core:
             core = Core()
         core.run()
 
     if not rest and not gui:
         return None
 
     if gui and rest:
         gui._set_flask(rest._app)
         return gui.run(**kwargs)
     else:
         app = rest or gui
+        assert app is not None  # Avoid pyright typing error
         return app.run(**kwargs)
 
 
-def __typing_get(l, type_):
-    return next(filter(lambda o: isinstance(o, type_), l), None)
+# Avoid black adding too many empty lines
+# fmt: off
+if sys.version_info >= (3, 10):
+    def __get_app(apps: t.Tuple[_AppType, ...], type_: t.Type[_AppTypeT]) -> t.Optional[_AppType]:
+        def filter_isinstance(tl: _AppType) -> TypeGuard[_AppTypeT]:
+            return isinstance(tl, type_)
+
+        return next(filter(filter_isinstance, apps), None)
+else:
+    def __get_app(apps: t.Tuple[_AppType, ...], type_: t.Type[_AppTypeT]) -> t.Optional[_AppType]:
+        return next(filter(lambda a: isinstance(a, type_), apps), None)
+# fmt: on
```

### Comparing `taipy-2.2.0/src/taipy/version.py` & `taipy-2.3.0.dev0/src/taipy/version.py`

 * *Files identical despite different names*

### Comparing `taipy-2.2.0/tests/test_run.py` & `taipy-2.3.0.dev0/tests/test_run.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from unittest import mock
 
 from src.taipy._run import _run
+from taipy.core import Core
 from taipy.gui import Gui
 from taipy.rest import Rest
-from taipy.core import Core
 
 
 @mock.patch("taipy.gui.Gui.run")
 def test_run_pass_with_gui(gui_run):
     _run(Gui())
     gui_run.assert_called_once()
```

