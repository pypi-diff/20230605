# Comparing `tmp/spectrochempy-0.6.4.tar.gz` & `tmp/spectrochempy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.4.tar", last modified: Sat May 20 17:55:20 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.5.tar", last modified: Mon Jun  5 21:34:28 2023, max compression
```

## Comparing `spectrochempy-0.6.4.tar` & `spectrochempy-0.6.5.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/environment_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/requirements/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.671194 spectrochempy-0.6.4/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-20 17:55:20.719194 spectrochempy-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.683194 spectrochempy-0.6.4/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71573 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/kinetic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/nmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/analysis/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    36669 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/_check_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/application/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.691194 spectrochempy-0.6.4/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   119937 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74644 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    53899 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.695194 spectrochempy-0.6.4/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.699194 spectrochempy-0.6.4/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28400 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.699194 spectrochempy-0.6.4/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    29889 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    39297 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45433 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.703194 spectrochempy-0.6.4/spectrochempy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa_keller_massart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_chrom1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/analysis/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_lstsq_single_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/fitting/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/nddataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/nddataset/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/plotting/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.707194 spectrochempy-0.6.4/spectrochempy/examples/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_baseline_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/processing/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/examples/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/plot_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/project/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/examples/read/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_generic_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_nmr_from_bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_raman_from_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/read/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/examples/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.711194 spectrochempy-0.6.4/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/numutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.715194 spectrochempy-0.6.4/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-20 17:55:01.000000 spectrochempy-0.6.4/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:55:20.687193 spectrochempy-0.6.4/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 17:55:20.000000 spectrochempy-0.6.4/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.147763 spectrochempy-0.6.5/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.147763 spectrochempy-0.6.5/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71573 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/kinetic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/nmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/analysis/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36669 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/_check_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/plot_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119937 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74571 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53489 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28400 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19381 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29889 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39297 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45418 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa_keller_massart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_chrom1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_lstsq_single_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/nddataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_baseline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/examples/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/plot_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/examples/read/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_generic_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_nmr_from_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_raman_from_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/traittypes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/numutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-05 21:34:28.000000 spectrochempy-0.6.5/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.4/.codeclimate.yml` & `spectrochempy-0.6.5/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/.conda/meta.yaml` & `spectrochempy-0.6.5/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/.gitignore` & `spectrochempy-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/.pre-commit-config.yaml` & `spectrochempy-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/.pylintrc` & `spectrochempy-0.6.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/.zenodo.json` & `spectrochempy-0.6.5/.zenodo.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-06-05'", "'version'": "'0.6.5'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-05-20",
+    "publication_date": "2023-06-05",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.4"
+    "version": "0.6.5"
 }
```

### Comparing `spectrochempy-0.6.4/CITATION.cff` & `spectrochempy-0.6.5/CITATION.cff`

 * *Files 23% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-05-20'
+date-released: '2023-06-05'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.4
+version: 0.6.5
```

