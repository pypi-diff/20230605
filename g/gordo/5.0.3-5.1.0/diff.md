# Comparing `tmp/gordo-5.0.3.tar.gz` & `tmp/gordo-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gordo-5.0.3.tar", last modified: Tue May 30 18:06:18 2023, max compression
+gzip compressed data, was "gordo-5.1.0.tar", last modified: Mon Jun  5 15:32:12 2023, max compression
```

## Comparing `gordo-5.0.3.tar` & `gordo-5.1.0.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 18:04:09.000000 gordo-5.0.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 18:04:09.000000 gordo-5.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/dependabot.yml 
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/master-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 18:04:09.000000 gordo-5.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-30 18:04:09.000000 gordo-5.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 18:04:09.000000 gordo-5.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/.trivyignore
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-30 18:04:09.000000 gordo-5.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-30 18:04:09.000000 gordo-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-30 18:04:09.000000 gordo-5.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-30 18:06:18.781191 gordo-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-30 18:04:09.000000 gordo-5.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/benchmarks/load_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/load_test/task_set.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 18:04:09.000000 gordo-5.0.3/benchmarks/test_ml_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-30 18:04:09.000000 gordo-5.0.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/Gordo_C4.README
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/Gordo_C4.svg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)   113230 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/architecture_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/architecture_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/argo_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/_static/endpoint-metadata.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.761191 gordo-5.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/loader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/model-factories.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/register.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/transformer-funcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/model/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/machine/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/reporters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/serializer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/api/server/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/server/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/api/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/general/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/cluster_deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/general/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/docs/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/model_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/ml/model_output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-30 18:04:09.000000 gordo-5.0.3/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/Gordo-Workflow-High-Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/Pipelines-with-Gordo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/model-configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-30 18:04:09.000000 gordo-5.0.3/examples/test-project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-30 18:04:09.000000 gordo-5.0.3/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26331 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/exceptions_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/cli/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/anomaly/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/factories/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/transformer_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformer_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformer_funcs/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/machine/model/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/transformers/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/machine/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/reporters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/serializer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.769191 gordo-5.0.3/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/blueprints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/server/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/prometheus/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/config_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/normalized_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/config_elements/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/workflow_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/gordo/workflow/workflow_generator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 18:04:09.000000 gordo-5.0.3/gordo/workflow/workflow_generator/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.765191 gordo-5.0.3/gordo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:06:18.000000 gordo-5.0.3/gordo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 18:04:09.000000 gordo-5.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 18:04:09.000000 gordo-5.0.3/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/docs_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/full_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/mlflow_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/postgres_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/test_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-30 18:04:09.000000 gordo-5.0.3/requirements/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.757191 gordo-5.0.3/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.757191 gordo-5.0.3/resources/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/resources/grafana/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/how_to_modify_dashboard.md
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-30 18:04:09.000000 gordo-5.0.3/resources/grafana/dashboards/machines.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-30 18:04:09.000000 gordo-5.0.3/run_workflow_and_argo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/download_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/github_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 18:04:09.000000 gordo-5.0.3/scripts/trivy_scan.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:06:18.781191 gordo-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-30 18:04:09.000000 gordo-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/config-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.773191 gordo-5.0.3/tests/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/builder/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/cli/test_exception_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/metadata/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_factories_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_raw_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/model/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/test_mlflow_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/reporters/test_postgres_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/definition_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/serializer/test_serializer_load_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_anomaly_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_base_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_gordo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/server/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.777191 gordo-5.0.3/tests/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_sensor_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/util/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_config_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_normalized_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:06:18.781191 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/mocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-30 18:04:09.000000 gordo-5.0.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.641962 gordo-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:29:58.000000 gordo-5.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 15:29:58.000000 gordo-5.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.617962 gordo-5.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-05 15:29:58.000000 gordo-5.1.0/.github/dependabot.yml 
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.617962 gordo-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-05 15:29:58.000000 gordo-5.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 15:29:58.000000 gordo-5.1.0/.github/workflows/master-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-05 15:29:58.000000 gordo-5.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-05 15:29:58.000000 gordo-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-05 15:29:58.000000 gordo-5.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/.trivyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-05 15:29:58.000000 gordo-5.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-05 15:29:58.000000 gordo-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-05 15:29:58.000000 gordo-5.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-05 15:32:12.641962 gordo-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-05 15:29:58.000000 gordo-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.617962 gordo-5.1.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 15:29:58.000000 gordo-5.1.0/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/benchmarks/load_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 15:29:58.000000 gordo-5.1.0/benchmarks/load_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-05 15:29:58.000000 gordo-5.1.0/benchmarks/load_test/load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-05 15:29:58.000000 gordo-5.1.0/benchmarks/load_test/task_set.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-05 15:29:58.000000 gordo-5.1.0/benchmarks/test_ml_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-05 15:29:58.000000 gordo-5.1.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/Gordo_C4.README
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/Gordo_C4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   113230 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/architecture_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/architecture_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/argo_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/_static/endpoint-metadata.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/api/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/loader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/api/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/model-factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/register.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/transformer-funcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/model/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/machine/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/reporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/serializer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.621962 gordo-5.1.0/docs/api/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/server/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/api/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/docs/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/general/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/general/cluster_deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/general/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/general/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/docs/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/ml/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/ml/model_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/ml/model_output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 15:29:58.000000 gordo-5.1.0/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-05 15:29:58.000000 gordo-5.1.0/examples/Gordo-Workflow-High-Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-05 15:29:58.000000 gordo-5.1.0/examples/Pipelines-with-Gordo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-05 15:29:58.000000 gordo-5.1.0/examples/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-05 15:29:58.000000 gordo-5.1.0/examples/model-configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 15:29:58.000000 gordo-5.1.0/examples/test-project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-05 15:29:58.000000 gordo-5.1.0/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26331 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/builder/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/builder/local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/cli/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/cli/exceptions_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/cli/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/anomaly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/anomaly/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/machine/model/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/factories/feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/factories/lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/factories/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/machine/model/transformer_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/transformer_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/transformer_funcs/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/machine/model/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/transformers/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/machine/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/reporters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/reporters/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/reporters/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/serializer/from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/serializer/into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/serializer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/blueprints/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/blueprints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/server/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/prometheus/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/prometheus/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/util/disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.629962 gordo-5.1.0/gordo/workflow/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/config_elements/normalized_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/config_elements/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/gordo/workflow/workflow_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/workflow_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/workflow_generator/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/gordo/workflow/workflow_generator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/workflow_generator/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-05 15:29:58.000000 gordo-5.1.0/gordo/workflow/workflow_generator/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.625962 gordo-5.1.0/gordo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:32:12.000000 gordo-5.1.0/gordo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 15:29:58.000000 gordo-5.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-05 15:29:58.000000 gordo-5.1.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/docs_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/full_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/mlflow_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/postgres_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/test_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-06-05 15:29:58.000000 gordo-5.1.0/requirements/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.617962 gordo-5.1.0/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.617962 gordo-5.1.0/resources/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/resources/grafana/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-06-05 15:29:58.000000 gordo-5.1.0/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-05 15:29:58.000000 gordo-5.1.0/resources/grafana/dashboards/how_to_modify_dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-06-05 15:29:58.000000 gordo-5.1.0/resources/grafana/dashboards/machines.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-06-05 15:29:58.000000 gordo-5.1.0/run_workflow_and_argo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-05 15:29:58.000000 gordo-5.1.0/scripts/download_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-05 15:29:58.000000 gordo-5.1.0/scripts/github_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-05 15:29:58.000000 gordo-5.1.0/scripts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-05 15:29:58.000000 gordo-5.1.0/scripts/trivy_scan.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:32:12.641962 gordo-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-05 15:29:58.000000 gordo-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/config-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/builder/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/builder/test_local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/builder/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/cli/test_exception_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.633962 gordo-5.1.0/tests/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/metadata/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_factories_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_raw_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/model/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/reporters/test_mlflow_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/reporters/test_postgres_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/serializer/definition_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/serializer/test_serializer_from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/serializer/test_serializer_into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/serializer/test_serializer_load_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_anomaly_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_base_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_gordo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/server/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/util/test_disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/util/test_sensor_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_normalized_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.637962 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:32:12.641962 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    28554 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/mocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-05 15:29:58.000000 gordo-5.1.0/tests/utils.py
```

### Comparing `gordo-5.0.3/.github/workflows/main.yml` & `gordo-5.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/.github/workflows/master-ci.yml` & `gordo-5.1.0/.github/workflows/master-ci.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/.github/workflows/release.yml` & `gordo-5.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/.gitignore` & `gordo-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/Dockerfile` & `gordo-5.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/LICENSE` & `gordo-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/Makefile` & `gordo-5.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/PKG-INFO` & `gordo-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.3
+Version: 5.1.0
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.3 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.1.0 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
```

### Comparing `gordo-5.0.3/README.md` & `gordo-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/benchmarks/load_test/README.md` & `gordo-5.1.0/benchmarks/load_test/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/benchmarks/load_test/load_test.py` & `gordo-5.1.0/benchmarks/load_test/load_test.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/benchmarks/test_ml_server.py` & `gordo-5.1.0/benchmarks/test_ml_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/Makefile` & `gordo-5.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/_static/Gordo_C4.svg` & `gordo-5.1.0/docs/_static/Gordo_C4.svg`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/_static/architecture_diagram.png` & `gordo-5.1.0/docs/_static/architecture_diagram.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/_static/architecture_diagram.py` & `gordo-5.1.0/docs/_static/architecture_diagram.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/_static/argo_logo.png` & `gordo-5.1.0/docs/_static/argo_logo.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/_static/endpoint-metadata.png` & `gordo-5.1.0/docs/_static/endpoint-metadata.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/builder.rst` & `gordo-5.1.0/docs/api/builder.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/machine/metadata.rst` & `gordo-5.1.0/docs/api/machine/metadata.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/machine/model/anomaly.rst` & `gordo-5.1.0/docs/api/machine/model/anomaly.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/machine/model/model-factories.rst` & `gordo-5.1.0/docs/api/machine/model/model-factories.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/serializer.rst` & `gordo-5.1.0/docs/api/serializer.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/util.rst` & `gordo-5.1.0/docs/api/util.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/api/workflow.rst` & `gordo-5.1.0/docs/api/workflow.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/conf.py` & `gordo-5.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/general/cluster_deployment.rst` & `gordo-5.1.0/docs/general/cluster_deployment.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/general/endpoints.rst` & `gordo-5.1.0/docs/general/endpoints.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/ml/model_configuration.rst` & `gordo-5.1.0/docs/ml/model_configuration.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/ml/model_output.rst` & `gordo-5.1.0/docs/ml/model_output.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/docs/overview.rst` & `gordo-5.1.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/examples/Gordo-Workflow-High-Level.ipynb` & `gordo-5.1.0/examples/Gordo-Workflow-High-Level.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/examples/Pipelines-with-Gordo.ipynb` & `gordo-5.1.0/examples/Pipelines-with-Gordo.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/examples/config.yaml` & `gordo-5.1.0/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/examples/model-configuration.yaml` & `gordo-5.1.0/examples/model-configuration.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/examples/test-project.yaml` & `gordo-5.1.0/examples/test-project.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/functions.sh` & `gordo-5.1.0/functions.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/__init__.py` & `gordo-5.1.0/gordo/__init__.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/builder/build_model.py` & `gordo-5.1.0/gordo/builder/build_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/builder/local_build.py` & `gordo-5.1.0/gordo/builder/local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/builder/utils.py` & `gordo-5.1.0/gordo/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/cli/cli.py` & `gordo-5.1.0/gordo/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/cli/custom_types.py` & `gordo-5.1.0/gordo/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/cli/exceptions_reporter.py` & `gordo-5.1.0/gordo/cli/exceptions_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/cli/workflow_generator.py` & `gordo-5.1.0/gordo/cli/workflow_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,31 +84,32 @@
     keda_prometheus_query = context["keda_prometheus_query"]
     if keda_prometheus_query:
         template = Environment(loader=BaseLoader).from_string(keda_prometheus_query)
         kwargs = {k: context[k] for k in KEDA_PROMETHEUS_QUERY_ARGS}
         return template.render(**kwargs)
 
 
-def prepare_resources_labels(value: str) -> List[Tuple[str, Any]]:
+def prepare_resources_labels(
+    value: str, argument: str = "--resources-labels"
+) -> List[Tuple[str, Any]]:
     resources_labels: List[Tuple[str, Any]] = []
     if value:
         try:
             json_value = json.loads(value)
         except json.JSONDecodeError as e:
             raise click.ClickException(
-                '"--resources-labels=%s" contains invalid JSON value: %s'
-                % (value, str(e))
+                '"%s=%s" contains invalid JSON value: %s' % (argument, value, str(e))
             )
         if isinstance(json_value, dict):
             resources_labels = cast(List[Tuple[str, Any]], list(json_value.items()))
         else:
             type_name = type(json_value).__name__
             raise click.ClickException(
-                '"--resources-labels=%s" contains value with type "%s" instead "dict"'
-                % (value, type_name)
+                '"%s=%s" contains value with type %s instead of dict'
+                % (argument, value, type_name)
             )
     return resources_labels
 
 
 def prepare_argo_version(argo_binary: Optional[str] = None) -> str:
     if argo_binary is not None:
         raw_argo_version = determine_argo_version(argo_binary)
@@ -309,14 +310,26 @@
 @click.option(
     "--resources-labels",
     help="Additional labels for resources. Have to be empty string or a dictionary in JSON format",
     envvar=f"{PREFIX}_RESOURCE_LABELS",
     default="",
 )
 @click.option(
+    "--model-builder-labels",
+    help="Additional labels for model-builder workflow step. Have to be empty string or a dictionary in JSON format",
+    envvar=f"{PREFIX}_MODEL_BUILDER_LABELS",
+    default="",
+)
+@click.option(
+    "--server-labels",
+    help="Additional labels for gordo-server. Have to be empty string or a dictionary in JSON format",
+    envvar=f"{PREFIX}_SERVER_LABELS",
+    default="",
+)
+@click.option(
     "--server-termination-grace-period",
     help="terminationGracePeriodSeconds for the gordo server",
     envvar=f"{PREFIX}_SERVER_TERMINATION_GRACE_PERIOD",
     type=int,
     default=60,
 )
 @click.option(
@@ -405,14 +418,21 @@
 
     validate_generate_context(context)
 
     context["argo_version"] = prepare_argo_version(context.get("argo_binary"))
 
     context["resources_labels"] = prepare_resources_labels(context["resources_labels"])
 
+    context["model_builder_labels"] = prepare_resources_labels(
+        context["model_builder_labels"], "--model-builder-labels"
+    )
+    context["server_labels"] = prepare_resources_labels(
+        context["server_labels"], "--server-labels"
+    )
+
     if context["pod_security_context"]:
         pod_security_context = cast(PodSecurityContext, context["pod_security_context"])
         context["pod_security_context"] = pod_security_context.dict(exclude_none=True)
 
     if context["security_context"]:
         security_context = cast(SecurityContext, context["security_context"])
         context["security_context"] = security_context.dict(exclude_none=True)
```

