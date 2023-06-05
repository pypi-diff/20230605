# Comparing `tmp/reboundx-3.9.2.tar.gz` & `tmp/reboundx-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reboundx-3.9.2.tar", last modified: Thu Feb  9 22:02:37 2023, max compression
+gzip compressed data, was "reboundx-3.9.3.tar", last modified: Thu Mar  2 21:11:50 2023, max compression
```

## Comparing `reboundx-3.9.2.tar` & `reboundx-3.9.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-02-09 22:02:37.220717 reboundx-3.9.2/
--rw-r--r--   0 dtamayo    (502) staff       (20)    35147 2022-08-15 22:36:03.000000 reboundx-3.9.2/LICENSE
--rw-r--r--   0 dtamayo    (502) staff       (20)      115 2022-08-15 22:36:03.000000 reboundx-3.9.2/MANIFEST.in
--rw-r--r--   0 dtamayo    (502) staff       (20)     3110 2023-02-09 22:02:37.220407 reboundx-3.9.2/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)     2336 2023-02-09 22:02:16.000000 reboundx-3.9.2/README.rst
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-02-09 22:02:37.190854 reboundx-3.9.2/reboundx/
--rw-r--r--   0 dtamayo    (502) staff       (20)     1557 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/__init__.py
--rw-r--r--   0 dtamayo    (502) staff       (20)      145 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/constants.py
--rw-r--r--   0 dtamayo    (502) staff       (20)      357 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/data.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    18361 2023-02-09 22:01:39.000000 reboundx-3.9.2/reboundx/extras.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     5114 2023-02-09 22:01:39.000000 reboundx-3.9.2/reboundx/params.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    31740 2023-02-09 22:01:39.000000 reboundx-3.9.2/reboundx/reboundx.h
--rw-r--r--   0 dtamayo    (502) staff       (20)      994 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/simulationarchive.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     2069 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/testing.py
--rw-r--r--   0 dtamayo    (502) staff       (20)      663 2022-08-15 22:36:03.000000 reboundx-3.9.2/reboundx/tools.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-02-09 22:02:37.198833 reboundx-3.9.2/reboundx.egg-info/
--rw-r--r--   0 dtamayo    (502) staff       (20)     3110 2023-02-09 22:02:36.000000 reboundx-3.9.2/reboundx.egg-info/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)     1079 2023-02-09 22:02:37.000000 reboundx-3.9.2/reboundx.egg-info/SOURCES.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2023-02-09 22:02:36.000000 reboundx-3.9.2/reboundx.egg-info/dependency_links.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-12-27 17:14:45.000000 reboundx-3.9.2/reboundx.egg-info/not-zip-safe
--rw-r--r--   0 dtamayo    (502) staff       (20)       22 2023-02-09 22:02:37.000000 reboundx-3.9.2/reboundx.egg-info/requires.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       21 2023-02-09 22:02:37.000000 reboundx-3.9.2/reboundx.egg-info/top_level.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       38 2023-02-09 22:02:37.220793 reboundx-3.9.2/setup.cfg
--rw-r--r--   0 dtamayo    (502) staff       (20)     6227 2023-02-09 22:02:16.000000 reboundx-3.9.2/setup.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-02-09 22:02:37.220000 reboundx-3.9.2/src/
--rw-r--r--   0 dtamayo    (502) staff       (20)     6912 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/central_force.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    39274 2023-02-09 22:02:16.000000 reboundx-3.9.2/src/core.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     6880 2023-01-10 22:49:44.000000 reboundx-3.9.2/src/core.h
--rw-r--r--   0 dtamayo    (502) staff       (20)     5285 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/exponential_migration.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    10163 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/gr.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    16401 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/gr_full.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     5748 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/gr_potential.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     9964 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/gravitational_harmonics.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     4111 2023-01-10 22:49:44.000000 reboundx-3.9.2/src/inner_disk_edge.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    26551 2022-12-23 18:59:37.000000 reboundx-3.9.2/src/input.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2493 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/integrate_force.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     1418 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/integrator_euler.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     5010 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/integrator_implicit_midpoint.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2433 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/integrator_rk2.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     3547 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/integrator_rk4.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     7400 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/interpolation.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2941 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/linkedlist.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2105 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/linkedlist.h
--rw-r--r--   0 dtamayo    (502) staff       (20)     3318 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/modify_mass.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     7646 2023-02-09 22:01:39.000000 reboundx-3.9.2/src/modify_orbits_direct.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     6862 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/modify_orbits_forces.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    13060 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/output.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     6682 2022-12-22 23:33:59.000000 reboundx-3.9.2/src/radiation_forces.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    31740 2023-02-09 22:01:39.000000 reboundx-3.9.2/src/reboundx.h
--rw-r--r--   0 dtamayo    (502) staff       (20)    10697 2023-02-09 22:01:39.000000 reboundx-3.9.2/src/rebxtools.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2802 2023-02-09 22:01:39.000000 reboundx-3.9.2/src/rebxtools.h
--rw-r--r--   0 dtamayo    (502) staff       (20)     4858 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/steppers.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    11379 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/stochastic_forces.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    10500 2023-01-10 22:49:44.000000 reboundx-3.9.2/src/tides_constant_time_lag.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    17619 2023-02-09 22:01:39.000000 reboundx-3.9.2/src/tides_spin.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     4537 2023-01-10 22:49:44.000000 reboundx-3.9.2/src/track_min_distance.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     9960 2023-01-10 22:49:44.000000 reboundx-3.9.2/src/type_I_migration.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    13961 2022-08-15 22:36:03.000000 reboundx-3.9.2/src/yarkovsky_effect.c
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-03-02 21:11:50.952574 reboundx-3.9.3/
+-rw-r--r--   0 dtamayo    (502) staff       (20)    35147 2022-08-15 22:36:03.000000 reboundx-3.9.3/LICENSE
+-rw-r--r--   0 dtamayo    (502) staff       (20)      115 2022-08-15 22:36:03.000000 reboundx-3.9.3/MANIFEST.in
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3110 2023-03-02 21:11:50.952315 reboundx-3.9.3/PKG-INFO
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2336 2023-03-02 21:11:28.000000 reboundx-3.9.3/README.rst
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-03-02 21:11:50.932720 reboundx-3.9.3/reboundx/
+-rw-r--r--   0 dtamayo    (502) staff       (20)     1557 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/__init__.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)      145 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/constants.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)      357 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/data.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    18361 2023-02-09 22:01:39.000000 reboundx-3.9.3/reboundx/extras.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     5114 2023-02-09 22:01:39.000000 reboundx-3.9.3/reboundx/params.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    31740 2023-02-09 22:01:39.000000 reboundx-3.9.3/reboundx/reboundx.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)      994 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/simulationarchive.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2069 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/testing.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)      663 2022-08-15 22:36:03.000000 reboundx-3.9.3/reboundx/tools.py
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-03-02 21:11:50.935437 reboundx-3.9.3/reboundx.egg-info/
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3110 2023-03-02 21:11:50.000000 reboundx-3.9.3/reboundx.egg-info/PKG-INFO
+-rw-r--r--   0 dtamayo    (502) staff       (20)     1079 2023-03-02 21:11:50.000000 reboundx-3.9.3/reboundx.egg-info/SOURCES.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)        1 2023-03-02 21:11:50.000000 reboundx-3.9.3/reboundx.egg-info/dependency_links.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-12-27 17:14:45.000000 reboundx-3.9.3/reboundx.egg-info/not-zip-safe
+-rw-r--r--   0 dtamayo    (502) staff       (20)       22 2023-03-02 21:11:50.000000 reboundx-3.9.3/reboundx.egg-info/requires.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)       21 2023-03-02 21:11:50.000000 reboundx-3.9.3/reboundx.egg-info/top_level.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)       38 2023-03-02 21:11:50.952616 reboundx-3.9.3/setup.cfg
+-rw-r--r--   0 dtamayo    (502) staff       (20)     6227 2023-03-02 21:11:28.000000 reboundx-3.9.3/setup.py
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-03-02 21:11:50.951965 reboundx-3.9.3/src/
+-rw-r--r--   0 dtamayo    (502) staff       (20)     6912 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/central_force.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    39274 2023-03-02 21:11:28.000000 reboundx-3.9.3/src/core.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     6880 2023-01-10 22:49:44.000000 reboundx-3.9.3/src/core.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)     5285 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/exponential_migration.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    10163 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/gr.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    16401 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/gr_full.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     5748 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/gr_potential.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     9964 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/gravitational_harmonics.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     4111 2023-01-10 22:49:44.000000 reboundx-3.9.3/src/inner_disk_edge.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    26551 2022-12-23 18:59:37.000000 reboundx-3.9.3/src/input.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2493 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/integrate_force.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     1418 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/integrator_euler.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     5010 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/integrator_implicit_midpoint.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2433 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/integrator_rk2.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3547 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/integrator_rk4.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     7400 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/interpolation.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2941 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/linkedlist.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2105 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/linkedlist.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3318 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/modify_mass.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     7646 2023-02-09 22:01:39.000000 reboundx-3.9.3/src/modify_orbits_direct.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     6862 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/modify_orbits_forces.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    13060 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/output.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     6682 2022-12-22 23:33:59.000000 reboundx-3.9.3/src/radiation_forces.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    31740 2023-02-09 22:01:39.000000 reboundx-3.9.3/src/reboundx.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)    10697 2023-02-09 22:01:39.000000 reboundx-3.9.3/src/rebxtools.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2802 2023-02-09 22:01:39.000000 reboundx-3.9.3/src/rebxtools.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)     4858 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/steppers.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    11379 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/stochastic_forces.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    10500 2023-01-10 22:49:44.000000 reboundx-3.9.3/src/tides_constant_time_lag.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    17618 2023-03-02 21:11:28.000000 reboundx-3.9.3/src/tides_spin.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     4537 2023-01-10 22:49:44.000000 reboundx-3.9.3/src/track_min_distance.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     9960 2023-01-10 22:49:44.000000 reboundx-3.9.3/src/type_I_migration.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    13961 2022-08-15 22:36:03.000000 reboundx-3.9.3/src/yarkovsky_effect.c
```

### Comparing `reboundx-3.9.2/LICENSE` & `reboundx-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/PKG-INFO` & `reboundx-3.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reboundx
-Version: 3.9.2
+Version: 3.9.3
 Summary: A library for including additional forces in REBOUND
 Home-page: https://github.com/dtamayo/reboundx
 Author: Daniel Tamayo
 Author-email: tamayo.daniel@gmail.com
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.2-green.svg?style=flat
+.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.3-green.svg?style=flat
     :target: https://reboundx.readthedocs.org
 .. image:: https://badge.fury.io/py/reboundx.svg
     :target: https://badge.fury.io/py/reboundx
 .. image:: https://travis-ci.org/dtamayo/reboundx.svg?branch=master
     :target: https://travis-ci.org/dtamayo/reboundx
 .. image:: https://coveralls.io/repos/dtamayo/reboundx/badge.svg?branch=master&service=github 
     :target: https://coveralls.io/github/dtamayo/reboundx?branch=master
