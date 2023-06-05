# Comparing `tmp/gemseo-pymoo-1.1.1.tar.gz` & `tmp/gemseo-pymoo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-pymoo-1.1.1.tar", last modified: Thu Feb 16 08:07:05 2023, max compression
+gzip compressed data, was "gemseo-pymoo-1.1.2.tar", last modified: Mon Jun  5 10:37:11 2023, max compression
```

## Comparing `gemseo-pymoo-1.1.1.tar` & `gemseo-pymoo-1.1.2.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.871837 gemseo-pymoo-1.1.1/
--rw-r--r--   0 ad        (1000) ad        (1000)      450 2022-03-24 10:38:50.000000 gemseo-pymoo-1.1.1/.gitattributes
--rw-r--r--   0 ad        (1000) ad        (1000)      191 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/.gitignore
--rw-r--r--   0 ad        (1000) ad        (1000)      265 2022-10-27 15:24:30.000000 gemseo-pymoo-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 ad        (1000) ad        (1000)     2491 2022-07-27 19:27:02.000000 gemseo-pymoo-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 ad        (1000) ad        (1000)     9105 2022-03-24 10:38:50.000000 gemseo-pymoo-1.1.1/.pylintrc
--rw-r--r--   0 ad        (1000) ad        (1000)     1341 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/CHANGELOG.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     1814 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/CREDITS.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-pymoo-1.1.1/LICENSE.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.833837 gemseo-pymoo-1.1.1/LICENSES/
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-pymoo-1.1.1/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.834837 gemseo-pymoo-1.1.1/LICENSES/headers/
--rw-r--r--   0 ad        (1000) ad        (1000)      729 2022-03-24 13:18:51.000000 gemseo-pymoo-1.1.1/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      334 2022-03-24 13:18:51.000000 gemseo-pymoo-1.1.1/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      710 2022-03-24 13:18:51.000000 gemseo-pymoo-1.1.1/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2745 2023-02-16 08:07:05.871837 gemseo-pymoo-1.1.1/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     1628 2022-07-28 09:20:50.000000 gemseo-pymoo-1.1.1/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)      611 2022-07-19 15:02:00.000000 gemseo-pymoo-1.1.1/pyproject.toml
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.837837 gemseo-pymoo-1.1.1/requirements/
--rw-r--r--   0 ad        (1000) ad        (1000)       79 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/requirements/check.in
--rw-r--r--   0 ad        (1000) ad        (1000)      538 2022-07-19 15:02:00.000000 gemseo-pymoo-1.1.1/requirements/check.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       12 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/requirements/dist.in
--rw-r--r--   0 ad        (1000) ad        (1000)     1495 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/requirements/dist.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1666 2022-10-27 15:24:30.000000 gemseo-pymoo-1.1.1/requirements/doc.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2421 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/requirements/test-python3.10.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2584 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/requirements/test-python3.7.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2419 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/requirements/test-python3.8.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2419 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/requirements/test-python3.9.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1674 2023-02-16 08:07:05.873837 gemseo-pymoo-1.1.1/setup.cfg
--rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-03-24 13:07:04.000000 gemseo-pymoo-1.1.1/setup.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.827837 gemseo-pymoo-1.1.1/src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.837837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/
--rw-r--r--   0 ad        (1000) ad        (1000)      830 2022-05-13 11:59:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.840837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/
--rw-r--r--   0 ad        (1000) ad        (1000)      835 2022-05-13 11:59:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.842837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/
--rw-r--r--   0 ad        (1000) ad        (1000)      881 2022-07-19 15:01:03.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.843837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/core/
--rw-r--r--   0 ad        (1000) ad        (1000)      911 2022-07-19 15:01:03.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/core/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)    18983 2022-10-27 15:24:30.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/core/pymoo_problem_adapater.py
--rw-r--r--   0 ad        (1000) ad        (1000)    36781 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/lib_pymoo.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.845837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/
--rw-r--r--   0 ad        (1000) ad        (1000)     3052 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_GA_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     3055 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA2_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     3513 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA3_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     3396 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_RNSGA3_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     3514 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_UNSGA3_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)    15966 2022-05-13 11:59:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt_result_mo.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1500 2022-07-19 15:01:03.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/stop_criteria.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.849837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/
--rw-r--r--   0 ad        (1000) ad        (1000)     1096 2022-06-14 19:33:37.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Compromise_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)      446 2022-05-13 11:59:15.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/HighTradeOff_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)      948 2022-06-14 19:33:37.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Petal_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1018 2022-06-14 19:33:37.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Radar_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1060 2022-05-13 11:59:15.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/ScatterPareto_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1033 2022-07-19 15:01:03.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5787 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/compromise.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.850837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/
--rw-r--r--   0 ad        (1000) ad        (1000)      901 2023-02-16 08:06:16.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/MultiObjectiveDiagram_options.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1033 2022-07-19 15:01:03.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     8184 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/multi_objective_diagram.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3899 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/plot_features.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3136 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/high_tradeoff.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2196 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/petal.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2339 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/radar.py
--rw-r--r--   0 ad        (1000) ad        (1000)     8369 2022-06-15 10:44:26.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/scatter_pareto.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.851837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/
--rw-r--r--   0 ad        (1000) ad        (1000)      845 2022-05-13 11:59:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.853837 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/
--rw-r--r--   0 ad        (1000) ad        (1000)      903 2022-05-13 11:59:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     6836 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/chankong_haimes.py
--rw-r--r--   0 ad        (1000) ad        (1000)    14773 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/knapsack.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4895 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/viennet.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.839837 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/
--rw-r--r--   0 ad        (1000) ad        (1000)     2745 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     3244 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/SOURCES.txt
--rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/dependency_links.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       45 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/entry_points.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      102 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/requires.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       13 2023-02-16 08:07:05.000000 gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/top_level.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.854837 gemseo-pymoo-1.1.1/tests/
--rw-r--r--   0 ad        (1000) ad        (1000)      826 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.854837 gemseo-pymoo-1.1.1/tests/algos/
--rw-r--r--   0 ad        (1000) ad        (1000)      851 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/algos/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.855837 gemseo-pymoo-1.1.1/tests/algos/opt/
--rw-r--r--   0 ad        (1000) ad        (1000)      834 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/algos/opt/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7290 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/algos/opt/test_opt_result_mo.py
--rw-r--r--   0 ad        (1000) ad        (1000)    22970 2022-10-27 15:24:30.000000 gemseo-pymoo-1.1.1/tests/algos/opt/test_pymoo_algos.py
--rw-r--r--   0 ad        (1000) ad        (1000)      881 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/conftest.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.856837 gemseo-pymoo-1.1.1/tests/post/
--rw-r--r--   0 ad        (1000) ad        (1000)      843 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/post/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.829837 gemseo-pymoo-1.1.1/tests/post/baseline_images/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.867837 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/
--rw-r--r--   0 ad        (1000) ad        (1000)   232642 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/compromise_viennet_aasf.png
--rw-r--r--   0 ad        (1000) ad        (1000)   224850 2022-05-13 11:18:33.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/compromise_viennet_perp_dist.png
--rw-r--r--   0 ad        (1000) ad        (1000)   213539 2022-05-13 11:18:33.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/high_tradeoff_viennet_no_extra.png
--rw-r--r--   0 ad        (1000) ad        (1000)    61518 2022-04-19 08:53:46.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/petal_viennet_tchebi.png
--rw-r--r--   0 ad        (1000) ad        (1000)    62064 2022-04-19 08:53:46.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/petal_viennet_weighted_sum.png
--rw-r--r--   0 ad        (1000) ad        (1000)    54950 2022-04-19 08:53:46.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/radar_viennet_asf.png
--rw-r--r--   0 ad        (1000) ad        (1000)    49698 2022-04-19 08:53:46.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/radar_viennet_pbi.png
--rw-r--r--   0 ad        (1000) ad        (1000)   215889 2022-05-13 11:18:33.000000 gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/scatter_pareto_viennet.png
--rw-r--r--   0 ad        (1000) ad        (1000)    10014 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/post/test_pymoo_post.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.869837 gemseo-pymoo-1.1.1/tests/problems/
--rw-r--r--   0 ad        (1000) ad        (1000)      828 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/problems/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 08:07:05.871837 gemseo-pymoo-1.1.1/tests/problems/analytical/
--rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-05-13 11:59:33.000000 gemseo-pymoo-1.1.1/tests/problems/analytical/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2203 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/problems/analytical/test_chankong_haimes.py
--rw-r--r--   0 ad        (1000) ad        (1000)     6336 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/problems/analytical/test_knapsack.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1739 2022-06-15 09:35:50.000000 gemseo-pymoo-1.1.1/tests/problems/analytical/test_viennet.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3211 2022-07-21 12:18:54.000000 gemseo-pymoo-1.1.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.415946 gemseo-pymoo-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/CREDITS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.398947 gemseo-pymoo-1.1.2/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.398947 gemseo-pymoo-1.1.2/LICENSES/headers/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/LICENSES/headers/BSD-0-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-06-05 10:37:11.415946 gemseo-pymoo-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.400946 gemseo-pymoo-1.1.2/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/check.in
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/check.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/dist.in
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/dist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/test-python3.10.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/test-python3.8.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/requirements/test-python3.9.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-05 10:37:11.416946 gemseo-pymoo-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.392947 gemseo-pymoo-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.401947 gemseo-pymoo-1.1.2/src/gemseo_pymoo/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.403946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.403946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.404946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/core/
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18969 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/core/pymoo_problem_adapater.py
+-rw-rw-rw-   0 root         (0) root         (0)    36842 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/lib_pymoo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.405946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/
+-rw-rw-rw-   0 root         (0) root         (0)     3052 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_GA_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     3055 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA2_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA3_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_RNSGA3_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_UNSGA3_options.json
+-rw-rw-rw-   0 root         (0) root         (0)    15844 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt_result_mo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/stop_criteria.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.407946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Compromise_options.json
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/HighTradeOff_options.json
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Petal_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Radar_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/ScatterPareto_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5786 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/compromise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.408946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/MultiObjectiveDiagram_options.json
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8183 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/multi_objective_diagram.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/plot_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     3144 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/high_tradeoff.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/petal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/radar.py
+-rw-rw-rw-   0 root         (0) root         (0)     8368 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/scatter_pareto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.408946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.409946 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6885 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/chankong_haimes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14841 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/knapsack.py
+-rw-rw-rw-   0 root         (0) root         (0)     4910 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/viennet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.402947 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 10:37:11.000000 gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.409946 gemseo-pymoo-1.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.410946 gemseo-pymoo-1.1.2/tests/algos/
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/algos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.410946 gemseo-pymoo-1.1.2/tests/algos/opt/
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/algos/opt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7337 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/algos/opt/test_opt_result_mo.py
+-rw-rw-rw-   0 root         (0) root         (0)    22960 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/algos/opt/test_pymoo_algos.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.411946 gemseo-pymoo-1.1.2/tests/post/
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.394947 gemseo-pymoo-1.1.2/tests/post/baseline_images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.413946 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/
+-rw-rw-rw-   0 root         (0) root         (0)   232642 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/compromise_viennet_aasf.png
+-rw-rw-rw-   0 root         (0) root         (0)   224850 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/compromise_viennet_perp_dist.png
+-rw-rw-rw-   0 root         (0) root         (0)   213539 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/high_tradeoff_viennet_no_extra.png
+-rw-rw-rw-   0 root         (0) root         (0)    61518 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/petal_viennet_tchebi.png
+-rw-rw-rw-   0 root         (0) root         (0)    62064 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/petal_viennet_weighted_sum.png
+-rw-rw-rw-   0 root         (0) root         (0)    54950 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/radar_viennet_asf.png
+-rw-rw-rw-   0 root         (0) root         (0)    49698 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/radar_viennet_pbi.png
+-rw-rw-rw-   0 root         (0) root         (0)   215889 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/scatter_pareto_viennet.png
+-rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/post/test_pymoo_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.414946 gemseo-pymoo-1.1.2/tests/problems/
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/problems/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:37:11.415946 gemseo-pymoo-1.1.2/tests/problems/analytical/
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/problems/analytical/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/problems/analytical/test_chankong_haimes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6336 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/problems/analytical/test_knapsack.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tests/problems/analytical/test_viennet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2023-06-05 10:36:54.000000 gemseo-pymoo-1.1.2/tox.ini
```

### Comparing `gemseo-pymoo-1.1.1/.pylintrc` & `gemseo-pymoo-1.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/CHANGELOG.rst` & `gemseo-pymoo-1.1.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
 
