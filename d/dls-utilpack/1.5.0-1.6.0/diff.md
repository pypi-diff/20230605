# Comparing `tmp/dls-utilpack-1.5.0.tar.gz` & `tmp/dls-utilpack-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-utilpack-1.5.0.tar", last modified: Tue May 30 09:33:26 2023, max compression
+gzip compressed data, was "dls-utilpack-1.6.0.tar", last modified: Mon Jun  5 16:58:46 2023, max compression
```

## Comparing `dls-utilpack-1.5.0.tar` & `dls-utilpack-1.6.0.tar`

### file list

```diff
@@ -1,131 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.336641 dls-utilpack-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.324641 dls-utilpack-1.5.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.324641 dls-utilpack-1.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-30 09:33:26.336641 dls-utilpack-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.324641 dls-utilpack-1.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.328641 dls-utilpack-1.5.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:33:26.336641 dls-utilpack-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.324641 dls-utilpack-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.332641 dls-utilpack-1.5.0/src/dls_utilpack/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/global_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/isodatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/modify_process_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/qualname.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/require.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/search_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/visit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/src/dls_utilpack/whatenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.332641 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 09:33:26.000000 dls-utilpack-1.5.0/src/dls_utilpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.336641 dls-utilpack-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:33:26.336641 dls-utilpack-1.5.0/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_sigint1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_sigint2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_visit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-30 09:33:14.000000 dls-utilpack-1.5.0/tests/test_whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/src/dls_utilpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/client_context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/global_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/isodatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/modify_process_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/require.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/search_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/server_context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_server_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sigint1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sigint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_whatenv.py
```

### Comparing `dls-utilpack-1.5.0/.dae-devops/Makefile` & `dls-utilpack-1.6.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/conventions.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/developing.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/devops.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/docs_structure.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/documenting.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/installing.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/docs/testing.rst` & `dls-utilpack-1.6.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.dae-devops/project.yaml` & `dls-utilpack-1.6.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.devcontainer/Dockerfile` & `dls-utilpack-1.6.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.devcontainer/devcontainer.json` & `dls-utilpack-1.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/CONTRIBUTING.rst` & `dls-utilpack-1.6.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/actions/install_requirements/action.yml` & `dls-utilpack-1.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/dependabot.yml` & `dls-utilpack-1.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/pages/index.html` & `dls-utilpack-1.6.0/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/pages/make_switcher.py` & `dls-utilpack-1.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/workflows/code.yml` & `dls-utilpack-1.6.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/workflows/docs.yml` & `dls-utilpack-1.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/workflows/docs_clean.yml` & `dls-utilpack-1.6.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.github/workflows/linkcheck.yml` & `dls-utilpack-1.6.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.gitignore` & `dls-utilpack-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.gitlab-ci.yml` & `dls-utilpack-1.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/.vscode/launch.json` & `dls-utilpack-1.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/LICENSE` & `dls-utilpack-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/Makefile` & `dls-utilpack-1.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/PKG-INFO` & `dls-utilpack-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.5.0
+Version: 1.6.0
 Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.5.0/docs/conf.py` & `dls-utilpack-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/docs/images/dls-favicon.ico` & `dls-utilpack-1.6.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/docs/images/dls-logo.svg` & `dls-utilpack-1.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/docs/reference/modules.rst` & `dls-utilpack-1.6.0/docs/reference/modules.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/pyproject.toml` & `dls-utilpack-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/__main__.py` & `dls-utilpack-1.6.0/src/dls_utilpack/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/bash_composer.py` & `dls-utilpack-1.6.0/src/dls_utilpack/bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/callsign.py` & `dls-utilpack-1.6.0/src/dls_utilpack/callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/datatypes.py` & `dls-utilpack-1.6.0/src/dls_utilpack/datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/describe.py` & `dls-utilpack-1.6.0/src/dls_utilpack/describe.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/envvar.py` & `dls-utilpack-1.6.0/src/dls_utilpack/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/exceptions.py` & `dls-utilpack-1.6.0/src/dls_utilpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/explain.py` & `dls-utilpack-1.6.0/src/dls_utilpack/explain.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/hazzathread.py` & `dls-utilpack-1.6.0/src/dls_utilpack/hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/ignore.py` & `dls-utilpack-1.6.0/src/dls_utilpack/ignore.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/import_class.py` & `dls-utilpack-1.6.0/src/dls_utilpack/import_class.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/module.py` & `dls-utilpack-1.6.0/src/dls_utilpack/module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/profiler.py` & `dls-utilpack-1.6.0/src/dls_utilpack/profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/require.py` & `dls-utilpack-1.6.0/src/dls_utilpack/require.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/sanitize.py` & `dls-utilpack-1.6.0/src/dls_utilpack/sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/search_file.py` & `dls-utilpack-1.6.0/src/dls_utilpack/search_file.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/signal.py` & `dls-utilpack-1.6.0/src/dls_utilpack/signal.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/substitute.py` & `dls-utilpack-1.6.0/src/dls_utilpack/substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/thing.py` & `dls-utilpack-1.6.0/src/dls_utilpack/thing.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 class Thing:
     """
     Class for a named thing with traits.
     """
 
     def __init__(self, thing_type: str, specification, predefined_uuid=None):
         self.__thing_type = thing_type
