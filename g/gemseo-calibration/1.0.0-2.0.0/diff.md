# Comparing `tmp/gemseo-calibration-1.0.0.tar.gz` & `tmp/gemseo-calibration-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-calibration-1.0.0.tar", last modified: Thu Jul 28 09:49:48 2022, max compression
+gzip compressed data, was "gemseo-calibration-2.0.0.tar", last modified: Mon Jun  5 12:03:39 2023, max compression
```

## Comparing `gemseo-calibration-1.0.0.tar` & `gemseo-calibration-2.0.0.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.141438 gemseo-calibration-1.0.0/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      450 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/.gitattributes
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      197 2022-07-22 13:34:38.000000 gemseo-calibration-1.0.0/.gitignore
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2450 2022-07-25 06:57:34.000000 gemseo-calibration-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2491 2022-07-26 08:01:51.000000 gemseo-calibration-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     9105 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/.pylintrc
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      953 2022-07-27 19:23:31.000000 gemseo-calibration-1.0.0/CHANGELOG.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1798 2022-07-22 13:56:03.000000 gemseo-calibration-1.0.0/CREDITS.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2022-03-24 13:18:51.000000 gemseo-calibration-1.0.0/LICENSE.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.123438 gemseo-calibration-1.0.0/LICENSES/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7652 2022-03-24 13:18:51.000000 gemseo-calibration-1.0.0/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.124438 gemseo-calibration-1.0.0/LICENSES/headers/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      729 2022-03-24 13:18:51.000000 gemseo-calibration-1.0.0/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      334 2022-03-24 13:18:51.000000 gemseo-calibration-1.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      710 2022-03-24 13:18:51.000000 gemseo-calibration-1.0.0/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2531 2022-07-28 09:49:48.141438 gemseo-calibration-1.0.0/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1400 2022-07-27 19:24:04.000000 gemseo-calibration-1.0.0/README.rst
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.119438 gemseo-calibration-1.0.0/doc_src/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.119438 gemseo-calibration-1.0.0/doc_src/examples/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.125438 gemseo-calibration-1.0.0/doc_src/examples/calibration/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      427 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/README.rst
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     4088 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3816 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_1param.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     5531 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_mesh.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1903 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_missing_values.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     7082 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_noise.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      611 2022-07-19 15:02:00.000000 gemseo-calibration-1.0.0/pyproject.toml
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.128438 gemseo-calibration-1.0.0/requirements/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       79 2022-06-07 09:46:46.000000 gemseo-calibration-1.0.0/requirements/check.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      596 2022-07-26 08:01:39.000000 gemseo-calibration-1.0.0/requirements/check.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       12 2022-06-07 09:46:46.000000 gemseo-calibration-1.0.0/requirements/dist.in
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1373 2022-07-26 08:01:56.000000 gemseo-calibration-1.0.0/requirements/dist.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2231 2022-07-28 08:40:44.000000 gemseo-calibration-1.0.0/requirements/doc.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2923 2022-07-28 08:40:30.000000 gemseo-calibration-1.0.0/requirements/test-python3.10.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3179 2022-07-28 08:39:47.000000 gemseo-calibration-1.0.0/requirements/test-python3.7.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2921 2022-07-28 08:40:02.000000 gemseo-calibration-1.0.0/requirements/test-python3.8.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2921 2022-07-28 08:40:16.000000 gemseo-calibration-1.0.0/requirements/test-python3.9.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1630 2022-07-28 09:49:48.142438 gemseo-calibration-1.0.0/setup.cfg
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      839 2022-07-22 13:56:04.000000 gemseo-calibration-1.0.0/setup.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.119438 gemseo-calibration-1.0.0/src/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.129438 gemseo-calibration-1.0.0/src/gemseo_calibration/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      652 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/CalibrationScenario_input.json
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      212 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/CalibrationScenario_output.json
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      847 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    12487 2022-07-22 13:33:28.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/calibrator.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3606 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measure.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.132438 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      846 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2453 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/factory.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1231 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/iae.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2700 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/integrated_measure.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1229 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/ise.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1201 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mae.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1370 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mean_measure.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1199 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mse.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.133438 gemseo-calibration-1.0.0/src/gemseo_calibration/post/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      835 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.134438 gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      521 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/DataVersusModel_options.json
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      825 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2248 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/post.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3685 2022-06-07 11:22:40.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/factory.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3545 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post/multiple_scatter.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1822 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/post_processor.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     8953 2022-07-22 13:33:28.000000 gemseo-calibration-1.0.0/src/gemseo_calibration/scenario.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.130438 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2531 2022-07-28 09:49:48.000000 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/PKG-INFO
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3262 2022-07-28 09:49:48.000000 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/SOURCES.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        1 2022-07-28 09:49:48.000000 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/dependency_links.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       87 2022-07-28 09:49:48.000000 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/requires.txt
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)       19 2022-07-28 09:49:48.000000 gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/top_level.txt
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.135438 gemseo-calibration-1.0.0/tests/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      463 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/NewCalibrationPostProcessor_options.json
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      770 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1789 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/conftest.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.136438 gemseo-calibration-1.0.0/tests/data/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      460 2022-02-24 16:55:13.000000 gemseo-calibration-1.0.0/tests/data/NewCalibrationPostProcessor_options.json
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      770 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/data/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1650 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/data/measures.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1968 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/data/post.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.137438 gemseo-calibration-1.0.0/tests/measures/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      770 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/measures/__init__.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1166 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/measures/test_mae.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3705 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/measures/test_mean_error.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1294 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/measures/test_mse.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.138438 gemseo-calibration-1.0.0/tests/post/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      770 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.120438 gemseo-calibration-1.0.0/tests/post/baseline_images/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.140438 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    17965 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/default.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    19149 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    19139 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_color.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    19138 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_colors.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    19007 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_components.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    17977 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_color.png
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.140438 gemseo-calibration-1.0.0/tests/post/data_versus_model/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)      770 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/data_versus_model/__init__.py
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.120438 gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/
-drwxr-xr-x   0 antoine.dechaume  (1000) antoine.dechaume  (1000)        0 2022-07-28 09:49:48.141438 gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    21273 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_y.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)    21072 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_z.png
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3260 2022-07-25 05:46:20.000000 gemseo-calibration-1.0.0/tests/post/data_versus_model/test_data_versus_model.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2371 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/post/test_factory.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3360 2022-07-25 05:46:20.000000 gemseo-calibration-1.0.0/tests/post/test_multiple_scatter.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     4032 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/test_calibrator.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     2906 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/test_measure.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     1522 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/test_post_processor.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     6214 2022-06-07 09:42:29.000000 gemseo-calibration-1.0.0/tests/test_scenario.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3699 2022-07-22 13:33:28.000000 gemseo-calibration-1.0.0/tests/test_scenario_with_meshed_output.py
--rw-r--r--   0 antoine.dechaume  (1000) antoine.dechaume  (1000)     3222 2022-07-25 05:47:41.000000 gemseo-calibration-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.477694 gemseo-calibration-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/CREDITS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.461694 gemseo-calibration-2.0.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.462694 gemseo-calibration-2.0.0/LICENSES/headers/
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/LICENSES/headers/BSD-0-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-06-05 12:03:39.477694 gemseo-calibration-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.455694 gemseo-calibration-2.0.0/doc_src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.455694 gemseo-calibration-2.0.0/doc_src/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.463694 gemseo-calibration-2.0.0/doc_src/examples/calibration/
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3835 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_1param.py
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_missing_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_noise.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.465694 gemseo-calibration-2.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/check.in
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/check.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/dist.in
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/dist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/test-python3.10.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/test-python3.8.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/requirements/test-python3.9.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-06-05 12:03:39.478694 gemseo-calibration-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.456694 gemseo-calibration-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.466694 gemseo-calibration-2.0.0/src/gemseo_calibration/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/CalibrationScenario_input.json
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/CalibrationScenario_output.json
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12555 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/calibrator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.469694 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/iae.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/integrated_measure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/ise.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mae.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mean_measure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.470694 gemseo-calibration-2.0.0/src/gemseo_calibration/post/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.470694 gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/DataVersusModel_options.json
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/post.py
+-rw-rw-rw-   0 root         (0) root         (0)     4837 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post/multiple_scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/post_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8999 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/src/gemseo_calibration/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.467694 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-06-05 12:03:39.000000 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-06-05 12:03:39.000000 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:03:39.000000 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-05 12:03:39.000000 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-05 12:03:39.000000 gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.472694 gemseo-calibration-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/NewCalibrationPostProcessor_options.json
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1697 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.473694 gemseo-calibration-2.0.0/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/data/NewCalibrationPostProcessor_options.json
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/data/measures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/data/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.474694 gemseo-calibration-2.0.0/tests/measures/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/measures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/measures/test_mae.py
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/measures/test_mean_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/measures/test_mse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.474694 gemseo-calibration-2.0.0/tests/post/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.457694 gemseo-calibration-2.0.0/tests/post/baseline_images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.476694 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/
+-rw-rw-rw-   0 root         (0) root         (0)    17965 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/default.png
+-rw-rw-rw-   0 root         (0) root         (0)    19149 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs.png
+-rw-rw-rw-   0 root         (0) root         (0)    19139 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_color.png
+-rw-rw-rw-   0 root         (0) root         (0)    19138 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_colors.png
+-rw-rw-rw-   0 root         (0) root         (0)    19007 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_components.png
+-rw-rw-rw-   0 root         (0) root         (0)    17977 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_color.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.476694 gemseo-calibration-2.0.0/tests/post/data_versus_model/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/data_versus_model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.458694 gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:03:39.477694 gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/
+-rw-rw-rw-   0 root         (0) root         (0)    21273 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_y.png
+-rw-rw-rw-   0 root         (0) root         (0)    21072 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_z.png
+-rw-rw-rw-   0 root         (0) root         (0)     3931 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/data_versus_model/test_data_versus_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1553 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3465 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/post/test_multiple_scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/test_calibrator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/test_measure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/test_post_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/test_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tests/test_scenario_with_meshed_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-05 12:03:22.000000 gemseo-calibration-2.0.0/tox.ini
```

### Comparing `gemseo-calibration-1.0.0/.pylintrc` & `gemseo-calibration-2.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/CREDITS.rst` & `gemseo-calibration-2.0.0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/LICENSE.txt` & `gemseo-calibration-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/LICENSES/LGPLv3.txt` & `gemseo-calibration-2.0.0/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-calibration-2.0.0/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/LICENSES/headers/LGPL-3.0.txt` & `gemseo-calibration-2.0.0/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/PKG-INFO` & `gemseo-calibration-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-calibration
-Version: 1.0.0
+Version: 2.0.0
 Summary: Capability to calibrate GEMSEO disciplines from data.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-calibration
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-calibration/-/issues
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
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-calibration-1.0.0/README.rst` & `gemseo-calibration-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration.py` & `gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 prior = ParameterSpace()
 prior.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
 prior.add_variable("b", l_b=0.0, u_b=10.0, value=0.0)
 
 #######################################################################################
 # Secondly,
 # we have reference output data over the input space :math:`[0.,3.]`:
-reference.set_cache_policy("MemoryFullCache")
+reference.set_cache_policy(reference.CacheType.MEMORY_FULL)
 reference.execute({"x": array([1.0])})
 reference.execute({"x": array([2.0])})
-reference_data = reference.cache.export_to_dataset(by_group=True)
+reference_data = reference.cache.to_dataset().to_dict_of_arrays(False)
 
 #######################################################################################
 # From these information sources,
 # we can build and execute a :class:`.CalibrationScenario`
 # to find the value of the parameters :math:`a` and :math:`b`
 # which minimizes a :class:`.CalibrationMeasure`
 # taking into account the outputs :math:`y` and :math:`z`:
```

### Comparing `gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_1param.py` & `gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_1param.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 # we have a prior information about the parameters, that is :math:`a\in[0,10]`:
 prior = ParameterSpace()
 prior.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
 
 #######################################################################################
 # Secondly,
 # we have reference output data over the input space :math:`[0.,3.]`:
-reference.set_cache_policy("MemoryFullCache")
+reference.set_cache_policy(reference.CacheType.MEMORY_FULL)
 reference.execute({"x": array([1.0])})
-reference_data = reference.cache.export_to_dataset(by_group=True)
+reference_data = reference.cache.to_dataset().to_dict_of_arrays(False)
 
 #######################################################################################
 # From this unique observation,
 # we can build and execute a :class:`.CalibrationScenario`
 # to find the value of the parameter :math:`a`
 # which minimizes a :class:`.CalibrationMeasure`
 # taking into account the outputs :math:`y`:
```

### Comparing `gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_mesh.py` & `gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_mesh.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,42 +33,42 @@
 # In practice,
 # we could imagine a model having an output related to a mesh :math:`\gamma`
 # whose size and nodes would depend on the model inputs.
 # Thus, this mesh is also an output of the model.
 
 
 class Model(MDODiscipline):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.input_grammar.initialize_from_data_names(["x", "a", "b"])
-        self.output_grammar.initialize_from_data_names(["y", "z", "mesh"])
+        self.input_grammar.update_from_names(["x", "a", "b"])
+        self.output_grammar.update_from_names(["y", "z", "mesh"])
         self.default_inputs = {"x": array([0.0]), "a": array([0.0]), "b": array([0.0])}
 
-    def _run(self):
+    def _run(self) -> None:
         x_input = self.local_data["x"]
         a_parameter = self.local_data["a"]
         b_parameter = self.local_data["b"]
         y_output = a_parameter * x_input
         z_mesh = linspace(0, 1, 5)
         z_output = b_parameter * x_input[0] * z_mesh
         self.store_local_data(y=y_output, z=z_output, mesh=z_mesh)
 
 
 #######################################################################################
 # This is a model of a our reference data source,
 # which a kind of oracle providing input-output data
 # without the mathematical relationship behind it:
 class ReferenceModel(MDODiscipline):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.input_grammar.initialize_from_data_names(["x"])
-        self.output_grammar.initialize_from_data_names(["y", "z", "mesh"])
+        self.input_grammar.update_from_names(["x"])
+        self.output_grammar.update_from_names(["y", "z", "mesh"])
         self.default_inputs = {"x": array([0.0])}
 
-    def _run(self):
+    def _run(self) -> None:
         x_input = self.local_data["x"]
         y_output = 2 * x_input
         z_mesh = linspace(0, 1, 5)
         z_output = 3 * x_input[0] * z_mesh
         self.store_local_data(y=y_output, z=z_output, mesh=z_mesh)
 
 
@@ -88,18 +88,18 @@
 prior.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
 prior.add_variable("b", l_b=0.0, u_b=10.0, value=0.0)
 
 #######################################################################################
 # Secondly,
 # we have reference output data over the input space :math:`[0.,3.]`:
 reference = ReferenceModel()
-reference.set_cache_policy("MemoryFullCache")
+reference.set_cache_policy(reference.CacheType.MEMORY_FULL)
 reference.execute({"x": array([1.0])})
 reference.execute({"x": array([2.0])})
-reference_data = reference.cache.export_to_dataset(by_group=True)
+reference_data = reference.cache.to_dataset().to_dict_of_arrays(False)
 
 #######################################################################################
 # From these information sources,
 # we can build and execute a :class:`.CalibrationScenario`
 # to find the values of the parameters :math:`a` and :math:`b`
 # which minimizes a :class:`.CalibrationMeasure`
 # taking into account the outputs :math:`y` and :math:`z`:
```

### Comparing `gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_missing_values.py` & `gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_missing_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING
 # FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 # NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 from __future__ import annotations
 
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_calibration.scenario import CalibrationMeasure
 from gemseo_calibration.scenario import CalibrationScenario
 from numpy import array
 from numpy import NaN
 
 model = AnalyticDiscipline({"y": "a*x", "z": "b*x"}, name="model")
 
 prior = ParameterSpace()
 prior.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
 prior.add_variable("b", l_b=0.0, u_b=10.0, value=0.0)
 
-reference_data = Dataset()
 data = array(
     [[1, 1.0, 2.0, NaN], [2, 1.0, NaN, 3.0], [3, 2.0, 4.0, NaN], [4, 2.0, NaN, 6.0]]
 )
-reference_data.set_from_array(
+reference_data = Dataset.from_array(
     data,
-    variables=["index", "x", "y", "z"],
-    groups={"index": "inputs", "x": "inputs", "y": "outputs", "z": "outputs"},
-)
+    variable_names=["index", "x", "y", "z"],
+    variable_names_to_group_names={
+        "index": "inputs",
+        "x": "inputs",
+        "y": "outputs",
+        "z": "outputs",
+    },
+).to_dict_of_arrays(False)
 
 control_outputs = [CalibrationMeasure("y", "MSE"), CalibrationMeasure("z", "MSE")]
 calibration = CalibrationScenario(model, "x", control_outputs, prior)
 calibration.execute(
     {"algo": "NLOPT_COBYLA", "reference_data": reference_data, "max_iter": 100}
 )
```

### Comparing `gemseo-calibration-1.0.0/doc_src/examples/calibration/plot_calibration_with_noise.py` & `gemseo-calibration-2.0.0/doc_src/examples/calibration/plot_calibration_with_noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from __future__ import annotations
 
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
 from gemseo.core.chain import MDOChain
 from gemseo.core.doe_scenario import DOEScenario
 from gemseo.disciplines.analytic import AnalyticDiscipline
-from gemseo.disciplines.scenario_adapter import MDOScenarioAdapter
+from gemseo.disciplines.scenario_adapters.mdo_scenario_adapter import MDOScenarioAdapter
 from gemseo_calibration.scenario import CalibrationMeasure
 from gemseo_calibration.scenario import CalibrationScenario
 from matplotlib import pyplot as plt
 from numpy import array
 from numpy import linspace
 
 model = AnalyticDiscipline({"y": "a*x**2+b*x+c"}, name="model")
@@ -39,15 +39,15 @@
 #######################################################################################
 # This is a model of a our reference data source,
 # which a kind of oracle providing input-output data
 # without the mathematical relationship behind it:
 original_model = AnalyticDiscipline({"y": "2*x**2-1.5*x+0.75"}, name="model")
 
 reference = MDOChain([original_model, AnalyticDiscipline({"y": "y+u"}, name="noise")])
-reference.set_cache_policy("MemoryFullCache")
+reference.set_cache_policy(reference.CacheType.MEMORY_FULL)
 
 #######################################################################################
 # This reference model contains a random additive term :math:`u`
 # normally distributed with mean :math:`\mu` and standard deviation :math:`\sigma`.
 # This means that the observations of :math:`f:x\mapsto 2*x^2-0.5*x` are noised.
 
 #######################################################################################
@@ -96,15 +96,15 @@
 
 #######################################################################################
 # Then,
 # this :class:`.MDOScenarioAdapter` is embedded in a :class:`.DOEScenario`
 # in charge to sample it over the uncertain space.
 scenario = DOEScenario([adapter], "DisciplinaryOpt", "y", noise_space)
 scenario.execute({"algo": "OT_LHSC", "n_samples": 5})
-reference_data = reference.cache.export_to_dataset(by_group=True)
+reference_data = reference.cache.to_dataset().to_dict_of_arrays(False)
 
 #######################################################################################
 # From these information sources,
 # we can build and execute a :class:`.CalibrationScenario`
 # to find the value of the parameters :math:`a`, :math:`b` and :math:`c`
 # which minimizes a :class:`.CalibrationMeasure` related to the output :math:`y`:
 calibration = CalibrationScenario(model, "x", CalibrationMeasure("y", "MSE"), prior)
```

### Comparing `gemseo-calibration-1.0.0/pyproject.toml` & `gemseo-calibration-2.0.0/pyproject.toml`

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

### Comparing `gemseo-calibration-1.0.0/requirements/dist.txt` & `gemseo-calibration-2.0.0/requirements/dist.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile requirements/dist.in
 #
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.8.0
+build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-commonmark==0.9.1
-    # via rich
-cryptography==37.0.4
+cryptography==40.0.2
     # via secretstorage
-docutils==0.19
+docutils==0.20
     # via readme-renderer
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
+jaraco-classes==3.2.3
+    # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==23.7.0
+keyring==23.13.1
     # via twine
-packaging==21.3
-    # via build
-pep517==0.12.0
+markdown-it-py==2.2.0
+    # via rich
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+packaging==23.1
     # via build
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.12.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyparsing==3.0.9
-    # via packaging
-readme-renderer==35.0
+pyproject-hooks==1.0.0
+    # via build
+readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.3.5
     # via twine
-secretstorage==3.3.2
+secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
-    #   pep517
-twine==4.0.1
+    #   pyproject-hooks
+twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.11
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.8.1
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-calibration-1.0.0/requirements/doc.txt` & `gemseo-calibration-2.0.0/requirements/doc.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
 fastjsonschema==2.16.1
     # via gemseo
 fonttools==4.34.4
     # via matplotlib
-gemseo[all]==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-calibration (setup.py)
 genson==1.2.2
     # via gemseo
 graphviz==0.20
     # via gemseo
 h5py==3.6.0
     # via gemseo