```

### Comparing `reboundx-3.9.2/README.rst` & `reboundx-3.9.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.2-green.svg?style=flat
+.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.3-green.svg?style=flat
     :target: https://reboundx.readthedocs.org
 .. image:: https://badge.fury.io/py/reboundx.svg
     :target: https://badge.fury.io/py/reboundx
 .. image:: https://travis-ci.org/dtamayo/reboundx.svg?branch=master
     :target: https://travis-ci.org/dtamayo/reboundx
 .. image:: https://coveralls.io/repos/dtamayo/reboundx/badge.svg?branch=master&service=github 
     :target: https://coveralls.io/github/dtamayo/reboundx?branch=master
```

### Comparing `reboundx-3.9.2/reboundx/__init__.py` & `reboundx-3.9.3/reboundx/__init__.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/extras.py` & `reboundx-3.9.3/reboundx/extras.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/params.py` & `reboundx-3.9.3/reboundx/params.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/reboundx.h` & `reboundx-3.9.3/reboundx/reboundx.h`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/simulationarchive.py` & `reboundx-3.9.3/reboundx/simulationarchive.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/testing.py` & `reboundx-3.9.3/reboundx/testing.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx/tools.py` & `reboundx-3.9.3/reboundx/tools.py`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/reboundx.egg-info/PKG-INFO` & `reboundx-3.9.3/reboundx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reboundx
-Version: 3.9.2
+Version: 3.9.3
 Summary: A library for including additional forces in REBOUND
 Home-page: https://github.com/dtamayo/reboundx
 Author: Daniel Tamayo
 Author-email: tamayo.daniel@gmail.com
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.2-green.svg?style=flat
+.. image:: https://img.shields.io/badge/REBOUNDx-v3.9.3-green.svg?style=flat
     :target: https://reboundx.readthedocs.org
 .. image:: https://badge.fury.io/py/reboundx.svg
     :target: https://badge.fury.io/py/reboundx
 .. image:: https://travis-ci.org/dtamayo/reboundx.svg?branch=master
     :target: https://travis-ci.org/dtamayo/reboundx
 .. image:: https://coveralls.io/repos/dtamayo/reboundx/badge.svg?branch=master&service=github 
     :target: https://coveralls.io/github/dtamayo/reboundx?branch=master