+Version 1.1.2 (June 2023)
+*************************
+
+Update to GEMSEO 5.
+
+
 Version 1.1.1 (February 2023)
 *****************************
 
 Fixed
 -----
 
 - The missing json file to validate the post processor options.
```

### Comparing `gemseo-pymoo-1.1.1/CREDITS.rst` & `gemseo-pymoo-1.1.2/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/LICENSE.txt` & `gemseo-pymoo-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/LICENSES/LGPLv3.txt` & `gemseo-pymoo-1.1.2/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-pymoo-1.1.2/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/LICENSES/headers/LGPL-3.0.txt` & `gemseo-pymoo-1.1.2/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/PKG-INFO` & `gemseo-pymoo-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: gemseo-pymoo
-Version: 1.1.1
+Version: 1.1.2
 Summary: A GEMSEO wrapper for pymoo optimization algorithms.
 Home-page: https://www.irt-saintexupery.com
 Author: Francois Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-pymoo
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-pymoo/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-pymoo-1.1.1/README.rst` & `gemseo-pymoo-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/pyproject.toml` & `gemseo-pymoo-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # logging settings identical to the defaults of gemseo.api.configure_logger()
 log_file_level = "INFO"
 log_file_date_format = "%H:%M:%S"
 log_file_format = "%(levelname)8s - %(asctime)s: %(message)s"
 # filterwarnings = ignore::pytest.PytestExperimentalApiWarning
 
 [tool.black]