```

### Comparing `gemseo-calibration-1.0.0/requirements/test-python3.10.txt` & `gemseo-calibration-2.0.0/requirements/test-python3.10.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,148 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==21.4.0
-    # via pytest
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-calibration (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-dill==0.3.5.1
+dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-calibration (setup.py)
 genson==1.2.2
     # via gemseo
-graphviz==0.20
+graphviz==0.20.1
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
-joblib==1.1.0
+joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-calibration (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.8.5
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.22.4
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
     #   gemseo-calibration (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
-openturns==1.18
+openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.4.3
-    # via gemseo
-pdfo==1.2
+pandas==2.0.0
     # via gemseo
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.1
+psutil==5.9.5
     # via openturns
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-calibration (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-calibration (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-calibration (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
+pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.30.0
     # via gemseo
-scikit-learn==1.1.1
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
 six==1.16.0
     # via python-dateutil
-sympy==1.10.1
+strenum==0.4.10
+    # via gemseo
+sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.11
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
```

### Comparing `gemseo-calibration-1.0.0/requirements/test-python3.7.txt` & `gemseo-calibration-2.0.0/requirements/test-python3.9.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,175 +1,152 @@
 #
-# This file is autogenerated by pip-compile with python 3.7
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==21.4.0
-    # via pytest
-cached-property==1.5.2
-    # via h5py
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-calibration (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-dill==0.3.5.1
+dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-calibration (setup.py)
 genson==1.2.2
     # via gemseo
-graphviz==0.20
+graphviz==0.20.1
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
-    # via
-    #   gemseo
-    #   pluggy
-    #   pytest
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
-joblib==1.1.0
+joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-calibration (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.6.3
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.21.6
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
     #   gemseo-calibration (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
-openturns==1.18
+openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.3.5
-    # via gemseo
-pdfo==1.2
+pandas==2.0.0
     # via gemseo
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.1
+psutil==5.9.5
     # via openturns
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-calibration (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-calibration (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-calibration (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
+pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.30.0
     # via gemseo
-scikit-learn==1.0.2
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
-singledispatchmethod==1.0
-    # via gemseo
 six==1.16.0
     # via python-dateutil
-sympy==1.10.1
+strenum==0.4.10
+    # via gemseo
+sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
-    # via
-    #   gemseo
-    #   importlib-metadata
-    #   kiwisolver
-urllib3==1.26.11
+typing-extensions==4.5.0
+    # via gemseo
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-calibration-1.0.0/requirements/test-python3.8.txt` & `gemseo-calibration-2.0.0/requirements/test-python3.8.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,161 +1,152 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==21.4.0
-    # via pytest
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.0
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-calibration (setup.py)
-coverage[toml]==6.4.2
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
-dill==0.3.5.1
+dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
+exceptiongroup==1.1.1
+    # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.1
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.34.4
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.0.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-calibration (setup.py)
 genson==1.2.2
     # via gemseo
-graphviz==0.20
+graphviz==0.20.1
     # via gemseo
-h5py==3.6.0
+h5py==3.8.0
     # via gemseo
-idna==3.3
+idna==3.4
     # via requests
-iniconfig==1.1.1
+importlib-resources==5.12.0
+    # via matplotlib
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
-joblib==1.1.0
+joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-calibration (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.8.5
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.22.4
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
     #   gemseo-calibration (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
-openturns==1.18
+openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.4.3
+pandas==2.0.0
     # via gemseo
-pdfo==1.2
-    # via gemseo
-pillow==9.2.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.1
+psutil==5.9.5
     # via openturns
-py==1.11.0
-    # via
-    #   pytest
-    #   pytest-forked
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.1.2
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-calibration (setup.py)
     #   pytest-cov
-    #   pytest-forked
     #   pytest-xdist
-pytest-cov==3.0.0
+pytest-cov==4.0.0
     # via gemseo-calibration (setup.py)
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-xdist==2.5.0
+pytest-xdist==3.3.0
     # via gemseo-calibration (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.1
+pytz==2023.3
     # via pandas
-pyxdsm==2.2.1
+pyxdsm==2.2.2
     # via gemseo
-requests==2.28.1
+requests==2.30.0
     # via gemseo
-scikit-learn==1.1.1
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
 six==1.16.0
     # via python-dateutil
-sympy==1.10.1
+strenum==0.4.10
+    # via gemseo
+sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.0
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.3.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.11
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.0.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-calibration-1.0.0/setup.cfg` & `gemseo-calibration-2.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,26 @@
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
 	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
-	gemseo[all] >=4.0.0
+	gemseo[all] >=5
 	matplotlib
 	numpy
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
@@ -59,19 +58,21 @@
 
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
-	tests/*.py:D
-	src/*.py:D
-	doc_src/*.py:D,T001
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-calibration-1.0.0/setup.py` & `gemseo-calibration-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/CalibrationScenario_input.json` & `gemseo-calibration-2.0.0/src/gemseo_calibration/CalibrationScenario_input.json`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/__init__.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/calibrator.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/calibrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 from collections import namedtuple
 from typing import Any
 from typing import Iterable
 from typing import Sequence
 
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.doe.lib_custom import CustomDOE
-from gemseo.core.dataset import Dataset
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.doe_scenario import DOEScenario
 from gemseo.core.grammars.json_grammar import JSONGrammar
-from gemseo.disciplines.scenario_adapter import MDOScenarioAdapter
+from gemseo.disciplines.scenario_adapters.mdo_scenario_adapter import MDOScenarioAdapter
 from numpy import array
+from numpy import hstack
 
 from gemseo_calibration.measure import CalibrationMeasure as CalibrationMeasure_
+from gemseo_calibration.measure import DataType
 from gemseo_calibration.measures.factory import CalibrationMeasureFactory
 
 CalibrationMeasure = namedtuple(
     "CalibrationMeasure", "output,measure,mesh,weight", defaults=["MSE", None, None]
 )
 
 LOGGER = logging.getLogger(__name__)
@@ -55,15 +56,15 @@
         self,
         disciplines: MDODiscipline | list[MDODiscipline],
         input_names: str | Iterable[str],
         control_outputs: CalibrationMeasure | Sequence[CalibrationMeasure],
         parameter_names: str | Iterable[str],
         formulation: str = "MDF",
         **formulation_options: Any,
-    ) -> None:  # noqa: D205,D212,D415
+    ) -> None:
         """
         Args:
             disciplines: The disciplines
                 whose parameters must be calibrated from the reference data.
             input_names: The names of the inputs to be considered for the calibration.
             control_outputs: The names of the outputs used to calibrate the disciplines
                 with the name of the calibration measure and the corresponding weight
@@ -75,15 +76,15 @@
                 or ``CalibrationMeasure(output="z", measure="MSE", mesh="z_mesh")``
                 Lastly, ``CalibrationMeasure`` can be imported
                 from :mod:`gemseo-calibration.scenario`.
             parameter_names: The names of the parameters to be calibrated.
             formulation: The name of a formulation
                 to manage the multidisciplinary coupling.
             **formulation_options: The options of the formulation.
-        """
+        """  # noqa: D205,D212,D415
         self.__measure_factory = CalibrationMeasureFactory()
         input_names = self.__to_iterable(input_names, str)
         control_outputs = self.__to_iterable(control_outputs, CalibrationMeasure)
         parameter_names = self.__to_iterable(parameter_names, str)
         disciplines = self.__to_iterable(disciplines, MDODiscipline)
         control_output = control_outputs[0]
         objective_name = control_output.output
@@ -115,15 +116,15 @@
         }
 
         self.__names_to_measures = {}
         self.__measures = []
         self.objective_name, output_names = self.add_measure(control_outputs)
         super().__init__(doe_scenario, parameter_names, output_names, name="Calibrator")
         self.__update_output_grammar()
-        self.__reference_data = None
+        self.__reference_data = {}
 
     @staticmethod
     def __to_iterable(obj: Any, cls: type) -> Iterable[Any]:
         """Cast an object to an iterable.
 
         Args:
             obj: The object to cast.
@@ -142,44 +143,44 @@
 
     def __update_output_grammar(self) -> None:
         """Redefine the output grammar from the names of the output measures.
 
         E.g. MSE(y,z) is the name of the MSE measure applied to the outputs y and z.
         """
         output_grammar = JSONGrammar("outputs")
-        output_grammar.update(self.__names_to_measures.keys())
+        output_grammar.update_from_names(self.__names_to_measures.keys())
         self.output_grammar = output_grammar
 
-    def set_reference_data(self, reference_data: Dataset) -> None:
+    def set_reference_data(self, reference_data: DataType) -> None:
         """Pass the reference data to the scenario and to the measures.
 
         Args:
             reference_data: The reference data with which to compare the discipline.
         """
         self.__reference_data = reference_data
         design_space = self.scenario.design_space
         for name in design_space:
             del design_space[name]
-            design_space.add_variable(name, size=reference_data.sizes[name])
+            design_space.add_variable(name, size=reference_data[name].shape[1])
 
-        inputs = self.scenario.get_optim_variables_names()
-        input_data = reference_data.get_data_by_names(inputs, False)
-        self.scenario.default_inputs[self.__ALGO_OPTIONS][self.__SAMPLES] = input_data
+        self.scenario.default_inputs[self.__ALGO_OPTIONS][self.__SAMPLES] = hstack(
+            reference_data[name] for name in self.scenario.get_optim_variable_names()
+        )
         for measure in self.__measures:
             measure.set_reference_data(self.__reference_data)
 
-    def _run(self):
+    def _run(self) -> None:
         root_logger = logging.getLogger()
         saved_level = root_logger.level
         root_logger.setLevel(logging.WARNING)
         super()._run()
         root_logger.setLevel(saved_level)
 
-    def _post_run(self):
-        model_dataset = self.scenario.export_to_dataset()
+    def _post_run(self) -> None:
+        model_dataset = self.scenario.to_dataset().to_dict_of_arrays(False)
         for name, measure in self.__names_to_measures.items():
             self.local_data[name] = array([measure(model_dataset)])
 
     @property
     def maximize_objective_measure(self) -> bool:
         """Whether to maximize the calibration measure related to the objectives."""
         return self.__names_to_measures[self.objective_name].maximize
@@ -298,10 +299,10 @@
         else:
             measure = self.__measure_factory.create(
                 control_output.measure, output_name=control_output.output
             )
             return measure, [control_output.output]
 
     @property
-    def reference_data(self) -> Dataset:
+    def reference_data(self) -> DataType:
         """The reference data used for the calibration."""
         return self.__reference_data
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measure.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measure.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,40 +12,50 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """A module to measure the consistency or the inconsistency between two data sets."""
 from __future__ import annotations
 
 from typing import ClassVar
+from typing import Dict
 
-from gemseo.core.dataset import Dataset
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from numpy import infty
 from numpy import nanmax
 from numpy import nanmin
 from numpy import ndarray
 
+DataType = Dict[str, ndarray]
+"""The type of data.
+
+The data are set as ``{variable_name: variable_values}``
+where ``variable_values`` is a 2D NumPy array
+whose rows are the samples and columns are the components of the variable.
+"""
+
 
 class CalibrationMeasure(MDOFunction):
     """A measure of the consistency (or inconsistency) between two data sets."""
 
     output_name: str
     """The name of the output used by the measure for calibration."""
 
     maximize: ClassVar[bool] = False
     """Whether to maximize the calibration measure."""
 
     def __init__(
-        self, output_name: str, name: str | None = None, f_type: str | None = None
+        self,
+        output_name: str,
+        name: str = "",
+        f_type: MDOFunction.FunctionType = MDOFunction.FunctionType.NONE,
     ) -> None:
-        # noqa: D205,D212,D415
         """
         Args:
             output_name: The name of the output to be taken into account by the measure.
-        """
+        """  # noqa: D205,D212,D415
         self.output_name = output_name
         super().__init__(None, name or self._compute_name(), f_type=f_type)
         self._lower_bound = -infty
         self._upper_bound = infty
         self._reference_data = []
 
     @property
@@ -53,15 +63,15 @@
         """The full name of the output."""
         return self.output_name
 
     def _compute_name(self) -> str:
         """Return the name of the measure."""
         return f"{self.__class__.__name__}({self.output_name})"
 
-    def set_reference_data(self, reference_dataset: Dataset) -> None:
+    def set_reference_data(self, reference_dataset: DataType) -> None:
         """Define the reference input-output data set.
 
         Args:
             reference_dataset: The reference input-output data set.
         """
         self._reference_data = reference_dataset[self.output_name]
         self._lower_bound = nanmin(self._reference_data)
@@ -72,30 +82,27 @@
 
         Args:
             data: The value of the output.
         """
         self._lower_bound = min(data.min(), self._lower_bound)
         self._upper_bound = max(data.max(), self._upper_bound)
 
-    def __call__(self, model_dataset: Dataset) -> float:
+    def __call__(self, model_dataset: DataType) -> float:
         """Measure the (in)consistency between the model dataset and the reference one.
 
         Args:
             model_dataset: The model dataset.
 
         Returns:
             The measure of the (in)consistency between the model and reference datasets.
         """
         raise NotImplementedError
 
     @staticmethod
-    def _compare_data(
-        data: ndarray,
-        other_data: ndarray,
-    ) -> ndarray:
+    def _compare_data(data: ndarray, other_data: ndarray) -> ndarray:
         """Compare two data arrays.
 
         Args:
             data: The first data array.
             other_data: The second data array.
 
         Returns:
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/__init__.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/iae.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/iae.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,9 @@
 from gemseo_calibration.measures.integrated_measure import IntegratedMeasure
 
 
 class IAE(IntegratedMeasure):
     """The integrated absolute error between the model and reference output data."""
 
     @staticmethod
-    def _compare_data(
-        data: ndarray,
-        other_data: ndarray,
-    ) -> ndarray:
+    def _compare_data(data: ndarray, other_data: ndarray) -> ndarray:
         return abs(data - other_data)
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/integrated_measure.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/integrated_measure.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,49 +11,47 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """A module to compute the integrated measure between two data sets."""
 from __future__ import annotations
 
-from gemseo.core.dataset import Dataset
 from numpy import interp
 from numpy import mean
 from numpy import trapz as integrate
 
 from gemseo_calibration.measure import CalibrationMeasure
+from gemseo_calibration.measure import DataType
 
 
 class IntegratedMeasure(CalibrationMeasure):
     """An abstract integrated measure between two output data sets."""
 
     mesh_name: str
     """The name of the 1D mesh."""
 
     def __init__(
         self,
         output_name: str,
         mesh_name: str,
-        name: str | None = None,
-        f_type: str | None = None,
+        name: str = "",
+        f_type: CalibrationMeasure.FunctionType = CalibrationMeasure.FunctionType.NONE,
     ) -> None:
-        # noqa: D205 D212 D415
         """
         Args:
             mesh_name: The name of the 1D mesh.
-        """
+        """  # noqa: D205 D212 D415
         self.mesh_name = mesh_name
         self.__reference_mesh = None
         super().__init__(output_name, name=name, f_type=f_type)
 
     def _compute_name(self) -> str:
         return f"{self.__class__.__name__}({self.output_name};{self.mesh_name})"
 
-    def __call__(self, model_dataset: Dataset) -> float:
-        # noqa: D102
+    def __call__(self, model_dataset: DataType) -> float:  # noqa: D102
         model_data = model_dataset[self.output_name]
         model_mesh = model_dataset[self.mesh_name]
         self._update_bounds(model_data)
         return mean(
             [
                 integrate(
                     self._compare_data(
@@ -63,15 +61,13 @@
                     self.__reference_mesh[i],
                 )
                 for i in range(len(model_data))
             ]
         )
 
     @property
-    def full_output_name(self) -> str:
-        # noqa: D102
+    def full_output_name(self) -> str:  # noqa: D102
         return f"{self.output_name}[{self.mesh_name}]"
 
-    def set_reference_data(self, reference_dataset: Dataset) -> None:
-        # noqa: D102
+    def set_reference_data(self, reference_dataset: DataType) -> None:  # noqa: D102
         self.__reference_mesh = reference_dataset[self.mesh_name]
         super().set_reference_data(reference_dataset)
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/ise.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mse.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-"""Compute the integrated square error between the model and reference output data."""
+"""Compute the mean square error between the model and reference output data."""
 from __future__ import annotations
 
 from numpy import ndarray
 
-from gemseo_calibration.measures.integrated_measure import IntegratedMeasure
+from gemseo_calibration.measures.mean_measure import MeanMeasure
 
 
-class ISE(IntegratedMeasure):
-    """The integrated square error between the model and reference output data."""
+class MSE(MeanMeasure):
+    """The mean square error between the model and reference output data."""
 
     @staticmethod
-    def _compare_data(
-        data: ndarray,
-        other_data: ndarray,
-    ) -> ndarray:
+    def _compare_data(data: ndarray, other_data: ndarray) -> ndarray:
         return (data - other_data) ** 2
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mae.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mae.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,9 @@
 from gemseo_calibration.measures.mean_measure import MeanMeasure
 
 
 class MAE(MeanMeasure):
     """The mean absolute error between the model and reference output data."""
 
     @staticmethod
-    def _compare_data(
-        data: ndarray,
-        other_data: ndarray,
-    ) -> ndarray:
+    def _compare_data(data: ndarray, other_data: ndarray) -> ndarray:
         return abs(data - other_data)
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mean_measure.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/measures/mean_measure.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,24 +11,20 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """A module to compute the mean measure between the model and reference data."""
 from __future__ import annotations
 
-from gemseo.core.dataset import Dataset
 from numpy import nanmean
 
 from gemseo_calibration.measure import CalibrationMeasure
+from gemseo_calibration.measure import DataType
 
 
 class MeanMeasure(CalibrationMeasure):
     """An abstract mean measure between the model and reference output data."""
 
-    def __call__(
-        self,
-        model_dataset: Dataset,
-    ) -> float:
-        # noqa: D102
+    def __call__(self, model_dataset: DataType) -> float:  # noqa: D102
         model_data = model_dataset[self.output_name]
         self._update_bounds(model_data)
         return nanmean(self._compare_data(self._reference_data, model_data))
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/measures/mse.py` & `gemseo-calibration-2.0.0/tests/measures/test_mae.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,24 +8,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-"""Compute the mean square error between the model and reference output data."""
+"""Test the calibration measure MAE."""
 from __future__ import annotations
 
-from numpy import ndarray
+from gemseo_calibration.measures.mae import MAE
+from numpy import array
+from numpy.testing import assert_array_equal
 
-from gemseo_calibration.measures.mean_measure import MeanMeasure
 
-
-class MSE(MeanMeasure):
-    """The mean square error between the model and reference output data."""
-
-    @staticmethod
-    def _compare_data(
-        data: ndarray,
-        other_data: ndarray,
-    ) -> ndarray:
-        return (data - other_data) ** 2
+def test_compute_output_error():
+    """Test that the static method _compute_output_error returns an absolute error."""
+    output_error = MAE._compare_data(array([0.0]), array([2.0]))
+    assert_array_equal(output_error, array([2.0]))
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post/__init__.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/__init__.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post/data_versus_model/post.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post/data_versus_model/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,48 +13,39 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Plot the model data versus the reference data."""
 from __future__ import annotations
 
 import logging
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
+from numpy import newaxis
 
 from gemseo_calibration.post.multiple_scatter import MultipleScatter
 from gemseo_calibration.post_processor import CalibrationPostProcessor
 
 LOGGER = logging.getLogger(__name__)
 
 
 class DataVersusModel(CalibrationPostProcessor):
     """Scatter plot of the model data versus the reference ones."""
 
-    def _plot(
-        self,
-        output: str,
-    ) -> None:
+    def _plot(self, output: str) -> None:
         opt_name = f"Opt[{output}]"
         init_name = f"Init[{output}]"
         ref_name = f"Ref[{output}]"
 
         dataset = Dataset()
         dataset.add_variable(
-            opt_name,
-            self._posterior_model_data.get_data_by_names(output, False).mean(1)[
-                :, None
-            ],
+            opt_name, self._posterior_model_data[output].mean(1)[:, newaxis]
         )
         dataset.add_variable(
-            init_name,
-            self._prior_model_data.get_data_by_names(output, False).mean(1)[:, None],
-        )
-        dataset.add_variable(
-            ref_name,
-            self._reference_data.get_data_by_names(output, False).mean(1)[:, None],
+            init_name, self._prior_model_data[output].mean(1)[:, newaxis]
         )
+        dataset.add_variable(ref_name, self._reference_data[output].mean(1)[:, newaxis])
         plot = MultipleScatter(dataset, x=ref_name, y=[init_name, opt_name])
         plot.color = ["blue", "red"]
         plot.xlabel = "Reference"
         plot.ylabel = "Model"
         plot.labels = {opt_name: "After calibration", init_name: "Before calibration"}
         figures = plot.execute(save=False, show=False)
         for figure in figures:
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post/factory.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,87 +12,114 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """A factory to post-process  a :class:`.CalibrationScenario`."""
 from __future__ import annotations
 
 import logging
+from pathlib import Path
+from typing import Any
 
 from gemseo.algos.opt_problem import OptimizationProblem
-from gemseo.core.dataset import Dataset
-from gemseo.core.factory import Factory
+from gemseo.datasets.dataset import Dataset
 from gemseo.post.post_factory import PostFactory
 
 from gemseo_calibration.post_processor import CalibrationPostProcessor
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CalibrationPostFactory(PostFactory):
     """A factory for calibration post-processing."""
 
-    def __init__(self) -> None:  # noqa: D107
-        self.factory = Factory(CalibrationPostProcessor, ("gemseo_calibration.post",))
-        self.executed_post = []
+    _CLASS = CalibrationPostProcessor
+    _MODULE_NAMES = ("gemseo_calibration.post",)
 
     def execute(
         self,
         opt_problem: str | OptimizationProblem,
         reference_data: Dataset,
         prior_model_data: Dataset,
         posterior_model_data: Dataset,
         post_name: str,
-        **options,
+        save: bool = True,
+        show: bool = False,
+        file_path: str | Path = "",
+        directory_path: str | Path = "",
+        file_name: str = "",
+        file_extension: str = "",
+        **options: Any,
     ) -> CalibrationPostProcessor:
         """Compute the post-processing.
 
         Args:
             opt_problem: The optimization problem containing the data to post-process.
             reference_data: The reference data used during the calibration stage.
             prior_model_data: The model data before the calibration stage.
             posterior_model_data: The model data after the calibration stage.
             post_name: The name of the post-processing method.
-            **options: The options of the post-processing method.
+            save: Whether to save the figure.
+            show: Whether to display the figure.
+            file_path: The path of the file to save the figures.
+                If the extension is missing, use ``file_extension``.
+                If empty,
+                create a file path
+                from ``directory_path``, ``file_name`` and ``file_extension``.
+            directory_path: The path of the directory to save the figures.
+                If empty, use the current working directory.
+            file_name: The name of the file to save the figures.
+                If empty, use a default one generated by the post-processing.
+            file_extension: A file extension, e.g. 'png', 'pdf', 'svg', ...
+                If empty, use a default file extension.
+            **options: The options of the post-processor.
 
         Returns:
             The executed post-processing of the optimization problem.
         """
         if isinstance(opt_problem, str):
-            opt_problem = OptimizationProblem.import_hdf(opt_problem)
+            opt_problem = OptimizationProblem.from_hdf(opt_problem)
         post = self.create(
+            post_name,
             opt_problem,
             reference_data,
             prior_model_data,
             posterior_model_data,
-            post_name,
         )
-        post.execute(**options)
+        post.execute(
+            save=save,
+            show=show,
+            file_path=file_path or None,
+            directory_path=directory_path or None,
+            file_name=file_name or None,
+            file_extension=file_extension or None,
+            **options,
+        )
         self.executed_post.append(post)
         return post
 
     def create(
         self,
+        post_name: str,
         opt_problem: OptimizationProblem,
         reference_data: Dataset,
         prior_model_data: Dataset,
         posterior_model_data: Dataset,
-        post_name: str,
     ) -> CalibrationPostProcessor:
         """Create the post-processing.
 
         Args:
             opt_problem: The optimization problem containing the data to post-process.
             reference_data: The reference data used during the calibration stage.
             prior_model_data: The model data before the calibration stage.
             posterior_model_data: The model data after the calibration stage.
             post_name: The name of the post-processing method.
 
         Returns:
             The post-processing of the optimization problem.
         """
-        return self.factory.create(
+        return super().create(
             post_name,
             reference_data=reference_data,
             prior_model_data=prior_model_data,
             posterior_model_data=posterior_model_data,
             opt_problem=opt_problem,
         )
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post/multiple_scatter.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post/multiple_scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,82 +15,81 @@
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial
 #                           documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 r"""Overlay several scatter plots from a :class:`.Dataset`.
 
-A :class:`Scatter` plot
-represents a set of points :math:`\{x_i,y_i\}_{1\leq i \leq n}`
-as markers on a classical plot,
-while a :class:`MultipleScatter` plot
-represents a set of points :math:`\{x_i,y_{i,1},\ldots,y_{i,d}\}_{1\leq i \leq n}`
-as markers on a classical plot,
-with one color per series :math:`\{y_i\}_{1\leq i \leq n}`.
+A :class:`Scatter` plot represents a set of points :math:`\{x_i,y_i\}_{1\leq i \leq n}`
+as markers on a classical plot, while a :class:`MultipleScatter` plot represents a set
+of points :math:`\{x_i,y_{i,1},\ldots,y_{i,d}\}_{1\leq i \leq n}` as markers on a
+classical plot, with one color per series :math:`\{y_i\}_{1\leq i \leq n}`.
 """
 from __future__ import annotations
 
+from types import MappingProxyType
 from typing import Iterable
 from typing import Mapping
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.post.dataset.dataset_plot import DatasetPlot
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
 
 class MultipleScatter(DatasetPlot):
     """Overlay several scatter y_i versus x."""
 
     def __init__(
         self,
         dataset: Dataset,
         x: str,
         y: str | Iterable[str],
-        x_comp: str = 0,
-        y_comp: Mapping[str, int] = None,
+        x_comp: int = 0,
+        y_comp: Mapping[str, int] = MappingProxyType({}),
     ) -> None:
-        # noqa: D205 D212 D415
         """
         Args:
             x: The name of the variable on the x-axis.
             y: The names of the variables on the y-axis.
             x_comp: The component of x.
             y_comp: The components of y,
                 where the names are the names of the variables
                 and the values are the components.
-                If None or if a name is missing,
+                If empty or if a name is missing,
                 use the first component.
-        """
+        """  # noqa: D205 D212 D415
         super().__init__(dataset=dataset, x=x, y=y, x_comp=x_comp, y_comp=y_comp)
 
     def _plot(
         self,
-        fig: None | Figure = None,
-        axes: None | Axes = None,
+        fig: Figure | None = None,
+        axes: Axes | None = None,
     ) -> list[Figure]:
         x = self._param.x
         y = self._param.y
         if isinstance(y, str):
             y = [y]
 
         y_comp = self._param.y_comp or {}
         for name in y:
             y_comp[name] = y_comp.get(name, 0)
 
-        reference = self.dataset.get_data_by_names(x, False)[:, self._param.x_comp]
+        reference = self.dataset.get_view(variable_names=x).to_numpy()[
+            :, self._param.x_comp
+        ]
 
         fig, axes = self._get_figure_and_axes(fig, axes)
         bounds = [min(reference), max(reference)]
         axes.plot(bounds, bounds, color="gray", linestyle="--", marker="o")
         self._set_color(len(y))
         for index, name in enumerate(y):
             axes.plot(
                 reference,
-                self.dataset.get_data_by_names(name, False)[:, y_comp[name]],
+                self.dataset.get_view(variable_names=name).to_numpy()[:, y_comp[name]],
                 color=self.color[index],
                 marker="o",
                 linestyle="",
                 label=self.labels.get(name, name),
             )
         axes.set_xlabel(self.xlabel)
         axes.set_ylabel(self.ylabel)
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/post_processor.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/post_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Base class for all calibration post-processing methods."""
 from __future__ import annotations
 
 from gemseo.algos.opt_problem import OptimizationProblem
-from gemseo.core.dataset import Dataset
 from gemseo.post.opt_post_processor import OptPostProcessor
 
+from gemseo_calibration.measure import DataType
+
 
 class CalibrationPostProcessor(OptPostProcessor):
     """Abstract class for optimization post-processing methods."""
 
     def __init__(
         self,
         opt_problem: OptimizationProblem,
-        reference_data: Dataset,
-        prior_model_data: Dataset,
-        posterior_model_data: Dataset,
+        reference_data: DataType,
+        prior_model_data: DataType,
+        posterior_model_data: DataType,
     ) -> None:
-        # noqa: D104, D205, D212, D415
         """
         Args:
             opt_problem: The optimization problem to run.
             reference_data: The reference data.
             prior_model_data: The model data before the calibration.
             posterior_model_data: The model data after the calibration.
-        """
+        """  # noqa: D205, D212, D415
         super().__init__(opt_problem)
         self._reference_data = reference_data
         self._prior_model_data = prior_model_data
         self._posterior_model_data = posterior_model_data
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration/scenario.py` & `gemseo-calibration-2.0.0/src/gemseo_calibration/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 import logging
 from typing import Any
 from typing import ClassVar
 from typing import Iterable
 from typing import Sequence
 
 from gemseo.algos.design_space import DesignSpace
-from gemseo.core.dataset import Dataset
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.mdo_scenario import MDOScenario
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from numpy import ndarray
 
 from gemseo_calibration.calibrator import CalibrationMeasure
 from gemseo_calibration.calibrator import Calibrator
+from gemseo_calibration.measure import DataType
 from gemseo_calibration.post.factory import CalibrationPostFactory
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CalibrationScenario(MDOScenario):
     """A :class:`.Scenario` to calibrate a multidisciplinary system from reference data.
@@ -51,33 +51,33 @@
         Just like inputs,
         the parameters should be defined in the input grammars of the disciplines.
 
     The parameters are calibrated with the method :meth:`.execute`
     from an optimizer and a reference input-output :class:`.Dataset`.
     """
 
-    prior_model_data: Dataset | None
+    prior_model_data: dict[str, ndarray]
     """The model data before the calibration."""
 
-    posterior_model_data: Dataset | None
+    posterior_model_data: dict[str, ndarray]
     """The model data after the calibration."""
 
     __REFERENCE_DATA: ClassVar[str] = "reference_data"
     """The input of the CalibrationScenario representing the reference data."""
 
     def __init__(
         self,
         disciplines: MDODiscipline | list[MDODiscipline],
         input_names: str | Iterable[str],
         control_outputs: CalibrationMeasure | Sequence[CalibrationMeasure],
         calibration_space: DesignSpace,
         formulation: str = "MDF",
-        name: str | None = None,
+        name: str = "",
         **formulation_options: Any,
-    ) -> None:  # noqa: D205,D212,D415
+    ) -> None:
         """
         Args:
             disciplines: The disciplines
                 whose parameters must be calibrated from the reference data.
             input_names: The names of the inputs to be considered for the calibration.
             control_outputs: The names of the outputs used to calibrate the disciplines
                 with the name of the calibration measure and the corresponding weight
@@ -90,26 +90,26 @@
                 Lastly, ``CalibrationMeasure`` can be imported
                 from :mod:`gemseo-calibration.scenario`.
             calibration_space: The space of the parameters to be calibrated,
                 whose current values are consider as a prior for calibration.
             formulation: The name of a formulation
                 to manage the multidisciplinary coupling.
             name: A name for this calibration scenario.
-                If ``None``, use the name of the class.
+                If empty, use the name of the class.
             **formulation_options: The options of the formulation.
-        """
+        """  # noqa: D205,D212,D415
         self.__prior_parameters = calibration_space.get_current_value(as_dict=True)
         self.__posterior_parameters = {}
-        self.prior_model_data = None
-        self.posterior_model_data = None
+        self.prior_model_data = {}
+        self.posterior_model_data = {}
         calibrator = Calibrator(
             disciplines,
             input_names,
             control_outputs,
-            calibration_space.variables_names,
+            calibration_space.variable_names,
             formulation=formulation,
             **formulation_options,
         )
         super().__init__(
             [calibrator],
             "DisciplinaryOpt",
             calibrator.objective_name,
@@ -118,44 +118,48 @@
             maximize_objective=calibrator.maximize_objective_measure,
         )
         self.__calibration_post_factory = CalibrationPostFactory()
 
     def _run_algorithm(self) -> None:
         self.calibrator.set_reference_data(self.local_data[self.__REFERENCE_DATA])
         self.calibrator.execute()
-        self.prior_model_data = self.calibrator.scenario.export_to_dataset()
+        self.prior_model_data = self.calibrator.scenario.to_dataset().to_dict_of_arrays(
+            False
+        )
         super()._run_algorithm()
         self.__posterior_parameters = self.design_space.array_to_dict(
             self.optimization_result.x_opt
         )
         self.calibrator.default_inputs = self.posterior_parameters
         self.calibrator.execute()
-        self.posterior_model_data = self.calibrator.scenario.export_to_dataset()
+        self.posterior_model_data = (
+            self.calibrator.scenario.to_dataset().to_dict_of_arrays(False)
+        )
 
     @property
     def calibrator(self) -> Calibrator:
         """The discipline computing calibration measures from the parameter values."""
         return self.formulation.disciplines[0]
 
     @property
-    def prior_parameters(self) -> dict[str, ndarray]:
+    def prior_parameters(self) -> DataType:
         """The values of the parameters before the calibration stage."""
         return self.__prior_parameters
 
     @property
-    def posterior_parameters(self) -> dict[str, ndarray]:
+    def posterior_parameters(self) -> DataType:
         """The values of the parameters after the calibration stage."""
         return self.__posterior_parameters
 
     def add_constraint(
         self,
         control_outputs: CalibrationMeasure | Iterable[CalibrationMeasure],
-        constraint_type: str = MDOFunction.TYPE_EQ,
-        constraint_name: str | None = None,
-        value: str | float = None,
+        constraint_type: MDOFunction.ConstraintType = MDOFunction.ConstraintType.EQ,
+        constraint_name: str = "",
+        value: float = 0.0,
         positive: bool = False,
     ) -> None:
         """Define a constraint from a calibration measure related to discipline outputs.
 
         Args:
             control_outputs: The names of the outputs used to calibrate the disciplines
                 with the name of the calibration measure and the corresponding weight
@@ -167,35 +171,35 @@
                 or ``CalibrationMeasure(output="z", measure="MSE", mesh="z_mesh")``
                 Lastly, ``CalibrationMeasure`` can be imported
                 from :mod:`gemseo-calibration.scenario`.
             constraint_type: The type of constraint,
                 ``"eq"`` for equality constraint and
                 ``"ineq"`` for inequality constraint.
             constraint_name: The name of the constraint to be stored.
-                If ``None``,
+                If empty,
                 the name of the constraint is generated from the output name.
             value: The value for which the constraint is active.
-                If ``None``, this value is 0.
             positive: Whether to consider the inequality constraint as positive.
         """
         if isinstance(control_outputs, CalibrationMeasure):
             control_outputs = [control_outputs]
 
-        output_name, _ = self.calibrator.add_measure(control_outputs)
         super().add_constraint(
-            output_name, constraint_type, constraint_name, value, positive
+            self.calibrator.add_measure(control_outputs)[0],
+            constraint_type,
+            constraint_name or None,
+            value or None,
+            positive,
         )
 
     @property
-    def posts(self) -> list[str]:
-        # noqa: D102
+    def posts(self) -> list[str]:  # noqa: D102
         return self.post_factory.posts + self.__calibration_post_factory.posts
 
-    def post_process(self, post_name: str, **options: Any) -> None:
-        # noqa: D102
+    def post_process(self, post_name: str, **options: Any) -> None:  # noqa: D102
         if post_name in self.__calibration_post_factory.posts:
             return self.__calibration_post_factory.execute(
                 self.formulation.opt_problem,
                 self.calibrator.reference_data,
                 self.prior_model_data,
                 self.posterior_model_data,
                 post_name,
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/PKG-INFO` & `gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-calibration
-Version: 1.0.0
+Version: 2.0.0
 Summary: Capability to calibrate GEMSEO disciplines from data.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-calibration
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-calibration/-/issues
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
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-calibration-1.0.0/src/gemseo_calibration.egg-info/SOURCES.txt` & `gemseo-calibration-2.0.0/src/gemseo_calibration.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 doc_src/examples/calibration/plot_calibration_with_noise.py
 requirements/check.in
 requirements/check.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/doc.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_calibration/CalibrationScenario_input.json
 src/gemseo_calibration/CalibrationScenario_output.json
 src/gemseo_calibration/__init__.py
 src/gemseo_calibration/calibrator.py
 src/gemseo_calibration/measure.py
```

### Comparing `gemseo-calibration-1.0.0/tests/__init__.py` & `gemseo-calibration-2.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/conftest.py` & `gemseo-calibration-2.0.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from matplotlib import pyplot as plt
 from numpy import array
+from numpy import ndarray
 
 
 @pytest.fixture(scope="package")
 def discipline() -> AnalyticDiscipline:
     """The discipline to be calibrated."""
     return AnalyticDiscipline({"y": "a*x", "z": "b*x"})
 
 
 @pytest.fixture(scope="package")
-def reference_data() -> Dataset:
+def reference_data() -> dict[str, ndarray]:
     """The reference data to calibrate the discipline."""
-    dataset = Dataset(by_group=False)
-    dataset.add_variable("x", array([[0.5], [1.0]]))
-    dataset.add_variable("y", array([[1.0], [2.0]]))
-    dataset.add_variable("z", array([[-1.0], [-2.0]]))
-    return dataset
+    return {
+        "x": array([[0.5], [1.0]]),
+        "y": array([[1.0], [2.0]]),
+        "z": array([[-1.0], [-2.0]]),
+    }
 
 
 @pytest.fixture
 def baseline_images(request):
     """Return the baseline_images contents.
 
     Used when the compare_images decorator has indirect set.
```

### Comparing `gemseo-calibration-1.0.0/tests/data/__init__.py` & `gemseo-calibration-2.0.0/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/data/measures.py` & `gemseo-calibration-2.0.0/tests/data/measures.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,44 +11,41 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Dummy calibration measures used for tests."""
 from __future__ import annotations
 
-from gemseo.core.dataset import Dataset
 from gemseo_calibration.measure import CalibrationMeasure
+from numpy import ndarray
 
 
 class MeasureCstr(CalibrationMeasure):
     """The calibration measure to be used as a constraint."""
 
-    def __call__(
+    def __call__(  # noqa: D102
         self,
-        model_dataset: Dataset,
+        model_dataset: dict[str, ndarray],
     ) -> float:
-        # noqa: D102
-        return model_dataset[1]["y"][0]
+        return model_dataset["y"][1, 0]
 
 
 class MeasureObj(CalibrationMeasure):
     """The calibration measure to be used as an objective."""
 
     maximize = True
 
-    def __call__(
+    def __call__(  # noqa: D102
         self,
-        model_dataset: Dataset,
+        model_dataset: dict[str, ndarray],
     ) -> float:
-        # noqa: D102
-        return model_dataset[0]["y"][0]
+        return model_dataset["y"][0, 0]
 
 
 class NewCalibrationMeasure(CalibrationMeasure):
     """The calibration measure returning zero."""
 
-    def __call__(
+    def __call__(  # noqa: D102
         self,
-        model_dataset: Dataset,
+        model_dataset: dict[str, ndarray],
     ) -> float:
-        # noqa: D102
         return 0.0
```

### Comparing `gemseo-calibration-1.0.0/tests/data/post.py` & `gemseo-calibration-2.0.0/tests/data/post.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,43 +11,40 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 
 from gemseo.algos.opt_problem import OptimizationProblem
-from gemseo.core.dataset import Dataset
 from gemseo.post.opt_post_processor import OptPostProcessor
 from gemseo_calibration.post_processor import CalibrationPostProcessor
+from numpy import ndarray
 
 
 class NewOptPostProcessor(OptPostProcessor):
     """A new optimization post-processor."""
 
-    pass
-
 
 class NewCalibrationPostProcessor(CalibrationPostProcessor):
     """A new calibration post-processor."""
 
     def __init__(
         self,
         opt_problem: OptimizationProblem,
-        reference_data: Dataset,
-        prior_model_data: Dataset,
-        posterior_model_data: Dataset,
-    ):  # type: (...) -> None
-        # noqa: D205 D212 D415
+        reference_data: dict[str, ndarray],
+        prior_model_data: dict[str, ndarray],
+        posterior_model_data: dict[str, ndarray],
+    ) -> None:
         """
         Args:
             opt_problem: The optimization problem to run.
             reference_data: The reference data.
             prior_model_data: The model data before the calibration.
             posterior_model_data: The model data after the calibration.
-        """
+        """  # noqa: D205 D212 D415
         super().__init__(
             opt_problem, reference_data, prior_model_data, posterior_model_data
         )
         self.executed = False
 
     def execute(self, **options) -> None:  # noqa: D102
         self.executed = True
```

### Comparing `gemseo-calibration-1.0.0/tests/measures/__init__.py` & `gemseo-calibration-2.0.0/tests/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/measures/test_mae.py` & `gemseo-calibration-2.0.0/tests/measures/test_mse.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-"""Test the calibration measure MAE."""
+"""Test the calibration measures MSE and ISE."""
 from __future__ import annotations
 
-from gemseo_calibration.measures.mae import MAE
+import pytest
+from gemseo_calibration.measures.ise import ISE
+from gemseo_calibration.measures.mse import MSE
 from numpy import array
 from numpy.testing import assert_array_equal
 
 
-def test_compute_output_error():
-    """Test that the static method _compute_output_error returns an absolute error."""
-    output_error = MAE._compare_data(array([0.0]), array([2.0]))
-    assert_array_equal(output_error, array([2.0]))
+@pytest.mark.parametrize("measure", [MSE, ISE])
+def test_compute_output_error(measure):
+    """Test that the static method _compute_output_error returns a squared error."""
+    output_error = measure._compare_data(array([0.0]), array([2.0]))
+    assert_array_equal(output_error, array([4.0]))
```

### Comparing `gemseo-calibration-1.0.0/tests/measures/test_mean_error.py` & `gemseo-calibration-2.0.0/tests/measures/test_mean_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,40 +12,41 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test the calibration measure MeanError."""
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
 from gemseo_calibration.measures.iae import IAE
 from gemseo_calibration.measures.mae import MAE
 from numpy import array
 from numpy import nan
+from numpy import ndarray
+from numpy import ones
 
 
 @pytest.fixture(scope="module")
 def reference_data():
     """Synthetic reference data containing two observations."""
-    data = Dataset()
-    data.add_variable("y", array([[1.0], [2.0], [2.0], [nan]]))
-    data.add_variable("z", array([[1.0] * 3, [2.0] * 3, [2.0] * 3, [nan, 2.0, 2.0]]))
-    return data
+    return {
+        "y": array([[1.0], [2.0], [2.0], [nan]]),
+        "z": array([[1.0] * 3, [2.0] * 3, [2.0] * 3, [nan, 2.0, 2.0]]),
+    }
 
 
 @pytest.fixture(scope="module")
-def model_data() -> Dataset:
+def model_data() -> dict[str, ndarray]:
     """Synthetic model data corresponding to the input values of the reference data."""
-    data = Dataset()
-    data.add_variable("x", array([[1.0], [2.0], [2.0], [2.0]]))
-    data.add_variable("y", array([[3.0], [4.0], [nan], [4.0]]))
-    data.add_variable(
-        "z", array([[2.0, 3.0, 4.0], [3.0, 4.0, 5.0], [nan, 4.0, 5.0], [3.0, 4.0, 5.0]])
-    )
-    return data
+    return {
+        "x": array([[1.0], [2.0], [2.0], [2.0]]),
+        "y": array([[3.0], [4.0], [nan], [4.0]]),
+        "z": array(
+            [[2.0, 3.0, 4.0], [3.0, 4.0, 5.0], [nan, 4.0, 5.0], [3.0, 4.0, 5.0]]
+        ),
+    }
 
 
 @pytest.mark.parametrize("output_name,expected", [("y", 2.0), ("z", 2.2)])
 def test_mean_error(reference_data, model_data, output_name, expected):
     """Test that the mean error works correctly for different outputs."""
     mae = MAE(output_name)
     mae.set_reference_data(reference_data)
@@ -54,44 +55,30 @@
 
 @pytest.mark.parametrize(
     "output_name,mesh_name,expected",
     [("y", None, 2.0), ("y", "m", 6.5)],
 )
 def test_mean_error_with_mesh(output_name, mesh_name, expected):
     """Test that the mean error works correctly in presence of indexed variables."""
+    reference_data = {"y": array([[1.0, 1.0, 1.0]]), "m": array([[0.0, 1.0, 3.0]])}
+    model_data = {"y": array([[2.0, 3.0, 4.0]]), "m": array([[0.0, 1.0, 3.0]])}
     if mesh_name is None:
         measure = MAE(output_name)
     else:
         measure = IAE(output_name, mesh_name)
         assert measure.full_output_name == "y[m]"
-
-    reference_data = Dataset(by_group=False)
-    reference_data.add_variable("y", array([[1.0, 1.0, 1.0]]))
-    reference_data.add_variable("m", array([[0.0, 1.0, 3.0]]))
-
-    model_data = Dataset(by_group=False)
-    model_data.add_variable("y", array([[2.0, 3.0, 4.0]]))
-    model_data.add_variable("m", array([[0.0, 1.0, 3.0]]))
-
     measure.set_reference_data(reference_data)
     assert measure(model_data) == expected
 
 
 @pytest.mark.parametrize(
     "reference_mesh,expected_measure", [([0.0, 1.0, 2.0, 3.0], 6.5), ([0.0, 3.0], 6.0)]
 )
 def test_mean_error_with_interpolation_over_reference_mesh(
     reference_mesh, expected_measure
 ):
     """Test that integrated measures handle interpolation over reference mesh."""
+    reference_data = {"y": ones((1, len(reference_mesh))), "m": array([reference_mesh])}
+    model_data = {"y": array([[2.0, 3.0, 4.0]]), "m": array([[0.0, 1.0, 3.0]])}
     measure = IAE("y", "m")
-
-    reference_data = Dataset(by_group=False)
-    reference_data.add_variable("y", array([[1.0] * len(reference_mesh)]))
-    reference_data.add_variable("m", array([reference_mesh]))
-
-    model_data = Dataset(by_group=False)
-    model_data.add_variable("y", array([[2.0, 3.0, 4.0]]))
-    model_data.add_variable("m", array([[0.0, 1.0, 3.0]]))
-
     measure.set_reference_data(reference_data)
     assert measure(model_data) == expected_measure
```

### Comparing `gemseo-calibration-1.0.0/tests/post/__init__.py` & `gemseo-calibration-2.0.0/tests/post/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/default.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/default.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_color.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_color.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_colors.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_and_colors.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_components.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_2_outputs_components.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/baseline_images/test_multiple_scatter/with_color.png` & `gemseo-calibration-2.0.0/tests/post/baseline_images/test_multiple_scatter/with_color.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/data_versus_model/__init__.py` & `gemseo-calibration-2.0.0/tests/post/data_versus_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_y.png` & `gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_y.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_z.png` & `gemseo-calibration-2.0.0/tests/post/data_versus_model/baseline_images/test_data_versus_model/output_z.png`

 * *Files identical despite different names*

### Comparing `gemseo-calibration-1.0.0/tests/post/data_versus_model/test_data_versus_model.py` & `gemseo-calibration-2.0.0/tests/post/data_versus_model/test_data_versus_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Test the class DataVersusModel."""
 from __future__ import annotations
 
 import pytest
 from gemseo.algos.parameter_space import ParameterSpace
 from gemseo.disciplines.analytic import AnalyticDiscipline
-from gemseo.utils.testing import image_comparison
+from gemseo.utils.testing.helpers import image_comparison
 from gemseo_calibration.calibrator import CalibrationMeasure
 from gemseo_calibration.post.data_versus_model.post import DataVersusModel
+from gemseo_calibration.post.factory import CalibrationPostFactory
 from gemseo_calibration.scenario import CalibrationScenario
 from numpy import array
 
 
 @pytest.fixture(scope="module")
 def calibration_scenario() -> CalibrationScenario:
     """A calibration scenario."""
@@ -39,15 +40,15 @@
     prior = ParameterSpace()
     prior.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
     prior.add_variable("b", l_b=0.0, u_b=10.0, value=0.0)
 
     reference.set_cache_policy("MemoryFullCache")
     reference.execute({"x": array([1.0])})
     reference.execute({"x": array([2.0])})
-    reference_data = reference.cache.export_to_dataset(by_group=False)
+    reference_data = reference.cache.to_dataset().to_dict_of_arrays(False)
 
     calibration = CalibrationScenario(
         model,
         "x",
         [CalibrationMeasure("y", "MSE"), CalibrationMeasure("z", "MSE")],
         prior,
     )
@@ -76,13 +77,30 @@
 def test_plot(
     kwargs,
     baseline_images,
     calibration_scenario,
     pyplot_close_all,
 ):
     """Test images created by DataVersusModel._plot against references."""
-    DataVersusModel(
+    CalibrationPostFactory().create(
+        "DataVersusModel",
         calibration_scenario.formulation.opt_problem,
         calibration_scenario.calibrator.reference_data,
         calibration_scenario.prior_model_data,
         calibration_scenario.posterior_model_data,
-    )._plot(**kwargs)
+    ).execute(save=False, **kwargs)
+
+
+def test_factory_plot(calibration_scenario):
+    """Check CalibrationPostFactory.execute()."""
+    factory = CalibrationPostFactory()
+    post = factory.execute(
+        calibration_scenario.formulation.opt_problem,
+        calibration_scenario.calibrator.reference_data,
+        calibration_scenario.prior_model_data,
+        calibration_scenario.posterior_model_data,
+        "DataVersusModel",
+        output="y",
+        save=False,
+    )
+    assert isinstance(post, DataVersusModel)
+    assert factory.executed_post[-1] == post
```

### Comparing `gemseo-calibration-1.0.0/tests/post/test_factory.py` & `gemseo-calibration-2.0.0/tests/post/test_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,51 +14,28 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test the :class:`.CalibrationPostFactory`."""
 from __future__ import annotations
 
 from pathlib import Path
 
 import pytest
-from gemseo.problems.analytical.rosenbrock import Rosenbrock
 from gemseo_calibration.post.factory import CalibrationPostFactory
 
 DATA = Path(__file__).parent / ".." / "data"
 
 
 @pytest.fixture
-def post_factory(monkeypatch):  # type: (...) -> CalibrationPostFactory
+def post_factory(monkeypatch) -> CalibrationPostFactory:
     """The factory of post-processors dedicated to calibration."""
     monkeypatch.setenv("GEMSEO_PATH", DATA)
     return CalibrationPostFactory()
 
 
 def test_init(post_factory):
     """Check that the factory is correctly initialized."""
-    assert (
-        post_factory.factory._Factory__base_class.__name__ == "CalibrationPostProcessor"
-    )
-
-
-def test_create(post_factory):
-    """Check that a post-processor is correctly created."""
-    post = post_factory.create(Rosenbrock(), 1, 2, 3, "NewCalibrationPostProcessor")
-    assert post.__class__.__name__ == "NewCalibrationPostProcessor"
-    assert post._reference_data == 1
-    assert post._prior_model_data == 2
-    assert post._posterior_model_data == 3
-
-
-def test_execute(post_factory):
-    """Check that a post-processor is correctly executed.
-
-    Args:
-        factory (CalibrationPostFactory): A factory
-            to post-process calibration scenarios.
-    """
-    post = post_factory.execute(Rosenbrock(), 1, 2, 3, "NewCalibrationPostProcessor")
-    assert post.executed
+    assert post_factory._CLASS.__name__ == "CalibrationPostProcessor"
 
 
 def test_posts(post_factory):
     """Check that a post-processor is correctly executed."""
-    assert "NewCalibrationPostProcessor" in post_factory.posts
-    assert "OptPostProcessor" not in post_factory.posts
+    assert "DataVersusModel" in post_factory.posts
+    assert "OptHistoryView" not in post_factory.posts
```

### Comparing `gemseo-calibration-1.0.0/tests/post/test_multiple_scatter.py` & `gemseo-calibration-2.0.0/tests/post/test_multiple_scatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,31 +17,34 @@
 #                           documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Test the class MultipleScatter plotting variable y_i versus a variable x."""
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
-from gemseo.utils.testing import image_comparison
+from gemseo.datasets.dataset import Dataset
+from gemseo.utils.testing.helpers import image_comparison
 from gemseo_calibration.post.multiple_scatter import MultipleScatter
 from matplotlib import pyplot as plt
 from numpy import array
 
 
 @pytest.fixture(scope="module")
 def dataset() -> Dataset:
     """A dataset containing 3 samples of variables x, y and z (dim(z)=2)."""
-    dataset = Dataset()
     sample1 = [0.0, 0.0, 1.0, 0.25]
     sample2 = [0.5, 0.5, 0.75, 0.75]
     sample3 = [1.0, 1.0, 0.25, 1.0]
     data_array = array([sample1, sample2, sample3])
-    sizes = {"x": 1, "y1": 1, "y2": 2}
-    dataset.set_from_array(data_array, variables=["x", "y1", "y2"], sizes=sizes)
+    variable_names_to_n_components = {"x": 1, "y1": 1, "y2": 2}
+    dataset = Dataset.from_array(
+        data_array,
+        variable_names=["x", "y1", "y2"],
+        variable_names_to_n_components=variable_names_to_n_components,
+    )
     return dataset
 
 
 # the test parameters, it maps a test name to the inputs and references outputs:
 # - the kwargs to be passed to MultipleScatter._plot
 # - the expected file names without extension to be compared
 TEST_PARAMETERS = {
```

### Comparing `gemseo-calibration-1.0.0/tests/test_calibrator.py` & `gemseo-calibration-2.0.0/tests/test_calibrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from pathlib import Path
 
 import pytest
 from gemseo_calibration.calibrator import CalibrationMeasure
 from gemseo_calibration.calibrator import Calibrator
 from numpy import array
+from numpy.testing import assert_equal
 
 DATA = Path(__file__).parent / "data"
 
 CSTR_NAME = "0.5*MeasureCstr[y]+0.5*MeasureCstr[z]"
 
 
 @pytest.fixture
@@ -52,15 +53,15 @@
     names_to_measures = adapter._Calibrator__names_to_measures
     assert str(names_to_measures["MeasureObj[y]"]) == "MeasureObj[y]"
     assert str(names_to_measures[CSTR_NAME]) == CSTR_NAME
 
 
 def test_init_data(adapter):
     """Check that there is no reference data after initialization."""
-    assert adapter.reference_data is None
+    assert adapter.reference_data == {}
 
 
 def test_init_grammars(adapter):
     """Check the value of the input and output grammars after initialization."""
     assert sorted(list(adapter.get_input_data_names())) == ["a", "b"]
     assert sorted(list(adapter.get_output_data_names())) == [
         "0.5*MeasureCstr[y]+0.5*MeasureCstr[z]",
@@ -72,21 +73,20 @@
     """Check the property 'maximize_objective_measure' after initialization."""
     assert adapter.maximize_objective_measure is True
 
 
 def test_set_reference_data(adapter, reference_data):
     """Check that the reference data are correctly passed."""
     adapter.set_reference_data(reference_data)
-    assert adapter.reference_data.name == reference_data.name
     assert adapter.scenario.default_inputs["algo"] == "CustomDOE"
     assert adapter.scenario.default_inputs["algo_options"]["samples"].shape == (2, 1)
     for measure in adapter._Calibrator__measures:
         assert len(measure._reference_data) == 2
 
-    assert adapter.reference_data == reference_data
+    assert_equal(adapter.reference_data, reference_data)
 
 
 def test_execute_default(adapter, reference_data):
     """Check the execution of the Calibrator with default input data."""
     adapter.set_reference_data(reference_data)
     adapter.execute()
     assert adapter.local_data["MeasureObj[y]"][0] == 0.25
```

### Comparing `gemseo-calibration-1.0.0/tests/test_measure.py` & `gemseo-calibration-2.0.0/tests/test_measure.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test the CalibrationMeasure and the CalibrationMeasureFactory."""
 from __future__ import annotations
 
 from pathlib import Path
 
 import pytest
-from gemseo.core.dataset import Dataset
 from gemseo_calibration.measure import CalibrationMeasure
 from gemseo_calibration.measures.factory import CalibrationMeasureFactory
 from numpy import array
 from numpy.testing import assert_equal
 
 DATA = Path(__file__).parent / "data"
 
@@ -44,18 +43,17 @@
     """Test the initialization of a CalibrationMeasure."""
     assert measure.output_name == "y"
     assert measure._reference_data == []
 
 
 def test_measure_set_reference_data(measure):
     """Test the method set_reference_data of CalibrationMeasure."""
-    dataset = Dataset(by_group=False)
-    dataset.add_variable("y", array([[2.0], [4.0]]))
+    dataset = {"y": array([[2.0], [4.0]])}
     measure.set_reference_data(dataset)
-    assert_equal(measure._reference_data, dataset.data["y"])
+    assert_equal(measure._reference_data, dataset["y"])
 
 
 def test_call(measure):
     """Test the method __call__ of CalibrationMeasure."""
     assert measure("mock") == 0.0
 
 
@@ -73,10 +71,16 @@
 
 def test_factory_is_available(factory):
     """Test the method is_available() of the CalibrationMeasureFactory."""
     assert factory.is_available("NewCalibrationMeasure")
     assert not factory.is_available("foo")
 
 
+def test_factory_is_integrated_measure(factory):
+    """Test the method is_integrated_measure()."""
+    assert factory.is_integrated_measure("ISE")
+    assert not factory.is_integrated_measure("MSE")
+
+
 def test_factory_measures(factory):
     """Test the property measures of the CalibrationMeasureFactory."""
     assert "NewCalibrationMeasure" in factory.measures
```

### Comparing `gemseo-calibration-1.0.0/tests/test_post_processor.py` & `gemseo-calibration-2.0.0/tests/test_post_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test the class CalibrationPostProcessor."""
 from __future__ import annotations
 
 from gemseo.post.opt_post_processor import OptPostProcessor
+from gemseo.post.opt_post_processor import OptPostProcessorOptionType
 from gemseo.problems.analytical.rosenbrock import Rosenbrock
 from gemseo_calibration.post_processor import CalibrationPostProcessor
 
 
 class NewCalibrationPostProcessor(CalibrationPostProcessor):
     """A new calibration post processor."""
 
+    def _plot(self, **options: OptPostProcessorOptionType) -> None:
+        return
+
 
 def test_post():
     """Test that the base class CalibrationPostProcessor is correctly initialized."""
     opt_problem = Rosenbrock()
     post = NewCalibrationPostProcessor(opt_problem, 1, 2, 3)
     assert post.opt_problem == opt_problem
     assert isinstance(post, OptPostProcessor)
```

### Comparing `gemseo-calibration-1.0.0/tests/test_scenario.py` & `gemseo-calibration-2.0.0/tests/test_scenario.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 def test_init(calibration_scenario):
     """Check the initialization of the CalibrationScenario + add of the constraint."""
     assert calibration_scenario.formulation_name == "DisciplinaryOpt"
     assert len(calibration_scenario.disciplines) == 1
     assert isinstance(calibration_scenario.disciplines[0], Calibrator)
-    assert calibration_scenario.design_space.variables_names == ["a", "b"]
+    assert calibration_scenario.design_space.variable_names == ["a", "b"]
     assert calibration_scenario.name == "calib"
     assert isinstance(calibration_scenario.calibrator, Calibrator)
     assert calibration_scenario.formulation._maximize_objective is True
 
 
 @pytest.mark.parametrize("list_of_disciplines", [False, True])
 @pytest.mark.parametrize("list_of_inputs", [False, True])
@@ -96,15 +96,15 @@
     output = CalibrationMeasure("y", "MeasureObj")
     outputs = [output] if list_of_outputs else output
     constraint = CalibrationMeasure("z", "MeasureCstr")
     constraints = [constraint] if list_of_constraints else constraint
     monkeypatch.setenv("GEMSEO_PATH", DATA)
     scenario = CalibrationScenario(disciplines, inputs, outputs, calibration_space)
     scenario.add_constraint(constraints)
-    assert scenario.calibrator.scenario.design_space.variables_names == ["x"]
+    assert scenario.calibrator.scenario.design_space.variable_names == ["x"]
     assert scenario.calibrator.scenario.formulation._objective_name == "y"
 
 
 def test_calibration_adapter(calibration_scenario):
     """Check the calibrator after initialization + add of the constraint."""
     names_to_measures = calibration_scenario.calibrator._Calibrator__names_to_measures
     assert sorted(list(names_to_measures.keys())) == [
@@ -124,15 +124,14 @@
 
 
 def test_execute(calibration_scenario, reference_data):
     """Test that the reference data are correctly passed during the execution."""
     calibration_scenario.execute(
         {"algo": "NLOPT_COBYLA", "reference_data": reference_data, "max_iter": 10}
     )
-    assert calibration_scenario.calibrator.reference_data.name == reference_data.name
     assert calibration_scenario.prior_parameters == {
         "a": array([0.5]),
         "b": array([0.5]),
     }
     assert (
         calibration_scenario.posterior_parameters
         != calibration_scenario.prior_parameters
```

### Comparing `gemseo-calibration-1.0.0/tests/test_scenario_with_meshed_output.py` & `gemseo-calibration-2.0.0/tests/test_scenario_with_meshed_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 
 import pytest
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.core.dataset import Dataset
 from gemseo.core.discipline import MDODiscipline
 from gemseo_calibration.calibrator import CalibrationMeasure
 from gemseo_calibration.scenario import CalibrationScenario
 from numpy import array
 from numpy import linspace
+from numpy import ndarray
 
 
 class Model(MDODiscipline):
     """The model to be calibrated."""
 
     def __init__(self):  # noqa: D107
         super().__init__()
-        self.input_grammar.update(["x", "a", "b"])
-        self.output_grammar.update(["y", "z", "mesh"])
+        self.input_grammar.update_from_names(["x", "a", "b"])
+        self.output_grammar.update_from_names(["y", "z", "mesh"])
         self.default_inputs = {"x": array([0.0]), "a": array([0.0]), "b": array([0.0])}
 
     def _run(self):  # noqa: D107
         x_input = self.local_data["x"]
         a_parameter = self.local_data["a"]
         b_parameter = self.local_data["b"]
         z_mesh = linspace(0, 1, 5)
@@ -44,16 +44,16 @@
 
 
 class ReferenceModel(MDODiscipline):
     """The model to be approximated."""
 
     def __init__(self):  # noqa: D107
         super().__init__()
-        self.input_grammar.update(["x"])
-        self.output_grammar.update(["y", "z", "mesh"])
+        self.input_grammar.update_from_names(["x"])
+        self.output_grammar.update_from_names(["y", "z", "mesh"])
         self.default_inputs = {"x": array([0.0])}
 
     def _run(self):  # noqa: D107
         x_input = self.local_data["x"]
         z_mesh = linspace(0, 1, 5)
         y_output = 2 * x_input * z_mesh
         z_output = 3 * x_input[0] * z_mesh
@@ -66,21 +66,21 @@
     space = ParameterSpace()
     space.add_variable("a", l_b=0.0, u_b=10.0, value=0.0)
     space.add_variable("b", l_b=0.0, u_b=10.0, value=0.0)
     return space
 
 
 @pytest.fixture(scope="module")
-def reference_data() -> Dataset:
+def reference_data() -> dict[str, ndarray]:
     """The reference dataset."""
     reference = ReferenceModel()
     reference.set_cache_policy("MemoryFullCache")
     reference.execute({"x": array([1.0])})
     reference.execute({"x": array([2.0])})
-    return reference.cache.export_to_dataset(by_group=True)
+    return reference.cache.to_dataset().to_dict_of_arrays(False)
 
 
 def test_execute(reference_data, calibration_space):
     """Check the execution of the calibration scenario with a meshed output."""
     outputs = [
         CalibrationMeasure(output="y", measure="MSE"),
         CalibrationMeasure(output="z", mesh="mesh", measure="ISE"),
```

### Comparing `gemseo-calibration-1.0.0/tox.ini` & `gemseo-calibration-2.0.0/tox.ini`

 * *Files 7% similar despite different names*

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
 deps = gemseo-calibration[test]
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