### Comparing `spectrochempy-0.6.4/Dockerfile` & `spectrochempy-0.6.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSE` & `spectrochempy-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.5/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.5/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.5/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.5/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.5/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/PKG-INFO` & `spectrochempy-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.4/README.md` & `spectrochempy-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/environment.yml` & `spectrochempy-0.6.5/environment.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/environment_dev.yml` & `spectrochempy-0.6.5/environment_dev.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/environment_test.yml` & `spectrochempy-0.6.5/environment_test.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/requirements/requirements.txt` & `spectrochempy-0.6.5/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/requirements/requirements_dev.txt` & `spectrochempy-0.6.5/requirements/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/requirements/requirements_test.txt` & `spectrochempy-0.6.5/requirements/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.5/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.5/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.5/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.5/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.5/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.5/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.5/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.5/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.5/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.5/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.5/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scripts/checkindex.py` & `spectrochempy-0.6.5/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/scripts/validate_docstrings.py` & `spectrochempy-0.6.5/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/setup.cfg` & `spectrochempy-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/setup.py` & `spectrochempy-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/__init__.py` & `spectrochempy-0.6.5/spectrochempy/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/_base.py` & `spectrochempy-0.6.5/spectrochempy/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/api.py` & `spectrochempy-0.6.5/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/efa.py` & `spectrochempy-0.6.5/spectrochempy/analysis/efa.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/fast_ica.py` & `spectrochempy-0.6.5/spectrochempy/analysis/fast_ica.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.5/spectrochempy/analysis/iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/kinetic_utilities.py` & `spectrochempy-0.6.5/spectrochempy/analysis/kinetic_utilities.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/linearregression.py` & `spectrochempy-0.6.5/spectrochempy/analysis/linearregression.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.5/spectrochempy/analysis/mcrals.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/nmf.py` & `spectrochempy-0.6.5/spectrochempy/analysis/nmf.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/optimize/__init__.py` & `spectrochempy-0.6.5/spectrochempy/analysis/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/optimize/_models.py` & `spectrochempy-0.6.5/spectrochempy/analysis/optimize/_models.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/optimize/_parameters.py` & `spectrochempy-0.6.5/spectrochempy/analysis/optimize/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/optimize/optimize.py` & `spectrochempy-0.6.5/spectrochempy/analysis/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.5/spectrochempy/analysis/pca.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.5/spectrochempy/analysis/peakfinding.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/pls.py` & `spectrochempy-0.6.5/spectrochempy/analysis/pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.5/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.5/spectrochempy/analysis/simplisma.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.5/spectrochempy/analysis/svd.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/api.py` & `spectrochempy-0.6.5/spectrochempy/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/_check_update.py` & `spectrochempy-0.6.5/spectrochempy/application/_check_update.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/application.py` & `spectrochempy-0.6.5/spectrochempy/application/application.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/datadir.py` & `spectrochempy-0.6.5/spectrochempy/application/datadir.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.5/spectrochempy/application/general_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/metaconfigurable.py` & `spectrochempy-0.6.5/spectrochempy/application/metaconfigurable.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.5/spectrochempy/application/plot_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/__init__.py` & `spectrochempy-0.6.5/spectrochempy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.5/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/npy.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -889,15 +889,14 @@
             if strunits == "":
                 strunits = "dimensionless"
         else:
             strunits = "unitless"
         return strunits
 
     def _repr_value(self):
-
         numpyprintoptions(precision=4, edgeitems=0, spc=1, linewidth=120)
 
         prefix = type(self).__name__ + ": "
         units = ""
 
         size = ""
         if not self.is_empty:
@@ -2065,17 +2064,16 @@
             units = ur.Unit(other)
 
         if self.has_units:
             oldunits = self._units
 
             try:
                 # noinspection PyUnresolvedReferences