-        self.__specification = specification
+
+        if specification is None:
+            self.__specification = {}
+        else:
+            self.__specification = specification
+
         self.__uuid = predefined_uuid
         if self.__uuid is None:
             self.__uuid = str(uuid.uuid4())
         self.__state = None
         self.__traits: Dict[str, Any] = {}
 
     # -----------------------------------------------------------------------------
```

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/things.py` & `dls-utilpack-1.6.0/src/dls_utilpack/things.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/version.py` & `dls-utilpack-1.6.0/src/dls_utilpack/version.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/visit.py` & `dls-utilpack-1.6.0/src/dls_utilpack/visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack/whatenv.py` & `dls-utilpack-1.6.0/src/dls_utilpack/whatenv.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack.egg-info/PKG-INFO` & `dls-utilpack-1.6.0/src/dls_utilpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.5.0
+Version: 1.6.0
 Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.5.0/src/dls_utilpack.egg-info/SOURCES.txt` & `dls-utilpack-1.6.0/src/dls_utilpack.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 docs/tutorials/index.rst
 docs/tutorials/tbd.rst
 src/dls_utilpack/__init__.py
 src/dls_utilpack/__main__.py
 src/dls_utilpack/_version.py
 src/dls_utilpack/bash_composer.py
 src/dls_utilpack/callsign.py
+src/dls_utilpack/client_context_base.py
 src/dls_utilpack/datatypes.py
 src/dls_utilpack/describe.py
 src/dls_utilpack/envvar.py
 src/dls_utilpack/exceptions.py
 src/dls_utilpack/explain.py
 src/dls_utilpack/global_signals.py
 src/dls_utilpack/hazzathread.py
@@ -69,14 +70,15 @@
 src/dls_utilpack/modify_process_title.py
 src/dls_utilpack/module.py
 src/dls_utilpack/profiler.py
 src/dls_utilpack/qualname.py
 src/dls_utilpack/require.py
 src/dls_utilpack/sanitize.py
 src/dls_utilpack/search_file.py
+src/dls_utilpack/server_context_base.py
 src/dls_utilpack/signal.py
 src/dls_utilpack/substitute.py
 src/dls_utilpack/thing.py
 src/dls_utilpack/things.py
 src/dls_utilpack/version.py
 src/dls_utilpack/visit.py
 src/dls_utilpack/whatenv.py
@@ -94,13 +96,14 @@
 tests/test_callsign.py
 tests/test_datatypes.py
 tests/test_hazzathread.py
 tests/test_import.py
 tests/test_module.py
 tests/test_profiler.py
 tests/test_sanitize.py
+tests/test_server_context.py
 tests/test_sigint1.py
 tests/test_sigint2.py
 tests/test_substitute.py
 tests/test_visit.py
 tests/test_whatenv.py
 tests/task_classes/task_z.py
```

### Comparing `dls-utilpack-1.5.0/tests/base.py` & `dls-utilpack-1.6.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/base_tester.py` & `dls-utilpack-1.6.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/conftest.py` & `dls-utilpack-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_bash_composer.py` & `dls-utilpack-1.6.0/tests/test_bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_callsign.py` & `dls-utilpack-1.6.0/tests/test_callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_datatypes.py` & `dls-utilpack-1.6.0/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_hazzathread.py` & `dls-utilpack-1.6.0/tests/test_hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_import.py` & `dls-utilpack-1.6.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_module.py` & `dls-utilpack-1.6.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_profiler.py` & `dls-utilpack-1.6.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_sanitize.py` & `dls-utilpack-1.6.0/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_sigint1.py` & `dls-utilpack-1.6.0/tests/test_sigint1.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_sigint2.py` & `dls-utilpack-1.6.0/tests/test_sigint2.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_substitute.py` & `dls-utilpack-1.6.0/tests/test_substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_visit.py` & `dls-utilpack-1.6.0/tests/test_visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.5.0/tests/test_whatenv.py` & `dls-utilpack-1.6.0/tests/test_whatenv.py`

 * *Files identical despite different names*

