# Comparing `tmp/hgutilities-1.0.3.tar.gz` & `tmp/hgutilities-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.3.tar", last modified: Mon Jun  5 20:39:56 2023, max compression
+gzip compressed data, was "hgutilities-1.0.4.tar", last modified: Mon Jun  5 21:39:12 2023, max compression
```

## Comparing `hgutilities-1.0.3.tar` & `hgutilities-1.0.4.tar`

### file list

```diff
@@ -1,68 +1,227 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.589147 hgutilities-1.0.3/
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.3/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:39:56.588866 hgutilities-1.0.3/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.3/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.557078 hgutilities-1.0.3/hgutilities/
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.562492 hgutilities-1.0.3/hgutilities/defaults/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.563188 hgutilities-1.0.3/hgutilities/defaults/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/defaults/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.566440 hgutilities-1.0.3/hgutilities/plotting/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.567265 hgutilities-1.0.3/hgutilities/plotting/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.567826 hgutilities-1.0.3/hgutilities/plotting/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/animate.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.574084 hgutilities-1.0.3/hgutilities/plotting/datatypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.574859 hgutilities-1.0.3/hgutilities/plotting/datatypes/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.575675 hgutilities-1.0.3/hgutilities/plotting/datatypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      219 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/bar.py
--rw-r-----   0 henry     (1000) henry     (1000)      992 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/bars.py
--rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/colorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)      244 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/data.py
--rw-r-----   0 henry     (1000) henry     (1000)      222 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/line.py
--rw-r-----   0 henry     (1000) henry     (1000)     1630 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/lines.py
--rw-r-----   0 henry     (1000) henry     (1000)      370 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/pie.py
--rw-r-----   0 henry     (1000) henry     (1000)      979 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/datatypes/surface.py
--rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.580530 hgutilities-1.0.3/hgutilities/plotting/plottypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.581286 hgutilities-1.0.3/hgutilities/plotting/plottypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     3209 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plot.py
--rw-r-----   0 henry     (1000) henry     (1000)     3354 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotbars.py
--rw-r-----   0 henry     (1000) henry     (1000)     2613 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)     6683 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotlines.py
--rw-r-----   0 henry     (1000) henry     (1000)     1249 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotpie.py
--rw-r-----   0 henry     (1000) henry     (1000)     3691 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plottypes/plotsurface.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.585054 hgutilities-1.0.3/hgutilities/plotting/plotutils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 20:37:43.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      690 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/figuresize.py
--rw-r-----   0 henry     (1000) henry     (1000)     4445 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/griddimensions.py
--rw-r-----   0 henry     (1000) henry     (1000)     4425 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/plotshape.py
--rw-r-----   0 henry     (1000) henry     (1000)     1287 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/plotting/plotutils/savefigure.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.588176 hgutilities-1.0.3/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:53:05.000000 hgutilities-1.0.3/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 20:39:56.559404 hgutilities-1.0.3/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7668 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     1912 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 20:39:56.000000 hgutilities-1.0.3/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 20:39:56.589240 hgutilities-1.0.3/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1302 2023-06-05 20:39:36.000000 hgutilities-1.0.3/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.836202 hgutilities-1.0.4/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.645320 hgutilities-1.0.4/.github/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.654662 hgutilities-1.0.4/.github/workflows/
+-rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-05 19:53:05.000000 hgutilities-1.0.4/.github/workflows/python-publish.yml
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.4/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7613 2023-06-05 21:39:12.835854 hgutilities-1.0.4/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.4/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.655418 hgutilities-1.0.4/hgutilities/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.659959 hgutilities-1.0.4/hgutilities/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.662277 hgutilities-1.0.4/hgutilities/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      541 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      730 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      352 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.666534 hgutilities-1.0.4/hgutilities/defaults/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.671049 hgutilities-1.0.4/hgutilities/defaults/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      594 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/defaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      678 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/docs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      333 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/inherit.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      589 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      504 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.685305 hgutilities-1.0.4/hgutilities/defaults/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)   154356 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1923 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3774 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      728 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2262 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3782 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3165 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4611 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1019 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      432 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1065 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3805 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      749 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2265 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3186 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.690242 hgutilities-1.0.4/hgutilities/plotting/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.693716 hgutilities-1.0.4/hgutilities/plotting/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      181 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      580 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      314 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.699841 hgutilities-1.0.4/hgutilities/plotting/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      504 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      771 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/create_animations.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      592 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/create_figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/plotting.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     9033 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/README.md
+-rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.729856 hgutilities-1.0.4/hgutilities/plotting/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     3616 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5849 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7105 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    12637 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3492 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4308 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      584 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      795 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      970 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1245 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2083 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2773 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     6113 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10132 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    11426 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    11376 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7542 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      519 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      822 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5102 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     8252 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5135 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4366 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4172 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2928 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4497 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3439 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1121 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1990 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3641 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7154 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3548 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      558 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/animate.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.737945 hgutilities-1.0.4/hgutilities/plotting/datatypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.746841 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      267 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      173 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      699 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      421 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1081 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      180 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      334 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      553 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.755552 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      676 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      850 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      345 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      742 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      639 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      637 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      963 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.780395 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      541 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      883 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1552 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      886 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      855 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      898 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1273 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      691 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      966 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      550 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      785 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2248 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2215 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      782 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      883 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1626 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2413 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      565 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1548 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1288 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      715 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2244 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      797 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1641 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      219 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/bar.py
+-rw-r-----   0 henry     (1000) henry     (1000)      992 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/bars.py
+-rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/colorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)      244 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/data.py
+-rw-r-----   0 henry     (1000) henry     (1000)      222 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/line.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1630 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/lines.py
+-rw-r-----   0 henry     (1000) henry     (1000)      370 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/pie.py
+-rw-r-----   0 henry     (1000) henry     (1000)      979 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/surface.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.786623 hgutilities-1.0.4/hgutilities/plotting/plottypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.788576 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      477 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.807730 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     3690 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1879 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3777 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1327 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1350 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2003 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4552 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7970 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1350 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1322 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3219 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3141 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3657 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3788 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2014 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4573 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1361 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3230 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3209 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3354 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotbars.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2613 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6683 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotlines.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1249 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotpie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3691 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotsurface.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.812225 hgutilities-1.0.4/hgutilities/plotting/plotutils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.822048 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     1138 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1838 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5357 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     8558 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5262 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1453 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2325 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1159 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5378 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1474 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      690 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/figuresize.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4445 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/griddimensions.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4425 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/plotshape.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1287 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/savefigure.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.825977 hgutilities-1.0.4/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.834975 hgutilities-1.0.4/hgutilities/utils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      474 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Dicts.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1546 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2364 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1385 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2695 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      311 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Strings.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      168 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      495 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1567 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1406 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/plots.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.659180 hgutilities-1.0.4/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7613 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)    10759 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 21:39:12.836318 hgutilities-1.0.4/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1342 2023-06-05 21:35:51.000000 hgutilities-1.0.4/setup.py
```

### Comparing `hgutilities-1.0.3/LICENSE.md` & `hgutilities-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/PKG-INFO` & `hgutilities-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.3
+Version: 1.0.4
 Summary: A triple of tools used for plotting, handling key-words, and utilities
-Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
-License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -88,8 +85,7 @@
 - more control over subplot placement
 - automatic paragraph organisation for documentation
 - better distribution of subplots over multiple figures
 - control over tick labels
 - horizontal bar charts
 - better file extension handling for Defaults package
 - inherit function should be able to take in a single attribute as a non-iterable
-
```

### Comparing `hgutilities-1.0.3/README.md` & `hgutilities-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/defaults/docs.py` & `hgutilities-1.0.4/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/defaults/inherit.py` & `hgutilities-1.0.4/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.4/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.4/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/__init__.py` & `hgutilities-1.0.4/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/animate.py` & `hgutilities-1.0.4/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.4/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.4/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.4/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.4/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/figure.py` & `hgutilities-1.0.4/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/figures.py` & `hgutilities-1.0.4/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotbars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotlines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.4/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.4/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.4/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.4/hgutilities/plotting/plotutils/savefigure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/utils/groups.py` & `hgutilities-1.0.4/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/utils/paths.py` & `hgutilities-1.0.4/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities/utils/plots.py` & `hgutilities-1.0.4/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.3/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.4/hgutilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.3
+Version: 1.0.4
 Summary: A triple of tools used for plotting, handling key-words, and utilities
-Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
-License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -88,8 +85,7 @@
 - more control over subplot placement
 - automatic paragraph organisation for documentation
 - better distribution of subplots over multiple figures
 - control over tick labels
 - horizontal bar charts
 - better file extension handling for Defaults package
 - inherit function should be able to take in a single attribute as a non-iterable
-
```

### Comparing `hgutilities-1.0.3/setup.py` & `hgutilities-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
     name="hgutilities",
     version=VERSION,
     author="Henry Ginn",
     author_email="<henryginn137@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    setup_requires=['setuptools_scm'],
+    include_package_data=True,
     install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
     keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