-                if new.meta.larmor:  # _origin in ['topspin', 'nmr']
-                    # noinspection PyUnresolvedReferences
-                    set_nmr_context(new.meta.larmor)
+                if new._implements("Coord") and new.larmor:
+                    set_nmr_context(new.larmor)
                     with ur.context("nmr"):
                         new = self._unittransform(new, units)
 
                 # particular case of dimensionless units: absorbance and transmittance
                 else:
                     if f"{oldunits:P}" in ["transmittance", "absolute_transmittance"]:
                         if f"{units:P}" == "absorbance":
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/coord.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,23 @@
         -----
         The data are always returned as a 1D array of float rounded to the number
         of significant digits given by the `sigdigits` parameters.
         If the spacing between the data is constant with the accuracy given by the
         significant digits, the data are thus linearized
         and the `linear` attribute is set to True.
         """
-        return super().data
+        data = super().data
+        # now eventually round the data to the number of significant digits
+        # for displaying (internally _data as its full precision)
+        if data is not None and len(data) > 0 and self._rounding:
+            maxval = np.max(np.abs(data))
+            rounding = 3
+            nd = get_n_decimals(maxval, self.sigdigits) if maxval > 0 else rounding
+            data = np.around(data, max(nd, rounding))
+        return data
 
     @data.setter
     def data(self, data):
         # set the data
         self._set_data(data)
 
         # check if data is 1D
@@ -252,24 +260,14 @@
 
             # First try to linearize the data if it is not a datetime
             self._linear = False
             self.linearize(self._sigdigits)
             if self._linear:
                 return
 
-            # well, the data cannot be linearized with the given significant digits,
-            # now eventually round the data to the number of significant digits
-            # if self._data.size < 1:  # pragma: no cover
-            #     nd = self.sigdigits + 1
-            if self._rounding:
-                maxval = np.max(np.abs(self._data))
-                rounding = 2
-                nd = get_n_decimals(maxval, self.sigdigits) if maxval > 0 else rounding
-                self._data = np.around(self._data, max(nd, rounding))
-
     @property
     def default(self):
         # this is in case default is called on a coord, while it is a coordset property
         return self
 
     # ----------------------------------------------------------------------------------
     # hidden properties (for the documentation, only - we remove the docstring)
@@ -835,15 +833,18 @@
         spacing = spacings(self._data, sigdigits)
 
         makeitlinear = is_number(spacing)
 
         if not makeitlinear and is_iterable(spacing):
             # may be the variation in % are small enough (0.1%)
             variation = (
-                (np.max(spacing) - np.min(spacing)) * 100.0 / np.max(spacing) / 2.0
+                (np.max(spacing) - np.min(spacing))
+                * 100.0
+                / np.abs(np.max(spacing))
+                / 2.0
             )
             if variation <= self._linearize_below:
                 makeitlinear = True
 
         if makeitlinear:
             # single spacing with this precision
             # we set the number with their full precision
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/coordset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.5/spectrochempy/core/dataset/nddataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,14 @@
 
     # ----------------------------------------------------------------------------------
     # Initialisation
     # ----------------------------------------------------------------------------------
     def __init__(
         self, data=None, coordset=None, coordunits=None, coordtitles=None, **kwargs
     ):
-
         super().__init__(data, **kwargs)
 
         self._created = datetime.utcnow()
         self.description = kwargs.pop("description", "")
         self.author = kwargs.pop("author", get_user_and_node())
 
         history = kwargs.pop("history", None)
@@ -316,15 +315,14 @@
             # "referencedata",
             # "baselinedata",
             # "state",
             # "ranges",
         ] + NDIO().__dir__()
 
     def __getitem__(self, items, **kwargs):
-
         saveditems = items
 
         # coordinate selection to test first
         if isinstance(items, str):
             try:
                 return self._coordset[items]
             except Exception:
@@ -374,44 +372,31 @@
 
         new.history = f"Slice extracted: ({saveditems})"
         return new
 
     def __getattr__(self, item):
         # when the attribute was not found
         if (
-            item
+            item.startswith("_")
+            or item
             in [
-                "__numpy_ufunc__",
                 "interface",
-                "_pytestfixturefunction",
-                "__dataclass_fields__",
-                "_ipython_canary_method_should_not_exist_",
-                "_baseclass",
-                "_fill_value",
-                "_ax_lines",
-                "_axcb",
                 "clevels",
-                "__wrapped__",
                 "coords",
-                "__await__",
-                "__aiter__",
-                "__name__",
-                "__qualname__",
             ]
             or "_validate" in item
             or "_changed" in item
         ):
             # raise an error so that traits, ipython operation and more ...
             # will be handled correctly
             raise AttributeError
 
         # syntax such as ds.x, ds.y, etc...
 
         if item[0] in self.dims or self._coordset:
-
             # look also properties
             attribute = None
             index = 0
             # print(item)
             if len(item) > 2 and item[1] == "_":
                 attribute = item[1:]
                 item = item[0]
@@ -581,15 +566,14 @@
         if date.tzinfo is not None:
             # make the date utc naive
             date = date.replace(tzinfo=None)
         return date
 
     @tr.observe(tr.All)
     def _anytrait_changed(self, change):
-
         # ex: change {
         #   'owner': object, # The HasTraits instance
         #   'new': 6, # The new value
         #   'old': 5, # The old value
         #   'name': "foo", # The name of the changed trait
         #   'type': 'change', # The event type of the notification, usually 'change'
         # }
@@ -702,15 +686,14 @@
 
     def _valid_coordset(self, coords):
         # uses in coords_validate and setattr
         if coords is None:
             return
 
         for k, coord in enumerate(coords):
-
             if (
                 coord is not None
                 and not isinstance(coord, CoordSet)
                 and coord.data is None
             ):
                 continue
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.5/spectrochempy/core/plotters/multiplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.5/spectrochempy/core/plotters/plot1d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.5/spectrochempy/core/plotters/plot2d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.5/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.5/spectrochempy/core/plotters/plotly.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/align.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/apodization.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/autosub.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/baseline.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/concatenate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 
 # ======================================================================================
 # Private methods
 # ======================================================================================
 def _fft(data):
     if data.dtype == typequaternion:
-
         dr = get_component(data, "R")
         fr = np.fft.fftshift(np.fft.fft(dr), -1)
         di = get_component(data, "I")
         fi = np.fft.fftshift(np.fft.fft(di), -1)
 
         # rebuild the quaternion
         data = as_quaternion(fr, fi)
@@ -45,15 +44,14 @@
         data = np.fft.fftshift(np.fft.fft(data), -1)
 
     return data
 
 
 def _ifft(data):
     if data.dtype == typequaternion:
-
         fr = get_component(data, "R")
         dr = np.fft.ifft(np.fft.ifftshift(fr, -1))
         fi = get_component(data, "I")
         di = np.fft.ifft(np.fft.ifftshift(fi, -1))
 
         # rebuild the quaternion
         data = as_quaternion(dr, di)
@@ -62,15 +60,14 @@
         data = np.fft.ifft(np.fft.ifftshift(data, -1))
 
     return data
 
 
 def _fft_positive(data):
     if data.dtype == typequaternion:
-
         dr = get_component(data, "R")
         fr = np.fft.fftshift(np.fft.ifft(dr).astype(data.dtype)) * data.shape[-1]
         di = get_component(data, "I")
         fi = np.fft.fftshift(np.fft.ifft(di).astype(data.dtype)) * data.shape[-1]
 
         # rebuild the quaternion
         data = as_quaternion(fr, fi)
@@ -79,15 +76,14 @@
         data = np.fft.fftshift(np.fft.ifft(data).astype(data.dtype)) * data.shape[-1]
 
     return data
 
 
 def _ifft_positive(data):
     if data.dtype == typequaternion:
-
         fr = get_component(data, "R")
         dr = np.fft.fft(np.fft.ifftshift(fr, -1)) * data.shape[-1]
         fi = get_component(data, "I")
         di = np.fft.fft(np.fft.ifftshift(fi, -1)) * data.shape[-1]
 
         # rebuild the quaternion
         data = as_quaternion(dr, di)
@@ -252,15 +248,14 @@
     --------
     fft : Direct Fourier transform.
     """
     return fft(dataset, size=size, inv=True, **kwargs)
 
 
 def fft(dataset, size=None, sizeff=None, inv=False, ppm=True, **kwargs):