```

### Comparing `reboundx-3.9.2/reboundx.egg-info/SOURCES.txt` & `reboundx-3.9.3/reboundx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/setup.py` & `reboundx-3.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DREBXGITHASH="+ghash
 except:
-    ghash_arg = "-DREBXGITHASH=04a99bdcf707e3841b6ddb82403aed2b5689cd08" #GITHASHAUTOUPDATE
+    ghash_arg = "-DREBXGITHASH=3a0c067df909d23fe613142dc832421dc048bfd4" #GITHASHAUTOUPDATE
 
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
         if "PYODIDE" in os.environ:
             return None
 
@@ -76,15 +76,15 @@
                     )
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='reboundx',
-    version='3.9.2',
+    version='3.9.3',
     description='A library for including additional forces in REBOUND',
     long_description=long_description,
     url='https://github.com/dtamayo/reboundx',
     author='Daniel Tamayo',
     author_email='tamayo.daniel@gmail.com',
     license='GPL',
     classifiers=[
```

### Comparing `reboundx-3.9.2/src/central_force.c` & `reboundx-3.9.3/src/central_force.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/core.c` & `reboundx-3.9.3/src/core.c`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #include "rebound.h"
 #include "linkedlist.h"
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* rebx_build_str = __DATE__ " " __TIME__; // Date and time build string.
-const char* rebx_version_str = "3.9.2";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* rebx_version_str = "3.9.3";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* rebx_githash_str = STRINGIFY(REBXGITHASH);             // This line gets updated automatically. Do not edit manually.
 
 
 
 /*****************************
  Initialization routines.
  ****************************/
```

### Comparing `reboundx-3.9.2/src/core.h` & `reboundx-3.9.3/src/core.h`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/exponential_migration.c` & `reboundx-3.9.3/src/exponential_migration.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/gr.c` & `reboundx-3.9.3/src/gr.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/gr_full.c` & `reboundx-3.9.3/src/gr_full.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/gr_potential.c` & `reboundx-3.9.3/src/gr_potential.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/gravitational_harmonics.c` & `reboundx-3.9.3/src/gravitational_harmonics.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/inner_disk_edge.c` & `reboundx-3.9.3/src/inner_disk_edge.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/input.c` & `reboundx-3.9.3/src/input.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/integrate_force.c` & `reboundx-3.9.3/src/integrate_force.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/integrator_euler.c` & `reboundx-3.9.3/src/integrator_euler.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/integrator_implicit_midpoint.c` & `reboundx-3.9.3/src/integrator_implicit_midpoint.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/integrator_rk2.c` & `reboundx-3.9.3/src/integrator_rk2.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/integrator_rk4.c` & `reboundx-3.9.3/src/integrator_rk4.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/interpolation.c` & `reboundx-3.9.3/src/interpolation.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/linkedlist.c` & `reboundx-3.9.3/src/linkedlist.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/linkedlist.h` & `reboundx-3.9.3/src/linkedlist.h`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/modify_mass.c` & `reboundx-3.9.3/src/modify_mass.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/modify_orbits_direct.c` & `reboundx-3.9.3/src/modify_orbits_direct.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/modify_orbits_forces.c` & `reboundx-3.9.3/src/modify_orbits_forces.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/output.c` & `reboundx-3.9.3/src/output.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/radiation_forces.c` & `reboundx-3.9.3/src/radiation_forces.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/reboundx.h` & `reboundx-3.9.3/src/reboundx.h`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/rebxtools.c` & `reboundx-3.9.3/src/rebxtools.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/rebxtools.h` & `reboundx-3.9.3/src/rebxtools.h`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/steppers.c` & `reboundx-3.9.3/src/steppers.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/stochastic_forces.c` & `reboundx-3.9.3/src/stochastic_forces.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/tides_constant_time_lag.c` & `reboundx-3.9.3/src/tides_constant_time_lag.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/tides_spin.c` & `reboundx-3.9.3/src/tides_spin.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file    spin.c
+ * @file    tides_spin.c
  * @brief   Add self-consistent spin, tidal and dynamical equations of motion for bodies with structure
  * @author  Tiger Lu <tiger.lu@yale.edu>, Dan Tamayo <tamayo.daniel@gmail.com>, Hanno, Rein <hanno.rein@utoronto.ca>
  *
  * @section     LICENSE
  * Copyright (c) 2015 Dan Tamayo, Hanno Rein
  *
  * This file is part of reboundx.
@@ -25,23 +25,23 @@
  * Tables always must be preceded and followed by a blank line.  See http://docutils.sourceforge.net/docs/user/rst/quickstart.html for a primer on rst.
  * $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
  *
  * $Tides$       // Effect category (must be the first non-blank line after dollar signs and between dollar signs to be detected by script).
  *
  * ======================= ===============================================
  * Authors                 Tiger Lu, Hanno Rein, D. Tamayo, Sam Hadden, Rosemary Mardling, Sarah Millholland, Gregory Laughlin
- * Implementation Paper    Lu et al., 2023 (in review).
+ * Implementation Paper    Lu et al., 2023. <https://arxiv.org/abs/2303.00006>`_.
  * Based on                `Eggleton et al. 1998 <https://ui.adsabs.harvard.edu/abs/1998ApJ...499..853E/abstract>`_.
  * C Example               :ref:`c_example_tides_spin_pseudo_synchronization`, :ref:`c_example_tides_spin_migration_driven_obliquity_tides`, :ref:`c_example_tides_spin_kozai`.
  * Python Example          `SpinsIntro.ipynb <https://github.com/dtamayo/reboundx/blob/master/ipython_examples/SpinsIntro.ipynb>`_, `TidesSpinPseudoSynchronization.ipynb <https://github.com/dtamayo/reboundx/blob/master/ipython_examples/TidesSpinPseudoSynchronization.ipynb>`_, `TidesSpinEarthMoon.ipynb <https://github.com/dtamayo/reboundx/blob/master/ipython_examples/TidesSpinEarthMoon.ipynb>`_.
  * ======================= ===============================================
  *
  * This effect consistently tracks both the spin and orbital evolution of bodies under constant-time lag tides raised on both the primary and on the orbiting bodies.
  * In all cases, we need to set masses for all the particles that will feel these tidal forces. Particles with only mass are point particles.
- * 
+ *
  * Particles are assumed to have structure (i.e - physical extent & distortion from spin) if the following parameters are set: physical radius particles[i].r, potential Love number of degree 2 k2 (Q/(1-Q) in Eggleton 1998), and the spin angular rotation frequency vector Omega.
  * If we wish to evolve a body's spin components, the fully dimensional moment of inertia I must be set as well. If this parameter is not set, the spin components will be stationary.
  * Finally, if we wish to consider the effects of tides raised on a specific body, we must set the constant time lag tau as well.
  *
  * For spins that are synchronized with a circular orbit, the constant time lag can be related to the tidal quality factor Q as tau = 1/(2*n*tau), with n the orbital mean motion.
  * See Lu et. al (in review) and Eggleton et. al (1998) above for discussion.
  *
@@ -199,15 +199,15 @@
                 const double dx = pi->x - pj->x;
                 const double dy = pi->y - pj->y;
                 const double dz = pi->z - pj->z;
 
                 const double mi = pi->m;
                 const double mj = pj->m;
                 const double mu_ij = (mi * mj) / (mi + mj);
-                
+
                 struct reb_vec3d tf = rebx_calculate_spin_orbit_accelerations(pi, pj, sim->G, *k2, sigma_in, Omega);
                 // Eggleton et. al 1998 spin EoM (equation 36)
                 yDot[3*Nspins] += ((dy * tf.z - dz * tf.y) * (-mu_ij / *I));
                 yDot[3*Nspins + 1] += ((dz * tf.x - dx * tf.z) * (-mu_ij / *I));
                 yDot[3*Nspins + 2] += ((dx * tf.y - dy * tf.x) * (-mu_ij / *I));
             }
           }
@@ -316,15 +316,15 @@
               if (i==j){
                   continue;
               }
               struct reb_particle* target = &particles[j]; // j raises tides on i
               if (source->m == 0 || target->m == 0){
                   continue;
               }
-                
+
               rebx_spin_orbit_accelerations(source, target, G, *k2, sigma_in, *Omega);
           }
       }
     }
 }
 
 // Calculate potential of conservative piece of interaction between a point mass target and a source with a tidally and rotationally induced quadrupole
```

### Comparing `reboundx-3.9.2/src/track_min_distance.c` & `reboundx-3.9.3/src/track_min_distance.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/type_I_migration.c` & `reboundx-3.9.3/src/type_I_migration.c`

 * *Files identical despite different names*

### Comparing `reboundx-3.9.2/src/yarkovsky_effect.c` & `reboundx-3.9.3/src/yarkovsky_effect.c`

 * *Files identical despite different names*

