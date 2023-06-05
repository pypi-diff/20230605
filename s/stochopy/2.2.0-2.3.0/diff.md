# Comparing `tmp/stochopy-2.2.0.tar.gz` & `tmp/stochopy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stochopy-2.2.0.tar", last modified: Mon Nov 22 08:24:50 2021, max compression
+gzip compressed data, was "stochopy-2.3.0.tar", last modified: Mon Jun  5 19:52:58 2023, max compression
```

## Comparing `stochopy-2.2.0.tar` & `stochopy-2.3.0.tar`

### file list

```diff
@@ -1,108 +1,66 @@
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.542099 stochopy-2.2.0/
--rw-rw-rw-   0        0        0     5436 2020-09-29 08:21:19.000000 stochopy-2.2.0/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1851 2020-09-29 08:21:19.000000 stochopy-2.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1548 2020-09-29 08:21:19.000000 stochopy-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       90 2020-09-29 08:21:19.000000 stochopy-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5968 2021-11-22 08:24:50.542704 stochopy-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5153 2021-11-22 07:55:54.000000 stochopy-2.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.288580 stochopy-2.2.0/examples/
--rw-rw-rw-   0        0        0        0 2020-10-04 05:09:34.000000 stochopy-2.2.0/examples/README.rst
--rw-rw-rw-   0        0        0     1685 2021-11-22 07:55:31.000000 stochopy-2.2.0/examples/basic_usage.py
--rw-rw-rw-   0        0        0       95 2020-09-29 08:21:19.000000 stochopy-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      976 2021-11-22 08:24:50.556232 stochopy-2.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.296550 stochopy-2.2.0/stochopy/
--rw-rw-rw-   0        0        0      210 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/__about__.py
--rw-rw-rw-   0        0        0      163 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.338096 stochopy-2.2.0/stochopy/__pycache__/
--rw-rw-rw-   0        0        0      358 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/__pycache__/__about__.cpython-38.pyc
--rw-rw-rw-   0        0        0      306 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1397 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/__pycache__/_common.cpython-38.pyc
--rw-rw-rw-   0        0        0      953 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/_common.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.340432 stochopy-2.2.0/stochopy/factory/
--rw-rw-rw-   0        0        0       26 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/factory/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.346060 stochopy-2.2.0/stochopy/factory/__pycache__/
--rw-rw-rw-   0        0        0      176 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/factory/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     3586 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/factory/__pycache__/benchmark.cpython-38.pyc
--rw-rw-rw-   0        0        0     3162 2021-11-22 07:39:35.000000 stochopy-2.2.0/stochopy/factory/benchmark.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.351390 stochopy-2.2.0/stochopy/optimize/
--rw-rw-rw-   0        0        0      391 2021-11-06 08:31:59.000000 stochopy-2.2.0/stochopy/optimize/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.359199 stochopy-2.2.0/stochopy/optimize/__pycache__/
--rw-rw-rw-   0        0        0      428 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     4789 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/__pycache__/_common.cpython-38.pyc
--rw-rw-rw-   0        0        0     3957 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/__pycache__/_helpers.cpython-38.pyc
--rw-rw-rw-   0        0        0     5972 2021-11-22 07:46:19.000000 stochopy-2.2.0/stochopy/optimize/_common.py
--rw-rw-rw-   0        0        0     3731 2021-11-22 07:46:18.000000 stochopy-2.2.0/stochopy/optimize/_helpers.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.365023 stochopy-2.2.0/stochopy/optimize/cmaes/
--rw-rw-rw-   0        0        0       65 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/cmaes/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.371029 stochopy-2.2.0/stochopy/optimize/cmaes/__pycache__/
--rw-rw-rw-   0        0        0      220 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/cmaes/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     9054 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/cmaes/__pycache__/_cmaes.cpython-38.pyc
--rw-rw-rw-   0        0        0     1752 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/cmaes/__pycache__/_constraints.cpython-38.pyc
--rw-rw-rw-   0        0        0    13107 2021-11-22 07:46:19.000000 stochopy-2.2.0/stochopy/optimize/cmaes/_cmaes.py
--rw-rw-rw-   0        0        0     2401 2021-11-22 07:46:18.000000 stochopy-2.2.0/stochopy/optimize/cmaes/_constraints.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.376082 stochopy-2.2.0/stochopy/optimize/cpso/
--rw-rw-rw-   0        0        0       64 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/cpso/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.381659 stochopy-2.2.0/stochopy/optimize/cpso/__pycache__/
--rw-rw-rw-   0        0        0      218 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/cpso/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1786 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/cpso/__pycache__/_constraints.cpython-38.pyc
--rw-rw-rw-   0        0        0     9737 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/cpso/__pycache__/_cpso.cpython-38.pyc
--rw-rw-rw-   0        0        0     1624 2021-11-22 07:41:06.000000 stochopy-2.2.0/stochopy/optimize/cpso/_constraints.py
--rw-rw-rw-   0        0        0    12653 2021-11-22 08:13:41.000000 stochopy-2.2.0/stochopy/optimize/cpso/_cpso.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.389233 stochopy-2.2.0/stochopy/optimize/de/
--rw-rw-rw-   0        0        0       62 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/de/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.397803 stochopy-2.2.0/stochopy/optimize/de/__pycache__/
--rw-rw-rw-   0        0        0      214 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/de/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      888 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/de/__pycache__/_constraints.cpython-38.pyc
--rw-rw-rw-   0        0        0     9222 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/de/__pycache__/_de.cpython-38.pyc
--rw-rw-rw-   0        0        0     1286 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/de/__pycache__/_strategy.cpython-38.pyc
--rw-rw-rw-   0        0        0      554 2021-11-22 07:41:24.000000 stochopy-2.2.0/stochopy/optimize/de/_constraints.py
--rw-rw-rw-   0        0        0    11582 2021-11-22 08:04:14.000000 stochopy-2.2.0/stochopy/optimize/de/_de.py
--rw-rw-rw-   0        0        0      958 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/de/_strategy.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.403225 stochopy-2.2.0/stochopy/optimize/na/
--rw-rw-rw-   0        0        0       62 2021-11-06 08:31:59.000000 stochopy-2.2.0/stochopy/optimize/na/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.409948 stochopy-2.2.0/stochopy/optimize/na/__pycache__/
--rw-rw-rw-   0        0        0      214 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/na/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     7179 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/na/__pycache__/_na.cpython-38.pyc
--rw-rw-rw-   0        0        0     9072 2021-11-22 08:15:13.000000 stochopy-2.2.0/stochopy/optimize/na/_na.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.417279 stochopy-2.2.0/stochopy/optimize/pso/
--rw-rw-rw-   0        0        0       63 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/pso/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.423524 stochopy-2.2.0/stochopy/optimize/pso/__pycache__/
--rw-rw-rw-   0        0        0      216 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/pso/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     5262 2021-11-22 07:07:22.000000 stochopy-2.2.0/stochopy/optimize/pso/__pycache__/_pso.cpython-38.pyc
--rw-rw-rw-   0        0        0     5447 2021-11-22 07:06:35.000000 stochopy-2.2.0/stochopy/optimize/pso/_pso.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.428938 stochopy-2.2.0/stochopy/optimize/vdcma/
--rw-rw-rw-   0        0        0       65 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/optimize/vdcma/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.480528 stochopy-2.2.0/stochopy/optimize/vdcma/__pycache__/
--rw-rw-rw-   0        0        0      220 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/optimize/vdcma/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     9406 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/optimize/vdcma/__pycache__/_vdcma.cpython-38.pyc
--rw-rw-rw-   0        0        0    14076 2021-11-22 07:46:19.000000 stochopy-2.2.0/stochopy/optimize/vdcma/_vdcma.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.489253 stochopy-2.2.0/stochopy/sample/
--rw-rw-rw-   0        0        0      189 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/sample/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.500427 stochopy-2.2.0/stochopy/sample/__pycache__/
--rw-rw-rw-   0        0        0      308 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/sample/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      421 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/sample/__pycache__/_common.cpython-38.pyc
--rw-rw-rw-   0        0        0     3267 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/sample/__pycache__/_helpers.cpython-38.pyc
--rw-rw-rw-   0        0        0      251 2021-11-22 07:42:43.000000 stochopy-2.2.0/stochopy/sample/_common.py
--rw-rw-rw-   0        0        0     3023 2021-11-22 07:46:18.000000 stochopy-2.2.0/stochopy/sample/_helpers.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.507617 stochopy-2.2.0/stochopy/sample/hmc/
--rw-rw-rw-   0        0        0       59 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/sample/hmc/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.516681 stochopy-2.2.0/stochopy/sample/hmc/__pycache__/
--rw-rw-rw-   0        0        0      212 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/sample/hmc/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     6557 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/sample/hmc/__pycache__/_hmc.cpython-38.pyc
--rw-rw-rw-   0        0        0     8015 2021-11-22 08:14:17.000000 stochopy-2.2.0/stochopy/sample/hmc/_hmc.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.521600 stochopy-2.2.0/stochopy/sample/mcmc/
--rw-rw-rw-   0        0        0       60 2020-09-29 08:21:19.000000 stochopy-2.2.0/stochopy/sample/mcmc/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.529970 stochopy-2.2.0/stochopy/sample/mcmc/__pycache__/
--rw-rw-rw-   0        0        0      214 2021-11-22 00:56:11.000000 stochopy-2.2.0/stochopy/sample/mcmc/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     4442 2021-11-22 08:10:34.000000 stochopy-2.2.0/stochopy/sample/mcmc/__pycache__/_mcmc.cpython-38.pyc
--rw-rw-rw-   0        0        0     5794 2021-11-22 08:14:28.000000 stochopy-2.2.0/stochopy/sample/mcmc/_mcmc.py
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.329345 stochopy-2.2.0/stochopy.egg-info/
--rw-rw-rw-   0        0        0     5968 2021-11-22 08:24:50.000000 stochopy-2.2.0/stochopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3022 2021-11-22 08:24:50.000000 stochopy-2.2.0/stochopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-22 08:24:50.000000 stochopy-2.2.0/stochopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2021-11-22 08:24:50.000000 stochopy-2.2.0/stochopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-11-22 08:24:50.000000 stochopy-2.2.0/stochopy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-11-22 08:24:50.536925 stochopy-2.2.0/test/
--rw-rw-rw-   0        0        0      566 2021-11-22 07:43:03.000000 stochopy-2.2.0/test/test_factory.py
--rw-rw-rw-   0        0        0     4664 2021-11-22 07:46:20.000000 stochopy-2.2.0/test/test_optimize.py
--rw-rw-rw-   0        0        0      957 2021-11-22 07:46:20.000000 stochopy-2.2.0/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.867728 stochopy-2.3.0/
+-rw-rw-rw-   0        0        0     5436 2022-08-29 13:39:48.000000 stochopy-2.3.0/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1851 2022-08-29 13:39:48.000000 stochopy-2.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1548 2022-08-29 13:39:48.000000 stochopy-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0       90 2022-08-29 13:39:48.000000 stochopy-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6026 2023-06-05 19:52:58.867728 stochopy-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5160 2023-06-05 17:15:58.000000 stochopy-2.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.802302 stochopy-2.3.0/examples/
+-rw-rw-rw-   0        0        0        0 2022-08-29 13:39:48.000000 stochopy-2.3.0/examples/README.rst
+-rw-rw-rw-   0        0        0     1685 2022-08-29 13:39:48.000000 stochopy-2.3.0/examples/basic_usage.py
+-rw-rw-rw-   0        0        0       95 2022-08-29 13:39:48.000000 stochopy-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1084 2023-06-05 19:52:58.869726 stochopy-2.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.806302 stochopy-2.3.0/stochopy/
+-rw-rw-rw-   0        0        0        5 2023-06-05 17:10:59.000000 stochopy-2.3.0/stochopy/VERSION
+-rw-rw-rw-   0        0        0      159 2023-06-05 17:11:16.000000 stochopy-2.3.0/stochopy/__about__.py
+-rw-rw-rw-   0        0        0      163 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/__init__.py
+-rw-rw-rw-   0        0        0      953 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/_common.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.836310 stochopy-2.3.0/stochopy/factory/
+-rw-rw-rw-   0        0        0       26 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/factory/__init__.py
+-rw-rw-rw-   0        0        0     3162 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/factory/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.840310 stochopy-2.3.0/stochopy/optimize/
+-rw-rw-rw-   0        0        0      391 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/__init__.py
+-rw-rw-rw-   0        0        0     5972 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/_common.py
+-rw-rw-rw-   0        0        0     3802 2023-06-05 17:05:22.000000 stochopy-2.3.0/stochopy/optimize/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.843316 stochopy-2.3.0/stochopy/optimize/cmaes/
+-rw-rw-rw-   0        0        0       65 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/cmaes/__init__.py
+-rw-rw-rw-   0        0        0    13625 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/cmaes/_cmaes.py
+-rw-rw-rw-   0        0        0     2399 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/cmaes/_constraints.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.846313 stochopy-2.3.0/stochopy/optimize/cpso/
+-rw-rw-rw-   0        0        0       64 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/cpso/__init__.py
+-rw-rw-rw-   0        0        0     1624 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/cpso/_constraints.py
+-rw-rw-rw-   0        0        0    13356 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/cpso/_cpso.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.850309 stochopy-2.3.0/stochopy/optimize/de/
+-rw-rw-rw-   0        0        0       62 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/de/__init__.py
+-rw-rw-rw-   0        0        0      554 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/de/_constraints.py
+-rw-rw-rw-   0        0        0    12283 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/de/_de.py
+-rw-rw-rw-   0        0        0      958 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/de/_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.852727 stochopy-2.3.0/stochopy/optimize/na/
+-rw-rw-rw-   0        0        0       62 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/na/__init__.py
+-rw-rw-rw-   0        0        0     9826 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/na/_na.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.853727 stochopy-2.3.0/stochopy/optimize/pso/
+-rw-rw-rw-   0        0        0       63 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/pso/__init__.py
+-rw-rw-rw-   0        0        0     5663 2023-06-05 16:58:18.000000 stochopy-2.3.0/stochopy/optimize/pso/_pso.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.855728 stochopy-2.3.0/stochopy/optimize/vdcma/
+-rw-rw-rw-   0        0        0       65 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/optimize/vdcma/__init__.py
+-rw-rw-rw-   0        0        0    14576 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/optimize/vdcma/_vdcma.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.859728 stochopy-2.3.0/stochopy/sample/
+-rw-rw-rw-   0        0        0      189 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/sample/__init__.py
+-rw-rw-rw-   0        0        0      251 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/sample/_common.py
+-rw-rw-rw-   0        0        0     3021 2023-06-05 17:07:15.000000 stochopy-2.3.0/stochopy/sample/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.861729 stochopy-2.3.0/stochopy/sample/hmc/
+-rw-rw-rw-   0        0        0       59 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/sample/hmc/__init__.py
+-rw-rw-rw-   0        0        0     8015 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/sample/hmc/_hmc.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.863730 stochopy-2.3.0/stochopy/sample/mcmc/
+-rw-rw-rw-   0        0        0       60 2022-08-29 13:39:48.000000 stochopy-2.3.0/stochopy/sample/mcmc/__init__.py
+-rw-rw-rw-   0        0        0     5884 2023-06-05 17:58:08.000000 stochopy-2.3.0/stochopy/sample/mcmc/_mcmc.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.834304 stochopy-2.3.0/stochopy.egg-info/
+-rw-rw-rw-   0        0        0     6026 2023-06-05 19:52:58.000000 stochopy-2.3.0/stochopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-06-05 19:52:58.000000 stochopy-2.3.0/stochopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 19:52:58.000000 stochopy-2.3.0/stochopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-05 19:52:58.000000 stochopy-2.3.0/stochopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-05 19:52:58.000000 stochopy-2.3.0/stochopy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 19:52:58.866728 stochopy-2.3.0/tests/
+-rw-rw-rw-   0        0        0      566 2022-08-29 13:39:48.000000 stochopy-2.3.0/tests/test_factory.py
+-rw-rw-rw-   0        0        0     4664 2022-08-29 13:39:48.000000 stochopy-2.3.0/tests/test_optimize.py
+-rw-rw-rw-   0        0        0      957 2022-08-29 13:39:48.000000 stochopy-2.3.0/tests/test_sample.py
```

### Comparing `stochopy-2.2.0/CODE_OF_CONDUCT.rst` & `stochopy-2.3.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/CONTRIBUTING.rst` & `stochopy-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/LICENSE` & `stochopy-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/PKG-INFO` & `stochopy-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: stochopy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python library for stochastic numerical optimization
 Home-page: https://github.com/keurfonluu/stochopy
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/stochopy
 Project-URL: Issues, https://github.com/keurfonluu/stochopy/issues
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 stochopy
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **stochopy** provides functions for sampling or optimizing objective functions with or without constraints. Its API is directly inspired by **scipy**'s own optimization submodule which should make the switch from one module to another straightforward.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/stochopy/master/.github/sample.gif
    :alt: sample-pso
    :width: 100%
    :align: center
@@ -159,13 +160,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/stochopy.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/stochopy
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4058008.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.4058008
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/Python%20package
+.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/ci.yml
    :target: https://github.com/keurfonluu/stochopy
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/stochopy/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/stochopy/doc.yml?label=docs
    :target: https://keurfonluu.github.io/stochopy/
-
```

### Comparing `stochopy-2.2.0/README.rst` & `stochopy-2.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 stochopy
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **stochopy** provides functions for sampling or optimizing objective functions with or without constraints. Its API is directly inspired by **scipy**'s own optimization submodule which should make the switch from one module to another straightforward.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/stochopy/master/.github/sample.gif
    :alt: sample-pso
    :width: 100%
    :align: center
@@ -138,12 +138,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/stochopy.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/stochopy
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4058008.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.4058008
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/Python%20package
+.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/ci.yml
    :target: https://github.com/keurfonluu/stochopy
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/stochopy/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/stochopy/doc.yml?label=docs
    :target: https://keurfonluu.github.io/stochopy/