-
     """
     Apply a complex fast fourier transform.
 
     For multidimensional NDDataset,
     the apodization is by default performed on the last dimension.
 
     The data in the last dimension MUST be in time-domain (or without dimension)
@@ -532,15 +527,15 @@
 
             newcoord = Coord.arange(size) * deltat
             newcoord.name = x.name
             newcoord.title = "time"
             newcoord.ito("us")
 
         if is_nmr and not inv:
-            newcoord.meta.larmor = bf1  # needed for ppm transformation
+            newcoord.larmor = bf1  # needed for ppm transformation
             ppm = kwargs.get("ppm", True)
             if ppm:
                 newcoord.ito("ppm")
                 newcoord.title = rf"$\delta\ {nucleus}$"
 
         new.coordset[dim] = newcoord
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/filter.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/filter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/phasing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/shift.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/smooth.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/smooth.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/utils.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.5/spectrochempy/core/processors/zero_filling.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.5/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/project/project.py` & `spectrochempy-0.6.5/spectrochempy/core/project/project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/download.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/importer.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_carroucell.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_labspec.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_omnic.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_opus.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             f"`read_opus` import method"
         )
     # todo: read background
 
     # xaxis
     fxv = opus_data["AB Data Parameter"]["FXV"]
     lxv = opus_data["AB Data Parameter"]["LXV"]
-    xaxis = Coord.linspace(fxv, lxv, npt)
+    xaxis = Coord.linspace(fxv, lxv, npt, title="wavenumbers", units="cm^-1")
 
     # yaxis
     name = opus_data["Sample"]["SNM"]
     acqdate = opus_data["AB Data Parameter"]["DAT"]
     acqtime = opus_data["AB Data Parameter"]["TIM"]
     gmt_offset_hour = float(acqtime.split("GMT")[1].split(")")[0])
     if len(acqdate.split("/")[0]) == 2:
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_quadera.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_soc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_spc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_topspin.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,14 @@
         expno = f_expno.name
         f_name = parents[3]
 
     acqus_files = _get_files(f_expno, "acqu")
     procs_files = _get_files(f_procno, "proc")
 
     if not processed:
-
         dic, data = read_fid(f_expno, acqus_files=acqus_files, procs_files=procs_files)
 
         # apply a -90 phase shift to be compatible with topspin
         data = data * np.exp(-1j * np.pi / 2.0)
 
         # Look the case when the reshaping was not correct
         # for example, this happen when the number
@@ -812,15 +811,14 @@
             data = data[..., :ntd]
 
         # Eliminate the digital filter
         if kwargs.get("remove_digital_filter", True) and dic["acqus"]["DECIM"] > 1:
             data = _remove_digital_filter(dic, data)
 
     else:
-
         dic, datalist = read_pdata(
             f_procno,
             acqus_files=acqus_files,
             procs_files=procs_files,
             all_components=True,
         )
         if isinstance(datalist, list):
@@ -867,22 +865,20 @@
         )
 
     # read the acqu and proc
     valid_keys = list(zip(*nmr_valid_meta))[0]
     keys_units = dict(nmr_valid_meta)
 
     for item in keys:
-
         if item[:4] in ["acqu", "proc"]:
             dim = parmode
             if len(item) > 4 and item[4] in ["2", "3"]:
                 dim = parmode + 1 - int(item[4])
 
             for key in sorted(dic[item]):
-
                 if key.startswith("_") or key.lower() not in valid_keys:
                     continue
 
                 value = dic[item][key]
                 units = ur(keys_units[key.lower()]) if keys_units[key.lower()] else None
 
                 if units is not None:
@@ -896,15 +892,14 @@
 
                 try:
                     meta[key.lower()][dim] = value
                 except Exception:
                     pass
 
         else:
-
             meta[item.lower()] = dic[item]
 
     # Warning: from now all parameter keys are lowercase.
 
     # correct some initial values
 
     meta.encoding = [0] * (parmode + 1)
@@ -997,25 +992,25 @@
             # the axis is in time units
             dw = (1.0 / meta.sw_h[axis]).to("us")
             coordpoints = np.arange(meta.td[axis])
             coord = Coord(
                 coordpoints * dw, title=f"F{axis + 1} acquisition time"
             )  # TODO: use AQSEQ for >2D data
 
-            coord.meta.larmor = meta.sfo1[axis]
+            coord.larmor = meta.sfo1[axis]
             coords.append(coord)
         else:
             size = meta.si[axis]
             sizem = max(size - 1, 1)
             deltaf = -meta.sw_h[axis] / sizem
             first = meta.sfo1[axis] - meta.sf[axis] - deltaf * sizem / 2.0
 
             coordpoints = np.arange(size) * deltaf + first
             coord = Coord(coordpoints)
-            coord.meta.larmor = meta.sfo1[axis]  # needed for ppm transformation
+            coord.larmor = meta.sfo1[axis]  # needed for ppm transformation
             coord.ito("ppm")
             if meta.nuc1 is not None:
                 nuc1 = meta.nuc1[axis]
                 regex = r"([^a-zA-Z]+)([a-zA-Z]+)"
                 m = re.match(regex, nuc1)
                 mass = m[1]
                 name = m[2]
```

### Comparing `spectrochempy-0.6.4/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.5/spectrochempy/core/readers/read_zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.5/spectrochempy/core/script/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.5/spectrochempy/core/units/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.5/spectrochempy/core/writers/exporter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.5/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.5/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.5/spectrochempy/core/writers/write_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.5/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_efa_keller_massart.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa_keller_massart.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_fast_ica.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_fast_ica.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_iris.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_chrom1.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_chrom1.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_mcrals_kinetics.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_kinetics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_nmf.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_nmf.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_iris.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pca_spec.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_spec.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_pls.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/analysis/plot_simplisma.py` & `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_simplisma.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_fit.py` & `spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_fit.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/fitting/plot_lstsq_single_equation.py` & `spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_lstsq_single_equation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_coordinates.py` & `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_create_dataset.py` & `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_create_dataset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/nddataset/plot_units.py` & `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_units.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/plotting/plot_plotting.py` & `spectrochempy-0.6.5/spectrochempy/examples/plotting/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/processing/plot_baseline_correction.py` & `spectrochempy-0.6.5/spectrochempy/examples/processing/plot_baseline_correction.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_em.py` & `spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_em.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/processing/plot_proc_sp.py` & `spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_sp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/project/plot_project.py` & `spectrochempy-0.6.5/spectrochempy/examples/project/plot_project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/read/plot_generic_read.py` & `spectrochempy-0.6.5/spectrochempy/examples/read/plot_generic_read.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_omnic.py` & `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_omnic.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_IR_from_opus.py` & `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_opus.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_nmr_from_bruker.py` & `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_nmr_from_bruker.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/examples/read/plot_read_raman_from_labspec.py` & `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_raman_from_labspec.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.5/spectrochempy/extern/nmrglue.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.5/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.5/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.5/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.5/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/citation.py` & `spectrochempy-0.6.5/spectrochempy/utils/citation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/compare.py` & `spectrochempy-0.6.5/spectrochempy/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/constants.py` & `spectrochempy-0.6.5/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.5/spectrochempy/utils/coordrange.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/decorators.py` & `spectrochempy-0.6.5/spectrochempy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.5/spectrochempy/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.5/spectrochempy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/fake.py` & `spectrochempy-0.6.5/spectrochempy/utils/fake.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/file.py` & `spectrochempy-0.6.5/spectrochempy/utils/file.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.5/spectrochempy/utils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/misc.py` & `spectrochempy-0.6.5/spectrochempy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/numutils.py` & `spectrochempy-0.6.5/spectrochempy/utils/numutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/objects.py` & `spectrochempy-0.6.5/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/optional.py` & `spectrochempy-0.6.5/spectrochempy/utils/optional.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.5/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/packages.py` & `spectrochempy-0.6.5/spectrochempy/utils/packages.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/plots.py` & `spectrochempy-0.6.5/spectrochempy/utils/plots.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/print.py` & `spectrochempy-0.6.5/spectrochempy/utils/print.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.5/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/system.py` & `spectrochempy-0.6.5/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/testing.py` & `spectrochempy-0.6.5/spectrochempy/utils/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,16 +202,18 @@
                     )
             else:
                 raise AssertionError(f"{other} has no units")
 
     return True
 
 
-def compare_coords(this, other, approx=False, decimal=6, data_only=False):
+def compare_coords(this, other, approx=False, decimal=3, data_only=False):
 
+    # TODO: compare base on signficant digit for coordinate instead of decimals
+    #  (that may not work for very small coordinates numbers)
     from spectrochempy.core.units import ur
 
     def compare(x, y):
         return _compare(x, y, decimal)
 
     eq = True
     thistype = this._implements()
@@ -414,15 +416,15 @@
                         oattr is None and sattr is not None
                     ):
                         raise AssertionError("One of the coordset is None")
                     elif sattr is None and oattr is None:
                         pass
                     else:
                         for item in zip(sattr, oattr):
-                            res = compare_coords(*item, approx=approx, decimal=decimal)
+                            res = compare_coords(*item, approx=True, decimal=3)
                             if not res:
                                 raise AssertionError(f"coords differs:\n{res}")
                 else:
                     eq &= np.all(sattr == oattr)
                 if not eq:
                     raise AssertionError(
                         f"The {attr} attributes of {this} and {other} are "
@@ -455,15 +457,15 @@
 def assert_dataset_equal(nd1, nd2, **kwargs):
     kwargs["approx"] = False
     assert_dataset_almost_equal(nd1, nd2, **kwargs)
     return True
 
 
 def assert_dataset_almost_equal(nd1, nd2, **kwargs):
-    decimal = kwargs.get("decimal", 6)
+    decimal = kwargs.get("decimal", 3)
     approx = kwargs.get("approx", True)
     # if data_only is True, compare only based on data (not labels and so on)
     # except if dataset is label only!.
     data_only = kwargs.get("data_only", False)
     compare_datasets(nd1, nd2, approx=approx, decimal=decimal, data_only=data_only)
     return True
```

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/traits.py` & `spectrochempy-0.6.5/spectrochempy/utils/traits.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/version.py` & `spectrochempy-0.6.5/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.5/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/utils/zip.py` & `spectrochempy-0.6.5/spectrochempy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.5/spectrochempy/widgets/baselinecorrector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.5/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.4/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.5/spectrochempy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.4/spectrochempy.egg-info/SOURCES.txt` & `spectrochempy-0.6.5/spectrochempy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