### Comparing `gordo-5.0.3/gordo/machine/encoders.py` & `gordo-5.1.0/gordo/machine/encoders.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/loader.py` & `gordo-5.1.0/gordo/machine/loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/machine.py` & `gordo-5.1.0/gordo/machine/machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/metadata/metadata.py` & `gordo-5.1.0/gordo/machine/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/anomaly/base.py` & `gordo-5.1.0/gordo/machine/model/anomaly/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/anomaly/diff.py` & `gordo-5.1.0/gordo/machine/model/anomaly/diff.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/base.py` & `gordo-5.1.0/gordo/machine/model/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/factories/feedforward_autoencoder.py` & `gordo-5.1.0/gordo/machine/model/factories/feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/factories/lstm_autoencoder.py` & `gordo-5.1.0/gordo/machine/model/factories/lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/factories/utils.py` & `gordo-5.1.0/gordo/machine/model/factories/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/models.py` & `gordo-5.1.0/gordo/machine/model/models.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/register.py` & `gordo-5.1.0/gordo/machine/model/register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/transformer_funcs/general.py` & `gordo-5.1.0/gordo/machine/model/transformer_funcs/general.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/transformers/imputer.py` & `gordo-5.1.0/gordo/machine/model/transformers/imputer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/model/utils.py` & `gordo-5.1.0/gordo/machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/machine/validators.py` & `gordo-5.1.0/gordo/machine/validators.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/reporters/base.py` & `gordo-5.1.0/gordo/reporters/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/reporters/mlflow.py` & `gordo-5.1.0/gordo/reporters/mlflow.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/reporters/postgres.py` & `gordo-5.1.0/gordo/reporters/postgres.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/serializer/from_definition.py` & `gordo-5.1.0/gordo/serializer/from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/serializer/into_definition.py` & `gordo-5.1.0/gordo/serializer/into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/serializer/serializer.py` & `gordo-5.1.0/gordo/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/serializer/utils.py` & `gordo-5.1.0/gordo/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/blueprints/anomaly.py` & `gordo-5.1.0/gordo/server/blueprints/anomaly.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/blueprints/base.py` & `gordo-5.1.0/gordo/server/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/model_io.py` & `gordo-5.1.0/gordo/server/model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/prometheus/metrics.py` & `gordo-5.1.0/gordo/server/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/prometheus/server.py` & `gordo-5.1.0/gordo/server/prometheus/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/properties.py` & `gordo-5.1.0/gordo/server/properties.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/server.py` & `gordo-5.1.0/gordo/server/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/server/utils.py` & `gordo-5.1.0/gordo/server/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/util/disk_registry.py` & `gordo-5.1.0/gordo/util/disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/util/utils.py` & `gordo-5.1.0/gordo/util/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/util/version.py` & `gordo-5.1.0/gordo/util/version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/utils.py` & `gordo-5.1.0/gordo/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/workflow/config_elements/normalized_config.py` & `gordo-5.1.0/gordo/workflow/config_elements/normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/workflow/config_elements/schemas.py` & `gordo-5.1.0/gordo/workflow/config_elements/schemas.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/workflow/workflow_generator/helpers.py` & `gordo-5.1.0/gordo/workflow/workflow_generator/helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template` & `gordo-5.1.0/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # project_revision: Current revision of this project, e.g. the git commit-sha.
 # containing start and end dates (if tags are shared across machines the earliest train start date and latest train end date is taken)
 # model_builder_resources_requests_memory: Memory requests of the model builder in unit `M`
 # model_builder_resources_requests_cpu: CPU requests of the model builder in unit `m`
 # model_builder_resources_limits_memory: Memory limit of the model builder in unit `M`
 # model_builder_resources_limits_cpu: CPU limit of the model builder in unit `m`
 