```

### Comparing `stochopy-2.2.0/examples/basic_usage.py` & `stochopy-2.3.0/examples/basic_usage.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/setup.cfg` & `stochopy-2.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 746f 6368 6f70 790d 0a76 6572   = stochopy..ver
-00000020: 7369 6f6e 203d 2032 2e32 2e30 0d0a 6175  sion = 2.2.0..au
-00000030: 7468 6f72 203d 204b 6575 7266 6f6e 204c  thor = Keurfon L
-00000040: 7575 0d0a 656d 6169 6c20 3d20 6b65 7572  uu..email = keur
-00000050: 666f 6e6c 7575 406f 7574 6c6f 6f6b 2e63  fonluu@outlook.c
-00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-00000070: 3d20 5079 7468 6f6e 206c 6962 7261 7279  = Python library
-00000080: 2066 6f72 2073 746f 6368 6173 7469 6320   for stochastic 
-00000090: 6e75 6d65 7269 6361 6c20 6f70 7469 6d69  numerical optimi
-000000a0: 7a61 7469 6f6e 0d0a 7572 6c20 3d20 6874  zation..url = ht
-000000b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000c0: 2f6b 6575 7266 6f6e 6c75 752f 7374 6f63  /keurfonluu/stoc
-000000d0: 686f 7079 0d0a 7072 6f6a 6563 745f 7572  hopy..project_ur
-000000e0: 6c73 203d 200d 0a09 436f 6465 3d68 7474  ls = ...Code=htt
-000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000100: 6b65 7572 666f 6e6c 7575 2f73 746f 6368  keurfonluu/stoch
-00000110: 6f70 790d 0a09 4973 7375 6573 3d68 7474  opy...Issues=htt
-00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000130: 6b65 7572 666f 6e6c 7575 2f73 746f 6368  keurfonluu/stoch
-00000140: 6f70 792f 6973 7375 6573 0d0a 6c6f 6e67  opy/issues..long
-00000150: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000160: 696c 653a 2052 4541 444d 452e 7273 740d  ile: README.rst.
-00000170: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000180: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000190: 2074 6578 742f 782d 7273 740d 0a6c 6963   text/x-rst..lic
-000001a0: 656e 7365 203d 2042 5344 2033 2d43 6c61  ense = BSD 3-Cla
-000001b0: 7573 6520 4c69 6365 6e73 650d 0a70 6c61  use License..pla
-000001c0: 7466 6f72 6d73 203d 2061 6e79 0d0a 636c  tforms = any..cl
-000001d0: 6173 7369 6669 6572 7320 3d20 0d0a 094c  assifiers = ...L
-000001e0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001f0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
-00000200: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-00000210: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000220: 6e64 6570 656e 6465 6e74 0d0a 0944 6576  ndependent...Dev
-00000230: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000240: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-00000250: 6e2f 5374 6162 6c65 0d0a 0950 726f 6772  n/Stable...Progr
-00000260: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000270: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e36  :: Python :: 3.6
-00000280: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000290: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002a0: 6e20 3a3a 2033 2e37 0d0a 0950 726f 6772  n :: 3.7...Progr
-000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000002d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002f0: 6e20 3a3a 2033 2e39 0d0a 0d0a 5b6f 7074  n :: 3.9....[opt
-00000300: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
-00000310: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
-00000320: 5f72 6571 7569 7265 7320 3d20 0d0a 0969  _requires = ...i
-00000330: 6d70 6f72 746c 6962 5f6d 6574 6164 6174  mportlib_metadat
-00000340: 610d 0a09 6e75 6d70 790d 0a09 6a6f 626c  a...numpy...jobl
-00000350: 6962 203e 3d20 302e 3132 0d0a 7079 7468  ib >= 0.12..pyth
-00000360: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000370: 2033 2e36 0d0a 7365 7475 705f 7265 7175   3.6..setup_requ
-00000380: 6972 6573 203d 200d 0a09 7365 7475 7074  ires = ...setupt
-00000390: 6f6f 6c73 203e 3d20 3432 0d0a 0977 6865  ools >= 42...whe
-000003a0: 656c 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  el....[egg_info]
-000003b0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000003c0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000020: 7369 6f6e 203d 2066 696c 653a 2073 746f  sion = file: sto
+00000030: 6368 6f70 792f 5645 5253 494f 4e0d 0a61  chopy/VERSION..a
+00000040: 7574 686f 7220 3d20 4b65 7572 666f 6e20  uthor = Keurfon 
+00000050: 4c75 750d 0a65 6d61 696c 203d 206b 6575  Luu..email = keu
+00000060: 7266 6f6e 6c75 7540 6f75 746c 6f6f 6b2e  rfonluu@outlook.
+00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
+00000080: 203d 2050 7974 686f 6e20 6c69 6272 6172   = Python librar
+00000090: 7920 666f 7220 7374 6f63 6861 7374 6963  y for stochastic
+000000a0: 206e 756d 6572 6963 616c 206f 7074 696d   numerical optim
+000000b0: 697a 6174 696f 6e0d 0a75 726c 203d 2068  ization..url = h
+000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000d0: 6d2f 6b65 7572 666f 6e6c 7575 2f73 746f  m/keurfonluu/sto
+000000e0: 6368 6f70 790d 0a70 726f 6a65 6374 5f75  chopy..project_u
+000000f0: 726c 7320 3d20 0d0a 0943 6f64 653d 6874  rls = ...Code=ht
+00000100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000110: 2f6b 6575 7266 6f6e 6c75 752f 7374 6f63  /keurfonluu/stoc
+00000120: 686f 7079 0d0a 0949 7373 7565 733d 6874  hopy...Issues=ht
+00000130: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000140: 2f6b 6575 7266 6f6e 6c75 752f 7374 6f63  /keurfonluu/stoc
+00000150: 686f 7079 2f69 7373 7565 730d 0a6c 6f6e  hopy/issues..lon
+00000160: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00000170: 6669 6c65 3a20 5245 4144 4d45 2e72 7374  file: README.rst
+00000180: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000190: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000001a0: 3d20 7465 7874 2f78 2d72 7374 0d0a 6c69  = text/x-rst..li
+000001b0: 6365 6e73 6520 3d20 4253 4420 332d 436c  cense = BSD 3-Cl
+000001c0: 6175 7365 204c 6963 656e 7365 0d0a 706c  ause License..pl
+000001d0: 6174 666f 726d 7320 3d20 616e 790d 0a63  atforms = any..c
+000001e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001f0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000200: 7070 726f 7665 6420 3a3a 2042 5344 204c  pproved :: BSD L
+00000210: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+00000220: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000230: 496e 6465 7065 6e64 656e 740d 0a09 4465  Independent...De
+00000240: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000250: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+00000260: 6f6e 2f53 7461 626c 650d 0a09 5072 6f67  on/Stable...Prog
+00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000290: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
+000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002b0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
+000002c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002e0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000300: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000310: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000320: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000330: 2e31 310d 0a0d 0a5b 6f70 7469 6f6e 735d  .11....[options]
+00000340: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000350: 643a 0d0a 696e 7374 616c 6c5f 7265 7175  d:..install_requ
+00000360: 6972 6573 203d 200d 0a09 696d 706f 7274  ires = ...import
+00000370: 6c69 625f 6d65 7461 6461 7461 0d0a 096e  lib_metadata...n
+00000380: 756d 7079 0d0a 096a 6f62 6c69 6220 3e3d  umpy...joblib >=
+00000390: 2030 2e31 320d 0a70 7974 686f 6e5f 7265   0.12..python_re
+000003a0: 7175 6972 6573 203d 203e 3d20 332e 370d  quires = >= 3.7.
+000003b0: 0a73 6574 7570 5f72 6571 7569 7265 7320  .setup_requires 
+000003c0: 3d20 0d0a 0973 6574 7570 746f 6f6c 7320  = ...setuptools 
+000003d0: 3e3d 2034 320d 0a09 7768 6565 6c0d 0a0d  >= 42...wheel...
+000003e0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000003f0: 655f 6461 7461 5d0d 0a73 746f 6368 6f70  e_data]..stochop
+00000400: 7920 3d20 0d0a 0956 4552 5349 4f4e 0d0a  y = ...VERSION..
+00000410: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000420: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000430: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `stochopy-2.2.0/stochopy/_common.py` & `stochopy-2.3.0/stochopy/_common.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/factory/benchmark.py` & `stochopy-2.3.0/stochopy/factory/benchmark.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/optimize/__pycache__/_helpers.cpython-38.pyc` & `stochopy-2.3.0/stochopy/optimize/_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,248 +1,238 @@
-00000000: 550d 0d0a 0000 0000 ca4a 9b61 930e 0000  U........J.a....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 6701 5a02  d.l.m.Z...d.g.Z.
-00000040: 6900 5a03 4700 6403 6404 8400 6404 6501  i.Z.G.d.d...d.e.
-00000050: 8303 5a04 6405 6406 8400 5a05 640b 640a  ..Z.d.d...Z.d.d.
-00000060: 6402 8401 5a06 6407 5300 290c e902 0000  d...Z.d.S.).....
-00000070: 0029 01da 0a42 6173 6552 6573 756c 74da  .)...BaseResult.
-00000080: 086d 696e 696d 697a 6563 0000 0000 0000  .minimizec......
-00000090: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-000000a0: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000000b0: 015a 0364 0253 0029 03da 0e4f 7074 696d  .Z.d.S.)...Optim
-000000c0: 697a 6552 6573 756c 7461 9102 0000 0a20  izeResulta..... 
-000000d0: 2020 2052 6570 7265 7365 6e74 2074 6865     Represent the
-000000e0: 206f 7074 696d 697a 6174 696f 6e20 7265   optimization re
-000000f0: 7375 6c74 2e0a 0a20 2020 2041 7474 7269  sult...    Attri
-00000100: 6275 7465 730a 2020 2020 2d2d 2d2d 2d2d  butes.    ------
-00000110: 2d2d 2d2d 0a20 2020 2078 203a 2061 7272  ----.    x : arr
-00000120: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
-00000130: 5468 6520 736f 6c75 7469 6f6e 206f 6620  The solution of 
-00000140: 7468 6520 6f70 7469 6d69 7a61 7469 6f6e  the optimization
-00000150: 2e0a 2020 2020 7375 6363 6573 7320 3a20  ..    success : 
-00000160: 626f 6f6c 0a20 2020 2020 2020 2057 6865  bool.        Whe
-00000170: 7468 6572 206f 7220 6e6f 7420 7468 6520  ther or not the 
-00000180: 6f70 7469 6d69 7a65 7220 6578 6974 6564  optimizer exited
-00000190: 2073 7563 6365 7373 6675 6c6c 792e 0a20   successfully.. 
-000001a0: 2020 2073 7461 7475 7320 3a20 696e 740a     status : int.
-000001b0: 2020 2020 2020 2020 5465 726d 696e 6174          Terminat
-000001c0: 696f 6e20 7374 6174 7573 206f 6620 7468  ion status of th
-000001d0: 6520 6f70 7469 6d69 7a65 722e 2049 7473  e optimizer. Its
-000001e0: 2076 616c 7565 2064 6570 656e 6473 206f   value depends o
-000001f0: 6e20 7468 6520 756e 6465 726c 7969 6e67  n the underlying
-00000200: 2073 6f6c 7665 722e 2052 6566 6572 2074   solver. Refer t
-00000210: 6f20 6d65 7373 6167 6520 666f 7220 6465  o message for de
-00000220: 7461 696c 732e 0a20 2020 206d 6573 7361  tails..    messa
-00000230: 6765 203a 2073 7472 0a20 2020 2020 2020  ge : str.       
-00000240: 2044 6573 6372 6970 7469 6f6e 206f 6620   Description of 
-00000250: 7468 6520 6361 7573 6520 6f66 2074 6865  the cause of the
-00000260: 2074 6572 6d69 6e61 7469 6f6e 2e0a 2020   termination..  
-00000270: 2020 6675 6e20 3a20 7363 616c 6172 0a20    fun : scalar. 
-00000280: 2020 2020 2020 2054 6865 2073 6f6c 7574         The solut
-00000290: 696f 6e20 6675 6e63 7469 6f6e 2076 616c  ion function val
-000002a0: 7565 2e0a 2020 2020 6e69 7420 3a20 696e  ue..    nit : in
-000002b0: 740a 2020 2020 2020 2020 4e75 6d62 6572  t.        Number
-000002c0: 206f 6620 6974 6572 6174 696f 6e73 2070   of iterations p
-000002d0: 6572 666f 726d 6564 2062 7920 7468 6520  erformed by the 
-000002e0: 6f70 7469 6d69 7a65 722e 0a0a 2020 2020  optimizer...    
-000002f0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
-00000300: 2020 2020 5468 6572 6520 6d61 7920 6265      There may be
-00000310: 2061 6464 6974 696f 6e61 6c20 6174 7472   additional attr
-00000320: 6962 7574 6573 206e 6f74 206c 6973 7465  ibutes not liste
-00000330: 6420 6162 6f76 6520 6465 7065 6e64 696e  d above dependin
-00000340: 6720 6f66 2074 6865 2073 7065 6369 6669  g of the specifi
-00000350: 6320 736f 6c76 6572 2e0a 0a20 2020 204e  c solver...    N
-00000360: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000370: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000380: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fa9  name__..__doc__.
-00000390: 0072 0900 0000 7209 0000 00fa 3c63 3a5c  .r....r.....<c:\
-000003a0: 5573 6572 735c 6b65 7572 665c 4769 7448  Users\keurf\GitH
-000003b0: 7562 5c73 746f 6368 6f70 795c 7374 6f63  ub\stochopy\stoc
-000003c0: 686f 7079 5c6f 7074 696d 697a 655c 5f68  hopy\optimize\_h
-000003d0: 656c 7065 7273 2e70 7972 0400 0000 0b00  elpers.pyr......
-000003e0: 0000 7304 0000 0008 0104 1872 0400 0000  ..s........r....
-000003f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000400: 0003 0000 0043 0000 0073 0c00 0000 7c01  .....C...s....|.
-00000410: 7400 7c00 3c00 6401 5300 2902 7a19 5265  t.|.<.d.S.).z.Re
-00000420: 6769 7374 6572 2061 206e 6577 206f 7074  gister a new opt
-00000430: 696d 697a 6572 2e4e a901 da0e 5f6f 7074  imizer.N...._opt
-00000440: 696d 697a 6572 5f6d 6170 2902 da04 6e61  imizer_map)...na
-00000450: 6d65 7203 0000 0072 0900 0000 7209 0000  mer....r....r...
-00000460: 0072 0a00 0000 da08 7265 6769 7374 6572  .r......register
-00000470: 2700 0000 7302 0000 0000 0272 0e00 0000  '...s......r....
-00000480: 4e72 0900 0000 da02 6465 6307 0000 0000  Nr......dec.....
-00000490: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
-000004a0: 0000 0073 2a00 0000 7c05 7208 7c05 6e02  ...s*...|.r.|.n.
-000004b0: 6900 7d05 7400 7c04 1900 6600 7c00 7c01  i.}.t.|...f.|.|.
-000004c0: 7c02 7c03 7c06 6401 9c05 7c05 9702 8e01  |.|.|.d...|.....
-000004d0: 5300 2902 61a8 0900 000a 2020 2020 4d69  S.).a.....    Mi
-000004e0: 6e69 6d69 7a65 2061 6e20 6f62 6a65 6374  nimize an object
-000004f0: 6976 6520 6675 6e63 7469 6f6e 2075 7369  ive function usi
-00000500: 6e67 2061 2073 746f 6368 6173 7469 6320  ng a stochastic 
-00000510: 616c 676f 7269 7468 6d2e 0a0a 2020 2020  algorithm...    
-00000520: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000530: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6675  ---------.    fu
-00000540: 6e20 3a20 6361 6c6c 6162 6c65 0a20 2020  n : callable.   
-00000550: 2020 2020 2054 6865 206f 626a 6563 7469       The objecti
-00000560: 7665 2066 756e 6374 696f 6e20 746f 2062  ve function to b
-00000570: 6520 6d69 6e69 6d69 7a65 642e 204d 7573  e minimized. Mus
-00000580: 7420 6265 2069 6e20 7468 6520 666f 726d  t be in the form
-00000590: 2060 6066 2878 2c20 2a61 7267 7329 6060   ``f(x, *args)``
-000005a0: 2c20 7768 6572 6520 6060 7860 6020 6973  , where ``x`` is
-000005b0: 2074 6865 2061 7267 756d 656e 7420 696e   the argument in
-000005c0: 2074 6865 2066 6f72 6d20 6f66 2061 2031   the form of a 1
-000005d0: 2d44 2061 7272 6179 2061 6e64 2061 7267  -D array and arg
-000005e0: 7320 6973 2061 2074 7570 6c65 206f 6620  s is a tuple of 
-000005f0: 616e 7920 6164 6469 7469 6f6e 616c 2066  any additional f
-00000600: 6978 6564 2070 6172 616d 6574 6572 7320  ixed parameters 
-00000610: 6e65 6564 6564 2074 6f20 636f 6d70 6c65  needed to comple
-00000620: 7465 6c79 2073 7065 6369 6679 2074 6865  tely specify the
-00000630: 2066 756e 6374 696f 6e2e 0a20 2020 2062   function..    b
-00000640: 6f75 6e64 7320 3a20 6172 7261 795f 6c69  ounds : array_li
-00000650: 6b65 0a20 2020 2020 2020 2042 6f75 6e64  ke.        Bound
-00000660: 7320 666f 7220 7661 7269 6162 6c65 732e  s for variables.
-00000670: 2060 6028 6d69 6e2c 206d 6178 2960 6020   ``(min, max)`` 
-00000680: 7061 6972 7320 666f 7220 6561 6368 2065  pairs for each e
-00000690: 6c65 6d65 6e74 2069 6e20 6060 7860 602c  lement in ``x``,
-000006a0: 2064 6566 696e 696e 6720 7468 6520 6669   defining the fi
-000006b0: 6e69 7465 206c 6f77 6572 2061 6e64 2075  nite lower and u
-000006c0: 7070 6572 2062 6f75 6e64 7320 666f 7220  pper bounds for 
-000006d0: 7468 6520 6f70 7469 6d69 7a69 6e67 2061  the optimizing a
-000006e0: 7267 756d 656e 7420 6f66 2060 6066 756e  rgument of ``fun
-000006f0: 6060 2e20 4974 2069 7320 7265 7175 6972  ``. It is requir
-00000700: 6564 2074 6f20 6861 7665 2060 606c 656e  ed to have ``len
-00000710: 2862 6f75 6e64 7329 203d 3d20 6c65 6e28  (bounds) == len(
-00000720: 7829 6060 2e20 6060 6c65 6e28 626f 756e  x)``. ``len(boun
-00000730: 6473 2960 6020 6973 2075 7365 6420 746f  ds)`` is used to
-00000740: 2064 6574 6572 6d69 6e65 2074 6865 206e   determine the n
-00000750: 756d 6265 7220 6f66 2070 6172 616d 6574  umber of paramet
-00000760: 6572 7320 696e 2060 6078 6060 2e0a 2020  ers in ``x``..  
-00000770: 2020 7830 203a 2061 7272 6179 5f6c 696b    x0 : array_lik
-00000780: 6520 6f72 204e 6f6e 652c 206f 7074 696f  e or None, optio
-00000790: 6e61 6c2c 2064 6566 6175 6c74 204e 6f6e  nal, default Non
-000007a0: 650a 2020 2020 2020 2020 496e 6974 6961  e.        Initia
-000007b0: 6c20 6775 6573 732e 2044 6570 656e 6469  l guess. Dependi
-000007c0: 6e67 206f 6e20 7468 6520 736f 6c76 6572  ng on the solver
-000007d0: 2c20 6172 7261 7920 6f66 2072 6561 6c20  , array of real 
-000007e0: 656c 656d 656e 7473 206f 6620 7369 7a65  elements of size
-000007f0: 2028 6060 6e64 696d 6060 2c29 206f 7220   (``ndim``,) or 
-00000800: 7769 7468 2073 6861 7065 2028 6060 706f  with shape (``po
-00000810: 7073 697a 6560 602c 2060 606e 6469 6d60  psize``, ``ndim`
-00000820: 6029 2c20 7768 6572 6520 6060 6e64 696d  `), where ``ndim
-00000830: 6060 2069 7320 7468 6520 6e75 6d62 6572  `` is the number
-00000840: 206f 6620 696e 6465 7065 6e64 656e 7420   of independent 
-00000850: 7661 7269 6162 6c65 7320 616e 6420 6060  variables and ``
-00000860: 706f 7073 697a 6560 6020 6973 2074 6865  popsize`` is the
-00000870: 2074 6f74 616c 2070 6f70 756c 6174 696f   total populatio
-00000880: 6e20 7369 7a65 2069 6620 7468 6520 736f  n size if the so
-00000890: 6c76 6572 2069 7320 706f 7075 6c61 7469  lver is populati
-000008a0: 6f6e 2d62 6173 6564 2e0a 2020 2020 6172  on-based..    ar
-000008b0: 6773 203a 2074 7570 6c65 2c20 6f70 7469  gs : tuple, opti
-000008c0: 6f6e 616c 2c20 6465 6661 756c 7420 4e6f  onal, default No
-000008d0: 6e65 0a20 2020 2020 2020 2045 7874 7261  ne.        Extra
-000008e0: 2061 7267 756d 656e 7473 2070 6173 7365   arguments passe
-000008f0: 6420 746f 2074 6865 206f 626a 6563 7469  d to the objecti
-00000900: 7665 2066 756e 6374 696f 6e2e 0a20 2020  ve function..   
-00000910: 206d 6574 686f 6420 3a20 7374 722c 206f   method : str, o
-00000920: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00000930: 2027 6465 270a 2020 2020 2020 2020 5479   'de'.        Ty
-00000940: 7065 206f 6620 736f 6c76 6572 2e20 5368  pe of solver. Sh
-00000950: 6f75 6c64 2062 6520 6f6e 6520 6f66 3a0a  ould be one of:.
-00000960: 0a20 2020 2020 2020 2020 2d20 2763 6d61  .         - 'cma
-00000970: 6573 270a 2020 2020 2020 2020 202d 2027  es'.         - '
-00000980: 6370 736f 270a 2020 2020 2020 2020 202d  cpso'.         -
-00000990: 2027 6465 270a 2020 2020 2020 2020 202d   'de'.         -
-000009a0: 2027 6e61 270a 2020 2020 2020 2020 202d   'na'.         -
-000009b0: 2027 7073 6f27 0a20 2020 2020 2020 2020   'pso'.         
-000009c0: 2d20 2776 6463 6d61 270a 0a20 2020 206f  - 'vdcma'..    o
-000009d0: 7074 696f 6e73 203a 2064 6963 7420 6f72  ptions : dict or
-000009e0: 204e 6f6e 652c 206f 7074 696f 6e61 6c2c   None, optional,
-000009f0: 2064 6566 6175 6c74 204e 6f6e 650a 2020   default None.  
-00000a00: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
-00000a10: 7279 206f 6620 736f 6c76 6572 206f 7074  ry of solver opt
-00000a20: 696f 6e73 2e20 416c 6c20 6d65 7468 6f64  ions. All method
-00000a30: 7320 6163 6365 7074 2074 6865 2066 6f6c  s accept the fol
-00000a40: 6c6f 7769 6e67 2067 656e 6572 6963 206f  lowing generic o
-00000a50: 7074 696f 6e73 3a0a 0a20 2020 2020 2020  ptions:..       
-00000a60: 2020 2d20 6d61 7869 7465 7220 2869 6e74    - maxiter (int
-00000a70: 293a 206d 6178 696d 756d 206e 756d 6265  ): maximum numbe
-00000a80: 7220 6f66 2069 7465 7261 7469 6f6e 7320  r of iterations 
-00000a90: 746f 2070 6572 666f 726d 0a20 2020 2020  to perform.     
-00000aa0: 2020 2020 2d20 7365 6564 2028 696e 7420      - seed (int 
-00000ab0: 6f72 204e 6f6e 6529 3a20 7365 6564 2066  or None): seed f
-00000ac0: 6f72 2072 616e 646f 6d20 6e75 6d62 6572  or random number
-00000ad0: 2067 656e 6572 6174 6f72 0a20 2020 2020   generator.     
-00000ae0: 2020 2020 2d20 7265 7475 726e 5f61 6c6c      - return_all
-00000af0: 2028 626f 6f6c 293a 2073 6574 2074 6f20   (bool): set to 
-00000b00: 5472 7565 2074 6f20 7265 7475 726e 2061  True to return a
-00000b10: 6e20 6172 7261 7920 6f66 2061 6c6c 2074  n array of all t
-00000b20: 6865 2073 6f6c 7574 696f 6e73 2061 7420  he solutions at 
-00000b30: 6561 6368 2069 7465 7261 7469 6f6e 2e0a  each iteration..
-00000b40: 0a20 2020 2063 616c 6c62 6163 6b20 3a20  .    callback : 
-00000b50: 6361 6c6c 6162 6c65 206f 7220 4e6f 6e65  callable or None
-00000b60: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
-00000b70: 756c 7420 4e6f 6e65 0a20 2020 2020 2020  ult None.       
-00000b80: 2043 616c 6c65 6420 6166 7465 7220 6561   Called after ea
-00000b90: 6368 2069 7465 7261 7469 6f6e 2e20 4974  ch iteration. It
-00000ba0: 2069 7320 6120 6361 6c6c 6162 6c65 2077   is a callable w
-00000bb0: 6974 6820 7468 6520 7369 676e 6174 7572  ith the signatur
-00000bc0: 6520 6060 6361 6c6c 6261 636b 2858 2c20  e ``callback(X, 
-00000bd0: 4f70 7469 6d69 7a65 5265 7375 6c74 2073  OptimizeResult s
-00000be0: 7461 7465 2960 602c 2077 6865 7265 2060  tate)``, where `
-00000bf0: 6058 6060 2069 7320 7468 6520 6375 7272  `X`` is the curr
-00000c00: 656e 7420 706f 7075 6c61 7469 6f6e 2061  ent population a
-00000c10: 6e64 2060 6073 7461 7465 6060 2069 7320  nd ``state`` is 
-00000c20: 6120 7061 7274 6961 6c20 3a63 6c61 7373  a partial :class
-00000c30: 3a60 7374 6f63 686f 7079 2e6f 7074 696d  :`stochopy.optim
-00000c40: 697a 652e 4f70 7469 6d69 7a65 5265 7375  ize.OptimizeResu
-00000c50: 6c74 6020 6f62 6a65 6374 2077 6974 6820  lt` object with 
-00000c60: 7468 6520 7361 6d65 2066 6965 6c64 7320  the same fields 
-00000c70: 6173 2074 6865 206f 6e65 7320 6672 6f6d  as the ones from
-00000c80: 2074 6865 2072 6574 7572 6e20 2865 7863   the return (exc
-00000c90: 6570 7420 6060 2273 7563 6365 7373 2260  ept ``"success"`
-00000ca0: 602c 2060 6022 7374 6174 7573 2260 6020  `, ``"status"`` 
-00000cb0: 616e 6420 6060 226d 6573 7361 6765 2260  and ``"message"`
-00000cc0: 6029 2e0a 0a20 2020 2052 6574 7572 6e73  `)...    Returns
-00000cd0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00000ce0: 203a 636c 6173 733a 6073 746f 6368 6f70   :class:`stochop
-00000cf0: 792e 6f70 7469 6d69 7a65 2e4f 7074 696d  y.optimize.Optim
-00000d00: 697a 6552 6573 756c 7460 0a20 2020 2020  izeResult`.     
-00000d10: 2020 2054 6865 206f 7074 696d 697a 6174     The optimizat
-00000d20: 696f 6e20 7265 7375 6c74 2072 6570 7265  ion result repre
-00000d30: 7365 6e74 6564 2061 7320 6120 3a63 6c61  sented as a :cla
-00000d40: 7373 3a60 7374 6f63 686f 7079 2e6f 7074  ss:`stochopy.opt
-00000d50: 696d 697a 652e 4f70 7469 6d69 7a65 5265  imize.OptimizeRe
-00000d60: 7375 6c74 602e 2049 6d70 6f72 7461 6e74  sult`. Important
-00000d70: 2061 7474 7269 6275 7465 7320 6172 653a   attributes are:
-00000d80: 0a0a 2020 2020 2020 2020 202d 2060 6078  ..         - ``x
-00000d90: 6060 3a20 7468 6520 736f 6c75 7469 6f6e  ``: the solution
-00000da0: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
-00000db0: 2d20 6060 6675 6e60 603a 2074 6865 2073  - ``fun``: the s
-00000dc0: 6f6c 7574 696f 6e20 6675 6e63 7469 6f6e  olution function
-00000dd0: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
-00000de0: 2d20 6060 7375 6363 6573 7360 603a 2061  - ``success``: a
-00000df0: 2042 6f6f 6c65 616e 2066 6c61 6720 696e   Boolean flag in
-00000e00: 6469 6361 7469 6e67 2069 6620 7468 6520  dicating if the 
-00000e10: 6f70 7469 6d69 7a65 7220 6578 6974 6564  optimizer exited
-00000e20: 2073 7563 6365 7373 6675 6c6c 790a 2020   successfully.  
-00000e30: 2020 2020 2020 202d 2060 606d 6573 7361         - ``messa
-00000e40: 6765 6060 3a20 6120 7374 7269 6e67 2077  ge``: a string w
-00000e50: 6869 6368 2064 6573 6372 6962 6573 2074  hich describes t
-00000e60: 6865 2063 6175 7365 206f 6620 7468 6520  he cause of the 
-00000e70: 7465 726d 696e 6174 696f 6e0a 0a20 2020  termination..   
-00000e80: 2029 05da 0366 756e da06 626f 756e 6473   )...fun..bounds
-00000e90: da02 7830 da04 6172 6773 da08 6361 6c6c  ..x0..args..call
-00000ea0: 6261 636b 720b 0000 0029 0772 1000 0000  backr....).r....
-00000eb0: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000ec0: 066d 6574 686f 64da 076f 7074 696f 6e73  .method..options
-00000ed0: 7214 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000ee0: 0a00 0000 7203 0000 002c 0000 0073 1400  ....r....,...s..
-00000ef0: 0000 002d 0c02 0801 0200 0200 0200 0200  ...-............
-00000f00: 02ff 0401 02ff 2905 4e72 0900 0000 720f  ......).Nr....r.
-00000f10: 0000 004e 4e29 07da 075f 636f 6d6d 6f6e  ...NN)..._common
-00000f20: 7202 0000 00da 075f 5f61 6c6c 5f5f 720c  r......__all__r.
-00000f30: 0000 0072 0400 0000 720e 0000 0072 0300  ...r....r....r..
-00000f40: 0000 7209 0000 0072 0900 0000 7209 0000  ..r....r....r...
-00000f50: 0072 0a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000f60: 0100 0000 730c 0000 000c 0302 ff04 0504  ....s...........
-00000f70: 0310 1c08 05                             .....
+00000000: 6672 6f6d 202e 2e5f 636f 6d6d 6f6e 2069  from .._common i
+00000010: 6d70 6f72 7420 4261 7365 5265 7375 6c74  mport BaseResult
+00000020: 0d0a 0d0a 5f5f 616c 6c5f 5f20 3d20 5b0d  ....__all__ = [.
+00000030: 0a20 2020 2022 6d69 6e69 6d69 7a65 222c  .    "minimize",
+00000040: 0d0a 5d0d 0a0d 0a0d 0a5f 6f70 7469 6d69  ..]......_optimi
+00000050: 7a65 725f 6d61 7020 3d20 7b7d 0d0a 0d0a  zer_map = {}....
+00000060: 0d0a 636c 6173 7320 4f70 7469 6d69 7a65  ..class Optimize
+00000070: 5265 7375 6c74 2842 6173 6552 6573 756c  Result(BaseResul
+00000080: 7429 3a0d 0a20 2020 2022 2222 0d0a 2020  t):..    """..  
+00000090: 2020 5265 7072 6573 656e 7420 7468 6520    Represent the 
+000000a0: 6f70 7469 6d69 7a61 7469 6f6e 2072 6573  optimization res
+000000b0: 756c 742e 0d0a 0d0a 2020 2020 4174 7472  ult.....    Attr
+000000c0: 6962 7574 6573 0d0a 2020 2020 2d2d 2d2d  ibutes..    ----
+000000d0: 2d2d 2d2d 2d2d 0d0a 2020 2020 7820 3a20  ------..    x : 
+000000e0: 6172 7261 795f 6c69 6b65 0d0a 2020 2020  array_like..    
+000000f0: 2020 2020 5468 6520 736f 6c75 7469 6f6e      The solution
+00000100: 206f 6620 7468 6520 6f70 7469 6d69 7a61   of the optimiza
+00000110: 7469 6f6e 2e0d 0a20 2020 2073 7563 6365  tion...    succe
+00000120: 7373 203a 2062 6f6f 6c0d 0a20 2020 2020  ss : bool..     
+00000130: 2020 2057 6865 7468 6572 206f 7220 6e6f     Whether or no
+00000140: 7420 7468 6520 6f70 7469 6d69 7a65 7220  t the optimizer 
+00000150: 6578 6974 6564 2073 7563 6365 7373 6675  exited successfu
+00000160: 6c6c 792e 0d0a 2020 2020 7374 6174 7573  lly...    status
+00000170: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
+00000180: 5465 726d 696e 6174 696f 6e20 7374 6174  Termination stat
+00000190: 7573 206f 6620 7468 6520 6f70 7469 6d69  us of the optimi
+000001a0: 7a65 722e 2049 7473 2076 616c 7565 2064  zer. Its value d
+000001b0: 6570 656e 6473 206f 6e20 7468 6520 756e  epends on the un
+000001c0: 6465 726c 7969 6e67 2073 6f6c 7665 722e  derlying solver.
+000001d0: 2052 6566 6572 2074 6f20 6d65 7373 6167   Refer to messag
+000001e0: 6520 666f 7220 6465 7461 696c 732e 0d0a  e for details...
+000001f0: 2020 2020 6d65 7373 6167 6520 3a20 7374      message : st
+00000200: 720d 0a20 2020 2020 2020 2044 6573 6372  r..        Descr
+00000210: 6970 7469 6f6e 206f 6620 7468 6520 6361  iption of the ca
+00000220: 7573 6520 6f66 2074 6865 2074 6572 6d69  use of the termi
+00000230: 6e61 7469 6f6e 2e0d 0a20 2020 2066 756e  nation...    fun
+00000240: 203a 2073 6361 6c61 720d 0a20 2020 2020   : scalar..     
+00000250: 2020 2054 6865 2073 6f6c 7574 696f 6e20     The solution 
+00000260: 6675 6e63 7469 6f6e 2076 616c 7565 2e0d  function value..
+00000270: 0a20 2020 206e 6974 203a 2069 6e74 0d0a  .    nit : int..
+00000280: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+00000290: 6620 6974 6572 6174 696f 6e73 2070 6572  f iterations per
+000002a0: 666f 726d 6564 2062 7920 7468 6520 6f70  formed by the op
+000002b0: 7469 6d69 7a65 722e 0d0a 0d0a 2020 2020  timizer.....    
+000002c0: 4e6f 7465 0d0a 2020 2020 2d2d 2d2d 0d0a  Note..    ----..
+000002d0: 2020 2020 5468 6572 6520 6d61 7920 6265      There may be
+000002e0: 2061 6464 6974 696f 6e61 6c20 6174 7472   additional attr
+000002f0: 6962 7574 6573 206e 6f74 206c 6973 7465  ibutes not liste
+00000300: 6420 6162 6f76 6520 6465 7065 6e64 696e  d above dependin
+00000310: 6720 6f66 2074 6865 2073 7065 6369 6669  g of the specifi
+00000320: 6320 736f 6c76 6572 2e0d 0a0d 0a20 2020  c solver.....   
+00000330: 2022 2222 0d0a 0d0a 2020 2020 7061 7373   """....    pass
+00000340: 0d0a 0d0a 0d0a 6465 6620 7265 6769 7374  ......def regist
+00000350: 6572 286e 616d 652c 206d 696e 696d 697a  er(name, minimiz
+00000360: 6529 3a0d 0a20 2020 2022 2222 5265 6769  e):..    """Regi
+00000370: 7374 6572 2061 206e 6577 206f 7074 696d  ster a new optim
+00000380: 697a 6572 2e22 2222 0d0a 2020 2020 5f6f  izer."""..    _o
+00000390: 7074 696d 697a 6572 5f6d 6170 5b6e 616d  ptimizer_map[nam
+000003a0: 655d 203d 206d 696e 696d 697a 650d 0a0d  e] = minimize...
+000003b0: 0a0d 0a64 6566 206d 696e 696d 697a 6528  ...def minimize(
+000003c0: 6675 6e2c 2062 6f75 6e64 732c 2078 303d  fun, bounds, x0=
+000003d0: 4e6f 6e65 2c20 6172 6773 3d28 292c 206d  None, args=(), m
+000003e0: 6574 686f 643d 2264 6522 2c20 6f70 7469  ethod="de", opti
+000003f0: 6f6e 733d 4e6f 6e65 2c20 6361 6c6c 6261  ons=None, callba
+00000400: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2022  ck=None):..    "
+00000410: 2222 0d0a 2020 2020 4d69 6e69 6d69 7a65  ""..    Minimize
+00000420: 2061 6e20 6f62 6a65 6374 6976 6520 6675   an objective fu
+00000430: 6e63 7469 6f6e 2075 7369 6e67 2061 2073  nction using a s
+00000440: 746f 6368 6173 7469 6320 616c 676f 7269  tochastic algori
+00000450: 7468 6d2e 0d0a 0d0a 2020 2020 5061 7261  thm.....    Para
+00000460: 6d65 7465 7273 0d0a 2020 2020 2d2d 2d2d  meters..    ----
+00000470: 2d2d 2d2d 2d2d 0d0a 2020 2020 6675 6e20  ------..    fun 
+00000480: 3a20 6361 6c6c 6162 6c65 0d0a 2020 2020  : callable..    
+00000490: 2020 2020 5468 6520 6f62 6a65 6374 6976      The objectiv
+000004a0: 6520 6675 6e63 7469 6f6e 2074 6f20 6265  e function to be
+000004b0: 206d 696e 696d 697a 6564 2e20 4d75 7374   minimized. Must
+000004c0: 2062 6520 696e 2074 6865 2066 6f72 6d20   be in the form 
+000004d0: 6060 6628 782c 202a 6172 6773 2960 602c  ``f(x, *args)``,
+000004e0: 2077 6865 7265 2060 6078 6060 2069 7320   where ``x`` is 
+000004f0: 7468 6520 6172 6775 6d65 6e74 2069 6e20  the argument in 
+00000500: 7468 6520 666f 726d 206f 6620 6120 312d  the form of a 1-
+00000510: 4420 6172 7261 7920 616e 6420 6172 6773  D array and args
+00000520: 2069 7320 6120 7475 706c 6520 6f66 2061   is a tuple of a
+00000530: 6e79 2061 6464 6974 696f 6e61 6c20 6669  ny additional fi
+00000540: 7865 6420 7061 7261 6d65 7465 7273 206e  xed parameters n
+00000550: 6565 6465 6420 746f 2063 6f6d 706c 6574  eeded to complet
+00000560: 656c 7920 7370 6563 6966 7920 7468 6520  ely specify the 
+00000570: 6675 6e63 7469 6f6e 2e0d 0a20 2020 2062  function...    b
+00000580: 6f75 6e64 7320 3a20 6172 7261 795f 6c69  ounds : array_li
+00000590: 6b65 0d0a 2020 2020 2020 2020 426f 756e  ke..        Boun
+000005a0: 6473 2066 6f72 2076 6172 6961 626c 6573  ds for variables
+000005b0: 2e20 6060 286d 696e 2c20 6d61 7829 6060  . ``(min, max)``
+000005c0: 2070 6169 7273 2066 6f72 2065 6163 6820   pairs for each 
+000005d0: 656c 656d 656e 7420 696e 2060 6078 6060  element in ``x``
+000005e0: 2c20 6465 6669 6e69 6e67 2074 6865 2066  , defining the f
+000005f0: 696e 6974 6520 6c6f 7765 7220 616e 6420  inite lower and 
+00000600: 7570 7065 7220 626f 756e 6473 2066 6f72  upper bounds for
+00000610: 2074 6865 206f 7074 696d 697a 696e 6720   the optimizing 
+00000620: 6172 6775 6d65 6e74 206f 6620 6060 6675  argument of ``fu
+00000630: 6e60 602e 2049 7420 6973 2072 6571 7569  n``. It is requi
+00000640: 7265 6420 746f 2068 6176 6520 6060 6c65  red to have ``le
+00000650: 6e28 626f 756e 6473 2920 3d3d 206c 656e  n(bounds) == len
+00000660: 2878 2960 602e 2060 606c 656e 2862 6f75  (x)``. ``len(bou
+00000670: 6e64 7329 6060 2069 7320 7573 6564 2074  nds)`` is used t
+00000680: 6f20 6465 7465 726d 696e 6520 7468 6520  o determine the 
+00000690: 6e75 6d62 6572 206f 6620 7061 7261 6d65  number of parame
+000006a0: 7465 7273 2069 6e20 6060 7860 602e 0d0a  ters in ``x``...
+000006b0: 2020 2020 7830 203a 2061 7272 6179 5f6c      x0 : array_l
+000006c0: 696b 6520 6f72 204e 6f6e 652c 206f 7074  ike or None, opt
+000006d0: 696f 6e61 6c2c 2064 6566 6175 6c74 204e  ional, default N
+000006e0: 6f6e 650d 0a20 2020 2020 2020 2049 6e69  one..        Ini
+000006f0: 7469 616c 2067 7565 7373 2e20 4465 7065  tial guess. Depe
+00000700: 6e64 696e 6720 6f6e 2074 6865 2073 6f6c  nding on the sol
+00000710: 7665 722c 2061 7272 6179 206f 6620 7265  ver, array of re
+00000720: 616c 2065 6c65 6d65 6e74 7320 6f66 2073  al elements of s
+00000730: 697a 6520 2860 606e 6469 6d60 602c 2920  ize (``ndim``,) 
+00000740: 6f72 2077 6974 6820 7368 6170 6520 2860  or with shape (`
+00000750: 6070 6f70 7369 7a65 6060 2c20 6060 6e64  `popsize``, ``nd
+00000760: 696d 6060 292c 2077 6865 7265 2060 606e  im``), where ``n
+00000770: 6469 6d60 6020 6973 2074 6865 206e 756d  dim`` is the num
+00000780: 6265 7220 6f66 2069 6e64 6570 656e 6465  ber of independe
+00000790: 6e74 2076 6172 6961 626c 6573 2061 6e64  nt variables and
+000007a0: 2060 6070 6f70 7369 7a65 6060 2069 7320   ``popsize`` is 
+000007b0: 7468 6520 746f 7461 6c20 706f 7075 6c61  the total popula
+000007c0: 7469 6f6e 2073 697a 6520 6966 2074 6865  tion size if the
+000007d0: 2073 6f6c 7665 7220 6973 2070 6f70 756c   solver is popul
+000007e0: 6174 696f 6e2d 6261 7365 642e 0d0a 2020  ation-based...  
+000007f0: 2020 6172 6773 203a 2074 7570 6c65 2c20    args : tuple, 
+00000800: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
+00000810: 7420 4e6f 6e65 0d0a 2020 2020 2020 2020  t None..        
+00000820: 4578 7472 6120 6172 6775 6d65 6e74 7320  Extra arguments 
+00000830: 7061 7373 6564 2074 6f20 7468 6520 6f62  passed to the ob
+00000840: 6a65 6374 6976 6520 6675 6e63 7469 6f6e  jective function
+00000850: 2e0d 0a20 2020 206d 6574 686f 6420 3a20  ...    method : 
+00000860: 7374 722c 206f 7074 696f 6e61 6c2c 2064  str, optional, d
+00000870: 6566 6175 6c74 2027 6465 270d 0a20 2020  efault 'de'..   
+00000880: 2020 2020 2054 7970 6520 6f66 2073 6f6c       Type of sol
+00000890: 7665 722e 2053 686f 756c 6420 6265 206f  ver. Should be o
+000008a0: 6e65 206f 663a 0d0a 0d0a 2020 2020 2020  ne of:....      
+000008b0: 2020 202d 2027 636d 6165 7327 0d0a 2020     - 'cmaes'..  
+000008c0: 2020 2020 2020 202d 2027 6370 736f 270d         - 'cpso'.
+000008d0: 0a20 2020 2020 2020 2020 2d20 2764 6527  .         - 'de'
+000008e0: 0d0a 2020 2020 2020 2020 202d 2027 6e61  ..         - 'na
+000008f0: 270d 0a20 2020 2020 2020 2020 2d20 2770  '..         - 'p
+00000900: 736f 270d 0a20 2020 2020 2020 2020 2d20  so'..         - 
+00000910: 2776 6463 6d61 270d 0a0d 0a20 2020 206f  'vdcma'....    o
+00000920: 7074 696f 6e73 203a 2064 6963 7420 6f72  ptions : dict or
+00000930: 204e 6f6e 652c 206f 7074 696f 6e61 6c2c   None, optional,
+00000940: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
+00000950: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
+00000960: 6172 7920 6f66 2073 6f6c 7665 7220 6f70  ary of solver op
+00000970: 7469 6f6e 732e 2041 6c6c 206d 6574 686f  tions. All metho
+00000980: 6473 2061 6363 6570 7420 7468 6520 666f  ds accept the fo
+00000990: 6c6c 6f77 696e 6720 6765 6e65 7269 6320  llowing generic 
+000009a0: 6f70 7469 6f6e 733a 0d0a 0d0a 2020 2020  options:....    
+000009b0: 2020 2020 202d 206d 6178 6974 6572 2028       - maxiter (
+000009c0: 696e 7429 3a20 6d61 7869 6d75 6d20 6e75  int): maximum nu
+000009d0: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+000009e0: 6e73 2074 6f20 7065 7266 6f72 6d0d 0a20  ns to perform.. 
+000009f0: 2020 2020 2020 2020 2d20 7365 6564 2028          - seed (
+00000a00: 696e 7420 6f72 204e 6f6e 6529 3a20 7365  int or None): se
+00000a10: 6564 2066 6f72 2072 616e 646f 6d20 6e75  ed for random nu
+00000a20: 6d62 6572 2067 656e 6572 6174 6f72 0d0a  mber generator..
+00000a30: 2020 2020 2020 2020 202d 2072 6574 7572           - retur
+00000a40: 6e5f 616c 6c20 2862 6f6f 6c29 3a20 7365  n_all (bool): se
+00000a50: 7420 746f 2054 7275 6520 746f 2072 6574  t to True to ret
+00000a60: 7572 6e20 616e 2061 7272 6179 206f 6620  urn an array of 
+00000a70: 616c 6c20 7468 6520 736f 6c75 7469 6f6e  all the solution
+00000a80: 7320 6174 2065 6163 6820 6974 6572 6174  s at each iterat
+00000a90: 696f 6e0d 0a20 2020 2020 2020 2020 2d20  ion..         - 
+00000aa0: 7665 7262 6f73 6974 793a 2066 7261 6374  verbosity: fract
+00000ab0: 696f 6e20 6f66 2070 6f70 756c 6174 696f  ion of populatio
+00000ac0: 6e20 746f 2063 6f6e 7369 6465 7220 696e  n to consider in
+00000ad0: 2060 7265 7475 726e 5f61 6c6c 600d 0a0d   `return_all`...
+00000ae0: 0a20 2020 2063 616c 6c62 6163 6b20 3a20  .    callback : 
+00000af0: 6361 6c6c 6162 6c65 206f 7220 4e6f 6e65  callable or None
+00000b00: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
+00000b10: 756c 7420 4e6f 6e65 0d0a 2020 2020 2020  ult None..      
+00000b20: 2020 4361 6c6c 6564 2061 6674 6572 2065    Called after e
+00000b30: 6163 6820 6974 6572 6174 696f 6e2e 2049  ach iteration. I
+00000b40: 7420 6973 2061 2063 616c 6c61 626c 6520  t is a callable 
+00000b50: 7769 7468 2074 6865 2073 6967 6e61 7475  with the signatu
+00000b60: 7265 2060 6063 616c 6c62 6163 6b28 582c  re ``callback(X,
+00000b70: 204f 7074 696d 697a 6552 6573 756c 7420   OptimizeResult 
+00000b80: 7374 6174 6529 6060 2c20 7768 6572 6520  state)``, where 
+00000b90: 6060 5860 6020 6973 2074 6865 2063 7572  ``X`` is the cur
+00000ba0: 7265 6e74 2070 6f70 756c 6174 696f 6e20  rent population 
+00000bb0: 616e 6420 6060 7374 6174 6560 6020 6973  and ``state`` is
+00000bc0: 2061 2070 6172 7469 616c 203a 636c 6173   a partial :clas
+00000bd0: 733a 6073 746f 6368 6f70 792e 6f70 7469  s:`stochopy.opti
+00000be0: 6d69 7a65 2e4f 7074 696d 697a 6552 6573  mize.OptimizeRes
+00000bf0: 756c 7460 206f 626a 6563 7420 7769 7468  ult` object with
+00000c00: 2074 6865 2073 616d 6520 6669 656c 6473   the same fields
+00000c10: 2061 7320 7468 6520 6f6e 6573 2066 726f   as the ones fro
+00000c20: 6d20 7468 6520 7265 7475 726e 2028 6578  m the return (ex
+00000c30: 6365 7074 2060 6022 7375 6363 6573 7322  cept ``"success"
+00000c40: 6060 2c20 6060 2273 7461 7475 7322 6060  ``, ``"status"``
+00000c50: 2061 6e64 2060 6022 6d65 7373 6167 6522   and ``"message"
+00000c60: 6060 292e 0d0a 0d0a 2020 2020 5265 7475  ``).....    Retu
+00000c70: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+00000c80: 0d0a 2020 2020 3a63 6c61 7373 3a60 7374  ..    :class:`st
+00000c90: 6f63 686f 7079 2e6f 7074 696d 697a 652e  ochopy.optimize.
+00000ca0: 4f70 7469 6d69 7a65 5265 7375 6c74 600d  OptimizeResult`.
+00000cb0: 0a20 2020 2020 2020 2054 6865 206f 7074  .        The opt
+00000cc0: 696d 697a 6174 696f 6e20 7265 7375 6c74  imization result
+00000cd0: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+00000ce0: 6120 3a63 6c61 7373 3a60 7374 6f63 686f  a :class:`stocho
+00000cf0: 7079 2e6f 7074 696d 697a 652e 4f70 7469  py.optimize.Opti
+00000d00: 6d69 7a65 5265 7375 6c74 602e 2049 6d70  mizeResult`. Imp
+00000d10: 6f72 7461 6e74 2061 7474 7269 6275 7465  ortant attribute
+00000d20: 7320 6172 653a 0d0a 0d0a 2020 2020 2020  s are:....      
+00000d30: 2020 202d 2060 6078 6060 3a20 7468 6520     - ``x``: the 
+00000d40: 736f 6c75 7469 6f6e 2061 7272 6179 0d0a  solution array..
+00000d50: 2020 2020 2020 2020 202d 2060 6066 756e           - ``fun
+00000d60: 6060 3a20 7468 6520 736f 6c75 7469 6f6e  ``: the solution
+00000d70: 2066 756e 6374 696f 6e20 7661 6c75 650d   function value.
+00000d80: 0a20 2020 2020 2020 2020 2d20 6060 7375  .         - ``su
+00000d90: 6363 6573 7360 603a 2061 2042 6f6f 6c65  ccess``: a Boole
+00000da0: 616e 2066 6c61 6720 696e 6469 6361 7469  an flag indicati
+00000db0: 6e67 2069 6620 7468 6520 6f70 7469 6d69  ng if the optimi
+00000dc0: 7a65 7220 6578 6974 6564 2073 7563 6365  zer exited succe
+00000dd0: 7373 6675 6c6c 790d 0a20 2020 2020 2020  ssfully..       
+00000de0: 2020 2d20 6060 6d65 7373 6167 6560 603a    - ``message``:
+00000df0: 2061 2073 7472 696e 6720 7768 6963 6820   a string which 
+00000e00: 6465 7363 7269 6265 7320 7468 6520 6361  describes the ca
+00000e10: 7573 6520 6f66 2074 6865 2074 6572 6d69  use of the termi
+00000e20: 6e61 7469 6f6e 0d0a 0d0a 2020 2020 2222  nation....    ""
+00000e30: 220d 0a20 2020 206f 7074 696f 6e73 203d  "..    options =
+00000e40: 206f 7074 696f 6e73 2069 6620 6f70 7469   options if opti
+00000e50: 6f6e 7320 656c 7365 207b 7d0d 0a0d 0a20  ons else {}.... 
+00000e60: 2020 2072 6574 7572 6e20 5f6f 7074 696d     return _optim
+00000e70: 697a 6572 5f6d 6170 5b6d 6574 686f 645d  izer_map[method]
+00000e80: 280d 0a20 2020 2020 2020 2066 756e 3d66  (..        fun=f
+00000e90: 756e 2c20 626f 756e 6473 3d62 6f75 6e64  un, bounds=bound
+00000ea0: 732c 2078 303d 7830 2c20 6172 6773 3d61  s, x0=x0, args=a
+00000eb0: 7267 732c 2063 616c 6c62 6163 6b3d 6361  rgs, callback=ca
+00000ec0: 6c6c 6261 636b 2c20 2a2a 6f70 7469 6f6e  llback, **option
+00000ed0: 730d 0a20 2020 2029 0d0a                 s..    )..
```