-target-version = ['py37']
+target-version = ['py38']
```

### Comparing `gemseo-pymoo-1.1.1/requirements/check.txt` & `gemseo-pymoo-1.1.2/requirements/check.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile requirements/check.in
 #
 cfgv==3.3.1
     # via pre-commit
-distlib==0.3.4
+distlib==0.3.6
     # via virtualenv
-filelock==3.7.0
+filelock==3.12.0
     # via virtualenv
-identify==2.5.0
+identify==2.5.24
     # via pre-commit
-nodeenv==1.6.0
+nodeenv==1.8.0
     # via pre-commit
-platformdirs==2.5.2
+platformdirs==3.5.1
     # via virtualenv
-pre-commit==2.19.0
+pre-commit==3.3.1
     # via -r requirements/check.in
 pyyaml==6.0
     # via pre-commit
-six==1.16.0
-    # via virtualenv
-toml==0.10.2
-    # via pre-commit
-virtualenv==20.14.1
+virtualenv==20.23.0
     # via pre-commit
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `gemseo-pymoo-1.1.1/requirements/dist.txt` & `gemseo-pymoo-1.1.2/requirements/dist.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,79 +4,79 @@
 #
 #    pip-compile requirements/dist.in
 #
 bleach==6.0.0
     # via readme-renderer
 build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-cryptography==39.0.1
+cryptography==40.0.2
     # via secretstorage
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 idna==3.4
     # via requests
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 keyring==23.13.1
     # via twine
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-packaging==23.0
+packaging==23.1
     # via build
 pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.1
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
 twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.14
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.13.0
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-pymoo-1.1.1/requirements/doc.txt` & `gemseo-pymoo-1.1.2/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/requirements/test-python3.10.txt` & `gemseo-pymoo-1.1.2/requirements/test-python3.10.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,131 +1,133 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==22.2.0
-    # via pytest
 autograd==1.5
     # via pymoo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 cma==2.7
     # via pymoo
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-pymoo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 future==0.18.3
     # via autograd
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-pymoo (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
-    # via gemseo
+h5py==3.8.0
+    # via
+    #   gemseo
+    #   gemseo-pymoo (setup.py)
 idna==3.4
     # via requests
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   pymoo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.23.5
     # via
     #   autograd
     #   contourpy
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pymoo
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
+pandas==2.0.0
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pymoo==0.5.0
     # via gemseo-pymoo (setup.py)
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-pymoo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-pymoo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-pymoo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
     #   pymoo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
```

### Comparing `gemseo-pymoo-1.1.1/requirements/test-python3.7.txt` & `gemseo-pymoo-1.1.2/requirements/test-python3.9.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,140 +1,137 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==22.2.0
-    # via pytest
 autograd==1.5
     # via pymoo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 cma==2.7
     # via pymoo