+{% macro print_labels(labels) -%}{% if labels %}{% for label, value in labels %}"{{label}}": "{{value}}"
+{% endfor %}{% endif %}{% endmacro %}
+
 apiVersion: argoproj.io/v1alpha1
 kind: Workflow
 metadata:
   generateName: "{{project_name}}-{{project_revision}}-"
   annotations:
     gordo-models: '{{ machines|map(attribute="name")|list|tojson|safe }}'
   labels:
@@ -714,16 +717,16 @@
       labels:
         app: gordo-model-builder
         applications.gordo.equinor.com/project-name: "{{project_name}}"
         applications.gordo.equinor.com/project-revision: "{{project_revision}}"{% if project_workflow %}
         applications.gordo.equinor.com/project-workflow: "{{project_workflow}}"{% endif %}
         applications.gordo.equinor.com/model-name: "{{'{{inputs.parameters.machine-name}}'}}"{% if "metadata" in builder_runtime and "labels" in builder_runtime["metadata"] %}
 {{ builder_runtime["metadata"]["labels"] | yaml | indent(8, True) }}{% endif %}
-        {% if resources_labels is defined %}{% for label, value in resources_labels %}"{{label}}": "{{value}}"
-        {% endfor %}{% endif %}
+{{ print_labels(model_builder_labels) | indent(8, True) }}
+{{ print_labels(resources_labels) | indent(8, True) }}
     tolerations:
       - effect: NoSchedule
         key: kubernetes.azure.com/scalesetpriority
         operator: Equal
         value: spot
     inputs:
       parameters:
@@ -1061,16 +1064,16 @@
                       app: "{{'{{inputs.parameters.host-name}}'}}"
                       app.kubernetes.io/name: model-server-deployment
                       app.kubernetes.io/component: server
                       app.kubernetes.io/part-of: gordo
                       app.kubernetes.io/managed-by: gordo
                       applications.gordo.equinor.com/project-name: "{{project_name}}"
                       applications.gordo.equinor.com/project-revision: "{{project_revision}}"
-                      {% if resources_labels is defined %}{% for label, value in resources_labels %}"{{label}}": "{{value}}"
-                      {% endfor %}{% endif %}
+{{ print_labels(resources_labels) | indent(22, True) }}
+{{ print_labels(server_labels) | indent(22, True) }}
                     {% if owner_references is defined %}
                     ownerReferences: {{owner_references}}
                     {% endif %}
                   spec:
                     replicas: 1
                     selector:
                       matchLabels:
@@ -1080,14 +1083,15 @@
                     template:
                       metadata:
                         labels:
                           app: "{{'{{inputs.parameters.host-name}}'}}"
                           project: "{{project_name}}"
                           {% if resources_labels is defined %}{% for label, value in resources_labels %}"{{label}}": "{{value}}"
                           {% endfor %}{% endif %}
+{{ print_labels(server_labels) | indent(22, True) }}
                       spec:
                         priorityClassName: server-priority
                         terminationGracePeriodSeconds: {{ server_termination_grace_period|default(60, true) }}
                         containers:
                            - image: "{{ docker_registry }}/{{ docker_repository }}/{{ server_image }}:{{gordo_version}}"{% if image_pull_policy %}
                              imagePullPolicy: "{{image_pull_policy}}"{% endif %}
                              name: "gordoserver-{{ project_name }}"{% if security_context %}