### Comparing `stochopy-2.2.0/stochopy/optimize/_common.py` & `stochopy-2.3.0/stochopy/optimize/_common.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/optimize/cmaes/_cmaes.py` & `stochopy-2.3.0/stochopy/optimize/cmaes/_cmaes.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     seed=None,
     xtol=1.0e-8,
     ftol=1.0e-8,
     constraints=None,
     workers=1,
     backend=None,
     return_all=False,
+    verbosity=1.0,
     callback=None,
 ):
     """
     Minimize an objective function using Covariance Matrix Adaptation - Evolution Strategy (CMA-ES).
 
     Parameters
     ----------
@@ -66,15 +67,17 @@
         Parallel backend to use when ``workers`` is not ``0`` or ``1``:
 
          - 'loky': disable threading
          - 'threading': enable threading
          - 'mpi': use MPI (uses :mod:`mpi4py`)
 
     return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+        Set to True to return an array with shape (``nit``, ``verbosity`` * ``popsize``, ``ndim``) of all the solutions at each iteration.
+    verbosity : float, optional, default 1.0
+        Fraction of population to consider in `return_all`. If 0.0, returns the best solution at each iteration.
     callback : callable or None, optional, default None
         Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
 
     Returns
     -------
     :class:`stochopy.optimize.OptimizeResult`
         The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
@@ -125,14 +128,15 @@
         popsize,
         sigma,
         muperc,
         constraints,
         xtol,
         ftol,
         return_all,
+        verbosity,
         callback,
     )
     res = cmaes(fun, args, True, workers, backend, *optargs)
 
     return res
 
 
@@ -149,14 +153,15 @@
     popsize,
     sigma,
     muperc,
     constraints,
     xtol,
     ftol,
     return_all,
+    verbosity,
     callback,
 ):
     """Optimize with CMA-ES."""
     ndim = len(bounds)
     lower, upper = np.transpose(bounds)
 
     # Standardize and unstandardize
@@ -193,24 +198,25 @@
     # Initialize dynamic (internal) strategy parameters and constants
     pc = np.zeros(ndim)
     ps = np.zeros(ndim)
     B = np.eye(ndim)
     D = np.ones(ndim)
     C = np.eye(ndim)
     invsqrtC = np.eye(ndim)
-    chind = np.sqrt(ndim) * (1.0 - 1.0 / (4.0 * ndim) + 1.0 / (21.0 * ndim ** 2))
+    chind = np.sqrt(ndim) * (1.0 - 1.0 / (4.0 * ndim) + 1.0 / (21.0 * ndim**2))
 
     # Initialize boundaries weights
     bnd_weights = np.zeros(ndim)
     dfithist = np.ones(1)
 
     # Initialize arrays
     if return_all:
-        xall = np.empty((maxiter, popsize, ndim))
-        funall = np.empty((maxiter, popsize))
+        nout = int(np.ceil(verbosity * popsize))
+        xall = np.empty((maxiter, max(1, nout), ndim))
+        funall = np.empty((maxiter, max(1, nout)))
 
     # (mu, lambda)-CMA-ES
     nfev = 0
     eigeneval = 0
     arbestfitness = np.zeros(maxiter)
     ilim = int(10.0 + 30.0 * ndim / popsize)
     insigma = sigma
@@ -249,16 +255,22 @@
                 fun,
             )
         else:
             arfitness = fun(arxvalid)
         nfev += popsize
 
         if return_all:
-            xall[it - 1] = unstandardize(arxvalid)
-            funall[it - 1] = arfitness.copy()
+            if nout > 0:
+                xall[it - 1] = unstandardize(arxvalid[:nout])
+                funall[it - 1] = arfitness[:nout].copy()
+
+            else:
+                idx = arfitness.argmin()
+                xall[it - 1] = unstandardize(arxvalid[idx])
+                funall[it - 1] = arfitness[idx].copy()
 
         # Sort by fitness and compute weighted mean into xmean
         arindex = np.argsort(arfitness)
         xold = xmean.copy()
         xmean = np.dot(weights, arx[arindex[:mu], :])
 
         # Save best fitness
```

### Comparing `stochopy-2.2.0/stochopy/optimize/cmaes/_constraints.py` & `stochopy-2.3.0/stochopy/optimize/cmaes/_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # Clip to boundaries
     arxvalid = np.where(arxvalid < -1.0, -ones, arxvalid)
     arxvalid = np.where(arxvalid > 1.0, ones, arxvalid)
     arfitness = fun(arxvalid)
 
     # Get delta fitness values
     perc = np.percentile(arfitness, [25.0, 75.0])
-    delta = (perc[1] - perc[0]) / ndim / diagC.mean() / sigma ** 2
+    delta = (perc[1] - perc[0]) / ndim / diagC.mean() / sigma**2
 
     # Catch non-sensible values
     if delta == 0:
         delta = dfithist[dfithist > 0.0].min()
     elif not validfitval:
         dfithist = np.empty(0)
         validfitval = True
```

### Comparing `stochopy-2.2.0/stochopy/optimize/cpso/_constraints.py` & `stochopy-2.3.0/stochopy/optimize/cpso/_constraints.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/optimize/cpso/_cpso.py` & `stochopy-2.3.0/stochopy/optimize/cpso/_cpso.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     xtol=1.0e-8,
     ftol=1.0e-8,
     constraints=None,
     updating="immediate",
     workers=1,
     backend=None,
     return_all=False,
+    verbosity=1.0,
     callback=None,
 ):
     """
     Minimize an objective function using Competitive Particle Swarm Optimization (CPSO).
 
     Parameters
     ----------
@@ -75,15 +76,17 @@
         Parallel backend to use when ``workers`` is not ``0`` or ``1``:
 
          - 'loky': disable threading
          - 'threading': enable threading
          - 'mpi': use MPI (uses :mod:`mpi4py`)
 
     return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+        Set to True to return an array with shape (``nit``, ``verbosity`` * ``popsize``, ``ndim``) of all the solutions at each iteration.
+    verbosity : float, optional, default 1.0
+        Fraction of population to consider in `return_all`. If 0.0, returns the best solution at each iteration.
     callback : callable or None, optional, default None
         Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
 
     Returns
     -------
     :class:`stochopy.optimize.OptimizeResult`
         The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
@@ -164,14 +167,15 @@
         c1,
         c2,
         gamma,
         constraints,
         xtol,
         ftol,
         return_all,
+        verbosity,
         callback,
     )
     res = cpso(fun, args, sync, workers, backend, *optargs)
 
     return res
 
 
@@ -190,14 +194,15 @@
     c1,
     c2,
     gamma,
     constraints,
     xtol,
     ftol,
     return_all,
+    verbosity,
     callback,
 ):
     """Optimize with CPSO."""
     ndim = len(bounds)
     lower, upper = np.transpose(bounds)
 
     # Constraints
@@ -222,18 +227,27 @@
     # Initial best solution
     gbidx = np.argmin(pbestfit)
     gfit = pbestfit[gbidx]
     gbest = X[gbidx].copy()
 
     # Initialize arrays
     if return_all:
-        xall = np.empty((maxiter, popsize, ndim))
-        funall = np.empty((maxiter, popsize))
-        xall[0] = X.copy()
-        funall[0] = pfit.copy()
+        nout = int(np.ceil(verbosity * popsize))
+
+        if nout > 0:
+            xall = np.empty((maxiter, nout, ndim))
+            funall = np.empty((maxiter, nout))
+            xall[0] = X[:nout].copy()
+            funall[0] = pfit[:nout].copy()
+
+        else:
+            xall = np.empty((maxiter, 1, ndim))
+            funall = np.empty((maxiter, 1))
+            xall[0] = gbest
+            funall[0] = gfit
 
     # First iteration for callback
     if callback is not None:
         res = OptimizeResult(x=gbest, fun=gfit, nfev=popsize, nit=1)
         if return_all:
             res.update({"xall": xall[:1], "funall": funall[:1]})
 
@@ -265,16 +279,22 @@
             xtol,
             ftol,
             fun,
             cons,
         )
 
         if return_all:
-            xall[it - 1] = X.copy()
-            funall[it - 1] = pfit.copy()
+            if nout > 0:
+                xall[it - 1] = X[:nout].copy()
+                funall[it - 1] = pfit[:nout].copy()
+
+            else:
+                idx = pfit.argmin()
+                xall[it - 1] = X[idx].copy()
+                funall[it - 1] = pfit[idx].copy()
 
         converged = status is not None
 
         if callback is not None:
             res = OptimizeResult(x=gbest, fun=gfit, nfev=it * popsize, nit=it)
             if return_all:
                 res.update({"xall": xall[:it], "funall": funall[:it]})
```

### Comparing `stochopy-2.2.0/stochopy/optimize/de/_constraints.py` & `stochopy-2.3.0/stochopy/optimize/de/_constraints.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/optimize/de/_de.py` & `stochopy-2.3.0/stochopy/optimize/de/_de.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     xtol=1.0e-8,
     ftol=1.0e-8,
     constraints=None,
     updating="immediate",
     workers=1,
     backend=None,
     return_all=False,
+    verbosity=1.0,
     callback=None,
 ):
     """
     Minimize an objective function using Differential Evolution (DE).
 
     Parameters
     ----------
@@ -79,15 +80,17 @@
         Parallel backend to use when ``workers`` is not ``0`` or ``1``:
 
          - 'loky': disable threading
          - 'threading': enable threading
          - 'mpi': use MPI (uses :mod:`mpi4py`)
 
     return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+        Set to True to return an array with shape (``nit``, ``verbosity`` * ``popsize``, ``ndim``) of all the solutions at each iteration.
+    verbosity : float, optional, default 1.0
+        Fraction of population to consider in `return_all`. If 0.0, returns the best solution at each iteration.
     callback : callable or None, optional, default None
         Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
 
     Returns
     -------
     :class:`stochopy.optimize.OptimizeResult`
         The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
@@ -158,14 +161,15 @@
         F,
         CR,
         mut,
         constraints,
         xtol,
         ftol,
         return_all,
+        verbosity,
         callback,
     )
     res = de(fun, args, sync, workers, backend, *optargs)
 
     return res
 
 
@@ -183,14 +187,15 @@
     F,
     CR,
     mut,
     constraints,
     xtol,
     ftol,
     return_all,
+    verbosity,
     callback,
 ):
     """Optimize with DE."""
     ndim = len(bounds)
     lower, upper = np.transpose(bounds)
 
     # Constraints
@@ -210,18 +215,27 @@
     # Initial best solution
     gbidx = np.argmin(pbestfit)
     gfit = pbestfit[gbidx]
     gbest = X[gbidx].copy()
 
     # Initialize arrays
     if return_all:
-        xall = np.empty((maxiter, popsize, ndim))
-        funall = np.empty((maxiter, popsize))
-        xall[0] = X.copy()
-        funall[0] = pfit.copy()
+        nout = int(np.ceil(verbosity * popsize))
+
+        if nout > 0:
+            xall = np.empty((maxiter, nout, ndim))
+            funall = np.empty((maxiter, nout))
+            xall[0] = X[:nout].copy()
+            funall[0] = pfit[:nout].copy()
+
+        else:
+            xall = np.empty((maxiter, 1, ndim))
+            funall = np.empty((maxiter, 1))
+            xall[0] = gbest
+            funall[0] = gfit
 
     # First iteration for callback
     if callback is not None:
         res = OptimizeResult(x=gbest, fun=gfit, nfev=popsize, nit=1)
         if return_all:
             res.update({"xall": xall[:1], "funall": funall[:1]})
 
@@ -250,16 +264,22 @@
             ftol,
             fun,
             mut,
             cons,
         )
 
         if return_all:
-            xall[it - 1] = X.copy()
-            funall[it - 1] = pbestfit.copy()
+            if nout > 0:
+                xall[it - 1] = X[:nout].copy()
+                funall[it - 1] = pfit[:nout].copy()
+
+            else:
+                idx = pfit.argmin()
+                xall[it - 1] = X[idx].copy()
+                funall[it - 1] = pfit[idx].copy()
 
         converged = status is not None
 
         if callback is not None:
             res = OptimizeResult(x=gbest, fun=gfit, nfev=it * popsize, nit=it)
             if return_all:
                 res.update({"xall": xall[:it], "funall": funall[:it]})
@@ -278,20 +298,20 @@
     if return_all:
         res.update({"xall": xall[:it], "funall": funall[:it]})
 
     return res
 
 
 def delete_shuffle_sync(popsize):
-    """Delete current solution from population for mutation (synchronous)."""
+    """Delete current solution from population for mutation (synchroneous)."""
     return np.transpose([delete_shuffle_async(i, popsize) for i in range(popsize)])
 
 
 def delete_shuffle_async(i, popsize):
-    """Delete current solution from population for mutation (asynchronous)."""
+    """Delete current solution from population for mutation (asynchroneous)."""
     return np.random.permutation(np.delete(np.arange(popsize), i))
 
 
 def de_sync(
     it,
     X,
     U,
```

### Comparing `stochopy-2.2.0/stochopy/optimize/de/_strategy.py` & `stochopy-2.3.0/stochopy/optimize/de/_strategy.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy/optimize/na/_na.py` & `stochopy-2.3.0/stochopy/optimize/na/_na.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     nrperc=0.5,
     seed=None,
     xtol=1.0e-8,
     ftol=1.0e-8,
     workers=1,
     backend=None,
     return_all=False,
+    verbosity=1.0,
     callback=True,
 ):
     """
     Minimize an objective function using Neighborhood Algorithm (NA).
 
     Parameters
     ----------
@@ -55,15 +56,17 @@
         Parallel backend to use when ``workers`` is not ``0`` or ``1``:
 
          - 'loky': disable threading
          - 'threading': enable threading
          - 'mpi': use MPI (uses :mod:`mpi4py`)
 
     return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+        Set to True to return an array with shape (``nit``, ``verbosity`` * ``popsize``, ``ndim``) of all the solutions at each iteration.
+    verbosity : float, optional, default 1.0
+        Fraction of population to consider in `return_all`. If 0.0, returns the best solution at each iteration.
     callback : callable or None, optional, default None
         Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
 
     Returns
     -------
     :class:`stochopy.optimize.OptimizeResult`
         The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
@@ -116,14 +119,15 @@
         x0,
         maxiter,
         popsize,
         nrperc,
         xtol,
         ftol,
         return_all,
+        verbosity,
         callback,
     )
     res = na(fun, args, True, workers, backend, *optargs)
 
     return res
 
 
@@ -138,14 +142,15 @@
     x0,
     maxiter,
     popsize,
     nrperc,
     xtol,
     ftol,
     return_all,
+    verbosity,
     callback,
 ):
     """Optimize with Neighborhood Algorithm."""
     ndim = len(bounds)
     lower, upper = np.transpose(bounds)
 
     # Normalize and unnormalize
@@ -176,18 +181,27 @@
 
     # Store all models sampled
     Xall = X.copy()
     Xallfit = pfit.copy()
 
     # Initialize arrays
     if return_all:
-        xall = np.empty((maxiter, popsize, ndim))
-        funall = np.empty((maxiter, popsize))
-        xall[0] = unnormalize(X)
-        funall[0] = pfit.copy()
+        nout = int(np.ceil(verbosity * popsize))
+
+        if nout > 0:
+            xall = np.empty((maxiter, nout, ndim))
+            funall = np.empty((maxiter, nout))
+            xall[0] = X[:nout].copy()
+            funall[0] = pfit[:nout].copy()
+
+        else:
+            xall = np.empty((maxiter, 1, ndim))
+            funall = np.empty((maxiter, 1))
+            xall[0] = gbest
+            funall[0] = gfit
 
     # First iteration for callback
     if callback is not None:
         res = OptimizeResult(x=unnormalize(gbest), fun=gfit, nfev=popsize, nit=1)
         if return_all:
             res.update({"xall": xall[:1], "funall": funall[:1]})
 
@@ -206,22 +220,31 @@
         gbest, gfit, pfit, status = selection_sync(
             it, X, gbest, pbest, pbestfit, maxiter, xtol, ftol, fun
         )
         Xall = np.vstack((X, Xall))
         Xallfit = np.concatenate((pfit, Xallfit))
 
         if return_all:
-            xall[it - 1] = unnormalize(X)
-            funall[it - 1] = pfit.copy()
+            if nout > 0:
+                xall[it - 1] = unnormalize(X[:nout])
+                funall[it - 1] = pfit[:nout].copy()
+
+            else:
+                idx = pfit.argmin()
+                xall[it - 1] = unnormalize(X[idx])
+                funall[it - 1] = pfit[idx].copy()
 
         converged = status is not None
 
         if callback is not None:
             res = OptimizeResult(
-                x=unnormalize(gbest), fun=gfit, nfev=it * popsize, nit=it,
+                x=unnormalize(gbest),
+                fun=gfit,
+                nfev=it * popsize,
+                nit=it,
             )
             if return_all:
                 res.update({"xall": xall[:it], "funall": funall[:it]})
 
             callback(unnormalize(X), res)
 
     res = OptimizeResult(
```

### Comparing `stochopy-2.2.0/stochopy/optimize/pso/__pycache__/_pso.cpython-38.pyc` & `stochopy-2.3.0/stochopy/optimize/pso/_pso.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,329 +1,354 @@
-00000000: 550d 0d0a 0000 0000 7b41 9b61 4715 0000  U.......{A.aG...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0010 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6403 6701 5a04 6410 640e  m.Z...d.g.Z.d.d.
-00000050: 6403 8401 5a05 6503 640f 6505 8302 0100  d...Z.e.d.e.....
-00000060: 6404 5300 2911 e902 0000 00a9 01da 0463  d.S.)..........c
-00000070: 7073 6f29 01da 0872 6567 6973 7465 72da  pso)...register.
-00000080: 086d 696e 696d 697a 654e a900 e964 0000  .minimizeN...d..
-00000090: 00e9 0a00 0000 e798 dd93 8785 5ae7 3fe7  ............Z.?.
-000000a0: 55de 8e70 5af0 f73f e73a 8c30 e28e 7945  U..pZ..?.:.0..yE
-000000b0: 3eda 0969 6d6d 6564 6961 7465 e901 0000  >..immediate....
-000000c0: 0046 6312 0000 0000 0000 0000 0000 0013  .Fc.............
-000000d0: 0000 0014 0000 0043 0000 0073 3000 0000  .......C...s0...
-000000e0: 6401 7d12 7400 7c00 7c01 7c02 7c03 7c04  d.}.t.|.|.|.|.|.
-000000f0: 7c05 7c06 7c07 7c08 7c12 7c09 7c0a 7c0b  |.|.|.|.|.|.|.|.
-00000100: 7c0c 7c0d 7c0e 7c0f 7c10 7c11 8313 5300  |.|.|.|.|.|...S.
-00000110: 2902 618b 1100 000a 2020 2020 4d69 6e69  ).a.....    Mini
-00000120: 6d69 7a65 2061 6e20 6f62 6a65 6374 6976  mize an objectiv
-00000130: 6520 6675 6e63 7469 6f6e 2075 7369 6e67  e function using
-00000140: 2043 6f6d 7065 7469 7469 7665 2050 6172   Competitive Par
-00000150: 7469 636c 6520 5377 6172 6d20 4f70 7469  ticle Swarm Opti
-00000160: 6d69 7a61 7469 6f6e 2028 4350 534f 292e  mization (CPSO).
-00000170: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000180: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00000190: 2020 2020 6675 6e20 3a20 6361 6c6c 6162      fun : callab
-000001a0: 6c65 0a20 2020 2020 2020 2054 6865 206f  le.        The o
-000001b0: 626a 6563 7469 7665 2066 756e 6374 696f  bjective functio
-000001c0: 6e20 746f 2062 6520 6d69 6e69 6d69 7a65  n to be minimize
-000001d0: 642e 204d 7573 7420 6265 2069 6e20 7468  d. Must be in th
-000001e0: 6520 666f 726d 2060 6066 2878 2c20 2a61  e form ``f(x, *a
-000001f0: 7267 7329 6060 2c20 7768 6572 6520 6060  rgs)``, where ``
-00000200: 7860 6020 6973 2074 6865 2061 7267 756d  x`` is the argum
-00000210: 656e 7420 696e 2074 6865 2066 6f72 6d20  ent in the form 
-00000220: 6f66 2061 2031 2d44 2061 7272 6179 2061  of a 1-D array a
-00000230: 6e64 2061 7267 7320 6973 2061 2074 7570  nd args is a tup
-00000240: 6c65 206f 6620 616e 7920 6164 6469 7469  le of any additi
-00000250: 6f6e 616c 2066 6978 6564 2070 6172 616d  onal fixed param
-00000260: 6574 6572 7320 6e65 6564 6564 2074 6f20  eters needed to 
-00000270: 636f 6d70 6c65 7465 6c79 2073 7065 6369  completely speci
-00000280: 6679 2074 6865 2066 756e 6374 696f 6e2e  fy the function.
-00000290: 0a20 2020 2062 6f75 6e64 7320 3a20 6172  .    bounds : ar
-000002a0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-000002b0: 2042 6f75 6e64 7320 666f 7220 7661 7269   Bounds for vari
-000002c0: 6162 6c65 732e 2060 6028 6d69 6e2c 206d  ables. ``(min, m
-000002d0: 6178 2960 6020 7061 6972 7320 666f 7220  ax)`` pairs for 
-000002e0: 6561 6368 2065 6c65 6d65 6e74 2069 6e20  each element in 
-000002f0: 6060 7860 602c 2064 6566 696e 696e 6720  ``x``, defining 
-00000300: 7468 6520 6669 6e69 7465 206c 6f77 6572  the finite lower
-00000310: 2061 6e64 2075 7070 6572 2062 6f75 6e64   and upper bound
-00000320: 7320 666f 7220 7468 6520 6f70 7469 6d69  s for the optimi
-00000330: 7a69 6e67 2061 7267 756d 656e 7420 6f66  zing argument of
-00000340: 2060 6066 756e 6060 2e20 4974 2069 7320   ``fun``. It is 
-00000350: 7265 7175 6972 6564 2074 6f20 6861 7665  required to have
-00000360: 2060 606c 656e 2862 6f75 6e64 7329 203d   ``len(bounds) =
-00000370: 3d20 6c65 6e28 7829 6060 2e20 6060 6c65  = len(x)``. ``le
-00000380: 6e28 626f 756e 6473 2960 6020 6973 2075  n(bounds)`` is u
-00000390: 7365 6420 746f 2064 6574 6572 6d69 6e65  sed to determine
-000003a0: 2074 6865 206e 756d 6265 7220 6f66 2070   the number of p
-000003b0: 6172 616d 6574 6572 7320 696e 2060 6078  arameters in ``x
-000003c0: 6060 2e0a 2020 2020 7830 203a 2061 7272  ``..    x0 : arr
-000003d0: 6179 5f6c 696b 6520 6f72 204e 6f6e 652c  ay_like or None,
-000003e0: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-000003f0: 6c74 204e 6f6e 650a 2020 2020 2020 2020  lt None.        
-00000400: 496e 6974 6961 6c20 706f 7075 6c61 7469  Initial populati
-00000410: 6f6e 2e20 4172 7261 7920 6f66 2072 6561  on. Array of rea
-00000420: 6c20 656c 656d 656e 7473 2077 6974 6820  l elements with 
-00000430: 7368 6170 6520 2860 6070 6f70 7369 7a65  shape (``popsize
-00000440: 6060 2c20 6060 6e64 696d 6060 292c 2077  ``, ``ndim``), w
-00000450: 6865 7265 2060 606e 6469 6d60 6020 6973  here ``ndim`` is
-00000460: 2074 6865 206e 756d 6265 7220 6f66 2069   the number of i
-00000470: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00000480: 626c 6573 2e20 4966 2060 6078 3060 6020  bles. If ``x0`` 
-00000490: 6973 206e 6f74 2073 7065 6369 6669 6564  is not specified
-000004a0: 2c20 7468 6520 706f 7075 6c61 7469 6f6e  , the population
-000004b0: 2069 7320 696e 6974 6961 6c69 7a65 6420   is initialized 
-000004c0: 7573 696e 6720 4c61 7469 6e20 4879 7065  using Latin Hype
-000004d0: 7263 7562 6520 7361 6d70 6c69 6e67 2e0a  rcube sampling..
-000004e0: 2020 2020 6172 6773 203a 2074 7570 6c65      args : tuple
-000004f0: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
-00000500: 756c 7420 4e6f 6e65 0a20 2020 2020 2020  ult None.       
-00000510: 2045 7874 7261 2061 7267 756d 656e 7473   Extra arguments
-00000520: 2070 6173 7365 6420 746f 2074 6865 206f   passed to the o
-00000530: 626a 6563 7469 7665 2066 756e 6374 696f  bjective functio
-00000540: 6e2e 0a20 2020 206d 6178 6974 6572 203a  n..    maxiter :
-00000550: 2069 6e74 2c20 6f70 7469 6f6e 616c 2c20   int, optional, 
-00000560: 6465 6661 756c 7420 3130 300a 2020 2020  default 100.    
-00000570: 2020 2020 5468 6520 6d61 7869 6d75 6d20      The maximum 
-00000580: 6e75 6d62 6572 206f 6620 6765 6e65 7261  number of genera
-00000590: 7469 6f6e 7320 6f76 6572 2077 6869 6368  tions over which
-000005a0: 2074 6865 2065 6e74 6972 6520 706f 7075   the entire popu
-000005b0: 6c61 7469 6f6e 2069 7320 6576 6f6c 7665  lation is evolve
-000005c0: 642e 0a20 2020 2070 6f70 7369 7a65 203a  d..    popsize :
-000005d0: 2069 6e74 2c20 6f70 7469 6f6e 616c 2c20   int, optional, 
-000005e0: 6465 6661 756c 7420 3130 0a20 2020 2020  default 10.     
-000005f0: 2020 2054 6f74 616c 2070 6f70 756c 6174     Total populat
-00000600: 696f 6e20 7369 7a65 2e0a 2020 2020 696e  ion size..    in
-00000610: 6572 7469 6120 3a20 7363 616c 6172 2c20  ertia : scalar, 
-00000620: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00000630: 7420 302e 3732 3938 0a20 2020 2020 2020  t 0.7298.       
-00000640: 2049 6e65 7274 6961 6c20 7765 6967 6874   Inertial weight
-00000650: 2c20 6465 6e6f 7465 6420 6279 2077 2069  , denoted by w i
-00000660: 6e20 7468 6520 6c69 7465 7261 7475 7265  n the literature
-00000670: 2e20 4974 2073 686f 756c 6420 6265 2069  . It should be i
-00000680: 6e20 7468 6520 7261 6e67 6520 5b30 2c20  n the range [0, 
-00000690: 315d 2e0a 2020 2020 636f 676e 6974 6976  1]..    cognitiv
-000006a0: 6974 7920 3a20 7363 616c 6172 2c20 6f70  ity : scalar, op
-000006b0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-000006c0: 312e 3439 3631 380a 2020 2020 2020 2020  1.49618.        
-000006d0: 436f 676e 6974 696f 6e20 7061 7261 6d65  Cognition parame
-000006e0: 7465 722c 2064 656e 6f74 6564 2062 7920  ter, denoted by 
-000006f0: 6331 2069 6e20 7468 6520 6c69 7465 7261  c1 in the litera
-00000700: 7475 7265 2e20 4974 2073 686f 756c 6420  ture. It should 
-00000710: 6265 2069 6e20 7468 6520 7261 6e67 6520  be in the range 
-00000720: 5b30 2c20 345d 2e0a 2020 2020 736f 6369  [0, 4]..    soci
-00000730: 6162 696c 6974 793a 2073 6361 6c61 722c  ability: scalar,
-00000740: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-00000750: 6c74 2031 2e34 3936 3138 0a20 2020 2020  lt 1.49618.     
-00000760: 2020 2053 6f63 6961 6269 6c69 7479 2070     Sociability p
-00000770: 6172 616d 6574 6572 2c20 6465 6e6f 7465  arameter, denote
-00000780: 6420 6279 2063 3220 696e 2074 6865 206c  d by c2 in the l
-00000790: 6974 6572 6174 7572 652e 2049 7420 7368  iterature. It sh
-000007a0: 6f75 6c64 2062 6520 696e 2074 6865 2072  ould be in the r
-000007b0: 616e 6765 205b 302c 2034 5d2e 0a20 2020  ange [0, 4]..   
-000007c0: 2073 6565 6420 3a20 696e 7420 6f72 204e   seed : int or N
-000007d0: 6f6e 652c 206f 7074 696f 6e61 6c2c 2064  one, optional, d
-000007e0: 6566 6175 6c74 204e 6f6e 650a 2020 2020  efault None.    
-000007f0: 2020 2020 5365 6564 2066 6f72 2072 616e      Seed for ran
-00000800: 646f 6d20 6e75 6d62 6572 2067 656e 6572  dom number gener
-00000810: 6174 6f72 2e0a 2020 2020 7874 6f6c 203a  ator..    xtol :
-00000820: 2073 6361 6c61 722c 206f 7074 696f 6e61   scalar, optiona
-00000830: 6c2c 2064 6566 6175 6c74 2031 2e30 652d  l, default 1.0e-
-00000840: 380a 2020 2020 2020 2020 536f 6c75 7469  8.        Soluti
-00000850: 6f6e 2074 6f6c 6572 616e 6365 2066 6f72  on tolerance for
-00000860: 2074 6572 6d69 6e61 7469 6f6e 2e0a 2020   termination..  
-00000870: 2020 6674 6f6c 203a 2073 6361 6c61 722c    ftol : scalar,
-00000880: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-00000890: 6c74 2031 2e30 652d 380a 2020 2020 2020  lt 1.0e-8.      
-000008a0: 2020 4f62 6a65 6374 6976 6520 6675 6e63    Objective func
-000008b0: 7469 6f6e 2076 616c 7565 2074 6f6c 6572  tion value toler
-000008c0: 616e 6365 2066 6f72 2074 6572 6d69 6e61  ance for termina
-000008d0: 7469 6f6e 2e0a 2020 2020 636f 6e73 7472  tion..    constr
-000008e0: 6169 6e74 7320 3a20 7374 7220 6f72 204e  aints : str or N
-000008f0: 6f6e 652c 206f 7074 696f 6e61 6c2c 2064  one, optional, d
-00000900: 6566 6175 6c74 204e 6f6e 650a 2020 2020  efault None.    
-00000910: 2020 2020 436f 6e73 7472 6169 6e74 7320      Constraints 
-00000920: 6465 6669 6e69 7469 6f6e 3a0a 0a20 2020  definition:..   
-00000930: 2020 2020 2020 2d20 4e6f 6e65 3a20 6e6f        - None: no
-00000940: 2063 6f6e 7374 7261 696e 740a 2020 2020   constraint.    
-00000950: 2020 2020 202d 2027 5368 7269 6e6b 273a       - 'Shrink':
-00000960: 2069 6e66 6561 7369 626c 6520 736f 6c75   infeasible solu
-00000970: 7469 6f6e 7320 6172 6520 7265 7061 6972  tions are repair
-00000980: 6564 2062 7920 7368 7269 6e6b 696e 6720  ed by shrinking 
-00000990: 7061 7274 6963 6c65 7327 2076 656c 6f63  particles' veloc
-000009a0: 6974 7920 7665 6374 6f72 0a0a 2020 2020  ity vector..    
-000009b0: 7570 6461 7469 6e67 203a 2073 7472 207b  updating : str {
-000009c0: 2769 6d6d 6564 6961 7465 272c 2027 6465  'immediate', 'de
-000009d0: 6665 7272 6564 277d 2c20 6f70 7469 6f6e  ferred'}, option
-000009e0: 616c 2c20 6465 6661 756c 7420 2769 6d6d  al, default 'imm
-000009f0: 6564 6961 7465 270a 2020 2020 2020 2020  ediate'.        
-00000a00: 4966 2060 6027 696d 6d65 6469 6174 6527  If ``'immediate'
-00000a10: 6060 2c20 7468 6520 6265 7374 2073 6f6c  ``, the best sol
-00000a20: 7574 696f 6e20 7665 6374 6f72 2069 7320  ution vector is 
-00000a30: 636f 6e74 696e 756f 7573 6c79 2075 7064  continuously upd
-00000a40: 6174 6564 2077 6974 6869 6e20 6120 7369  ated within a si
-00000a50: 6e67 6c65 2067 656e 6572 6174 696f 6e2e  ngle generation.
-00000a60: 2054 6869 7320 6361 6e20 6c65 6164 2074   This can lead t
-00000a70: 6f20 6661 7374 6572 2063 6f6e 7665 7267  o faster converg
-00000a80: 656e 6365 2061 7320 6361 6e64 6964 6174  ence as candidat
-00000a90: 6520 736f 6c75 7469 6f6e 7320 6361 6e20  e solutions can 
-00000aa0: 7461 6b65 2061 6476 616e 7461 6765 206f  take advantage o
-00000ab0: 6620 636f 6e74 696e 756f 7573 2069 6d70  f continuous imp
-00000ac0: 726f 7665 6d65 6e74 7320 696e 2074 6865  rovements in the
-00000ad0: 2062 6573 7420 736f 6c75 7469 6f6e 2e20   best solution. 
-00000ae0: 5769 7468 2060 6027 6465 6665 7272 6564  With ``'deferred
-00000af0: 2760 602c 2074 6865 2062 6573 7420 736f  '``, the best so
-00000b00: 6c75 7469 6f6e 2076 6563 746f 7220 6973  lution vector is
-00000b10: 2075 7064 6174 6564 206f 6e63 6520 7065   updated once pe
-00000b20: 7220 6765 6e65 7261 7469 6f6e 2e20 4f6e  r generation. On
-00000b30: 6c79 2060 6027 6465 6665 7272 6564 2760  ly ``'deferred'`
-00000b40: 6020 6973 2063 6f6d 7061 7469 626c 6520  ` is compatible 
-00000b50: 7769 7468 2070 6172 616c 6c65 6c69 7a61  with paralleliza
-00000b60: 7469 6f6e 2c20 616e 6420 6973 206f 7665  tion, and is ove
-00000b70: 7272 6964 6465 6e20 7768 656e 2060 6077  rridden when ``w
-00000b80: 6f72 6b65 7273 6060 2069 7320 6e6f 7420  orkers`` is not 
-00000b90: 6060 3060 6020 6f72 2060 6031 6060 206f  ``0`` or ``1`` o
-00000ba0: 7220 6060 6261 636b 656e 6420 3d3d 2027  r ``backend == '
-00000bb0: 6d70 6927 6060 2e0a 2020 2020 776f 726b  mpi'``..    work
-00000bc0: 6572 7320 3a20 696e 742c 206f 7074 696f  ers : int, optio
-00000bd0: 6e61 6c2c 2064 6566 6175 6c74 2031 0a20  nal, default 1. 
-00000be0: 2020 2020 2020 2054 6865 2070 6f70 756c         The popul
-00000bf0: 6174 696f 6e20 6973 2073 7562 6469 7669  ation is subdivi
-00000c00: 6465 6420 696e 746f 2077 6f72 6b65 7273  ded into workers
-00000c10: 2073 6563 7469 6f6e 7320 616e 6420 6576   sections and ev
-00000c20: 616c 7561 7465 6420 696e 2070 6172 616c  aluated in paral
-00000c30: 6c65 6c20 2875 7365 7320 3a63 6c61 7373  lel (uses :class
-00000c40: 3a60 6a6f 626c 6962 2e50 6172 616c 6c65  :`joblib.Paralle
-00000c50: 6c60 292e 2053 7570 706c 7920 2d31 2074  l`). Supply -1 t
-00000c60: 6f20 7573 6520 616c 6c20 6176 6169 6c61  o use all availa
-00000c70: 626c 6520 4350 5520 636f 7265 732e 0a20  ble CPU cores.. 
-00000c80: 2020 2062 6163 6b65 6e64 203a 2073 7472     backend : str
-00000c90: 207b 276c 6f6b 7927 2c20 2774 6872 6561   {'loky', 'threa
-00000ca0: 6469 6e67 272c 2027 6d70 6927 7d2c 206f  ding', 'mpi'}, o
-00000cb0: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00000cc0: 2027 7468 7265 6164 696e 6727 0a20 2020   'threading'.   
-00000cd0: 2020 2020 2050 6172 616c 6c65 6c20 6261       Parallel ba
-00000ce0: 636b 656e 6420 746f 2075 7365 2077 6865  ckend to use whe
-00000cf0: 6e20 6060 776f 726b 6572 7360 6020 6973  n ``workers`` is
-00000d00: 206e 6f74 2060 6030 6060 206f 7220 6060   not ``0`` or ``
-00000d10: 3160 603a 0a0a 2020 2020 2020 2020 202d  1``:..         -
-00000d20: 2027 6c6f 6b79 273a 2064 6973 6162 6c65   'loky': disable
-00000d30: 2074 6872 6561 6469 6e67 0a20 2020 2020   threading.     
-00000d40: 2020 2020 2d20 2774 6872 6561 6469 6e67      - 'threading
-00000d50: 273a 2065 6e61 626c 6520 7468 7265 6164  ': enable thread
-00000d60: 696e 670a 2020 2020 2020 2020 202d 2027  ing.         - '
-00000d70: 6d70 6927 3a20 7573 6520 4d50 4920 2875  mpi': use MPI (u
-00000d80: 7365 7320 3a6d 6f64 3a60 6d70 6934 7079  ses :mod:`mpi4py
-00000d90: 6029 0a0a 2020 2020 7265 7475 726e 5f61  `)..    return_a
-00000da0: 6c6c 203a 2062 6f6f 6c2c 206f 7074 696f  ll : bool, optio
-00000db0: 6e61 6c2c 2064 6566 6175 6c74 2046 616c  nal, default Fal
-00000dc0: 7365 0a20 2020 2020 2020 2053 6574 2074  se.        Set t
-00000dd0: 6f20 5472 7565 2074 6f20 7265 7475 726e  o True to return
-00000de0: 2061 6e20 6172 7261 7920 7769 7468 2073   an array with s
-00000df0: 6861 7065 2028 6060 6e69 7460 602c 2060  hape (``nit``, `
-00000e00: 6070 6f70 7369 7a65 6060 2c20 6060 6e64  `popsize``, ``nd
-00000e10: 696d 6060 2920 6f66 2061 6c6c 2074 6865  im``) of all the
-00000e20: 2073 6f6c 7574 696f 6e73 2061 7420 6561   solutions at ea
-00000e30: 6368 2069 7465 7261 7469 6f6e 2e0a 2020  ch iteration..  
-00000e40: 2020 6361 6c6c 6261 636b 203a 2063 616c    callback : cal
-00000e50: 6c61 626c 6520 6f72 204e 6f6e 652c 206f  lable or None, o
-00000e60: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00000e70: 204e 6f6e 650a 2020 2020 2020 2020 4361   None.        Ca
-00000e80: 6c6c 6564 2061 6674 6572 2065 6163 6820  lled after each 
-00000e90: 6974 6572 6174 696f 6e2e 2049 7420 6973  iteration. It is
-00000ea0: 2061 2063 616c 6c61 626c 6520 7769 7468   a callable with
-00000eb0: 2074 6865 2073 6967 6e61 7475 7265 2060   the signature `
-00000ec0: 6063 616c 6c62 6163 6b28 582c 204f 7074  `callback(X, Opt
-00000ed0: 696d 697a 6552 6573 756c 7420 7374 6174  imizeResult stat
-00000ee0: 6529 6060 2c20 7768 6572 6520 6060 5860  e)``, where ``X`
-00000ef0: 6020 6973 2074 6865 2063 7572 7265 6e74  ` is the current
-00000f00: 2070 6f70 756c 6174 696f 6e20 616e 6420   population and 
-00000f10: 6060 7374 6174 6560 6020 6973 2061 2070  ``state`` is a p
-00000f20: 6172 7469 616c 203a 636c 6173 733a 6073  artial :class:`s
-00000f30: 746f 6368 6f70 792e 6f70 7469 6d69 7a65  tochopy.optimize
-00000f40: 2e4f 7074 696d 697a 6552 6573 756c 7460  .OptimizeResult`
-00000f50: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-00000f60: 2073 616d 6520 6669 656c 6473 2061 7320   same fields as 
-00000f70: 7468 6520 6f6e 6573 2066 726f 6d20 7468  the ones from th
-00000f80: 6520 7265 7475 726e 2028 6578 6365 7074  e return (except
-00000f90: 2060 6022 7375 6363 6573 7322 6060 2c20   ``"success"``, 
-00000fa0: 6060 2273 7461 7475 7322 6060 2061 6e64  ``"status"`` and
-00000fb0: 2060 6022 6d65 7373 6167 6522 6060 292e   ``"message"``).
-00000fc0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00000fd0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 3a63    -------.    :c
-00000fe0: 6c61 7373 3a60 7374 6f63 686f 7079 2e6f  lass:`stochopy.o
-00000ff0: 7074 696d 697a 652e 4f70 7469 6d69 7a65  ptimize.Optimize
-00001000: 5265 7375 6c74 600a 2020 2020 2020 2020  Result`.        
-00001010: 5468 6520 6f70 7469 6d69 7a61 7469 6f6e  The optimization
-00001020: 2072 6573 756c 7420 7265 7072 6573 656e   result represen
-00001030: 7465 6420 6173 2061 203a 636c 6173 733a  ted as a :class:
-00001040: 6073 746f 6368 6f70 792e 6f70 7469 6d69  `stochopy.optimi
-00001050: 7a65 2e4f 7074 696d 697a 6552 6573 756c  ze.OptimizeResul
-00001060: 7460 2e20 496d 706f 7274 616e 7420 6174  t`. Important at
-00001070: 7472 6962 7574 6573 2061 7265 3a0a 0a20  tributes are:.. 
-00001080: 2020 2020 2020 2020 2d20 6060 7860 603a          - ``x``:
-00001090: 2074 6865 2073 6f6c 7574 696f 6e20 6172   the solution ar
-000010a0: 7261 790a 2020 2020 2020 2020 202d 2060  ray.         - `
-000010b0: 6066 756e 6060 3a20 7468 6520 736f 6c75  `fun``: the solu
-000010c0: 7469 6f6e 2066 756e 6374 696f 6e20 7661  tion function va
-000010d0: 6c75 650a 2020 2020 2020 2020 202d 2060  lue.         - `
-000010e0: 6073 7563 6365 7373 6060 3a20 6120 426f  `success``: a Bo
-000010f0: 6f6c 6561 6e20 666c 6167 2069 6e64 6963  olean flag indic
-00001100: 6174 696e 6720 6966 2074 6865 206f 7074  ating if the opt
-00001110: 696d 697a 6572 2065 7869 7465 6420 7375  imizer exited su
-00001120: 6363 6573 7366 756c 6c79 0a20 2020 2020  ccessfully.     
-00001130: 2020 2020 2d20 6060 6d65 7373 6167 6560      - ``message`
-00001140: 603a 2061 2073 7472 696e 6720 7768 6963  `: a string whic
-00001150: 6820 6465 7363 7269 6265 7320 7468 6520  h describes the 
-00001160: 6361 7573 6520 6f66 2074 6865 2074 6572  cause of the ter
-00001170: 6d69 6e61 7469 6f6e 0a0a 2020 2020 5265  mination..    Re
-00001180: 6665 7265 6e63 6573 0a20 2020 202d 2d2d  ferences.    ---
-00001190: 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e 205b  -------.    .. [
-000011a0: 315d 204a 2e20 4b65 6e6e 6564 7920 616e  1] J. Kennedy an
-000011b0: 6420 522e 2045 6265 7268 6172 742c 202a  d R. Eberhart, *
-000011c0: 5061 7274 6963 6c65 2073 7761 726d 206f  Particle swarm o
-000011d0: 7074 696d 697a 6174 696f 6e2a 2c20 5072  ptimization*, Pr
-000011e0: 6f63 6565 6469 6e67 7320 6f66 2049 434e  oceedings of ICN
-000011f0: 4e27 3935 202d 2049 6e74 6572 6e61 7469  N'95 - Internati
-00001200: 6f6e 616c 2043 6f6e 6665 7265 6e63 6520  onal Conference 
-00001210: 6f6e 204e 6575 7261 6c20 4e65 7477 6f72  on Neural Networ
-00001220: 6b73 2c20 3139 3935 2c20 343a 2031 3934  ks, 1995, 4: 194
-00001230: 322d 3139 3438 0a20 2020 202e 2e20 5b32  2-1948.    .. [2
-00001240: 5d20 462e 2056 616e 2044 656e 2042 6572  ] F. Van Den Ber
-00001250: 6768 2c20 2a41 6e20 616e 616c 7973 6973  gh, *An analysis
-00001260: 206f 6620 7061 7274 6963 6c65 2073 7761   of particle swa
-00001270: 726d 206f 7074 696d 697a 6572 732a 2c20  rm optimizers*, 
-00001280: 556e 6976 6572 7369 7479 206f 6620 5072  University of Pr
-00001290: 6574 6f72 6961 2c20 3230 3031 0a0a 2020  etoria, 2001..  
-000012a0: 2020 4e72 0200 0000 2913 da03 6675 6eda    Nr....)...fun.
-000012b0: 0662 6f75 6e64 73da 0278 30da 0461 7267  .bounds..x0..arg
-000012c0: 73da 076d 6178 6974 6572 da07 706f 7073  s..maxiter..pops
-000012d0: 697a 65da 0769 6e65 7274 6961 da0b 636f  ize..inertia..co
-000012e0: 676e 6974 6976 6974 79da 0b73 6f63 6961  gnitivity..socia
-000012f0: 6269 6c69 7479 da04 7365 6564 da04 7874  bility..seed..xt
-00001300: 6f6c da04 6674 6f6c da0b 636f 6e73 7472  ol..ftol..constr
-00001310: 6169 6e74 73da 0875 7064 6174 696e 67da  aints..updating.
-00001320: 0777 6f72 6b65 7273 da07 6261 636b 656e  .workers..backen
-00001330: 64da 0a72 6574 7572 6e5f 616c 6cda 0863  d..return_all..c
-00001340: 616c 6c62 6163 6bda 0d63 6f6d 7065 7469  allback..competi
-00001350: 7469 7669 7479 7206 0000 0072 0600 0000  tivityr....r....
-00001360: fa3c 633a 5c55 7365 7273 5c6b 6575 7266  .<c:\Users\keurf
-00001370: 5c47 6974 4875 625c 7374 6f63 686f 7079  \GitHub\stochopy
-00001380: 5c73 746f 6368 6f70 795c 6f70 7469 6d69  \stochopy\optimi
-00001390: 7a65 5c70 736f 5c5f 7073 6f2e 7079 7205  ze\pso\_pso.pyr.
-000013a0: 0000 0009 0000 0073 2c00 0000 0057 0402  .......s,....W..
-000013b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000013c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000013d0: 0201 0201 0201 02ed da03 7073 6f29 104e  ..........pso).N
-000013e0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-000013f0: 0900 0000 720a 0000 0072 0a00 0000 4e72  ....r....r....Nr
-00001400: 0b00 0000 720b 0000 004e 720c 0000 0072  ....r....Nr....r
-00001410: 0d00 0000 4e46 4e29 06da 0072 0300 0000  ....NFN)...r....
-00001420: da08 5f68 656c 7065 7273 7204 0000 00da  .._helpersr.....
-00001430: 075f 5f61 6c6c 5f5f 7205 0000 0072 0600  .__all__r....r..
-00001440: 0000 7206 0000 0072 0600 0000 7221 0000  ..r....r....r!..
-00001450: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001460: 2a00 0000 0c01 0c03 02ff 0408 0001 0001  *...............
-00001470: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001480: 0001 0001 0001 0001 0001 00ee 0a70       .............p
+00000000: 6672 6f6d 202e 2e20 696d 706f 7274 2063  from .. import c
+00000010: 7073 6f0d 0a66 726f 6d20 2e2e 5f68 656c  pso..from .._hel
+00000020: 7065 7273 2069 6d70 6f72 7420 7265 6769  pers import regi
+00000030: 7374 6572 0d0a 0d0a 5f5f 616c 6c5f 5f20  ster....__all__ 
+00000040: 3d20 5b0d 0a20 2020 2022 6d69 6e69 6d69  = [..    "minimi
+00000050: 7a65 222c 0d0a 5d0d 0a0d 0a0d 0a64 6566  ze",..]......def
+00000060: 206d 696e 696d 697a 6528 0d0a 2020 2020   minimize(..    
+00000070: 6675 6e2c 0d0a 2020 2020 626f 756e 6473  fun,..    bounds
+00000080: 2c0d 0a20 2020 2078 303d 4e6f 6e65 2c0d  ,..    x0=None,.
+00000090: 0a20 2020 2061 7267 733d 2829 2c0d 0a20  .    args=(),.. 
+000000a0: 2020 206d 6178 6974 6572 3d31 3030 2c0d     maxiter=100,.
+000000b0: 0a20 2020 2070 6f70 7369 7a65 3d31 302c  .    popsize=10,
+000000c0: 0d0a 2020 2020 696e 6572 7469 613d 302e  ..    inertia=0.
+000000d0: 3732 3938 2c0d 0a20 2020 2063 6f67 6e69  7298,..    cogni
+000000e0: 7469 7669 7479 3d31 2e34 3936 3138 2c0d  tivity=1.49618,.
+000000f0: 0a20 2020 2073 6f63 6961 6269 6c69 7479  .    sociability
+00000100: 3d31 2e34 3936 3138 2c0d 0a20 2020 2073  =1.49618,..    s
+00000110: 6565 643d 4e6f 6e65 2c0d 0a20 2020 2078  eed=None,..    x
+00000120: 746f 6c3d 312e 3065 2d38 2c0d 0a20 2020  tol=1.0e-8,..   
+00000130: 2066 746f 6c3d 312e 3065 2d38 2c0d 0a20   ftol=1.0e-8,.. 
+00000140: 2020 2063 6f6e 7374 7261 696e 7473 3d4e     constraints=N
+00000150: 6f6e 652c 0d0a 2020 2020 7570 6461 7469  one,..    updati
+00000160: 6e67 3d22 696d 6d65 6469 6174 6522 2c0d  ng="immediate",.
+00000170: 0a20 2020 2077 6f72 6b65 7273 3d31 2c0d  .    workers=1,.
+00000180: 0a20 2020 2062 6163 6b65 6e64 3d4e 6f6e  .    backend=Non
+00000190: 652c 0d0a 2020 2020 7265 7475 726e 5f61  e,..    return_a
+000001a0: 6c6c 3d46 616c 7365 2c0d 0a20 2020 2076  ll=False,..    v
+000001b0: 6572 626f 7369 7479 3d31 2e30 2c0d 0a20  erbosity=1.0,.. 
+000001c0: 2020 2063 616c 6c62 6163 6b3d 4e6f 6e65     callback=None
+000001d0: 2c0d 0a29 3a0d 0a20 2020 2022 2222 0d0a  ,..):..    """..
+000001e0: 2020 2020 4d69 6e69 6d69 7a65 2061 6e20      Minimize an 
+000001f0: 6f62 6a65 6374 6976 6520 6675 6e63 7469  objective functi
+00000200: 6f6e 2075 7369 6e67 2043 6f6d 7065 7469  on using Competi
+00000210: 7469 7665 2050 6172 7469 636c 6520 5377  tive Particle Sw
+00000220: 6172 6d20 4f70 7469 6d69 7a61 7469 6f6e  arm Optimization
+00000230: 2028 4350 534f 292e 0d0a 0d0a 2020 2020   (CPSO).....    
+00000240: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00000250: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00000260: 6675 6e20 3a20 6361 6c6c 6162 6c65 0d0a  fun : callable..
+00000270: 2020 2020 2020 2020 5468 6520 6f62 6a65          The obje
+00000280: 6374 6976 6520 6675 6e63 7469 6f6e 2074  ctive function t
+00000290: 6f20 6265 206d 696e 696d 697a 6564 2e20  o be minimized. 
+000002a0: 4d75 7374 2062 6520 696e 2074 6865 2066  Must be in the f
+000002b0: 6f72 6d20 6060 6628 782c 202a 6172 6773  orm ``f(x, *args
+000002c0: 2960 602c 2077 6865 7265 2060 6078 6060  )``, where ``x``
+000002d0: 2069 7320 7468 6520 6172 6775 6d65 6e74   is the argument
+000002e0: 2069 6e20 7468 6520 666f 726d 206f 6620   in the form of 
+000002f0: 6120 312d 4420 6172 7261 7920 616e 6420  a 1-D array and 
+00000300: 6172 6773 2069 7320 6120 7475 706c 6520  args is a tuple 
+00000310: 6f66 2061 6e79 2061 6464 6974 696f 6e61  of any additiona
+00000320: 6c20 6669 7865 6420 7061 7261 6d65 7465  l fixed paramete
+00000330: 7273 206e 6565 6465 6420 746f 2063 6f6d  rs needed to com
+00000340: 706c 6574 656c 7920 7370 6563 6966 7920  pletely specify 
+00000350: 7468 6520 6675 6e63 7469 6f6e 2e0d 0a20  the function... 
+00000360: 2020 2062 6f75 6e64 7320 3a20 6172 7261     bounds : arra
+00000370: 795f 6c69 6b65 0d0a 2020 2020 2020 2020  y_like..        
+00000380: 426f 756e 6473 2066 6f72 2076 6172 6961  Bounds for varia
+00000390: 626c 6573 2e20 6060 286d 696e 2c20 6d61  bles. ``(min, ma
+000003a0: 7829 6060 2070 6169 7273 2066 6f72 2065  x)`` pairs for e
+000003b0: 6163 6820 656c 656d 656e 7420 696e 2060  ach element in `
+000003c0: 6078 6060 2c20 6465 6669 6e69 6e67 2074  `x``, defining t
+000003d0: 6865 2066 696e 6974 6520 6c6f 7765 7220  he finite lower 
+000003e0: 616e 6420 7570 7065 7220 626f 756e 6473  and upper bounds
+000003f0: 2066 6f72 2074 6865 206f 7074 696d 697a   for the optimiz
+00000400: 696e 6720 6172 6775 6d65 6e74 206f 6620  ing argument of 
+00000410: 6060 6675 6e60 602e 2049 7420 6973 2072  ``fun``. It is r
+00000420: 6571 7569 7265 6420 746f 2068 6176 6520  equired to have 
+00000430: 6060 6c65 6e28 626f 756e 6473 2920 3d3d  ``len(bounds) ==
+00000440: 206c 656e 2878 2960 602e 2060 606c 656e   len(x)``. ``len
+00000450: 2862 6f75 6e64 7329 6060 2069 7320 7573  (bounds)`` is us
+00000460: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
+00000470: 7468 6520 6e75 6d62 6572 206f 6620 7061  the number of pa
+00000480: 7261 6d65 7465 7273 2069 6e20 6060 7860  rameters in ``x`
+00000490: 602e 0d0a 2020 2020 7830 203a 2061 7272  `...    x0 : arr
+000004a0: 6179 5f6c 696b 6520 6f72 204e 6f6e 652c  ay_like or None,
+000004b0: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
+000004c0: 6c74 204e 6f6e 650d 0a20 2020 2020 2020  lt None..       
+000004d0: 2049 6e69 7469 616c 2070 6f70 756c 6174   Initial populat
+000004e0: 696f 6e2e 2041 7272 6179 206f 6620 7265  ion. Array of re
+000004f0: 616c 2065 6c65 6d65 6e74 7320 7769 7468  al elements with
+00000500: 2073 6861 7065 2028 6060 706f 7073 697a   shape (``popsiz
+00000510: 6560 602c 2060 606e 6469 6d60 6029 2c20  e``, ``ndim``), 
+00000520: 7768 6572 6520 6060 6e64 696d 6060 2069  where ``ndim`` i
+00000530: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00000540: 696e 6465 7065 6e64 656e 7420 7661 7269  independent vari
+00000550: 6162 6c65 732e 2049 6620 6060 7830 6060  ables. If ``x0``
+00000560: 2069 7320 6e6f 7420 7370 6563 6966 6965   is not specifie
+00000570: 642c 2074 6865 2070 6f70 756c 6174 696f  d, the populatio
+00000580: 6e20 6973 2069 6e69 7469 616c 697a 6564  n is initialized
+00000590: 2075 7369 6e67 204c 6174 696e 2048 7970   using Latin Hyp
+000005a0: 6572 6375 6265 2073 616d 706c 696e 672e  ercube sampling.
+000005b0: 0d0a 2020 2020 6172 6773 203a 2074 7570  ..    args : tup
+000005c0: 6c65 2c20 6f70 7469 6f6e 616c 2c20 6465  le, optional, de
+000005d0: 6661 756c 7420 4e6f 6e65 0d0a 2020 2020  fault None..    
+000005e0: 2020 2020 4578 7472 6120 6172 6775 6d65      Extra argume
+000005f0: 6e74 7320 7061 7373 6564 2074 6f20 7468  nts passed to th
+00000600: 6520 6f62 6a65 6374 6976 6520 6675 6e63  e objective func
+00000610: 7469 6f6e 2e0d 0a20 2020 206d 6178 6974  tion...    maxit
+00000620: 6572 203a 2069 6e74 2c20 6f70 7469 6f6e  er : int, option
+00000630: 616c 2c20 6465 6661 756c 7420 3130 300d  al, default 100.
+00000640: 0a20 2020 2020 2020 2054 6865 206d 6178  .        The max
+00000650: 696d 756d 206e 756d 6265 7220 6f66 2067  imum number of g
+00000660: 656e 6572 6174 696f 6e73 206f 7665 7220  enerations over 
+00000670: 7768 6963 6820 7468 6520 656e 7469 7265  which the entire
+00000680: 2070 6f70 756c 6174 696f 6e20 6973 2065   population is e
+00000690: 766f 6c76 6564 2e0d 0a20 2020 2070 6f70  volved...    pop
+000006a0: 7369 7a65 203a 2069 6e74 2c20 6f70 7469  size : int, opti
+000006b0: 6f6e 616c 2c20 6465 6661 756c 7420 3130  onal, default 10
+000006c0: 0d0a 2020 2020 2020 2020 546f 7461 6c20  ..        Total 
+000006d0: 706f 7075 6c61 7469 6f6e 2073 697a 652e  population size.
+000006e0: 0d0a 2020 2020 696e 6572 7469 6120 3a20  ..    inertia : 
+000006f0: 7363 616c 6172 2c20 6f70 7469 6f6e 616c  scalar, optional
+00000700: 2c20 6465 6661 756c 7420 302e 3732 3938  , default 0.7298
+00000710: 0d0a 2020 2020 2020 2020 496e 6572 7469  ..        Inerti
+00000720: 616c 2077 6569 6768 742c 2064 656e 6f74  al weight, denot
+00000730: 6564 2062 7920 7720 696e 2074 6865 206c  ed by w in the l
+00000740: 6974 6572 6174 7572 652e 2049 7420 7368  iterature. It sh
+00000750: 6f75 6c64 2062 6520 696e 2074 6865 2072  ould be in the r
+00000760: 616e 6765 205b 302c 2031 5d2e 0d0a 2020  ange [0, 1]...  
+00000770: 2020 636f 676e 6974 6976 6974 7920 3a20    cognitivity : 
+00000780: 7363 616c 6172 2c20 6f70 7469 6f6e 616c  scalar, optional
+00000790: 2c20 6465 6661 756c 7420 312e 3439 3631  , default 1.4961
+000007a0: 380d 0a20 2020 2020 2020 2043 6f67 6e69  8..        Cogni
+000007b0: 7469 6f6e 2070 6172 616d 6574 6572 2c20  tion parameter, 
+000007c0: 6465 6e6f 7465 6420 6279 2063 3120 696e  denoted by c1 in
+000007d0: 2074 6865 206c 6974 6572 6174 7572 652e   the literature.
+000007e0: 2049 7420 7368 6f75 6c64 2062 6520 696e   It should be in
+000007f0: 2074 6865 2072 616e 6765 205b 302c 2034   the range [0, 4
+00000800: 5d2e 0d0a 2020 2020 736f 6369 6162 696c  ]...    sociabil
+00000810: 6974 793a 2073 6361 6c61 722c 206f 7074  ity: scalar, opt
+00000820: 696f 6e61 6c2c 2064 6566 6175 6c74 2031  ional, default 1
+00000830: 2e34 3936 3138 0d0a 2020 2020 2020 2020  .49618..        
+00000840: 536f 6369 6162 696c 6974 7920 7061 7261  Sociability para
+00000850: 6d65 7465 722c 2064 656e 6f74 6564 2062  meter, denoted b
+00000860: 7920 6332 2069 6e20 7468 6520 6c69 7465  y c2 in the lite
+00000870: 7261 7475 7265 2e20 4974 2073 686f 756c  rature. It shoul
+00000880: 6420 6265 2069 6e20 7468 6520 7261 6e67  d be in the rang
+00000890: 6520 5b30 2c20 345d 2e0d 0a20 2020 2073  e [0, 4]...    s
+000008a0: 6565 6420 3a20 696e 7420 6f72 204e 6f6e  eed : int or Non
+000008b0: 652c 206f 7074 696f 6e61 6c2c 2064 6566  e, optional, def
+000008c0: 6175 6c74 204e 6f6e 650d 0a20 2020 2020  ault None..     
+000008d0: 2020 2053 6565 6420 666f 7220 7261 6e64     Seed for rand
+000008e0: 6f6d 206e 756d 6265 7220 6765 6e65 7261  om number genera
+000008f0: 746f 722e 0d0a 2020 2020 7874 6f6c 203a  tor...    xtol :
+00000900: 2073 6361 6c61 722c 206f 7074 696f 6e61   scalar, optiona
+00000910: 6c2c 2064 6566 6175 6c74 2031 2e30 652d  l, default 1.0e-
+00000920: 380d 0a20 2020 2020 2020 2053 6f6c 7574  8..        Solut
+00000930: 696f 6e20 746f 6c65 7261 6e63 6520 666f  ion tolerance fo
+00000940: 7220 7465 726d 696e 6174 696f 6e2e 0d0a  r termination...
+00000950: 2020 2020 6674 6f6c 203a 2073 6361 6c61      ftol : scala
+00000960: 722c 206f 7074 696f 6e61 6c2c 2064 6566  r, optional, def
+00000970: 6175 6c74 2031 2e30 652d 380d 0a20 2020  ault 1.0e-8..   
+00000980: 2020 2020 204f 626a 6563 7469 7665 2066       Objective f
+00000990: 756e 6374 696f 6e20 7661 6c75 6520 746f  unction value to
+000009a0: 6c65 7261 6e63 6520 666f 7220 7465 726d  lerance for term
+000009b0: 696e 6174 696f 6e2e 0d0a 2020 2020 636f  ination...    co
+000009c0: 6e73 7472 6169 6e74 7320 3a20 7374 7220  nstraints : str 
+000009d0: 6f72 204e 6f6e 652c 206f 7074 696f 6e61  or None, optiona
+000009e0: 6c2c 2064 6566 6175 6c74 204e 6f6e 650d  l, default None.
+000009f0: 0a20 2020 2020 2020 2043 6f6e 7374 7261  .        Constra
+00000a00: 696e 7473 2064 6566 696e 6974 696f 6e3a  ints definition:
+00000a10: 0d0a 0d0a 2020 2020 2020 2020 202d 204e  ....         - N
+00000a20: 6f6e 653a 206e 6f20 636f 6e73 7472 6169  one: no constrai
+00000a30: 6e74 0d0a 2020 2020 2020 2020 202d 2027  nt..         - '
+00000a40: 5368 7269 6e6b 273a 2069 6e66 6561 7369  Shrink': infeasi
+00000a50: 626c 6520 736f 6c75 7469 6f6e 7320 6172  ble solutions ar
+00000a60: 6520 7265 7061 6972 6564 2062 7920 7368  e repaired by sh
+00000a70: 7269 6e6b 696e 6720 7061 7274 6963 6c65  rinking particle
+00000a80: 7327 2076 656c 6f63 6974 7920 7665 6374  s' velocity vect
+00000a90: 6f72 0d0a 0d0a 2020 2020 7570 6461 7469  or....    updati
+00000aa0: 6e67 203a 2073 7472 207b 2769 6d6d 6564  ng : str {'immed
+00000ab0: 6961 7465 272c 2027 6465 6665 7272 6564  iate', 'deferred
+00000ac0: 277d 2c20 6f70 7469 6f6e 616c 2c20 6465  '}, optional, de
+00000ad0: 6661 756c 7420 2769 6d6d 6564 6961 7465  fault 'immediate
+00000ae0: 270d 0a20 2020 2020 2020 2049 6620 6060  '..        If ``
+00000af0: 2769 6d6d 6564 6961 7465 2760 602c 2074  'immediate'``, t
+00000b00: 6865 2062 6573 7420 736f 6c75 7469 6f6e  he best solution
+00000b10: 2076 6563 746f 7220 6973 2063 6f6e 7469   vector is conti
+00000b20: 6e75 6f75 736c 7920 7570 6461 7465 6420  nuously updated 
+00000b30: 7769 7468 696e 2061 2073 696e 676c 6520  within a single 
+00000b40: 6765 6e65 7261 7469 6f6e 2e20 5468 6973  generation. This
+00000b50: 2063 616e 206c 6561 6420 746f 2066 6173   can lead to fas
+00000b60: 7465 7220 636f 6e76 6572 6765 6e63 6520  ter convergence 
+00000b70: 6173 2063 616e 6469 6461 7465 2073 6f6c  as candidate sol
+00000b80: 7574 696f 6e73 2063 616e 2074 616b 6520  utions can take 
+00000b90: 6164 7661 6e74 6167 6520 6f66 2063 6f6e  advantage of con
+00000ba0: 7469 6e75 6f75 7320 696d 7072 6f76 656d  tinuous improvem
+00000bb0: 656e 7473 2069 6e20 7468 6520 6265 7374  ents in the best
+00000bc0: 2073 6f6c 7574 696f 6e2e 2057 6974 6820   solution. With 
+00000bd0: 6060 2764 6566 6572 7265 6427 6060 2c20  ``'deferred'``, 
+00000be0: 7468 6520 6265 7374 2073 6f6c 7574 696f  the best solutio
+00000bf0: 6e20 7665 6374 6f72 2069 7320 7570 6461  n vector is upda
+00000c00: 7465 6420 6f6e 6365 2070 6572 2067 656e  ted once per gen
+00000c10: 6572 6174 696f 6e2e 204f 6e6c 7920 6060  eration. Only ``
+00000c20: 2764 6566 6572 7265 6427 6060 2069 7320  'deferred'`` is 
+00000c30: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+00000c40: 7061 7261 6c6c 656c 697a 6174 696f 6e2c  parallelization,
+00000c50: 2061 6e64 2069 7320 6f76 6572 7269 6464   and is overridd
+00000c60: 656e 2077 6865 6e20 6060 776f 726b 6572  en when ``worker
+00000c70: 7360 6020 6973 206e 6f74 2060 6030 6060  s`` is not ``0``
+00000c80: 206f 7220 6060 3160 6020 6f72 2060 6062   or ``1`` or ``b
+00000c90: 6163 6b65 6e64 203d 3d20 276d 7069 2760  ackend == 'mpi'`
+00000ca0: 602e 0d0a 2020 2020 776f 726b 6572 7320  `...    workers 
+00000cb0: 3a20 696e 742c 206f 7074 696f 6e61 6c2c  : int, optional,
+00000cc0: 2064 6566 6175 6c74 2031 0d0a 2020 2020   default 1..    
+00000cd0: 2020 2020 5468 6520 706f 7075 6c61 7469      The populati
+00000ce0: 6f6e 2069 7320 7375 6264 6976 6964 6564  on is subdivided
+00000cf0: 2069 6e74 6f20 776f 726b 6572 7320 7365   into workers se
+00000d00: 6374 696f 6e73 2061 6e64 2065 7661 6c75  ctions and evalu
+00000d10: 6174 6564 2069 6e20 7061 7261 6c6c 656c  ated in parallel
+00000d20: 2028 7573 6573 203a 636c 6173 733a 606a   (uses :class:`j
+00000d30: 6f62 6c69 622e 5061 7261 6c6c 656c 6029  oblib.Parallel`)
+00000d40: 2e20 5375 7070 6c79 202d 3120 746f 2075  . Supply -1 to u
+00000d50: 7365 2061 6c6c 2061 7661 696c 6162 6c65  se all available
+00000d60: 2043 5055 2063 6f72 6573 2e0d 0a20 2020   CPU cores...   
+00000d70: 2062 6163 6b65 6e64 203a 2073 7472 207b   backend : str {
+00000d80: 276c 6f6b 7927 2c20 2774 6872 6561 6469  'loky', 'threadi
+00000d90: 6e67 272c 2027 6d70 6927 7d2c 206f 7074  ng', 'mpi'}, opt
+00000da0: 696f 6e61 6c2c 2064 6566 6175 6c74 2027  ional, default '
+00000db0: 7468 7265 6164 696e 6727 0d0a 2020 2020  threading'..    
+00000dc0: 2020 2020 5061 7261 6c6c 656c 2062 6163      Parallel bac
+00000dd0: 6b65 6e64 2074 6f20 7573 6520 7768 656e  kend to use when
+00000de0: 2060 6077 6f72 6b65 7273 6060 2069 7320   ``workers`` is 
+00000df0: 6e6f 7420 6060 3060 6020 6f72 2060 6031  not ``0`` or ``1
+00000e00: 6060 3a0d 0a0d 0a20 2020 2020 2020 2020  ``:....         
+00000e10: 2d20 276c 6f6b 7927 3a20 6469 7361 626c  - 'loky': disabl
+00000e20: 6520 7468 7265 6164 696e 670d 0a20 2020  e threading..   
+00000e30: 2020 2020 2020 2d20 2774 6872 6561 6469        - 'threadi
+00000e40: 6e67 273a 2065 6e61 626c 6520 7468 7265  ng': enable thre
+00000e50: 6164 696e 670d 0a20 2020 2020 2020 2020  ading..         
+00000e60: 2d20 276d 7069 273a 2075 7365 204d 5049  - 'mpi': use MPI
+00000e70: 2028 7573 6573 203a 6d6f 643a 606d 7069   (uses :mod:`mpi
+00000e80: 3470 7960 290d 0a0d 0a20 2020 2072 6574  4py`)....    ret
+00000e90: 7572 6e5f 616c 6c20 3a20 626f 6f6c 2c20  urn_all : bool, 
+00000ea0: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
+00000eb0: 7420 4661 6c73 650d 0a20 2020 2020 2020  t False..       
+00000ec0: 2053 6574 2074 6f20 5472 7565 2074 6f20   Set to True to 
+00000ed0: 7265 7475 726e 2061 6e20 6172 7261 7920  return an array 
+00000ee0: 7769 7468 2073 6861 7065 2028 6060 6e69  with shape (``ni
+00000ef0: 7460 602c 2060 6076 6572 626f 7369 7479  t``, ``verbosity
+00000f00: 6060 202a 2060 6070 6f70 7369 7a65 6060  `` * ``popsize``
+00000f10: 2c20 6060 6e64 696d 6060 2920 6f66 2061  , ``ndim``) of a
+00000f20: 6c6c 2074 6865 2073 6f6c 7574 696f 6e73  ll the solutions
+00000f30: 2061 7420 6561 6368 2069 7465 7261 7469   at each iterati
+00000f40: 6f6e 2e0d 0a20 2020 2076 6572 626f 7369  on...    verbosi
+00000f50: 7479 203a 2066 6c6f 6174 2c20 6f70 7469  ty : float, opti
+00000f60: 6f6e 616c 2c20 6465 6661 756c 7420 312e  onal, default 1.
+00000f70: 300d 0a20 2020 2020 2020 2046 7261 6374  0..        Fract
+00000f80: 696f 6e20 6f66 2070 6f70 756c 6174 696f  ion of populatio
+00000f90: 6e20 746f 2063 6f6e 7369 6465 7220 696e  n to consider in
+00000fa0: 2060 7265 7475 726e 5f61 6c6c 602e 2049   `return_all`. I
+00000fb0: 6620 302e 302c 2072 6574 7572 6e73 2074  f 0.0, returns t
+00000fc0: 6865 2062 6573 7420 736f 6c75 7469 6f6e  he best solution
+00000fd0: 2061 7420 6561 6368 2069 7465 7261 7469   at each iterati
+00000fe0: 6f6e 2e0d 0a20 2020 2063 616c 6c62 6163  on...    callbac
+00000ff0: 6b20 3a20 6361 6c6c 6162 6c65 206f 7220  k : callable or 
+00001000: 4e6f 6e65 2c20 6f70 7469 6f6e 616c 2c20  None, optional, 
+00001010: 6465 6661 756c 7420 4e6f 6e65 0d0a 2020  default None..  
+00001020: 2020 2020 2020 4361 6c6c 6564 2061 6674        Called aft
+00001030: 6572 2065 6163 6820 6974 6572 6174 696f  er each iteratio
+00001040: 6e2e 2049 7420 6973 2061 2063 616c 6c61  n. It is a calla
+00001050: 626c 6520 7769 7468 2074 6865 2073 6967  ble with the sig
+00001060: 6e61 7475 7265 2060 6063 616c 6c62 6163  nature ``callbac
+00001070: 6b28 582c 204f 7074 696d 697a 6552 6573  k(X, OptimizeRes
+00001080: 756c 7420 7374 6174 6529 6060 2c20 7768  ult state)``, wh
+00001090: 6572 6520 6060 5860 6020 6973 2074 6865  ere ``X`` is the
+000010a0: 2063 7572 7265 6e74 2070 6f70 756c 6174   current populat
+000010b0: 696f 6e20 616e 6420 6060 7374 6174 6560  ion and ``state`
+000010c0: 6020 6973 2061 2070 6172 7469 616c 203a  ` is a partial :
+000010d0: 636c 6173 733a 6073 746f 6368 6f70 792e  class:`stochopy.
+000010e0: 6f70 7469 6d69 7a65 2e4f 7074 696d 697a  optimize.Optimiz
+000010f0: 6552 6573 756c 7460 206f 626a 6563 7420  eResult` object 
+00001100: 7769 7468 2074 6865 2073 616d 6520 6669  with the same fi
+00001110: 656c 6473 2061 7320 7468 6520 6f6e 6573  elds as the ones
+00001120: 2066 726f 6d20 7468 6520 7265 7475 726e   from the return
+00001130: 2028 6578 6365 7074 2060 6022 7375 6363   (except ``"succ
+00001140: 6573 7322 6060 2c20 6060 2273 7461 7475  ess"``, ``"statu
+00001150: 7322 6060 2061 6e64 2060 6022 6d65 7373  s"`` and ``"mess
+00001160: 6167 6522 6060 292e 0d0a 0d0a 2020 2020  age"``).....    
+00001170: 5265 7475 726e 730d 0a20 2020 202d 2d2d  Returns..    ---
+00001180: 2d2d 2d2d 0d0a 2020 2020 3a63 6c61 7373  ----..    :class
+00001190: 3a60 7374 6f63 686f 7079 2e6f 7074 696d  :`stochopy.optim
+000011a0: 697a 652e 4f70 7469 6d69 7a65 5265 7375  ize.OptimizeResu
+000011b0: 6c74 600d 0a20 2020 2020 2020 2054 6865  lt`..        The
+000011c0: 206f 7074 696d 697a 6174 696f 6e20 7265   optimization re
+000011d0: 7375 6c74 2072 6570 7265 7365 6e74 6564  sult represented
+000011e0: 2061 7320 6120 3a63 6c61 7373 3a60 7374   as a :class:`st
+000011f0: 6f63 686f 7079 2e6f 7074 696d 697a 652e  ochopy.optimize.
+00001200: 4f70 7469 6d69 7a65 5265 7375 6c74 602e  OptimizeResult`.
+00001210: 2049 6d70 6f72 7461 6e74 2061 7474 7269   Important attri
+00001220: 6275 7465 7320 6172 653a 0d0a 0d0a 2020  butes are:....  
+00001230: 2020 2020 2020 202d 2060 6078 6060 3a20         - ``x``: 
+00001240: 7468 6520 736f 6c75 7469 6f6e 2061 7272  the solution arr
+00001250: 6179 0d0a 2020 2020 2020 2020 202d 2060  ay..         - `
+00001260: 6066 756e 6060 3a20 7468 6520 736f 6c75  `fun``: the solu
+00001270: 7469 6f6e 2066 756e 6374 696f 6e20 7661  tion function va
+00001280: 6c75 650d 0a20 2020 2020 2020 2020 2d20  lue..         - 
+00001290: 6060 7375 6363 6573 7360 603a 2061 2042  ``success``: a B
+000012a0: 6f6f 6c65 616e 2066 6c61 6720 696e 6469  oolean flag indi
+000012b0: 6361 7469 6e67 2069 6620 7468 6520 6f70  cating if the op
+000012c0: 7469 6d69 7a65 7220 6578 6974 6564 2073  timizer exited s
+000012d0: 7563 6365 7373 6675 6c6c 790d 0a20 2020  uccessfully..   
+000012e0: 2020 2020 2020 2d20 6060 6d65 7373 6167        - ``messag
+000012f0: 6560 603a 2061 2073 7472 696e 6720 7768  e``: a string wh
+00001300: 6963 6820 6465 7363 7269 6265 7320 7468  ich describes th
+00001310: 6520 6361 7573 6520 6f66 2074 6865 2074  e cause of the t
+00001320: 6572 6d69 6e61 7469 6f6e 0d0a 0d0a 2020  ermination....  
+00001330: 2020 5265 6665 7265 6e63 6573 0d0a 2020    References..  
+00001340: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00001350: 2020 2e2e 205b 315d 204a 2e20 4b65 6e6e    .. [1] J. Kenn
+00001360: 6564 7920 616e 6420 522e 2045 6265 7268  edy and R. Eberh
+00001370: 6172 742c 202a 5061 7274 6963 6c65 2073  art, *Particle s
+00001380: 7761 726d 206f 7074 696d 697a 6174 696f  warm optimizatio
+00001390: 6e2a 2c20 5072 6f63 6565 6469 6e67 7320  n*, Proceedings 
+000013a0: 6f66 2049 434e 4e27 3935 202d 2049 6e74  of ICNN'95 - Int
+000013b0: 6572 6e61 7469 6f6e 616c 2043 6f6e 6665  ernational Confe
+000013c0: 7265 6e63 6520 6f6e 204e 6575 7261 6c20  rence on Neural 
+000013d0: 4e65 7477 6f72 6b73 2c20 3139 3935 2c20  Networks, 1995, 
+000013e0: 343a 2031 3934 322d 3139 3438 0d0a 2020  4: 1942-1948..  
+000013f0: 2020 2e2e 205b 325d 2046 2e20 5661 6e20    .. [2] F. Van 
+00001400: 4465 6e20 4265 7267 682c 202a 416e 2061  Den Bergh, *An a
+00001410: 6e61 6c79 7369 7320 6f66 2070 6172 7469  nalysis of parti
+00001420: 636c 6520 7377 6172 6d20 6f70 7469 6d69  cle swarm optimi
+00001430: 7a65 7273 2a2c 2055 6e69 7665 7273 6974  zers*, Universit
+00001440: 7920 6f66 2050 7265 746f 7269 612c 2032  y of Pretoria, 2
+00001450: 3030 310d 0a0d 0a20 2020 2022 2222 0d0a  001....    """..
+00001460: 2020 2020 636f 6d70 6574 6974 6976 6974      competitivit
+00001470: 7920 3d20 4e6f 6e65 0d0a 0d0a 2020 2020  y = None....    
+00001480: 7265 7475 726e 2063 7073 6f28 0d0a 2020  return cpso(..  
+00001490: 2020 2020 2020 6675 6e2c 0d0a 2020 2020        fun,..    
+000014a0: 2020 2020 626f 756e 6473 2c0d 0a20 2020      bounds,..   
+000014b0: 2020 2020 2078 302c 0d0a 2020 2020 2020       x0,..      
+000014c0: 2020 6172 6773 2c0d 0a20 2020 2020 2020    args,..       
+000014d0: 206d 6178 6974 6572 2c0d 0a20 2020 2020   maxiter,..     
+000014e0: 2020 2070 6f70 7369 7a65 2c0d 0a20 2020     popsize,..   
+000014f0: 2020 2020 2069 6e65 7274 6961 2c0d 0a20       inertia,.. 
+00001500: 2020 2020 2020 2063 6f67 6e69 7469 7669         cognitivi
+00001510: 7479 2c0d 0a20 2020 2020 2020 2073 6f63  ty,..        soc
+00001520: 6961 6269 6c69 7479 2c0d 0a20 2020 2020  iability,..     
+00001530: 2020 2063 6f6d 7065 7469 7469 7669 7479     competitivity
+00001540: 2c0d 0a20 2020 2020 2020 2073 6565 642c  ,..        seed,
+00001550: 0d0a 2020 2020 2020 2020 7874 6f6c 2c0d  ..        xtol,.
+00001560: 0a20 2020 2020 2020 2066 746f 6c2c 0d0a  .        ftol,..
+00001570: 2020 2020 2020 2020 636f 6e73 7472 6169          constrai
+00001580: 6e74 732c 0d0a 2020 2020 2020 2020 7570  nts,..        up
+00001590: 6461 7469 6e67 2c0d 0a20 2020 2020 2020  dating,..       
+000015a0: 2077 6f72 6b65 7273 2c0d 0a20 2020 2020   workers,..     
+000015b0: 2020 2062 6163 6b65 6e64 2c0d 0a20 2020     backend,..   
+000015c0: 2020 2020 2072 6574 7572 6e5f 616c 6c2c       return_all,
+000015d0: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
+000015e0: 6974 792c 0d0a 2020 2020 2020 2020 6361  ity,..        ca
+000015f0: 6c6c 6261 636b 2c0d 0a20 2020 2029 0d0a  llback,..    )..
+00001600: 0d0a 0d0a 7265 6769 7374 6572 2822 7073  ....register("ps
+00001610: 6f22 2c20 6d69 6e69 6d69 7a65 290d 0a    o", minimize)..
```

### Comparing `stochopy-2.2.0/stochopy/optimize/pso/_pso.py` & `stochopy-2.3.0/stochopy/sample/mcmc/_mcmc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,173 @@
-from .. import cpso
-from .._helpers import register
+import numpy as np
+
+from .._common import in_search_space
+from .._helpers import SampleResult, register
 
 __all__ = [
-    "minimize",
+    "sample",
 ]
 
 
-def minimize(
+def sample(
     fun,
     bounds,
     x0=None,
     args=(),
     maxiter=100,
-    popsize=10,
-    inertia=0.7298,
-    cognitivity=1.49618,
-    sociability=1.49618,
+    stepsize=0.1,
+    perc=1.0,
     seed=None,
-    xtol=1.0e-8,
-    ftol=1.0e-8,
     constraints=None,
-    updating="immediate",
-    workers=1,
-    backend=None,
-    return_all=False,
+    return_all=True,
     callback=None,
 ):
     """
-    Minimize an objective function using Competitive Particle Swarm Optimization (CPSO).
+    Sample the variable space using the Metropolis-Hastings algorithm.
 
     Parameters
     ----------
     fun : callable
-        The objective function to be minimized. Must be in the form ``f(x, *args)``, where ``x`` is the argument in the form of a 1-D array and args is a tuple of any additional fixed parameters needed to completely specify the function.
+        The objective function to be sampled. Must be in the form ``f(x, *args)``, where ``x`` is the argument in the form of a 1-D array and args is a tuple of any additional fixed parameters needed to completely specify the function.
     bounds : array_like
-        Bounds for variables. ``(min, max)`` pairs for each element in ``x``, defining the finite lower and upper bounds for the optimizing argument of ``fun``. It is required to have ``len(bounds) == len(x)``. ``len(bounds)`` is used to determine the number of parameters in ``x``.
+        Bounds for variables. ``(min, max)`` pairs for each element in ``x``, defining the finite lower and upper bounds for the sampling argument of ``fun``. It is required to have ``len(bounds) == len(x)``. ``len(bounds)`` is used to determine the number of parameters in ``x``.
     x0 : array_like or None, optional, default None
-        Initial population. Array of real elements with shape (``popsize``, ``ndim``), where ``ndim`` is the number of independent variables. If ``x0`` is not specified, the population is initialized using Latin Hypercube sampling.
+        Initial sample. Array of real elements of size (``ndim``,), where ``ndim`` is the number of independent variables.
     args : tuple, optional, default None
         Extra arguments passed to the objective function.
     maxiter : int, optional, default 100
-        The maximum number of generations over which the entire population is evolved.
-    popsize : int, optional, default 10
-        Total population size.
-    inertia : scalar, optional, default 0.7298
-        Inertial weight, denoted by w in the literature. It should be in the range [0, 1].
-    cognitivity : scalar, optional, default 1.49618
-        Cognition parameter, denoted by c1 in the literature. It should be in the range [0, 4].
-    sociability: scalar, optional, default 1.49618
-        Sociability parameter, denoted by c2 in the literature. It should be in the range [0, 4].
+        Total number of samples to generate.
+    stepsize : scalar or array_like, optional, default 0.1
+        Standard deviation of Gaussian perturbation (as a fraction of feasible space defined by ``bounds``).
+    perc : scalar, optional, default 1.0
+        Number of dimensions to perturb at each iteration (as a fraction of total number of variables).
     seed : int or None, optional, default None
         Seed for random number generator.
-    xtol : scalar, optional, default 1.0e-8
-        Solution tolerance for termination.
-    ftol : scalar, optional, default 1.0e-8
-        Objective function value tolerance for termination.
     constraints : str or None, optional, default None
         Constraints definition:
 
          - None: no constraint
-         - 'Shrink': infeasible solutions are repaired by shrinking particles' velocity vector
-
-    updating : str {'immediate', 'deferred'}, optional, default 'immediate'
-        If ``'immediate'``, the best solution vector is continuously updated within a single generation. This can lead to faster convergence as candidate solutions can take advantage of continuous improvements in the best solution. With ``'deferred'``, the best solution vector is updated once per generation. Only ``'deferred'`` is compatible with parallelization, and is overridden when ``workers`` is not ``0`` or ``1`` or ``backend == 'mpi'``.
-    workers : int, optional, default 1
-        The population is subdivided into workers sections and evaluated in parallel (uses :class:`joblib.Parallel`). Supply -1 to use all available CPU cores.
-    backend : str {'loky', 'threading', 'mpi'}, optional, default 'threading'
-        Parallel backend to use when ``workers`` is not ``0`` or ``1``:
-
-         - 'loky': disable threading
-         - 'threading': enable threading
-         - 'mpi': use MPI (uses :mod:`mpi4py`)
+         - 'Reject': infeasible solutions are always rejected
 
-    return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+    return_all : bool, optional, default True
+        Set to True to return an array with shape (``maxiter``, ``ndim``) of all the samples.
     callback : callable or None, optional, default None
-        Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
+        Called after each iteration. It is a callable with the signature ``callback(xk, SampleResult state)``, where ``xk`` is the current population and ``state`` is a :class:`stochopy.sample.SampleResult` object with the same fields as the ones from the return.
 
     Returns
     -------
-    :class:`stochopy.optimize.OptimizeResult`
-        The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
-
-         - ``x``: the solution array
-         - ``fun``: the solution function value
-         - ``success``: a Boolean flag indicating if the optimizer exited successfully
-         - ``message``: a string which describes the cause of the termination
+    :class:`stochopy.sample.SampleResult`
+        The sampling result represented as a :class:`stochopy.sample.SampleResult`. Important attributes are:
 
-    References
-    ----------
-    .. [1] J. Kennedy and R. Eberhart, *Particle swarm optimization*, Proceedings of ICNN'95 - International Conference on Neural Networks, 1995, 4: 1942-1948
-    .. [2] F. Van Den Bergh, *An analysis of particle swarm optimizers*, University of Pretoria, 2001
+         - ``x``: the best sample array
+         - ``fun``: the best sample function value
+         - ``xall``: the samples array
+         - '`funall``: the samples' function value array
 
     """
-    competitivity = None
-
-    return cpso(
-        fun,
-        bounds,
-        x0,
-        args,
-        maxiter,
-        popsize,
-        inertia,
-        cognitivity,
-        sociability,
-        competitivity,
-        seed,
-        xtol,
-        ftol,
-        constraints,
-        updating,
-        workers,
-        backend,
-        return_all,
-        callback,
+    # Cost function
+    if not hasattr(fun, "__call__"):
+        raise TypeError()
+
+    # Dimensionality and search space
+    if np.ndim(bounds) != 2:
+        raise ValueError()
+
+    ndim = len(bounds)
+    lower, upper = np.transpose(bounds)
+
+    # Initial guess x0
+    if x0 is not None and len(x0) != ndim:
+        raise ValueError()
+
+    # Step size
+    if np.ndim(stepsize) == 0:
+        stepsize = np.full(ndim, stepsize)
+
+    if len(stepsize) != ndim:
+        raise ValueError()
+
+    stepsize *= 0.5 * (upper - lower)
+
+    # Number of dimensions to perturb per iteration
+    if not 0.0 <= perc <= 1.0:
+        raise ValueError()
+
+    ndim_per_iter = max(1, int(perc * ndim))
+
+    # Seed
+    if seed is not None:
+        np.random.seed(seed)
+
+    # Callback
+    if callback is not None and not hasattr(callback, "__call__"):
+        raise ValueError()
+
+    # Initialize arrays
+    xall = np.empty((maxiter, ndim))
+    funall = np.empty(maxiter)
+    xall[0] = x0 if x0 is not None else np.random.uniform(lower, upper)
+    funall[0] = fun(xall[0], *args)
+
+    # First iteration for callback
+    if callback is not None:
+        res = SampleResult(x=xall[0], fun=funall[0], nit=1, accept_ratio=1.0)
+        if return_all:
+            res.update({"xall": xall[:1], "funall": funall[:1]})
+
+        callback(xall[0], res)
+
+    # Metropolis-Hastings algorithm
+    i = 1
+    n_accepted = 0
+    imin, fmin = 0, np.Inf
+    while i < maxiter:
+        for j in np.arange(0, ndim, ndim_per_iter):
+            jmax = min(ndim, j + ndim_per_iter - 1)
+            perturbation = np.random.randn(jmax - j + 1) * stepsize[j : jmax + 1]
+
+            xall[i] = xall[i - 1].copy()
+            xall[i, j : jmax + 1] += perturbation
+
+            accept = False
+            if in_search_space(xall[i], lower, upper, constraints):
+                funall[i] = fun(xall[i], *args)
+                log_alpha = min(0.0, funall[i - 1] - funall[i])
+                accept = log_alpha > np.log(np.random.rand())
+
+            if accept:
+                n_accepted += 1
+                if funall[i] < fmin:
+                    imin, fmin = i, funall[i]
+            else:
+                xall[i] = xall[i - 1]
+                funall[i] = funall[i - 1]
+
+            i += 1
+            if callback is not None:
+                res = SampleResult(
+                    x=xall[imin],
+                    fun=funall[imin],
+                    nit=i,
+                    accept_ratio=n_accepted / i,
+                )
+                if return_all:
+                    res.update({"xall": xall[: i - 1], "funall": funall[: i - 1]})
+
+                callback(xall[i - 1], res)
+
+            if i == maxiter:
+                break
+
+    res = SampleResult(
+        x=xall[imin],
+        fun=fmin,
+        nit=maxiter,
+        accept_ratio=n_accepted / maxiter,
     )
+    if return_all:
+        res.update({"xall": xall, "funall": funall})
+
+    return res
 
 
-register("pso", minimize)
+register("mcmc", sample)
```

### Comparing `stochopy-2.2.0/stochopy/optimize/vdcma/_vdcma.py` & `stochopy-2.3.0/stochopy/optimize/vdcma/_vdcma.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     seed=None,
     xtol=1.0e-8,
     ftol=1.0e-8,
     constraints=None,
     workers=1,
     backend=None,
     return_all=False,
+    verbosity=1.0,
     callback=None,
 ):
     """
     Minimize an objective function using VD-CMA.
 
     Parameters
     ----------
@@ -67,15 +68,17 @@
         Parallel backend to use when ``workers`` is not ``0`` or ``1``:
 
          - 'loky': disable threading
          - 'threading': enable threading
          - 'mpi': use MPI (uses :mod:`mpi4py`)
 
     return_all : bool, optional, default False
-        Set to True to return an array with shape (``nit``, ``popsize``, ``ndim``) of all the solutions at each iteration.
+        Set to True to return an array with shape (``nit``, ``verbosity`` * ``popsize``, ``ndim``) of all the solutions at each iteration.
+    verbosity : float, optional, default 1.0
+        Fraction of population to consider in `return_all`. If 0.0, returns the best solution at each iteration.
     callback : callable or None, optional, default None
         Called after each iteration. It is a callable with the signature ``callback(X, OptimizeResult state)``, where ``X`` is the current population and ``state`` is a partial :class:`stochopy.optimize.OptimizeResult` object with the same fields as the ones from the return (except ``"success"``, ``"status"`` and ``"message"``).
 
     Returns
     -------
     :class:`stochopy.optimize.OptimizeResult`
         The optimization result represented as a :class:`stochopy.optimize.OptimizeResult`. Important attributes are:
@@ -126,14 +129,15 @@
         popsize,
         sigma,
         muperc,
         constraints,
         xtol,
         ftol,
         return_all,
+        verbosity,
         callback,
     )
     res = vdcma(fun, args, True, workers, backend, *optargs)
 
     return res
 
 
@@ -150,14 +154,15 @@
     popsize,
     sigma,
     muperc,
     constraints,
     xtol,
     ftol,
     return_all,
+    verbosity,
     callback,
 ):
     """Optimize with VD-CMA."""
     ndim = len(bounds)
     lower, upper = np.transpose(bounds)
 
     # Standardize and unstandardize
@@ -200,25 +205,26 @@
     dx = np.zeros(ndim)
     ps = 0.0
     dvec = np.ones(ndim)
     vvec = np.random.normal(0.0, 1.0, ndim) / np.sqrt(ndim)
     norm_v2 = np.dot(vvec, vvec)
     norm_v = np.sqrt(norm_v2)
     vn = vvec / norm_v
-    vnn = vn ** 2
+    vnn = vn**2
     pc = np.zeros(ndim)
 
     # Initialize boundaries weights
     bnd_weights = np.zeros(ndim)
     dfithist = np.ones(1)
 
     # Initialize arrays
     if return_all:
-        xall = np.empty((maxiter, popsize, ndim))
-        funall = np.empty((maxiter, popsize))
+        nout = int(np.ceil(verbosity * popsize))
+        xall = np.empty((maxiter, max(1, nout), ndim))
+        funall = np.empty((maxiter, max(1, nout)))
 
     # VD-CMA
     nfev = 0
     arbestfitness = np.zeros(maxiter)
     ilim = int(10 + 30 * ndim / popsize)
     insigma = sigma
     validfitval = False
@@ -232,15 +238,15 @@
         # Generate lambda offsprings
         arz = np.random.randn(popsize, ndim)
         ary = dvec * (
             arz + (np.sqrt(1.0 + norm_v2) - 1.0) * np.outer(np.dot(arz, vn), vn)
         )
         if flg_injection:
             ddx = dx / dvec
-            mnorm = (ddx ** 2).sum() - np.dot(ddx, vvec) ** 2 / (1.0 + norm_v2)
+            mnorm = (ddx**2).sum() - np.dot(ddx, vvec) ** 2 / (1.0 + norm_v2)
             dy = np.linalg.norm(np.random.randn(ndim)) / np.sqrt(mnorm) * dx
             ary[0] = dy
             ary[1] = -dy
         arx = xmean + sigma * ary
         arxvalid = arx.copy()
         diagC = np.diag(
             np.dot(
@@ -267,16 +273,22 @@
                 fun,
             )
         else:
             arfitness = fun(arxvalid)
         nfev += popsize
 
         if return_all:
-            xall[it - 1] = unstandardize(arxvalid)
-            funall[it - 1] = arfitness.copy()
+            if nout > 0:
+                xall[it - 1] = unstandardize(arxvalid[:nout])
+                funall[it - 1] = arfitness[:nout].copy()
+
+            else:
+                idx = arfitness.argmin()
+                xall[it - 1] = unstandardize(arxvalid[idx])
+                funall[it - 1] = arfitness[idx].copy()
 
         # Sort by fitness and compute weighted mean into xmean
         arindex = np.argsort(arfitness)
         dx = np.dot(weights, arx[arindex[:mu]]) - weights.sum() * xmean
         xold = xmean.copy()
         xmean += dx
 
@@ -300,24 +312,24 @@
             np.sqrt(cc * (2.0 - cc) * mueff) * np.dot(weights, ary[arindex[:mu]])
             if cond
             else 0.0
         )
 
         # Alpha and related variables
         gamma = 1.0 / np.sqrt(1.0 + norm_v2)
-        alpha = np.sqrt(norm_v2 ** 2 + (1.0 + norm_v2) / vnn.max() * (2.0 - gamma)) / (
+        alpha = np.sqrt(norm_v2**2 + (1.0 + norm_v2) / vnn.max() * (2.0 - gamma)) / (
             2.0 + norm_v2
         )
         if alpha < 1.0:
             beta = (4.0 - (2.0 - gamma) / vnn.max()) / (1.0 + 2.0 / norm_v2) ** 2
         else:
             alpha = 1.0
             beta = 0.0
-        bsca = 2.0 * alpha ** 2 - beta
-        avec = 2.0 - (bsca + 2.0 * alpha ** 2) * vnn
+        bsca = 2.0 * alpha**2 - beta
+        avec = 2.0 - (bsca + 2.0 * alpha**2) * vnn
         invavnn = vnn / avec
 
         # Rank-mu
         if cmu == 0.0:
             pvec_mu = np.zeros(ndim)
             qvec_mu = np.zeros(ndim)
         else:
@@ -358,15 +370,15 @@
         vvec += upfactor * ngv
         dvec += upfactor * ngd
 
         # Update the constants
         norm_v2 = np.dot(vvec, vvec)
         norm_v = np.sqrt(norm_v2)
         vn = vvec / norm_v
-        vnn = vn ** 2
+        vnn = vn**2
 
         # Check convergence
         status = converge(
             it,
             ndim,
             maxiter,
             xmean,
@@ -411,23 +423,23 @@
     return res
 
 
 def pvec_and_qvec(vn, norm_v2, y, weights=None):
     """Return pvec and qvec."""
     y_vn = np.dot(y, vn)
     if weights is None:
-        pvec = y ** 2 - norm_v2 / (1.0 + norm_v2) * (y_vn * y * vn) - 1.0
-        qvec = y_vn * y - (0.5 * (y_vn ** 2 + 1.0 + norm_v2)) * vn
+        pvec = y**2 - norm_v2 / (1.0 + norm_v2) * (y_vn * y * vn) - 1.0
+        qvec = y_vn * y - (0.5 * (y_vn**2 + 1.0 + norm_v2)) * vn
 
     else:
         pvec = np.dot(
-            weights, y ** 2 - norm_v2 / (1.0 + norm_v2) * (y_vn * (y * vn).T).T - 1.0
+            weights, y**2 - norm_v2 / (1.0 + norm_v2) * (y_vn * (y * vn).T).T - 1.0
         )
         qvec = np.dot(
-            weights, (y_vn * y.T).T - np.outer(0.5 * (y_vn ** 2 + 1.0 + norm_v2), vn)
+            weights, (y_vn * y.T).T - np.outer(0.5 * (y_vn**2 + 1.0 + norm_v2), vn)
         )
 
     return pvec, qvec
 
 
 def ngv_ngd(dvec, vn, vnn, norm_v, norm_v2, alpha, avec, bsca, invavnn, pvec, qvec):
     """Return ngv and ngd."""
```

### Comparing `stochopy-2.2.0/stochopy/sample/__pycache__/_helpers.cpython-38.pyc` & `stochopy-2.3.0/stochopy/sample/_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,205 +1,189 @@
-00000000: 550d 0d0a 0000 0000 ca4a 9b61 cf0b 0000  U........J.a....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 6701 5a02  d.l.m.Z...d.g.Z.
-00000040: 6900 5a03 4700 6403 6404 8400 6404 6501  i.Z.G.d.d...d.e.
-00000050: 8303 5a04 6405 6406 8400 5a05 640b 640a  ..Z.d.d...Z.d.d.
-00000060: 6402 8401 5a06 6407 5300 290c e902 0000  d...Z.d.S.).....
-00000070: 0029 01da 0a42 6173 6552 6573 756c 74da  .)...BaseResult.
-00000080: 0673 616d 706c 6563 0000 0000 0000 0000  .samplec........
-00000090: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000000a0: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000000b0: 0364 0253 0029 03da 0c53 616d 706c 6552  .d.S.)...SampleR
-000000c0: 6573 756c 7461 5601 0000 0a20 2020 2052  esultaV....    R
-000000d0: 6570 7265 7365 6e74 2074 6865 2073 616d  epresent the sam
-000000e0: 706c 696e 6720 7265 7375 6c74 2e0a 0a20  pling result... 
-000000f0: 2020 2041 7474 7269 6275 7465 730a 2020     Attributes.  
-00000100: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000110: 2078 203a 2061 7272 6179 5f6c 696b 650a   x : array_like.
-00000120: 2020 2020 2020 2020 5468 6520 6265 7374          The best
-00000130: 2073 6f6c 7574 696f 6e20 7361 6d70 6c65   solution sample
-00000140: 642e 0a20 2020 2066 756e 203a 2073 6361  d..    fun : sca
-00000150: 6c61 720a 2020 2020 2020 2020 5468 6520  lar.        The 
-00000160: 736f 6c75 7469 6f6e 2066 756e 6374 696f  solution functio
-00000170: 6e20 7661 6c75 652e 0a20 2020 206e 6974  n value..    nit
-00000180: 203a 2069 6e74 0a20 2020 2020 2020 204e   : int.        N
-00000190: 756d 6265 7220 6f66 2073 616d 706c 6573  umber of samples
-000001a0: 2067 656e 6572 6174 6564 2e0a 0a20 2020   generated...   
-000001b0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-000001c0: 0a20 2020 2054 6865 7265 206d 6179 2062  .    There may b
-000001d0: 6520 6164 6469 7469 6f6e 616c 2061 7474  e additional att
-000001e0: 7269 6275 7465 7320 6e6f 7420 6c69 7374  ributes not list
-000001f0: 6564 2061 626f 7665 2064 6570 656e 6469  ed above dependi
-00000200: 6e67 206f 6620 7468 6520 7370 6563 6966  ng of the specif
-00000210: 6963 2073 6f6c 7665 722e 0a0a 2020 2020  ic solver...    
-00000220: 4e29 04da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000230: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000240: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000250: a900 7209 0000 0072 0900 0000 fa3a 633a  ..r....r.....:c:
-00000260: 5c55 7365 7273 5c6b 6575 7266 5c47 6974  \Users\keurf\Git
-00000270: 4875 625c 7374 6f63 686f 7079 5c73 746f  Hub\stochopy\sto
-00000280: 6368 6f70 795c 7361 6d70 6c65 5c5f 6865  chopy\sample\_he
-00000290: 6c70 6572 732e 7079 7204 0000 000b 0000  lpers.pyr.......
-000002a0: 0073 0400 0000 0801 0412 7204 0000 0063  .s........r....c
-000002b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000002c0: 0300 0000 4300 0000 730c 0000 007c 0174  ....C...s....|.t
-000002d0: 007c 003c 0064 0153 0029 027a 1752 6567  .|.<.d.S.).z.Reg
-000002e0: 6973 7465 7220 6120 6e65 7720 7361 6d70  ister a new samp
-000002f0: 6c65 722e 4ea9 01da 0c5f 7361 6d70 6c65  ler.N...._sample
-00000300: 725f 6d61 7029 02da 046e 616d 6572 0300  r_map)...namer..
-00000310: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000320: 00da 0872 6567 6973 7465 7221 0000 0073  ...register!...s
-00000330: 0200 0000 0002 720e 0000 004e 7209 0000  ......r....Nr...
-00000340: 00da 046d 636d 6363 0700 0000 0000 0000  ...mcmcc........
-00000350: 0000 0000 0700 0000 0800 0000 4300 0000  ............C...
-00000360: 732a 0000 007c 0572 087c 056e 0269 007d  s*...|.r.|.n.i.}
-00000370: 0574 007c 0419 0066 007c 007c 017c 027c  .t.|...f.|.|.|.|
-00000380: 037c 0664 019c 057c 0597 028e 0153 0029  .|.d...|.....S.)
-00000390: 0261 3908 0000 0a20 2020 2053 616d 706c  .a9....    Sampl
-000003a0: 6520 7468 6520 7661 7269 6162 6c65 2073  e the variable s
-000003b0: 7061 6365 206f 6620 616e 206f 626a 6563  pace of an objec
-000003c0: 7469 7665 2066 756e 6374 696f 6e2e 0a0a  tive function...
-000003d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000003e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000003f0: 2020 6675 6e20 3a20 6361 6c6c 6162 6c65    fun : callable
-00000400: 0a20 2020 2020 2020 2054 6865 206f 626a  .        The obj
-00000410: 6563 7469 7665 2066 756e 6374 696f 6e20  ective function 
-00000420: 746f 2062 6520 7361 6d70 6c65 642e 204d  to be sampled. M
-00000430: 7573 7420 6265 2069 6e20 7468 6520 666f  ust be in the fo
-00000440: 726d 2060 6066 2878 2c20 2a61 7267 7329  rm ``f(x, *args)
-00000450: 6060 2c20 7768 6572 6520 6060 7860 6020  ``, where ``x`` 
-00000460: 6973 2074 6865 2061 7267 756d 656e 7420  is the argument 
-00000470: 696e 2074 6865 2066 6f72 6d20 6f66 2061  in the form of a
-00000480: 2031 2d44 2061 7272 6179 2061 6e64 2061   1-D array and a
-00000490: 7267 7320 6973 2061 2074 7570 6c65 206f  rgs is a tuple o
-000004a0: 6620 616e 7920 6164 6469 7469 6f6e 616c  f any additional
-000004b0: 2066 6978 6564 2070 6172 616d 6574 6572   fixed parameter
-000004c0: 7320 6e65 6564 6564 2074 6f20 636f 6d70  s needed to comp
-000004d0: 6c65 7465 6c79 2073 7065 6369 6679 2074  letely specify t
-000004e0: 6865 2066 756e 6374 696f 6e2e 0a20 2020  he function..   
-000004f0: 2062 6f75 6e64 7320 3a20 6172 7261 795f   bounds : array_
-00000500: 6c69 6b65 0a20 2020 2020 2020 2042 6f75  like.        Bou
-00000510: 6e64 7320 666f 7220 7661 7269 6162 6c65  nds for variable
-00000520: 732e 2060 6028 6d69 6e2c 206d 6178 2960  s. ``(min, max)`
-00000530: 6020 7061 6972 7320 666f 7220 6561 6368  ` pairs for each
-00000540: 2065 6c65 6d65 6e74 2069 6e20 6060 7860   element in ``x`
-00000550: 602c 2064 6566 696e 696e 6720 7468 6520  `, defining the 
-00000560: 6669 6e69 7465 206c 6f77 6572 2061 6e64  finite lower and
-00000570: 2075 7070 6572 2062 6f75 6e64 7320 666f   upper bounds fo
-00000580: 7220 7468 6520 7361 6d70 6c69 6e67 2061  r the sampling a
-00000590: 7267 756d 656e 7420 6f66 2060 6066 756e  rgument of ``fun
-000005a0: 6060 2e20 4974 2069 7320 7265 7175 6972  ``. It is requir
-000005b0: 6564 2074 6f20 6861 7665 2060 606c 656e  ed to have ``len
-000005c0: 2862 6f75 6e64 7329 203d 3d20 6c65 6e28  (bounds) == len(
-000005d0: 7829 6060 2e20 6060 6c65 6e28 626f 756e  x)``. ``len(boun
-000005e0: 6473 2960 6020 6973 2075 7365 6420 746f  ds)`` is used to
-000005f0: 2064 6574 6572 6d69 6e65 2074 6865 206e   determine the n
-00000600: 756d 6265 7220 6f66 2070 6172 616d 6574  umber of paramet
-00000610: 6572 7320 696e 2060 6078 6060 2e0a 2020  ers in ``x``..  
-00000620: 2020 7830 203a 2061 7272 6179 5f6c 696b    x0 : array_lik
-00000630: 6520 6f72 204e 6f6e 652c 206f 7074 696f  e or None, optio
-00000640: 6e61 6c2c 2064 6566 6175 6c74 204e 6f6e  nal, default Non
-00000650: 650a 2020 2020 2020 2020 496e 6974 6961  e.        Initia
-00000660: 6c20 7361 6d70 6c65 2e20 4172 7261 7920  l sample. Array 
-00000670: 6f66 2072 6561 6c20 656c 656d 656e 7473  of real elements
-00000680: 206f 6620 7369 7a65 2028 6060 6e64 696d   of size (``ndim
-00000690: 6060 2c29 2c20 7768 6572 6520 6060 6e64  ``,), where ``nd
-000006a0: 696d 6060 2069 7320 7468 6520 6e75 6d62  im`` is the numb
-000006b0: 6572 206f 6620 696e 6465 7065 6e64 656e  er of independen
-000006c0: 7420 7661 7269 6162 6c65 732e 0a20 2020  t variables..   
-000006d0: 2061 7267 7320 3a20 7475 706c 652c 206f   args : tuple, o
-000006e0: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-000006f0: 204e 6f6e 650a 2020 2020 2020 2020 4578   None.        Ex
-00000700: 7472 6120 6172 6775 6d65 6e74 7320 7061  tra arguments pa
-00000710: 7373 6564 2074 6f20 7468 6520 6f62 6a65  ssed to the obje
-00000720: 6374 6976 6520 6675 6e63 7469 6f6e 2e0a  ctive function..
-00000730: 2020 2020 6d65 7468 6f64 203a 2073 7472      method : str
-00000740: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
-00000750: 756c 7420 276d 636d 6327 0a20 2020 2020  ult 'mcmc'.     
-00000760: 2020 2054 7970 6520 6f66 2073 616d 706c     Type of sampl
-00000770: 6572 2e20 5368 6f75 6c64 2062 6520 6f6e  er. Should be on
-00000780: 6520 6f66 3a0a 0a20 2020 2020 2020 2020  e of:..         
-00000790: 2d20 276d 636d 6327 0a20 2020 2020 2020  - 'mcmc'.       
-000007a0: 2020 2d20 2768 6d63 270a 0a20 2020 206f    - 'hmc'..    o
-000007b0: 7074 696f 6e73 203a 2064 6963 7420 6f72  ptions : dict or
-000007c0: 204e 6f6e 652c 206f 7074 696f 6e61 6c2c   None, optional,
-000007d0: 2064 6566 6175 6c74 204e 6f6e 650a 2020   default None.  
-000007e0: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
-000007f0: 7279 206f 6620 7361 6d70 6c65 7220 6f70  ry of sampler op
-00000800: 7469 6f6e 732e 2041 6c6c 206d 6574 686f  tions. All metho
-00000810: 6473 2061 6363 6570 7420 7468 6520 666f  ds accept the fo
-00000820: 6c6c 6f77 696e 6720 6765 6e65 7269 6320  llowing generic 
-00000830: 6f70 7469 6f6e 733a 0a0a 2020 2020 2020  options:..      
-00000840: 2020 202d 206d 6178 6974 6572 2028 696e     - maxiter (in
-00000850: 7429 3a20 746f 7461 6c20 6e75 6d62 6572  t): total number
-00000860: 206f 6620 7361 6d70 6c65 7320 746f 2067   of samples to g
-00000870: 656e 6572 6174 650a 2020 2020 2020 2020  enerate.        
-00000880: 202d 2073 6565 6420 2869 6e74 206f 7220   - seed (int or 
-00000890: 4e6f 6e65 293a 2073 6565 6420 666f 7220  None): seed for 
-000008a0: 7261 6e64 6f6d 206e 756d 6265 7220 6765  random number ge
-000008b0: 6e65 7261 746f 720a 2020 2020 2020 2020  nerator.        
-000008c0: 202d 2072 6574 7572 6e5f 616c 6c20 2862   - return_all (b
-000008d0: 6f6f 6c29 3a20 7365 7420 746f 2054 7275  ool): set to Tru
-000008e0: 6520 746f 2072 6574 7572 6e20 616e 2061  e to return an a
-000008f0: 7272 6179 206f 6620 616c 6c20 7468 6520  rray of all the 
-00000900: 736f 6c75 7469 6f6e 7320 6174 2065 6163  solutions at eac
-00000910: 6820 6974 6572 6174 696f 6e0a 0a20 2020  h iteration..   
-00000920: 2063 616c 6c62 6163 6b20 3a20 6361 6c6c   callback : call
-00000930: 6162 6c65 206f 7220 4e6f 6e65 2c20 6f70  able or None, op
-00000940: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00000950: 4e6f 6e65 0a20 2020 2020 2020 2043 616c  None.        Cal
-00000960: 6c65 6420 6166 7465 7220 6561 6368 2069  led after each i
-00000970: 7465 7261 7469 6f6e 2e20 4974 2069 7320  teration. It is 
-00000980: 6120 6361 6c6c 6162 6c65 2077 6974 6820  a callable with 
-00000990: 7468 6520 7369 676e 6174 7572 6520 6060  the signature ``
-000009a0: 6361 6c6c 6261 636b 2878 6b2c 2053 616d  callback(xk, Sam
-000009b0: 706c 6552 6573 756c 7420 7374 6174 6529  pleResult state)
-000009c0: 6060 2c20 7768 6572 6520 6060 786b 6060  ``, where ``xk``
-000009d0: 2069 7320 7468 6520 6375 7272 656e 7420   is the current 
-000009e0: 706f 7075 6c61 7469 6f6e 2061 6e64 2060  population and `
-000009f0: 6073 7461 7465 6060 2069 7320 6120 3a63  `state`` is a :c
-00000a00: 6c61 7373 3a60 7374 6f63 686f 7079 2e73  lass:`stochopy.s
-00000a10: 616d 706c 652e 5361 6d70 6c65 5265 7375  ample.SampleResu
-00000a20: 6c74 6020 6f62 6a65 6374 2077 6974 6820  lt` object with 
-00000a30: 7468 6520 7361 6d65 2066 6965 6c64 7320  the same fields 
-00000a40: 6173 2074 6865 206f 6e65 7320 6672 6f6d  as the ones from
-00000a50: 2074 6865 2072 6574 7572 6e2e 0a0a 2020   the return...  
-00000a60: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00000a70: 2d2d 2d2d 2d0a 2020 2020 3a63 6c61 7373  -----.    :class
-00000a80: 3a60 7374 6f63 686f 7079 2e73 616d 706c  :`stochopy.sampl
-00000a90: 652e 5361 6d70 6c65 5265 7375 6c74 600a  e.SampleResult`.
-00000aa0: 2020 2020 2020 2020 5468 6520 7361 6d70          The samp
-00000ab0: 6c69 6e67 2072 6573 756c 7420 7265 7072  ling result repr
-00000ac0: 6573 656e 7465 6420 6173 2061 203a 636c  esented as a :cl
-00000ad0: 6173 733a 6073 746f 6368 6f70 792e 7361  ass:`stochopy.sa
-00000ae0: 6d70 6c65 2e53 616d 706c 6552 6573 756c  mple.SampleResul
-00000af0: 7460 2e20 496d 706f 7274 616e 7420 6174  t`. Important at
-00000b00: 7472 6962 7574 6573 2061 7265 3a0a 0a20  tributes are:.. 
-00000b10: 2020 2020 2020 2020 2d20 6060 7860 603a          - ``x``:
-00000b20: 2074 6865 2062 6573 7420 7361 6d70 6c65   the best sample
-00000b30: 2061 7272 6179 0a20 2020 2020 2020 2020   array.         
-00000b40: 2d20 6060 6675 6e60 603a 2074 6865 2062  - ``fun``: the b
-00000b50: 6573 7420 7361 6d70 6c65 2066 756e 6374  est sample funct
-00000b60: 696f 6e20 7661 6c75 650a 2020 2020 2020  ion value.      
-00000b70: 2020 202d 2060 6078 616c 6c60 603a 2074     - ``xall``: t
-00000b80: 6865 2073 616d 706c 6573 2061 7272 6179  he samples array
-00000b90: 0a20 2020 2020 2020 2020 2d20 2760 6675  .         - '`fu
-00000ba0: 6e61 6c6c 6060 3a20 7468 6520 7361 6d70  nall``: the samp
-00000bb0: 6c65 7327 2066 756e 6374 696f 6e20 7661  les' function va
-00000bc0: 6c75 6520 6172 7261 790a 0a20 2020 2029  lue array..    )
-00000bd0: 05da 0366 756e da06 626f 756e 6473 da02  ...fun..bounds..
-00000be0: 7830 da04 6172 6773 da08 6361 6c6c 6261  x0..args..callba
-00000bf0: 636b 720b 0000 0029 0772 1000 0000 7211  ckr....).r....r.
-00000c00: 0000 0072 1200 0000 7213 0000 00da 066d  ...r....r......m
-00000c10: 6574 686f 64da 076f 7074 696f 6e73 7214  ethod..optionsr.
-00000c20: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
-00000c30: 0000 7203 0000 0026 0000 0073 1400 0000  ..r....&...s....
-00000c40: 0029 0c02 0801 0200 0200 0200 0200 02ff  .)..............
-00000c50: 0401 02ff 2905 4e72 0900 0000 720f 0000  ....).Nr....r...
-00000c60: 004e 4e29 07da 075f 636f 6d6d 6f6e 7202  .NN)..._commonr.
-00000c70: 0000 00da 075f 5f61 6c6c 5f5f 720c 0000  .....__all__r...
-00000c80: 0072 0400 0000 720e 0000 0072 0300 0000  .r....r....r....
-00000c90: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000ca0: 0a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000cb0: 0000 730c 0000 000c 0302 ff04 0504 0310  ..s.............
-00000cc0: 1608 05                                  ...
+00000000: 6672 6f6d 202e 2e5f 636f 6d6d 6f6e 2069  from .._common i
+00000010: 6d70 6f72 7420 4261 7365 5265 7375 6c74  mport BaseResult
+00000020: 0d0a 0d0a 5f5f 616c 6c5f 5f20 3d20 5b0d  ....__all__ = [.
+00000030: 0a20 2020 2022 7361 6d70 6c65 222c 0d0a  .    "sample",..
+00000040: 5d0d 0a0d 0a0d 0a5f 7361 6d70 6c65 725f  ]......_sampler_
+00000050: 6d61 7020 3d20 7b7d 0d0a 0d0a 0d0a 636c  map = {}......cl
+00000060: 6173 7320 5361 6d70 6c65 5265 7375 6c74  ass SampleResult
+00000070: 2842 6173 6552 6573 756c 7429 3a0d 0a20  (BaseResult):.. 
+00000080: 2020 2022 2222 0d0a 2020 2020 5265 7072     """..    Repr
+00000090: 6573 656e 7420 7468 6520 7361 6d70 6c69  esent the sampli
+000000a0: 6e67 2072 6573 756c 742e 0d0a 0d0a 2020  ng result.....  
+000000b0: 2020 4174 7472 6962 7574 6573 0d0a 2020    Attributes..  
+000000c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+000000d0: 2020 7820 3a20 6172 7261 795f 6c69 6b65    x : array_like
+000000e0: 0d0a 2020 2020 2020 2020 5468 6520 6265  ..        The be
+000000f0: 7374 2073 6f6c 7574 696f 6e20 7361 6d70  st solution samp
+00000100: 6c65 642e 0d0a 2020 2020 6675 6e20 3a20  led...    fun : 
+00000110: 7363 616c 6172 0d0a 2020 2020 2020 2020  scalar..        
+00000120: 5468 6520 736f 6c75 7469 6f6e 2066 756e  The solution fun
+00000130: 6374 696f 6e20 7661 6c75 652e 0d0a 2020  ction value...  
+00000140: 2020 6e69 7420 3a20 696e 740d 0a20 2020    nit : int..   
+00000150: 2020 2020 204e 756d 6265 7220 6f66 2073       Number of s
+00000160: 616d 706c 6573 2067 656e 6572 6174 6564  amples generated
+00000170: 2e0d 0a0d 0a20 2020 204e 6f74 650d 0a20  .....    Note.. 
+00000180: 2020 202d 2d2d 2d0d 0a20 2020 2054 6865     ----..    The
+00000190: 7265 206d 6179 2062 6520 6164 6469 7469  re may be additi
+000001a0: 6f6e 616c 2061 7474 7269 6275 7465 7320  onal attributes 
+000001b0: 6e6f 7420 6c69 7374 6564 2061 626f 7665  not listed above
+000001c0: 2064 6570 656e 6469 6e67 206f 6620 7468   depending of th
+000001d0: 6520 7370 6563 6966 6963 2073 6f6c 7665  e specific solve
+000001e0: 722e 0d0a 0d0a 2020 2020 2222 220d 0a0d  r.....    """...
+000001f0: 0a20 2020 2070 6173 730d 0a0d 0a0d 0a64  .    pass......d
+00000200: 6566 2072 6567 6973 7465 7228 6e61 6d65  ef register(name
+00000210: 2c20 7361 6d70 6c65 293a 0d0a 2020 2020  , sample):..    
+00000220: 2222 2252 6567 6973 7465 7220 6120 6e65  """Register a ne
+00000230: 7720 7361 6d70 6c65 722e 2222 220d 0a20  w sampler.""".. 
+00000240: 2020 205f 7361 6d70 6c65 725f 6d61 705b     _sampler_map[
+00000250: 6e61 6d65 5d20 3d20 7361 6d70 6c65 0d0a  name] = sample..
+00000260: 0d0a 0d0a 6465 6620 7361 6d70 6c65 2866  ....def sample(f
+00000270: 756e 2c20 626f 756e 6473 2c20 7830 3d4e  un, bounds, x0=N
+00000280: 6f6e 652c 2061 7267 733d 2829 2c20 6d65  one, args=(), me
+00000290: 7468 6f64 3d22 6d63 6d63 222c 206f 7074  thod="mcmc", opt
+000002a0: 696f 6e73 3d4e 6f6e 652c 2063 616c 6c62  ions=None, callb
+000002b0: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
+000002c0: 2222 220d 0a20 2020 2053 616d 706c 6520  """..    Sample 
+000002d0: 7468 6520 7661 7269 6162 6c65 2073 7061  the variable spa
+000002e0: 6365 206f 6620 616e 206f 626a 6563 7469  ce of an objecti
+000002f0: 7665 2066 756e 6374 696f 6e2e 0d0a 0d0a  ve function.....
+00000300: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00000310: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00000320: 2020 2020 6675 6e20 3a20 6361 6c6c 6162      fun : callab
+00000330: 6c65 0d0a 2020 2020 2020 2020 5468 6520  le..        The 
+00000340: 6f62 6a65 6374 6976 6520 6675 6e63 7469  objective functi
+00000350: 6f6e 2074 6f20 6265 2073 616d 706c 6564  on to be sampled
+00000360: 2e20 4d75 7374 2062 6520 696e 2074 6865  . Must be in the
+00000370: 2066 6f72 6d20 6060 6628 782c 202a 6172   form ``f(x, *ar
+00000380: 6773 2960 602c 2077 6865 7265 2060 6078  gs)``, where ``x
+00000390: 6060 2069 7320 7468 6520 6172 6775 6d65  `` is the argume
+000003a0: 6e74 2069 6e20 7468 6520 666f 726d 206f  nt in the form o
+000003b0: 6620 6120 312d 4420 6172 7261 7920 616e  f a 1-D array an
+000003c0: 6420 6172 6773 2069 7320 6120 7475 706c  d args is a tupl
+000003d0: 6520 6f66 2061 6e79 2061 6464 6974 696f  e of any additio
+000003e0: 6e61 6c20 6669 7865 6420 7061 7261 6d65  nal fixed parame
+000003f0: 7465 7273 206e 6565 6465 6420 746f 2063  ters needed to c
+00000400: 6f6d 706c 6574 656c 7920 7370 6563 6966  ompletely specif
+00000410: 7920 7468 6520 6675 6e63 7469 6f6e 2e0d  y the function..
+00000420: 0a20 2020 2062 6f75 6e64 7320 3a20 6172  .    bounds : ar
+00000430: 7261 795f 6c69 6b65 0d0a 2020 2020 2020  ray_like..      
+00000440: 2020 426f 756e 6473 2066 6f72 2076 6172    Bounds for var
+00000450: 6961 626c 6573 2e20 6060 286d 696e 2c20  iables. ``(min, 
+00000460: 6d61 7829 6060 2070 6169 7273 2066 6f72  max)`` pairs for
+00000470: 2065 6163 6820 656c 656d 656e 7420 696e   each element in
+00000480: 2060 6078 6060 2c20 6465 6669 6e69 6e67   ``x``, defining
+00000490: 2074 6865 2066 696e 6974 6520 6c6f 7765   the finite lowe
+000004a0: 7220 616e 6420 7570 7065 7220 626f 756e  r and upper boun
+000004b0: 6473 2066 6f72 2074 6865 2073 616d 706c  ds for the sampl
+000004c0: 696e 6720 6172 6775 6d65 6e74 206f 6620  ing argument of 
+000004d0: 6060 6675 6e60 602e 2049 7420 6973 2072  ``fun``. It is r
+000004e0: 6571 7569 7265 6420 746f 2068 6176 6520  equired to have 
+000004f0: 6060 6c65 6e28 626f 756e 6473 2920 3d3d  ``len(bounds) ==
+00000500: 206c 656e 2878 2960 602e 2060 606c 656e   len(x)``. ``len
+00000510: 2862 6f75 6e64 7329 6060 2069 7320 7573  (bounds)`` is us
+00000520: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
+00000530: 7468 6520 6e75 6d62 6572 206f 6620 7061  the number of pa
+00000540: 7261 6d65 7465 7273 2069 6e20 6060 7860  rameters in ``x`
+00000550: 602e 0d0a 2020 2020 7830 203a 2061 7272  `...    x0 : arr
+00000560: 6179 5f6c 696b 6520 6f72 204e 6f6e 652c  ay_like or None,
+00000570: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
+00000580: 6c74 204e 6f6e 650d 0a20 2020 2020 2020  lt None..       
+00000590: 2049 6e69 7469 616c 2073 616d 706c 652e   Initial sample.
+000005a0: 2041 7272 6179 206f 6620 7265 616c 2065   Array of real e
+000005b0: 6c65 6d65 6e74 7320 6f66 2073 697a 6520  lements of size 
+000005c0: 2860 606e 6469 6d60 602c 292c 2077 6865  (``ndim``,), whe
+000005d0: 7265 2060 606e 6469 6d60 6020 6973 2074  re ``ndim`` is t
+000005e0: 6865 206e 756d 6265 7220 6f66 2069 6e64  he number of ind
+000005f0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
+00000600: 6573 2e0d 0a20 2020 2061 7267 7320 3a20  es...    args : 
+00000610: 7475 706c 652c 206f 7074 696f 6e61 6c2c  tuple, optional,
+00000620: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
+00000630: 2020 2020 2020 2045 7874 7261 2061 7267         Extra arg
+00000640: 756d 656e 7473 2070 6173 7365 6420 746f  uments passed to
+00000650: 2074 6865 206f 626a 6563 7469 7665 2066   the objective f
+00000660: 756e 6374 696f 6e2e 0d0a 2020 2020 6d65  unction...    me
+00000670: 7468 6f64 203a 2073 7472 2c20 6f70 7469  thod : str, opti
+00000680: 6f6e 616c 2c20 6465 6661 756c 7420 276d  onal, default 'm
+00000690: 636d 6327 0d0a 2020 2020 2020 2020 5479  cmc'..        Ty
+000006a0: 7065 206f 6620 7361 6d70 6c65 722e 2053  pe of sampler. S
+000006b0: 686f 756c 6420 6265 206f 6e65 206f 663a  hould be one of:
+000006c0: 0d0a 0d0a 2020 2020 2020 2020 202d 2027  ....         - '
+000006d0: 6d63 6d63 270d 0a20 2020 2020 2020 2020  mcmc'..         
+000006e0: 2d20 2768 6d63 270d 0a0d 0a20 2020 206f  - 'hmc'....    o
+000006f0: 7074 696f 6e73 203a 2064 6963 7420 6f72  ptions : dict or
+00000700: 204e 6f6e 652c 206f 7074 696f 6e61 6c2c   None, optional,
+00000710: 2064 6566 6175 6c74 204e 6f6e 650d 0a20   default None.. 
+00000720: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
+00000730: 6172 7920 6f66 2073 616d 706c 6572 206f  ary of sampler o
+00000740: 7074 696f 6e73 2e20 416c 6c20 6d65 7468  ptions. All meth
+00000750: 6f64 7320 6163 6365 7074 2074 6865 2066  ods accept the f
+00000760: 6f6c 6c6f 7769 6e67 2067 656e 6572 6963  ollowing generic
+00000770: 206f 7074 696f 6e73 3a0d 0a0d 0a20 2020   options:....   
+00000780: 2020 2020 2020 2d20 6d61 7869 7465 7220        - maxiter 
+00000790: 2869 6e74 293a 2074 6f74 616c 206e 756d  (int): total num
+000007a0: 6265 7220 6f66 2073 616d 706c 6573 2074  ber of samples t
+000007b0: 6f20 6765 6e65 7261 7465 0d0a 2020 2020  o generate..    
+000007c0: 2020 2020 202d 2073 6565 6420 2869 6e74       - seed (int
+000007d0: 206f 7220 4e6f 6e65 293a 2073 6565 6420   or None): seed 
+000007e0: 666f 7220 7261 6e64 6f6d 206e 756d 6265  for random numbe
+000007f0: 7220 6765 6e65 7261 746f 720d 0a20 2020  r generator..   
+00000800: 2020 2020 2020 2d20 7265 7475 726e 5f61        - return_a
+00000810: 6c6c 2028 626f 6f6c 293a 2073 6574 2074  ll (bool): set t
+00000820: 6f20 5472 7565 2074 6f20 7265 7475 726e  o True to return
+00000830: 2061 6e20 6172 7261 7920 6f66 2061 6c6c   an array of all
+00000840: 2074 6865 2073 6f6c 7574 696f 6e73 2061   the solutions a
+00000850: 7420 6561 6368 2069 7465 7261 7469 6f6e  t each iteration
+00000860: 0d0a 0d0a 2020 2020 6361 6c6c 6261 636b  ....    callback
+00000870: 203a 2063 616c 6c61 626c 6520 6f72 204e   : callable or N
+00000880: 6f6e 652c 206f 7074 696f 6e61 6c2c 2064  one, optional, d
+00000890: 6566 6175 6c74 204e 6f6e 650d 0a20 2020  efault None..   
+000008a0: 2020 2020 2043 616c 6c65 6420 6166 7465       Called afte
+000008b0: 7220 6561 6368 2069 7465 7261 7469 6f6e  r each iteration
+000008c0: 2e20 4974 2069 7320 6120 6361 6c6c 6162  . It is a callab
+000008d0: 6c65 2077 6974 6820 7468 6520 7369 676e  le with the sign
+000008e0: 6174 7572 6520 6060 6361 6c6c 6261 636b  ature ``callback
+000008f0: 2878 6b2c 2053 616d 706c 6552 6573 756c  (xk, SampleResul
+00000900: 7420 7374 6174 6529 6060 2c20 7768 6572  t state)``, wher
+00000910: 6520 6060 786b 6060 2069 7320 7468 6520  e ``xk`` is the 
+00000920: 6375 7272 656e 7420 706f 7075 6c61 7469  current populati
+00000930: 6f6e 2061 6e64 2060 6073 7461 7465 6060  on and ``state``
+00000940: 2069 7320 6120 3a63 6c61 7373 3a60 7374   is a :class:`st
+00000950: 6f63 686f 7079 2e73 616d 706c 652e 5361  ochopy.sample.Sa
+00000960: 6d70 6c65 5265 7375 6c74 6020 6f62 6a65  mpleResult` obje
+00000970: 6374 2077 6974 6820 7468 6520 7361 6d65  ct with the same
+00000980: 2066 6965 6c64 7320 6173 2074 6865 206f   fields as the o
+00000990: 6e65 7320 6672 6f6d 2074 6865 2072 6574  nes from the ret
+000009a0: 7572 6e2e 0d0a 0d0a 2020 2020 5265 7475  urn.....    Retu
+000009b0: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+000009c0: 0d0a 2020 2020 3a63 6c61 7373 3a60 7374  ..    :class:`st
+000009d0: 6f63 686f 7079 2e73 616d 706c 652e 5361  ochopy.sample.Sa
+000009e0: 6d70 6c65 5265 7375 6c74 600d 0a20 2020  mpleResult`..   
+000009f0: 2020 2020 2054 6865 2073 616d 706c 696e       The samplin
+00000a00: 6720 7265 7375 6c74 2072 6570 7265 7365  g result represe
+00000a10: 6e74 6564 2061 7320 6120 3a63 6c61 7373  nted as a :class
+00000a20: 3a60 7374 6f63 686f 7079 2e73 616d 706c  :`stochopy.sampl
+00000a30: 652e 5361 6d70 6c65 5265 7375 6c74 602e  e.SampleResult`.
+00000a40: 2049 6d70 6f72 7461 6e74 2061 7474 7269   Important attri
+00000a50: 6275 7465 7320 6172 653a 0d0a 0d0a 2020  butes are:....  
+00000a60: 2020 2020 2020 202d 2060 6078 6060 3a20         - ``x``: 
+00000a70: 7468 6520 6265 7374 2073 616d 706c 6520  the best sample 
+00000a80: 6172 7261 790d 0a20 2020 2020 2020 2020  array..         
+00000a90: 2d20 6060 6675 6e60 603a 2074 6865 2062  - ``fun``: the b
+00000aa0: 6573 7420 7361 6d70 6c65 2066 756e 6374  est sample funct
+00000ab0: 696f 6e20 7661 6c75 650d 0a20 2020 2020  ion value..     
+00000ac0: 2020 2020 2d20 6060 7861 6c6c 6060 3a20      - ``xall``: 
+00000ad0: 7468 6520 7361 6d70 6c65 7320 6172 7261  the samples arra
+00000ae0: 790d 0a20 2020 2020 2020 2020 2d20 2760  y..         - '`
+00000af0: 6675 6e61 6c6c 6060 3a20 7468 6520 7361  funall``: the sa
+00000b00: 6d70 6c65 7327 2066 756e 6374 696f 6e20  mples' function 
+00000b10: 7661 6c75 6520 6172 7261 790d 0a0d 0a20  value array.... 
+00000b20: 2020 2022 2222 0d0a 2020 2020 6f70 7469     """..    opti
+00000b30: 6f6e 7320 3d20 6f70 7469 6f6e 7320 6966  ons = options if
+00000b40: 206f 7074 696f 6e73 2065 6c73 6520 7b7d   options else {}
+00000b50: 0d0a 0d0a 2020 2020 7265 7475 726e 205f  ....    return _
+00000b60: 7361 6d70 6c65 725f 6d61 705b 6d65 7468  sampler_map[meth
+00000b70: 6f64 5d28 0d0a 2020 2020 2020 2020 6675  od](..        fu
+00000b80: 6e3d 6675 6e2c 2062 6f75 6e64 733d 626f  n=fun, bounds=bo
+00000b90: 756e 6473 2c20 7830 3d78 302c 2061 7267  unds, x0=x0, arg
+00000ba0: 733d 6172 6773 2c20 6361 6c6c 6261 636b  s=args, callback
+00000bb0: 3d63 616c 6c62 6163 6b2c 202a 2a6f 7074  =callback, **opt
+00000bc0: 696f 6e73 0d0a 2020 2020 290d 0a         ions..    )..
```

### Comparing `stochopy-2.2.0/stochopy/sample/hmc/_hmc.py` & `stochopy-2.3.0/stochopy/sample/hmc/_hmc.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/stochopy.egg-info/PKG-INFO` & `stochopy-2.3.0/stochopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: stochopy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python library for stochastic numerical optimization
 Home-page: https://github.com/keurfonluu/stochopy
 Author: Keurfon Luu
 License: BSD 3-Clause License
 Project-URL: Code, https://github.com/keurfonluu/stochopy
 Project-URL: Issues, https://github.com/keurfonluu/stochopy/issues
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 stochopy
 ========
 
-|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Travis| |DOI|
+|License| |Stars| |Pyversions| |Version| |Downloads| |Code style: black| |Codacy Badge| |Codecov| |Build| |Docs| |DOI|
 
 **stochopy** provides functions for sampling or optimizing objective functions with or without constraints. Its API is directly inspired by **scipy**'s own optimization submodule which should make the switch from one module to another straightforward.
 
 .. figure:: https://raw.githubusercontent.com/keurfonluu/stochopy/master/.github/sample.gif
    :alt: sample-pso
    :width: 100%
    :align: center
@@ -159,13 +160,12 @@
 
 .. |Codecov| image:: https://img.shields.io/codecov/c/github/keurfonluu/stochopy.svg?style=flat
    :target: https://codecov.io/gh/keurfonluu/stochopy
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4058008.svg?style=flat
    :target: https://doi.org/10.5281/zenodo.4058008
 
-.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/Python%20package
+.. |Build| image:: https://img.shields.io/github/workflow/status/keurfonluu/stochopy/ci.yml
    :target: https://github.com/keurfonluu/stochopy
 
-.. |Travis| image:: https://img.shields.io/travis/com/keurfonluu/stochopy/master?label=docs
+.. |Docs| image:: https://img.shields.io/github/actions/workflow/status/keurfonluu/stochopy/doc.yml?label=docs
    :target: https://keurfonluu.github.io/stochopy/
-
```

### Comparing `stochopy-2.2.0/test/test_factory.py` & `stochopy-2.3.0/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/test/test_optimize.py` & `stochopy-2.3.0/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `stochopy-2.2.0/test/test_sample.py` & `stochopy-2.3.0/tests/test_sample.py`

 * *Files identical despite different names*