-covdefaults==2.2.2
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-pymoo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 future==0.18.3
     # via autograd
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-pymoo (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
-    # via gemseo
-idna==3.4
-    # via requests
-importlib-metadata==4.13.0
+h5py==3.8.0
     # via
     #   gemseo
-    #   pluggy
-    #   pytest
+    #   gemseo-pymoo (setup.py)
+idna==3.4
+    # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.3
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   pymoo
-networkx==2.6.3
+networkx==3.1
     # via gemseo
-numpy==1.21.6
+numpy==1.23.5
     # via
     #   autograd
+    #   contourpy
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pymoo
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.3.5
+pandas==2.0.0
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pymoo==0.5.0
     # via gemseo-pymoo (setup.py)
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-pymoo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-pymoo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-pymoo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
     #   pymoo
-singledispatchmethod==1.0
-    # via gemseo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
-    # via
-    #   gemseo
-    #   importlib-metadata
-    #   kiwisolver
-urllib3==1.26.14
+typing-extensions==4.5.0
+    # via gemseo
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
-zipp==3.13.0
-    # via importlib-metadata
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-pymoo-1.1.1/requirements/test-python3.8.txt` & `gemseo-pymoo-1.1.2/requirements/test-python3.8.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,137 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==22.2.0
-    # via pytest
 autograd==1.5
     # via pymoo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 cma==2.7
     # via pymoo
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-pymoo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 docstring-inheritance==1.0.0
     # via gemseo
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
 future==0.18.3
     # via autograd
 gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-pymoo (setup.py)
 genson==1.2.2
     # via gemseo
-h5py==3.7.0
-    # via gemseo
+h5py==3.8.0
+    # via
+    #   gemseo
+    #   gemseo-pymoo (setup.py)
 idna==3.4
     # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   pymoo
-networkx==2.8.8
+networkx==3.1
     # via gemseo
-numpy==1.23.4
+numpy==1.23.5
     # via
     #   autograd
     #   contourpy
     #   gemseo
     #   gemseo-pymoo (setup.py)
     #   h5py
     #   matplotlib
     #   pandas
     #   pymoo
     #   pyxdsm
     #   scipy
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
+pandas==2.0.0
     # via
     #   gemseo
     #   gemseo-pymoo (setup.py)
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
 pymoo==0.5.0
     # via gemseo-pymoo (setup.py)
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-pymoo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-pymoo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-pymoo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
     #   pymoo
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-pymoo-1.1.1/setup.cfg` & `gemseo-pymoo-1.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -17,30 +17,29 @@
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
-python_requires = >=3.7, <3.10
+python_requires = >=3.8, <3.10
 install_requires = 
-	gemseo >=4.0.0
+	gemseo >=5
+	h5py
 	pymoo ==0.5.0
 	matplotlib
-	numpy
+	numpy <1.24
 	pandas
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
@@ -65,17 +64,21 @@
 
 [flake8]
 ignore = 
 	E501
 	D105
 	E203
 	W503
-select = B,C,D,E,F,G,N,T,W,B950
+	ANN101
+	ANN102
+	ANN401
+select = ANN,B,C,D,E,F,G,N,T,W,B950
 max-line-length = 88
 docstring-convention = google
 per-file-ignores = 
-	tests/*.py:D100,D104
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-pymoo-1.1.1/setup.py` & `gemseo-pymoo-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/core/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/core/pymoo_problem_adapater.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/core/pymoo_problem_adapater.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 from typing import Any
 from typing import Dict
 from typing import Tuple
 from typing import Union
 
 import h5py
 from gemseo.algos.design_space import DesignSpace
-from gemseo.algos.opt.opt_lib import OptimizationLibrary
+from gemseo.algos.opt.optimization_library import OptimizationLibrary
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.algos.stop_criteria import TerminationCriterion
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
-from gemseo.core.parallel_execution import ParallelExecution
+from gemseo.core.parallel_execution.callable_parallel_execution import (
+    CallableParallelExecution,
+)
 from numpy import allclose
 from numpy import atleast_1d
 from numpy import average
 from numpy import concatenate as np_concat
 from numpy import dtype as np_dtype
 from numpy import hstack
 from numpy import inf as np_inf
@@ -62,31 +64,30 @@
 
 def import_hdf(
     file_path: str,
     x_tolerance: float = 0.0,
 ) -> OptimizationProblem:
     """Import an optimization history from an HDF file.
 
-    It uses :meth:`gemseo.algos.opt_problem.OptimizationProblem.import_hdf` to import
+    It uses :meth:`gemseo.algos.opt_problem.OptimizationProblem.from_hdf` to import
     the optimization history from the HDF file. Afterwards, it replaces the
     :class:`gemseo.algos.opt_result.OptimizationResult` object in
     :attr:`gemseo.algos.opt_problem.OptimizationProblem.solution` by a
     :class:`gemseo_pymoo.algos.opt_result_mo.MultiObjectiveOptimizationResult` object.
 
     Args:
         file_path: The file containing the optimization history.
         x_tolerance: The tolerance on the design variables when reading the file.
 
     Returns:
         The read optimization problem.
     """
-    opt_pb = OptimizationProblem.import_hdf(file_path, x_tolerance)
+    opt_pb = OptimizationProblem.from_hdf(file_path, x_tolerance)
 
     with h5py.File(file_path, "r") as h5file:
-
         # Update solution.
         if opt_pb.SOLUTION_GROUP in h5file:
             pareto = Pareto(opt_pb) if opt_pb.solution.is_feasible else None
             opt_pb.solution = MultiObjectiveOptimizationResult(
                 **opt_pb.solution.__dict__, pareto=pareto
             )
 
@@ -127,15 +128,16 @@
         u_b=pymoo_pb.xu,
         var_type=pymoo_pb_options.pop("mask", "float"),
         value=0.5 * (pymoo_pb.xl + pymoo_pb.xu),
         size=pymoo_pb.n_var,
     )
 
     gemseo_pb = OptimizationProblem(
-        design_space, differentiation_method=OptimizationProblem.FINITE_DIFFERENCES
+        design_space,
+        differentiation_method=OptimizationProblem.ApproximationMode.FINITE_DIFFERENCES,
     )
     gemseo_pb.objective = MDOFunction(
         lambda x: pymoo_pb.evaluate(x, return_as_dictionary=True)["F"], "F"
     )
     if pymoo_pb.n_constr > 0:
         ineq = MDOFunction(
             lambda x: pymoo_pb.evaluate(x, return_as_dictionary=True)["G"], "G"
@@ -179,15 +181,15 @@
 
     _hv_history: list[float]
     """The hypervolume indicator for each generation."""
 
     _hv_ref_point: ndarray
     """The reference point used for computing the hypervolume indicator."""
 
-    _parallel: ParallelExecution | None
+    _parallel: CallableParallelExecution | None
     """The object handling the parallel execution."""
 
     _ineq_constraints: list[MDOFunction]
     """The problem's inequality constraints."""
 
     def __init__(
         self,
@@ -226,19 +228,17 @@
 
         # Set up for parallel execution.
         n_processes = options.pop("n_processes")
         if n_processes > 1:
             LOGGER.info(
                 "Running Optimization in parallel on n_processes = %d", n_processes
             )
-            self._parallel = ParallelExecution(
-                self._worker,
+            self._parallel = CallableParallelExecution(
+                [self._worker],
                 n_processes=n_processes,
-                use_threading=False,
-                wait_time_between_fork=0.0,
                 exceptions_to_re_raise=(TerminationCriterion,),
             )
         else:
             self._parallel = None
 
         # Design variables.
         design_space = opt_problem.design_space
@@ -256,15 +256,15 @@
         super().__init__(
             n_var=n_var,
             n_obj=opt_problem.objective.dim,
             n_constr=sum(constr.dim for constr in self._ineq_constraints),
             xl=lower_bounds,
             xu=upper_bounds,
             type_var=np_concat(
-                [design_space.get_type(var) for var in design_space.variables_names]
+                [design_space.get_type(var) for var in design_space.variable_names]
             ),
             **options,
         )
 
     def _evaluate(
         self,
         design_variables: ndarray,
@@ -332,17 +332,17 @@
 
         # Initialize the order as it is not necessarily guaranteed
         # when using parallel execution.
         for x_i in design_variables:
             if self.normalize_ds:
                 x_u = sample_to_design(x_i)
                 x_r = round_vect(x_u)
-                database.store(x_r, {}, add_iter=True)
+                database.store(x_r, {})
             else:
-                database.store(x_i, {}, add_iter=True)
+                database.store(x_i, {})
 
         # Define a callback function to store the samples on the fly
         # during the parallel execution.
         def store_callback(index: int, outputs: OPTLibraryOutputType) -> None:
             """Store the outputs in the database.
 
             The jacobian is ignored because we are dealing
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/lib_pymoo.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/lib_pymoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import Final
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
-from gemseo.algos.opt.opt_lib import OptimizationAlgorithmDescription
-from gemseo.algos.opt.opt_lib import OptimizationLibrary
+from gemseo.algos.opt.optimization_library import OptimizationAlgorithmDescription
+from gemseo.algos.opt.optimization_library import OptimizationLibrary
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.algos.opt_result import OptimizationResult
 from gemseo.algos.stop_criteria import TerminationCriterion
-from gemseo.utils.python_compatibility import Final
 from numpy import inf
 from numpy import ndarray
 from numpy import prod as np_prod
 from numpy import size as np_size
 from numpy import unique as np_unique
 from pymoo.algorithms.moo.nsga2 import NSGA2
 from pymoo.algorithms.moo.nsga3 import NSGA3
@@ -102,21 +102,23 @@
 
     handle_equality_constraints: bool = False
 
     handle_inequality_constraints: bool = True
 
     positive_constraints: bool = False
 
-    problem_type: str = OptimizationProblem.NON_LINEAR_PB
+    problem_type: OptimizationProblem.ProblemType = (
+        OptimizationProblem.ProblemType.NON_LINEAR
+    )
 
 
 class PymooOpt(OptimizationLibrary):
     """Pymoo optimization library interface.
 
-    See :class:`gemseo.algos.opt.opt_lib.OptimizationLibrary`.
+    See :class:`gemseo.algos.opt.optimization_library.OptimizationLibrary`.
     """
 
     N_PROCESSES: Final[str] = "n_processes"
     """The tag for the number of processes to use."""
 
     MAX_GEN: Final[str] = "max_gen"
     """The tag for the maximum number of generations allowed."""
@@ -838,15 +840,15 @@
         if len(self.problem.database) == 0:
             return MultiObjectiveOptimizationResult(
                 optimizer_name=self.algo_name,
                 message=message,
                 status=status,
                 n_obj_call=0,
             )
-        x_0 = self.problem.database.get_x_by_iter(0)
+        x_0 = self.problem.database.get_x_vect(1)
         # Compute the best feasible or infeasible point.
         f_opt, x_opt, is_feas, c_opt, c_opt_grad = self.problem.get_optimum()
 
         if f_opt is not None and not self.problem.minimize_objective:
             f_opt = -f_opt
 
         # There are no pareto efficient solutions for unfeasible problems.
@@ -857,15 +859,15 @@
             x_opt=x_opt,
             f_opt=f_opt,  # objective vector norm
             optimizer_name=self.algo_name,
             message=message,
             status=status,
             n_obj_call=self.problem.objective.n_calls,
             is_feasible=is_feas,
-            constraints_values=c_opt,
+            constraint_values=c_opt,
             constraints_grad=c_opt_grad,
             pareto=pareto,
         )
 
     def _check_design_space_exploration(self, design_variables: ndarray) -> None:
         """Check on the design space exploration.
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_GA_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_GA_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA2_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA2_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA3_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_NSGA3_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_RNSGA3_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_RNSGA3_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt/options/PYMOO_UNSGA3_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt/options/PYMOO_UNSGA3_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/opt_result_mo.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/opt_result_mo.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import logging
 from dataclasses import dataclass
 
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.algos.opt_result import OptimizationResult
 from gemseo.algos.opt_result import Value
 from gemseo.algos.pareto_front import compute_pareto_optimal_points
-from gemseo.core.dataset import Dataset
 from gemseo.third_party.prettytable import PrettyTable
 from gemseo.utils.string_tools import MultiLineString
 from numpy import all as np_all
 from numpy import argwhere
 from numpy import array
 from numpy import concatenate as np_concat
 from numpy import max as np_max
@@ -78,20 +77,20 @@
 
         # Point with the lowest norm (closest to the utopia point).
         self._min_norm_f, self._min_norm_x, self._min_norm = self.get_lowest_norm(
             self._front, self._set, self._utopia
         )
 
         # Get dataset as a dataframe.
-        df = self._problem.export_to_dataset().export_to_dataframe()
+        df = self._problem.to_dataset()
         df.index = df.index.astype(int)
 
         # Get design variables group,
         # and reorder the columns to match the design space order.
-        df_dp = df[Dataset.DESIGN_GROUP][problem.design_space.variables_names]
+        df_dp = df.get_view(variable_names=problem.design_space.variable_names)
         ind_anchor = [df.index[np_all(df_dp == p, axis=1)][0] for p in self._anchor_set]
         ind_min_norm = [
             df.index[np_all(df_dp == p, axis=1)][0] for p in self._min_norm_x
         ]
 
         # DataFrame with points of interest.
         df_anchor = df.loc[ind_anchor].droplevel(0, axis=1)
@@ -231,27 +230,26 @@
             gemseo_problem.get_ineq_constraints() + gemseo_problem.get_eq_constraints()
         )
 
         dv_history = zeros((n_iter, gemseo_problem.design_space.dimension))
         obj_history = zeros((n_iter, gemseo_problem.objective.dim))
         feasibility = zeros(n_iter)
 
+        iteration = 0
         for x_vect, out_val in gemseo_problem.database.items():
-            # Cast to int required for when importing from hdf file.
-            iteration = int(out_val["Iter"][0] - 1)
-
             dv_history[iteration] = x_vect.unwrap()
             if gemseo_problem.objective.name in out_val:
                 obj_history[iteration] = array(out_val[gemseo_problem.objective.name])
                 feasibility[iteration] = gemseo_problem.is_point_feasible(
                     out_val, constraints=constraints
                 )
             else:
                 obj_history[iteration] = float("nan")
                 feasibility[iteration] = False
+            iteration += 1
 
         pareto_opt_pts = compute_pareto_optimal_points(obj_history, feasibility)
         pareto_front = obj_history[pareto_opt_pts]
         pareto_set = dv_history[pareto_opt_pts]
 
         return pareto_front, pareto_set
 
@@ -309,17 +307,17 @@
             else:
                 content = [name]
             content += list(row.values)
             table.add_row(content)
         table.align = "r"
         return table
 
-    def __str__(self):
+    def __str__(self) -> str:
         obj_names = [self._problem.get_objective_name()]
-        c_names = self._problem.get_constraints_names()
+        c_names = self._problem.get_constraint_names()
         dv_names = self._problem.get_design_variable_names()
 
         msg = MultiLineString()
         msg.add(
             "Pareto optimal points : {} / {}",
             self._front.shape[0],
             len(self._problem.database),
@@ -370,15 +368,15 @@
 @dataclass
 class MultiObjectiveOptimizationResult(OptimizationResult):
     """The result of a multi-objective optimization."""
 
     pareto: Pareto | None = None
     """The pareto efficient solutions."""
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         msg = MultiLineString()
         msg.add("Multi-objective optimization result:")
         msg.indent()
         msg.add("Design variables: {}", self.x_opt)
         msg.add("Objective function: {}", self.f_opt)
         msg.add("Feasible solution: {}", self.is_feasible)
         msg.add("Pareto available: {}", self.pareto is not None)
@@ -386,15 +384,15 @@
             msg.indent()
             msg.add("Number of point: {}", self.pareto.front.shape[0])
             msg.add("Lowest norm: {}", self.f_opt)
             msg.add("Design variables: {}", self.x_opt)
             msg.dedent()
         return str(msg)
 
-    def __str__(self):
+    def __str__(self) -> str:
         msg = MultiLineString()
         msg.add("Multi-objective optimization result:")
         msg.indent()
         msg.add("Optimizer info:")
         msg.indent()
         msg.add("Status: {}", self.status)
         msg.add("Message: {}", self.message)
@@ -411,15 +409,15 @@
         return str(msg)
 
     def to_dict(self) -> dict[str, Value]:
         """Convert the multi-objective optimization result to a dictionary.
 
         The keys are the names of the optimization result fields,
         except for the constraint values, gradients and the :attr:`.pareto`.
-        The key ``"constr:y"`` maps to ``result.constraints_values["y"]``,
+        The key ``"constr:y"`` maps to ``result.constraint_values["y"]``,
         ``"constr_grad:y"`` maps to ``result.constraints_grad["y"]`` and
         ``"pareto:y"`` maps to ``result.pareto.y``.
 
         Returns:
             A dictionary representation of the optimization result.
         """
         dict_ = super().to_dict()
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/algos/stop_criteria.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/algos/stop_criteria.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Compromise_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Compromise_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Petal_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Petal_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/Radar_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/Radar_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/ScatterPareto_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/ScatterPareto_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/compromise.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/compromise.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Compromise(ScatterPareto):
     """Scatter plot with pareto front and compromise points.
 
-    See `Compromise Programming
-    <https://pymoo.org/mcdm/index.html#Compromise-Programming>`_.
+    See
+    `Compromise Programming <https://pymoo.org/mcdm/index.html#Compromise-Programming>`_.
     """
 
     fig_title = "Compromise Points"
 
     fig_name_prefix = "compromise"
 
     SCALARIZATION_FUNCTIONS: dict[str, str] = {
@@ -116,15 +116,14 @@
         # Initialize decomposition function.
         decomposition = get_decomposition(scalar_name, **scalar_options)
 
         # Prepare points to plot.
         points = []  # Points' coordinates.
         point_labels = []  # Points' labels.
         for weight in weights:
-
             # Apply decomposition.
             d_res = decomposition.do(
                 pareto.front,
                 weight,
                 utopian_point=pareto.utopia,
                 nadir_point=pareto.anti_utopia,
                 **scalar_options,
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/MultiObjectiveDiagram_options.json` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/MultiObjectiveDiagram_options.json`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/multi_objective_diagram.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/multi_objective_diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 
         # Initialize decomposition function.
         decomp = get_decomposition(scalar_name, **scalar_options)
 
         # Prepare points to plot.
         points, title = [], []
         for weight in weights:
-
             # Apply decomposition.
             d_res = decomp.do(
                 pareto.front,
                 weight,
                 utopian_point=pareto.utopia,
                 nadir_point=pareto.anti_utopia,
                 **scalar_options,
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/core/plot_features.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/core/plot_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         return min(z0, z1)
 
 
 class Annotation3D(Annotation):
     """Annotation for 3D plots."""
 
     _vertices_3d: ndarray
-    """The 2D array containing the starting and ending positions
-    of the vector to be annotated."""
+    """The 2D array containing the starting and ending positions of the vector to be
+    annotated."""
 
     def __init__(self, text: str, xyzs: ndarray, *args: Any, **kwargs: Any) -> None:
         """Instantiate a 3D annotation.
 
         Args:
             text: The annotation text.
             xyzs: 2D array containing the starting and ending positions of the vector to
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/high_tradeoff.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/high_tradeoff.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 class HighTradeOff(ScatterPareto):
     """Scatter plot with pareto front and high trade-off points.
 
-    See `High Trade-Off Points <https://pymoo.org/mcdm/index.html#nb-high-tradeoff>`_.
+    See High Trade-Off Points
+    `here<https://pymoo.org/mcdm/index.html#nb-high-tradeoff>`_.
     """
 
     fig_title = "High Trade-Off Points"
 
     fig_name_prefix = "high_tradeoff"
 
     prop_interest = dict(color="navy", alpha=1.0, s=30, zorder=3)
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/petal.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/petal.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/radar.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/radar.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from gemseo_pymoo.post.core.multi_objective_diagram import MultiObjectiveDiagram
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Radar(MultiObjectiveDiagram):
-    """`Radar plots <https://pymoo.org/visualization/radar.html>`_).
+    """`Radar plots <https://pymoo.org/visualization/radar.html>`_.
 
     Note:
         This post-processor assumes the optimization has converged to a well-defined
         pareto front.
     """
 
     def _plot(
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/post/scatter_pareto.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/post/scatter_pareto.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,14 @@
                 for point, label in zip(points, point_labels):
                     plot.add(point, label=label, **self.prop_interest)
         plot.do()
 
         # Create arrows.
         if plot_arrow:
             for point in points:
-
                 # Arrow vector.
                 vect = point - pareto.utopia
                 norm = np_norm(vect)
 
                 if n_obj == 2:
                     arr = FancyArrowPatch(pareto.utopia, point, **self.prop_arrow)
                     rot = 90 if vect[0] == 0 else degrees(arctan(vect[1] / vect[0]))
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/__init__.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/chankong_haimes.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/chankong_haimes.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,39 +87,39 @@
 
         super().__init__(design_space)
 
         # Set objective function.
         self.objective = MDOFunction(
             self.compute_objective,
             name="changkong_haimes",
-            f_type=MDOFunction.TYPE_OBJ,
+            f_type=MDOFunction.FunctionType.OBJ,
             jac=self.compute_objective_jacobian,
             expr="[2 + (x-2)**2 + (y-1)**2, 9*x - (y-1)**2]",
-            args=["x", "y"],
+            input_names=["x", "y"],
             dim=2,
         )
 
         ineq1 = MDOFunction(
             self.compute_constraint_1,
             name="ineq1",
-            f_type=MDOFunction.TYPE_INEQ,
+            f_type=MDOFunction.ConstraintType.INEQ,
             jac=self.compute_constraint_1_jacobian,
             expr="x**2 + y**2 - 225",
-            args=["x", "y"],
+            input_names=["x", "y"],
             dim=1,
         )
         self.add_ineq_constraint(ineq1)
 
         ineq2 = MDOFunction(
             self.compute_constraint_2,
             name="ineq2",
-            f_type=MDOFunction.TYPE_INEQ,
+            f_type=MDOFunction.ConstraintType.INEQ,
             jac=self.compute_constraint_2_jacobian,
             expr="x - 3*y + 10",
-            args=["x", "y"],
+            input_names=["x", "y"],
             dim=1,
         )
         self.add_ineq_constraint(ineq2)
 
     @staticmethod
     def compute_objective(design_variables: ndarray) -> ndarray:
         """Compute the objectives of the Chankong and Haimes function.
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/knapsack.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/knapsack.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
 """
 from __future__ import annotations
 
 import logging
 
 from gemseo.algos.design_space import DesignSpace
-from gemseo.algos.design_space import DesignVariableType
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from numpy import atleast_1d
 from numpy import ndarray
 from numpy import ones
 from numpy import sum as np_sum
 from numpy import zeros
@@ -179,57 +178,61 @@
         self.values = values
         self.weights = weights
         self.capacity_items = capacity_items
         self.capacity_weight = capacity_weight
 
         design_space = DesignSpace()
         design_space.add_variable(
-            "x", size=n_items, l_b=0, u_b=items_ub, var_type=DesignVariableType.INTEGER
+            "x",
+            size=n_items,
+            l_b=0,
+            u_b=items_ub,
+            var_type=DesignSpace.DesignVariableType.INTEGER,
         )
         if initial_guess is None:
             design_space.set_current_value(zeros(n_items))
         elif len(initial_guess) == n_items:
             design_space.set_current_value(zeros(n_items))
         else:
             raise ValueError(f"initial_guess must have {n_items} elements!")
 
         super().__init__(design_space)
 
         self.objective = MDOFunction(
             self.compute_knapsack_value,
             name="knapsack",
-            f_type=MDOFunction.TYPE_OBJ,
+            f_type=MDOFunction.FunctionType.OBJ,
             expr="sum(values * x)",
-            args=["x"],
+            input_names=["x"],
             dim=1,
         )
 
         # Maximize knapsack value.
         self.change_objective_sign()
 
         # Knapsack weight limit.
         if capacity_weight is not None:
             ineq_weight = MDOFunction(
                 self._compute_weight_constraint,
                 name="weight_surpass",
-                f_type=MDOFunction.TYPE_INEQ,
+                f_type=MDOFunction.ConstraintType.INEQ,
                 expr="sum(weights * x) - capacity_weight",
-                args=["x"],
+                input_names=["x"],
                 dim=1,
             )
             self.add_ineq_constraint(ineq_weight)
 
         # Knapsack number of items limit.
         if capacity_items is not None:
             ineq_items = MDOFunction(
                 self._compute_items_constraint,
                 name="items_surpass",
-                f_type=MDOFunction.TYPE_INEQ,
+                f_type=MDOFunction.ConstraintType.INEQ,
                 expr="sum(x) - capacity_items",
-                args=["x"],
+                input_names=["x"],
                 dim=1,
             )
             self.add_ineq_constraint(ineq_items)
 
     def _compute_weight_constraint(self, design_variables: ndarray) -> ndarray:
         """Compute the weight capacity constraint.
 
@@ -344,17 +347,17 @@
             initial_guess,
         )
 
         # Set objective function.
         self.objective = MDOFunction(
             self._compute_objective,
             name="knapsack",
-            f_type=MDOFunction.TYPE_OBJ,
+            f_type=MDOFunction.FunctionType.OBJ,
             expr="[-sum(values * x), sum(x)]",
-            args=["x"],
+            input_names=["x"],
             dim=2,
         )
 
         # Reset minimization goal.
         self.minimize_objective = True
 
     def _compute_objective(self, design_variables: ndarray) -> ndarray:
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo/problems/analytical/viennet.py` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo/problems/analytical/viennet.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 
         super().__init__(design_space)
 
         # Set objective function.
         self.objective = MDOFunction(
             self.compute_objective,
             name="viennet",
-            f_type=MDOFunction.TYPE_OBJ,
+            f_type=MDOFunction.FunctionType.OBJ,
             jac=self.compute_objective_jacobian,
             expr="[(x**2 + y**2) / 2 + sin(x**2 + y**2), 9*x - (y-1)**2,"
             "(3*x - 2*y + 4)**2 / 8 + (x - y + 1)^2 / 27 + 15,"
             "1 / (x**2 + y**2 + 1) - 1.1*exp(-(x**2 + y**2))]",
-            args=["x", "y"],
+            input_names=["x", "y"],
             dim=3,
         )
 
     @staticmethod
     def compute_objective(design_variables: ndarray) -> ndarray:
         """Compute the objectives of the Viennet function.
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/PKG-INFO` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: gemseo-pymoo
-Version: 1.1.1
+Version: 1.1.2
 Summary: A GEMSEO wrapper for pymoo optimization algorithms.
 Home-page: https://www.irt-saintexupery.com
 Author: Francois Gallard
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-pymoo
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-pymoo/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-pymoo-1.1.1/src/gemseo_pymoo.egg-info/SOURCES.txt` & `gemseo-pymoo-1.1.2/src/gemseo_pymoo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 LICENSES/headers/LGPL-3.0.txt
 requirements/check.in
 requirements/check.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/doc.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_pymoo/__init__.py
 src/gemseo_pymoo.egg-info/PKG-INFO
 src/gemseo_pymoo.egg-info/SOURCES.txt
 src/gemseo_pymoo.egg-info/dependency_links.txt
 src/gemseo_pymoo.egg-info/entry_points.txt
```

### Comparing `gemseo-pymoo-1.1.1/tests/__init__.py` & `gemseo-pymoo-1.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/algos/__init__.py` & `gemseo-pymoo-1.1.2/tests/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/algos/opt/__init__.py` & `gemseo-pymoo-1.1.2/tests/algos/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/algos/opt/test_opt_result_mo.py` & `gemseo-pymoo-1.1.2/tests/algos/opt/test_opt_result_mo.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,29 +82,32 @@
     for key in keys[2:]:
         database.get(key).pop(problem_2obj.objective.name)
     pareto = Pareto(problem_2obj)
 
     # Check problem property.
     assert pareto.problem == problem_2obj
 
-    obj0 = database.get_f_of_x(obj_name, keys[0])
-    obj1 = database.get_f_of_x(obj_name, keys[1])
+    obj0 = database.get_function_value(obj_name, keys[0])
+    obj1 = database.get_function_value(obj_name, keys[1])
     if len(pareto.front) == 1:
         assert (obj0 in pareto.front) or (obj1 in pareto.front)
     else:
         assert (obj0 in pareto.front) and (obj1 in pareto.front)
 
     # Check if the anchor points are in database.
     for anchor_point, anchor_obj in zip(pareto.anchor_set, pareto.anchor_front):
         assert_array_equal(
-            database.get_f_of_x(problem_2obj.objective.name, anchor_point), anchor_obj
+            database.get_function_value(problem_2obj.objective.name, anchor_point),
+            anchor_obj,
         )
 
     # Check if the minimum norm point is in database.
-    assert pareto.min_norm_f in database.get_func_history(problem_2obj.objective.name)
+    assert pareto.min_norm_f in database.get_function_history(
+        problem_2obj.objective.name
+    )
 
 
 def test_get_lowest_norm(result):
     """Test the method :meth:`gemseo_pymoo.algos.opt_result_mo.Pareto.get_lowest_norm`.
 
     Args:
         result: Fixture returning a
@@ -161,15 +164,15 @@
 
     Args:
         tmp_wd: Fixture to move into a temporary working directory.
         problem_2obj: Fixture returning the multi-objective
             optimization problem to export.
     """
     file_path = tmp_wd / "problem.h5"
-    problem_2obj.export_hdf(file_path)
+    problem_2obj.to_hdf(file_path)
 
     assert file_path.exists()
 
     problem_2obj_imported = import_hdf(file_path)
 
     assert isinstance(problem_2obj_imported.solution, MultiObjectiveOptimizationResult)
     assert isinstance(problem_2obj_imported.solution.pareto, Pareto)
@@ -181,15 +184,15 @@
 
     Args:
         tmp_wd: Fixture to move into a temporary working directory.
     """
     file_path = tmp_wd / "problem.h5"
 
     problem = Power2()
-    problem.export_hdf(file_path)
+    problem.to_hdf(file_path)
 
     assert file_path.exists()
 
     problem_imported = import_hdf(file_path)
 
     assert problem_imported.solution is None
     assert str(problem_imported.solution) == str(problem.solution)
```

### Comparing `gemseo-pymoo-1.1.1/tests/algos/opt/test_pymoo_algos.py` & `gemseo-pymoo-1.1.2/tests/algos/opt/test_pymoo_algos.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import logging
 from contextlib import nullcontext as does_not_raise
 from typing import Any
 
 import pytest
 from gemseo.algos.opt.opt_factory import OptimizersFactory
 from gemseo.algos.opt_problem import OptimizationProblem
-from gemseo.core.grammars.errors import InvalidDataException
+from gemseo.core.grammars.errors import InvalidDataError
 from gemseo.problems.analytical.binh_korn import BinhKorn
 from gemseo.problems.analytical.power_2 import Power2
 from gemseo.problems.analytical.rosenbrock import Rosenbrock
 from gemseo_pymoo.algos.opt.core.pymoo_problem_adapater import get_gemseo_opt_problem
 from gemseo_pymoo.problems.analytical.chankong_haimes import ChankongHaimes
 from gemseo_pymoo.problems.analytical.knapsack import MultiObjectiveKnapsack
 from gemseo_pymoo.problems.analytical.viennet import Viennet
@@ -123,15 +123,15 @@
     """Create a Power2 problem with integer variables and only inequality constraints.
 
     Returns:
         A :class:`.Power2` instance.
     """
     power2 = Power2()
     power2.constraints = power2.get_ineq_constraints()
-    power2.design_space.variables_types["x"] = array(["integer"] * 3)
+    power2.design_space.variable_types["x"] = array(["integer"] * 3)
 
     x_opt = array([1, 1, 0])
     f_opt = Power2().pow2(x_opt)
     power2.solution = (x_opt, f_opt)
 
     return power2
 
@@ -208,15 +208,15 @@
     elif algo_name == "PYMOO_RNSGA3":
         options["ref_points"] = array([[1.0], [2.0]])
 
     lib = opt_factory.create(algo_name)
     opt_grammar = lib.init_options_grammar(algo_name)
     try:
         opt_grammar.validate(options, raise_exception=True)
-    except InvalidDataException as exception:
+    except InvalidDataError as exception:
         pytest.fail(exception)
 
 
 @pytest.mark.parametrize(
     "pymoo_problem, expectation",
     [
         (
@@ -336,15 +336,15 @@
         args: The arguments for the optimization problem class.
         kwargs: The keyword arguments for the optimization problem class.
         x_opt: The design variables values at the optimum point.
         f_opt: The objective value at the optimum point.
     """
     problem = problem_class(*args, **kwargs)
     ds_dim = problem.design_space.dimension
-    problem.design_space.variables_types["x"] = array(["integer"] * ds_dim)
+    problem.design_space.variable_types["x"] = array(["integer"] * ds_dim)
 
     # Only inequality constraints are considered.
     problem.constraints = problem.get_ineq_constraints()
 
     options = dict(
         max_iter=2**11,
         stop_crit_n_hv=999,
```

### Comparing `gemseo-pymoo-1.1.1/tests/conftest.py` & `gemseo-pymoo-1.1.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test helpers."""
 from __future__ import annotations
 
-from gemseo.utils.pytest_conftest import *  # noqa: F401 F403
+from gemseo.utils.testing.pytest_conftest import *  # noqa: F401 F403
```

### Comparing `gemseo-pymoo-1.1.1/tests/post/__init__.py` & `gemseo-pymoo-1.1.2/tests/post/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/compromise_viennet_aasf.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/compromise_viennet_aasf.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/compromise_viennet_perp_dist.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/compromise_viennet_perp_dist.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/high_tradeoff_viennet_no_extra.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/high_tradeoff_viennet_no_extra.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/petal_viennet_tchebi.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/petal_viennet_tchebi.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/petal_viennet_weighted_sum.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/petal_viennet_weighted_sum.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/radar_viennet_asf.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/radar_viennet_asf.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/radar_viennet_pbi.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/radar_viennet_pbi.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/baseline_images/test_pymoo_post/scatter_pareto_viennet.png` & `gemseo-pymoo-1.1.2/tests/post/baseline_images/test_pymoo_post/scatter_pareto_viennet.png`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/post/test_pymoo_post.py` & `gemseo-pymoo-1.1.2/tests/post/test_pymoo_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from pathlib import Path
 
 import pytest
 from gemseo.algos.opt.opt_factory import OptimizersFactory
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.post.post_factory import PostFactory
 from gemseo.problems.analytical.power_2 import Power2
-from gemseo.utils.testing import image_comparison
+from gemseo.utils.testing.helpers import image_comparison
 from gemseo_pymoo.post.scatter_pareto import ScatterPareto
 from gemseo_pymoo.problems.analytical.chankong_haimes import ChankongHaimes
 from gemseo_pymoo.problems.analytical.viennet import Viennet
 from numpy import array
 
 
 @pytest.fixture
```

### Comparing `gemseo-pymoo-1.1.1/tests/problems/__init__.py` & `gemseo-pymoo-1.1.2/tests/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/problems/analytical/__init__.py` & `gemseo-pymoo-1.1.2/tests/problems/analytical/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/problems/analytical/test_chankong_haimes.py` & `gemseo-pymoo-1.1.2/tests/problems/analytical/test_chankong_haimes.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/problems/analytical/test_knapsack.py` & `gemseo-pymoo-1.1.2/tests/problems/analytical/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tests/problems/analytical/test_viennet.py` & `gemseo-pymoo-1.1.2/tests/problems/analytical/test_viennet.py`

 * *Files identical despite different names*

### Comparing `gemseo-pymoo-1.1.1/tox.ini` & `gemseo-pymoo-1.1.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 skip_install = true
-whitelist_externals =
-    git
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -66,35 +65,38 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-pymoo[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
+whitelist_externals =
+    pip-compile
+    check: pre-commit
 commands =
     doc: pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra doc -o requirements/doc.txt
     dist: pip-compile --upgrade requirements/dist.in
     check: pip-compile --upgrade requirements/check.in
     check: pre-commit autoupdate
 
-[testenv:update-deps-test-py{37,38,39,310}]
+[testenv:update-deps-test-py{38,39,310}]
 description = update the test envs dependencies
 extras = {[testenv]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
 commands =
```