```

### Comparing `gordo-5.0.3/gordo/workflow/workflow_generator/workflow_generator.py` & `gordo-5.1.0/gordo/workflow/workflow_generator/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo.egg-info/PKG-INFO` & `gordo-5.1.0/gordo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.3
+Version: 5.1.0
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.3 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.1.0 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
```

### Comparing `gordo-5.0.3/gordo.egg-info/SOURCES.txt` & `gordo-5.1.0/gordo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/gordo.egg-info/requires.txt` & `gordo-5.1.0/gordo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/pytest.ini` & `gordo-5.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/requirements/full_requirements.txt` & `gordo-5.1.0/requirements/full_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/requirements/test_requirements.txt` & `gordo-5.1.0/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json` & `gordo-5.1.0/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/resources/grafana/dashboards/machines.json` & `gordo-5.1.0/resources/grafana/dashboards/machines.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/run_workflow_and_argo.sh` & `gordo-5.1.0/run_workflow_and_argo.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/scripts/download_argo.py` & `gordo-5.1.0/scripts/download_argo.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/scripts/github_docker.py` & `gordo-5.1.0/scripts/github_docker.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/scripts/tests.sh` & `gordo-5.1.0/scripts/tests.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/scripts/trivy_scan.sh` & `gordo-5.1.0/scripts/trivy_scan.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/setup.py` & `gordo-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/config-test.yaml` & `gordo-5.1.0/tests/config-test.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/conftest.py` & `gordo-5.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/builder/test_builder.py` & `gordo-5.1.0/tests/gordo/builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/builder/test_local_build.py` & `gordo-5.1.0/tests/gordo/builder/test_local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/builder/test_utils.py` & `gordo-5.1.0/tests/gordo/builder/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/cli/test_cli.py` & `gordo-5.1.0/tests/gordo/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/cli/test_exception_reporter.py` & `gordo-5.1.0/tests/gordo/cli/test_exception_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/client/test_client.py` & `gordo-5.1.0/tests/gordo/client/test_client.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/metadata/test_metadata.py` & `gordo-5.1.0/tests/gordo/machine/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py` & `gordo-5.1.0/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_factories_utils.py` & `gordo-5.1.0/tests/gordo/machine/model/test_factories_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_feedforward_autoencoder.py` & `gordo-5.1.0/tests/gordo/machine/model/test_feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_lstm_autoencoder.py` & `gordo-5.1.0/tests/gordo/machine/model/test_lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_model.py` & `gordo-5.1.0/tests/gordo/machine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_raw_keras.py` & `gordo-5.1.0/tests/gordo/machine/model/test_raw_keras.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_register.py` & `gordo-5.1.0/tests/gordo/machine/model/test_register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_transformers.py` & `gordo-5.1.0/tests/gordo/machine/model/test_transformers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/model/test_utils.py` & `gordo-5.1.0/tests/gordo/machine/model/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/test_descriptors.py` & `gordo-5.1.0/tests/gordo/machine/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/test_loader.py` & `gordo-5.1.0/tests/gordo/machine/test_loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/machine/test_machine.py` & `gordo-5.1.0/tests/gordo/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/reporters/test_mlflow_reporter.py` & `gordo-5.1.0/tests/gordo/reporters/test_mlflow_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/reporters/test_postgres_reporter.py` & `gordo-5.1.0/tests/gordo/reporters/test_postgres_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/serializer/test_serializer_from_definition.py` & `gordo-5.1.0/tests/gordo/serializer/test_serializer_from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/serializer/test_serializer_into_definition.py` & `gordo-5.1.0/tests/gordo/serializer/test_serializer_into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/serializer/test_serializer_load_dump.py` & `gordo-5.1.0/tests/gordo/serializer/test_serializer_load_dump.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_anomaly_blueprint.py` & `gordo-5.1.0/tests/gordo/server/test_anomaly_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_base_blueprint.py` & `gordo-5.1.0/tests/gordo/server/test_base_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_gordo_server.py` & `gordo-5.1.0/tests/gordo/server/test_gordo_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_model_io.py` & `gordo-5.1.0/tests/gordo/server/test_model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_prometheus.py` & `gordo-5.1.0/tests/gordo/server/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/server/test_utils.py` & `gordo-5.1.0/tests/gordo/server/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/test_version.py` & `gordo-5.1.0/tests/gordo/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/util/test_disk_registry.py` & `gordo-5.1.0/tests/gordo/util/test_disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/util/test_version.py` & `gordo-5.1.0/tests/gordo/util/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_config_elements.py` & `gordo-5.1.0/tests/gordo/workflow/test_config_elements.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_helpers.py` & `gordo-5.1.0/tests/gordo/workflow/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_normalized_config.py` & `gordo-5.1.0/tests/gordo/workflow/test_normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py` & `gordo-5.1.0/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -785,7 +785,48 @@
     _generate_test_workflow_str(
         path_to_config_files,
         "config-test-simple.yml",
         args=["--argo-binary", "argo3"],
         argo_binary="argo3",
         argo_version="3.1.0",
     )
+
+
+def test_model_builder_labels(path_to_config_files: str):
+    workflow_str = _generate_test_workflow_str(
+        path_to_config_files,
+        "config-test-simple.yml",
+        args=[
+            "--model-builder-labels",
+            '{"model-builder-label1": "value1", "model-builder-label2": "value2"}',
+        ],
+    )
+    workflow = yaml.safe_load(workflow_str)
+    templates = workflow["spec"]["templates"]
+    model_builder_step = [
+        step for step in templates if step["name"] == "model-builder"
+    ][0]
+    labels = model_builder_step["metadata"]["labels"]
+    assert labels["model-builder-label1"] == "value1"
+    assert labels["model-builder-label2"] == "value2"
+
+
+def test_model_server_(path_to_config_files: str):
+    workflow_str = _generate_test_workflow_str(
+        path_to_config_files,
+        "config-test-simple.yml",
+        args=[
+            "--server-labels",
+            '{"server-label1": "value1", "server-label2": "value2"}',
+        ],
+    )
+    workflow = yaml.safe_load(workflow_str)
+    templates = workflow["spec"]["templates"]
+    gordo_server_step = [
+        step for step in templates if step["name"] == "gordo-server-deployment"
+    ][0]
+    parameters = gordo_server_step["steps"][0][0]["arguments"]["parameters"]
+    resource_step = [v for v in parameters if v["name"] == "resource"][0]
+    resource = yaml.safe_load(resource_step["value"])
+    labels = resource["metadata"]["labels"]
+    assert labels["server-label1"] == "value1"
+    assert labels["server-label2"] == "value2"
```

### Comparing `gordo-5.0.3/tests/test_examples.py` & `gordo-5.1.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.3/tests/utils.py` & `gordo-5.1.0/tests/utils.py`

 * *Files identical despite different names*

