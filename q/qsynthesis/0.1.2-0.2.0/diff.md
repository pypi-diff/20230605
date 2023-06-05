# Comparing `tmp/qsynthesis-0.1.2.tar.gz` & `tmp/qsynthesis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsynthesis-0.1.2.tar", last modified: Fri Nov 25 13:03:02 2022, max compression
+gzip compressed data, was "qsynthesis-0.2.0.tar", last modified: Mon Jun  5 11:56:08 2023, max compression
```

## Comparing `qsynthesis-0.1.2.tar` & `qsynthesis-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    34527 2022-11-25 13:02:57.000000 qsynthesis-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5997 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2022-11-25 13:02:57.000000 qsynthesis-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.061270 qsynthesis-0.1.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)     8507 2022-11-25 13:02:57.000000 qsynthesis-0.1.2/bin/qsynthesis-table-manager
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2022-11-25 13:02:57.000000 qsynthesis-0.1.2/bin/qsynthesis-table-server
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.061270 qsynthesis-0.1.2/qsynthesis/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7668 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7265 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_plhld.py
--rw-r--r--   0 runner    (1001) docker     (122)     2659 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_td.py
--rw-r--r--   0 runner    (1001) docker     (122)     9232 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_tdbu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/grammar/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/grammar/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)     5465 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/grammar/jitting.py
--rw-r--r--   0 runner    (1001) docker     (122)     6914 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/grammar/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4768 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/arch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3231 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/ast_viewer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     6551 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/popup_actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/plugin/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15959 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/ui/synthesis_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)    48346 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/plugin/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/tables/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24516 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/tables/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5730 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/tables/lookuptablelvldb.py
--rw-r--r--   0 runner    (1001) docker     (122)     3864 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/tables/lookuptablerest.py
--rw-r--r--   0 runner    (1001) docker     (122)    31020 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/tritonast.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22662 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/qsynthesis/utils/symexec.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/qsynthesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5997 2022-11-25 13:03:01.000000 qsynthesis-0.1.2/qsynthesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2022-11-25 13:03:02.000000 qsynthesis-0.1.2/qsynthesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 13:03:01.000000 qsynthesis-0.1.2/qsynthesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-11-25 13:03:01.000000 qsynthesis-0.1.2/qsynthesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-25 13:03:01.000000 qsynthesis-0.1.2/qsynthesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-25 13:03:02.065271 qsynthesis-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1577 2022-11-25 13:02:58.000000 qsynthesis-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8269 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/bin/qsynthesis-table-manager
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/bin/qsynthesis-table-server
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/qsynthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/qsynthesis/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_plhld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_td.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_tdbu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/qsynthesis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/grammar/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/grammar/jitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/grammar/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/qsynthesis/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/ast_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/popup_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/qsynthesis/plugin/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/ui/synthesis_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48346 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/plugin/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/qsynthesis/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22087 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/tables/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/tables/lookuptablelvldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/tables/lookuptablerest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31020 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/tritonast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/qsynthesis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22662 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/qsynthesis/utils/symexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:56:08.752182 qsynthesis-0.2.0/qsynthesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-05 11:56:08.000000 qsynthesis-0.2.0/qsynthesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 11:56:08.000000 qsynthesis-0.2.0/qsynthesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:56:08.000000 qsynthesis-0.2.0/qsynthesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-05 11:56:08.000000 qsynthesis-0.2.0/qsynthesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 11:56:08.000000 qsynthesis-0.2.0/qsynthesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 11:56:08.756182 qsynthesis-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-05 11:56:07.000000 qsynthesis-0.2.0/setup.py
```

### Comparing `qsynthesis-0.1.2/LICENSE` & `qsynthesis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/PKG-INFO` & `qsynthesis-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsynthesis
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python API to synthesize Triton AST's
 Home-page: https://github.com/quarkslab/qsynthesis
 Author: Robin David
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/qsynthesis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/qsynthesis/issues
 Project-URL: Source, https://github.com/quarkslab/qsynthesis
```

### Comparing `qsynthesis-0.1.2/README.md` & `qsynthesis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/bin/qsynthesis-table-manager` & `qsynthesis-0.2.0/bin/qsynthesis-table-manager`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 import logging
 import click
 import time
 import sys
 
 import qsynthesis
-from qsynthesis import TritonGrammar, BvOp, HashType, InputOutputOracleLevelDB
+from qsynthesis import TritonGrammar, BvOp, InputOutputOracleLevelDB
 
 
 def biased_input_generator(bitsize: int, var_num: int, input_number: int, bs: int, random_level: int = 2):
     n = max(var_num-3, random_level)
     minus_one = pow(2, bitsize)-1
     vals = [1, 0, minus_one] + [None] * n
     all_perms = list(permutations(vals, var_num))
@@ -42,19 +42,18 @@
 @click.option('--var-num', default=3, type=int, help="Number of variables")
 @click.option('--input-num', default=5, type=int, help="Number of inputs")
 @click.option('--random-level', type=int, default=2, help="Randomness level of inputs 0 means higlhly biased to use corner-case values (0,1,-1)")
 @click.option('--op-num', default=5, type=int, help="Operator number")
 @click.option("-v", "--verbosity", default=0, count=True, help="increase output verbosity")
 @click.option('--ops', type=str, default='', help='specifying operators to uses')
 @click.option('--inputs', type=str, default='', help='specifying input vector to use')
-@click.option('--hash-mode', default=HashType.MD5.name, type=click.Choice([x.name for x in HashType]), help="Hash function for keys in table")
 @click.option('--watchdog', type=float, help="Activate RAM watchdog (percentage of load when to stop)")
 @click.option('-c', '--cst', type=str, help="Constant to add in the generation process", multiple=True)
 @click.option('--linearization', is_flag=True, type=bool, default=False, help="If set activate linearization of expressions")
-def generate_command(output_file, limit, bitsize, var_num, input_num, random_level, op_num, verbosity, ops, inputs, hash_mode, watchdog, cst, linearization):
+def generate_command(output_file, limit, bitsize, var_num, input_num, random_level, op_num, verbosity, ops, inputs, watchdog, cst, linearization):
     """ Table generation utility """
     logging.basicConfig(level=logging.DEBUG if verbosity else logging.INFO, format='%(message)s')
 
     constants = [int(x, 16 if x.startswith("0x") else 10) for x in cst]
 
     try:
         import pydffi
@@ -88,15 +87,15 @@
     else:
         inputs = biased_input_generator(bitsize, var_num, input_num, bitsize, random_level)
         inputs = [{n: v for n, v in zip(vrs, i)} for i in inputs]
 
     grammar = TritonGrammar([(x, bitsize) for x in vrs], operators)
 
     logging.info(f"Watchdog value: {watchdog}")
-    ltm = InputOutputOracleLevelDB.create(out_dir.absolute(), grammar, inputs, HashType[hash_mode], constants)
+    ltm = InputOutputOracleLevelDB.create(out_dir.absolute(), grammar, inputs, constants)
     try:
         if watchdog:
             ltm.generate(bitsize, constants=constants, do_watch=True, watchdog_threshold=watchdog, linearize=linearization, limit=limit)
         else:
             ltm.generate(bitsize, constants=constants, linearize=linearization, limit=limit)
     except KeyboardInterrupt:
         logging.warning("Stop required")
@@ -113,15 +112,14 @@
     """Getting information of a given database"""
     logging.basicConfig(level=logging.INFO, format='%(message)s')
     table_file = Path(table_file)
 
     table = InputOutputOracleLevelDB.load(table_file)
 
     logging.info(f"Bitsize: {table.bitsize}")
-    logging.info(f"Hash mode: {table.hash_mode.name}")
     logging.info(f"Size: {table.size}")
     logging.info(f"Variables: {table.grammar.vars}")
     logging.info(f"Operators: {[x.name for x in table.grammar.ops]}")
     logging.info(f"Nb inputs: {len(table.inputs)}")
     l = []
     for i in table.inputs:
         for v in i.values():
@@ -139,16 +137,16 @@
     table = InputOutputOracleLevelDB.load(table_file)
     count = table.size
     good, bad = 0, 0
 
     for i, (h, expr) in enumerate(table):
         if i % 100 == 0:
             print(f"process {i}/{count} [KO:{bad}]\r", end="")
-        triton_exp = table.get_expr(expr)
-        outs = table.eval_expr_inputs(triton_exp)
+        triton_exp = table._get_expr(expr)
+        outs = table._eval_expr_inputs(triton_exp)
         if table.hash(outs) != h:
             logging.warning(f"Bad expression: {expr}  with [{outs}]")
         else:
             good += 1
     logging.info(f"[OK:{good}/{count}]{'': <15}")
```

### Comparing `qsynthesis-0.1.2/bin/qsynthesis-table-server` & `qsynthesis-0.2.0/bin/qsynthesis-table-server`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/__init__.py` & `qsynthesis-0.2.0/qsynthesis/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from qsynthesis.algorithms import TopDownSynthesizer, PlaceHolderSynthesizer
 from qsynthesis.grammar import TritonGrammar, BvOp
-from qsynthesis.tables import InputOutputOracleREST, InputOutputOracleLevelDB, HashType
+from qsynthesis.tables import InputOutputOracleREST, InputOutputOracleLevelDB
 from qsynthesis.utils.symexec import SimpleSymExec
 from qsynthesis.tritonast import TritonAst
 
 import logging
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 
 # Simple object used to retrieve the plugin in IDA
 qsynthesis_plugin = None
 
 
 def enable_logging(level: int = 0):
     logger = logging.getLogger("qsynthesis")
```

### Comparing `qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_base.py` & `qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_base.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_plhld.py` & `qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_plhld.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_td.py` & `qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_td.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/algorithms/synthesizer_tdbu.py` & `qsynthesis-0.2.0/qsynthesis/algorithms/synthesizer_tdbu.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/grammar/grammar.py` & `qsynthesis-0.2.0/qsynthesis/grammar/grammar.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/grammar/jitting.py` & `qsynthesis-0.2.0/qsynthesis/grammar/jitting.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/grammar/ops.py` & `qsynthesis-0.2.0/qsynthesis/grammar/ops.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/actions.py` & `qsynthesis-0.2.0/qsynthesis/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/arch.py` & `qsynthesis-0.2.0/qsynthesis/plugin/arch.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/ast_viewer.py` & `qsynthesis-0.2.0/qsynthesis/plugin/ast_viewer.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/dependencies.py` & `qsynthesis-0.2.0/qsynthesis/plugin/dependencies.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/popup_actions.py` & `qsynthesis-0.2.0/qsynthesis/plugin/popup_actions.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/processor.py` & `qsynthesis-0.2.0/qsynthesis/plugin/processor.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/slicer.py` & `qsynthesis-0.2.0/qsynthesis/plugin/slicer.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/ui/synthesis_ui.py` & `qsynthesis-0.2.0/qsynthesis/plugin/ui/synthesis_ui.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/plugin/view.py` & `qsynthesis-0.2.0/qsynthesis/plugin/view.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/tables/base.py` & `qsynthesis-0.2.0/qsynthesis/tables/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,14 @@
 from qsynthesis.tritonast import TritonAst
 from qsynthesis.types import AstNode, Hash, Optional, List, Dict, Union, Tuple, Iterable, Input, Output, BitSize, Any, \
                              Generator
 
 logger = logging.getLogger("qsynthesis")
 
 
-class HashType(IntEnum):
-    """
-    Hash types supported by the Lookup table database. In practice solely md5
-    is used, has it is the fastest of all
-    """
-    RAW = 1
-    FNV1A_128 = 2
-    MD5 = 3
-
-
 class _EvalCtx(object):
     """
     Small debugging Triton evaluation context. It is used when manipulating
     tables in a standalone manner. It enables obtaining TritonAst out of
     the databqse entries.
     """
     def __init__(self, grammar):
@@ -71,39 +61,38 @@
 
 
 class InputOutputOracle:
     """
     Base Lookup table class. Specify the interface that child class have to
     implement to be interoperable with other the synthesizer.
     """
-    def __init__(self, gr: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, f_name: Union[Path, str] = ""):
+    def __init__(self, gr: TritonGrammar, inputs: List[Input], f_name: Union[Path, str] = ""):
         """
-        Constructor making a I/O oracle from a grammar a set of inputs and an hash type.
+        Constructor making a I/O oracle from a grammar a set of inputs and a hash type.
 
         :param gr: triton grammar
         :param inputs: List of inputs
-        :param hash_mode: type of hash to be used as keys in tables
         :param f_name: file name of the table (when being loaded)
         """
         self._name = Path(f_name)
         self.grammar = gr
         self._bitsize = self.grammar.size
         self.expr_cache = {}
         self.lookup_count = 0
         self.lookup_found = 0
         self.cache_hit = 0
-        self.hash_mode = hash_mode
         self._ectx = None
         # generation related fields
         self.watchdog = None
         self.max_mem = 0
         self.stop = False
 
         self.inputs = inputs
 
+
     @property
     def size(self) -> int:
         """Size of the table (number of entries)
 
         :rtype: int
         """
         raise NotImplementedError("Should be implemented by child class")
@@ -225,75 +214,29 @@
     def input_number(self) -> int:
         """ Number of inputs used in this table
 
         :rtype: int
         """
         return len(self.inputs)
 
-    @staticmethod
-    def _fnv1a_128(outs: List[Output]) -> Hash:
+    def hash(self, outs: List[Output]) -> Hash:
         """
-        Hash the outputs using fnv1a_128 algorithm
+        Main hashing method that convert outputs to an hash.
+        The hash used is MD5. Note that hashed values are systematically
+        casted in an array of 64bit integers.
 
         :param outs: list of outputs to hash
         :type outs: List[:py:obj:`qsynthesis.types.Output`]
-        :returns: Hash value (int) corresponding to the fnv1a of outputs
+        :returns: Hash type (bytes, int ..) of the outputs
         :rtype: :py:obj:`qsynthesis.types.Hash`
         """
         a = array.array('Q', outs)
-        FNV1A_128_OFFSET = 0x6c62272e07bb014262b821756295c58d
-        FNV1A_128_PRIME = 0x1000000000000000000013b  # 2^88 + 2^8 + 0x3b
-
-        # Set the offset basis
-        hash = FNV1A_128_OFFSET
-
-        # For each character
-        for byte in a.tobytes():
-            # Xor with the current character
-            hash ^= byte
-            # Multiply by prime
-            hash *= FNV1A_128_PRIME
-            # Clamp
-            hash &= 0xffffffffffffffffffffffffffffffff
-        # Return the final hash as a number
-        return hash
-
-    @staticmethod
-    def _md5(outs: List[Output]) -> Hash:
-        """
-        Hash the outputs using MD5 algorithm. Outputs are transformed into an array.
-        That means the final bytes hashed are the concatenation of uint64 in little
-        endian.
-
-        :param outs: list of outputs to hash
-        :type outs: List[:py:obj:`qsynthesis.types.Output`]
-        :returns: Bytes corresponding to MD5 hash
-        :type: :py:obj:`qsynthesis.types.Hash`
-        """
-        a = array.array('Q', outs)
         h = hashlib.md5(a.tobytes())
         return h.digest()
 
-    def hash(self, outs: List[Output]) -> Hash:
-        """
-        Main hashing method that dispatch the outputs to the appropriate hashing
-        function depending on the ``hash_mode`` of the table.
-
-        :param outs: list of outputs to hash
-        :type outs: List[:py:obj:`qsynthesis.types.Output`]
-        :returns: Hash type (bytes, int ..) of the outputs
-        :rtype: :py:obj:`qsynthesis.types.Hash`
-        """
-        if self.hash_mode == HashType.RAW:
-            return tuple(outs)
-        elif self.hash_mode == HashType.FNV1A_128:
-            return self._fnv1a_128(outs)
-        elif self.hash_mode == HashType.MD5:
-            return self._md5(outs)
-
     def __iter__(self) -> Iterable[Tuple[Hash, str]]:
         """ Iterator of all the entries as an iterator of pair, hash, expression as string
 
         :rtype: Iterable[Tuple[:py:obj:`qsynthesis.types.Hash, str]]`
         """
         raise NotImplementedError("Should be implemented by child class")
 
@@ -444,30 +387,28 @@
         t0 = time()
 
         from qsynthesis.grammar import jitting  # Import it locally to make sure pydffi is not mandatory
         CU = jitting.make_compilation_unit(bitsize)
         N = self.input_number
         ArTy = jitting.get_native_array_type(bitsize, N)
 
-        hash_fun = lambda x: hashlib.md5(bytes(x)).digest() if self.hash_mode == HashType.MD5 else self.hash
-
         # Initialize worklist with variables
         worklist = [(ArTy(), k) for k in self.grammar.vars]
         for i, inp in enumerate(self.inputs):
             for v, k in worklist:
                 v[i] = inp[k]
 
         # Initialize worklist with constants
         csts = [(ArTy(), str(c)) for c in constants]
         for (ar, c) in csts:
             jitting.init_array_cst(ar, int(c), N, bitsize)
         worklist.extend(csts)
 
         # initialize set of hash
-        hash_set = set(hash_fun(x[0]) for x in worklist)
+        hash_set = set(self.hash(x[0]) for x in worklist)
 
         ops = sorted(self.grammar.non_terminal_operators, key=lambda x: x.arity == 1)  # sort operators to iterate on unary first
         cur_depth = 2
         blacklist = set()
         item_count = len(worklist)  # total number of expressions
 
         try:
@@ -495,15 +436,15 @@
                     is_both_constant = name1_cst & name2_cst
 
                     for op, op_eval in zip(ops, [jitting.get_op_eval_array(CU, x) for x in ops]):  # Iterate over all operators
                         if op.arity == 1:
                             new_vals = ArTy()
                             op_eval(new_vals, vals1, N)
 
-                            h = hash_fun(new_vals)
+                            h = self.hash(new_vals)
                             if h not in hash_set:
                                 if name1_cst:
                                     fmt = str(self._to_signed(new_vals[0]))  # any value is the new constant value
                                 else:
                                     fmt = f"{op.symbol}({name1})" if len(name1) > 1 else f"{op.symbol}{name1}"
                                 fmt = self._try_linearize(fmt, symbols) if linearize else fmt
                                 logger.debug(f"[add] {fmt: <20} {h}")
@@ -529,15 +470,15 @@
                             new_vals = ArTy()
 
                             op_eval(new_vals, vals1, vals2, N)
 
                             if is_both_constant:  # if both were constant use the constant as repr instead
                                 fmt = str(self._to_signed(new_vals[0]))
 
-                            h = hash_fun(new_vals)
+                            h = self.hash(new_vals)
                             if h not in hash_set:
                                 if linearize:
                                     fmt = self._try_linearize(fmt, symbols) if linearize else fmt
                                     if fmt in blacklist:  # if linearize check blacklist here
                                         continue
 
                                 logger.debug(f"[add] {fmt: <20} {h}")
@@ -556,53 +497,49 @@
                 cur_depth += 1
         except KeyboardInterrupt:
             logger.info("Stop required")
         # In the end
         self.stop = True
         t = time() - t0
         print(f"Depth {cur_depth} (size:{len(worklist)}) (Time:{int(t/60)}m{t%60:.5f}s) [RAM:{self.__size_to_str(self.max_mem)}]")
-        self.add_entries(worklist, calc_hash=True)
+        self.add_entries(worklist)
         if do_watch:
             self.watchdog.join()
 
     def add_entry(self, hash: Hash, value: str) -> None:
         """
         Abstract function to add an entry in the lookuptable.
 
         :param hash: already computed hash to add
         :type Hash: :py:obj:`qsynthesis.types.Hash`
         :param value: expression value to add in the table
         :type value: str
         """
         raise NotImplementedError("Should be implemented by child class")
 
-    def add_entries(self, worklist: List[Tuple[Hash, str]], calc_hash: bool = False) -> None:
+    def add_entries(self, worklist: List[Tuple[Hash, str]]) -> None:
         """
-        Add the given list of entries in the database. The boolean ``calc_hash`` indicates
-        whether hashes are already computed or not. If false the function should hash the
-        hash first.
+        Add the given list of entries in the database.
 
         :param worklist: list of entries to add
         :type worklist: List[Tuple[:py:obj:`qsynthesis.types.Hash`, str]]
-        :param calc_hash: whether or not hash should be performed on entries keys
         :returns: None
         """
         raise NotImplementedError("Should be implemented by child class")
 
     @staticmethod
-    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, constants: List[int] = []) -> 'InputOutputOracle':
+    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], constants: List[int] = []) -> 'InputOutputOracle':
         """
         Create a new empty lookup table with the given initial parameters, grammars, inputs
         and hash_mode.
 
         :param filename: filename of the table to create
         :param grammar: TritonGrammar object representing variables and operators
         :param inputs: list of inputs on which to perform evaluation
         :type inputs: List[:py:obj:`qsynthesis.types.Input`]
-        :param hash_mode: Hashing mode for keys
         :param constants: list of constants used
         :returns: lookuptable instance object
         """
         raise NotImplementedError("Should be implemented by child class")
 
     @staticmethod
     def load(file: Union[Path, str]) -> 'InputOutputOracle':
```

### Comparing `qsynthesis-0.1.2/qsynthesis/tables/lookuptablelvldb.py` & `qsynthesis-0.2.0/qsynthesis/tables/lookuptablelvldb.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,59 @@
 import json
 
 # third-party libs
 import plyvel
 
 # qsynthesis deps
 from qsynthesis.grammar import TritonGrammar, BvOp
-from qsynthesis.tables.base import InputOutputOracle, HashType
+from qsynthesis.tables.base import InputOutputOracle
 from qsynthesis.types import Optional, List, Union, Tuple, Iterator, Hash, Input
 
 
 META_KEY = b"metadatas"
 VARS_KEY = b"variables"
 INPUTS_KEY = b"inputs"
 SIZE_KEY = b"size"
 
 
 class InputOutputOracleLevelDB(InputOutputOracle):
     """
     Key-Value store oracle database based on Google Level-DB
     """
-    def __init__(self, grammar: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, f_name: str = ""):
+    def __init__(self, grammar: TritonGrammar, inputs: List[Input], f_name: str = ""):
         """
         Constructor making a InputOutputOracleLevelDB from a grammar a set of inputs and an hash type.
 
         :param grammar: triton grammar
         :param inputs: List of inputs
-        :param hash_mode: type of hash to be used as keys in tables
         :param f_name: file name of the table (when being loaded)
         """
-        super(InputOutputOracleLevelDB, self).__init__(grammar, inputs, hash_mode, f_name)
+        super(InputOutputOracleLevelDB, self).__init__(grammar, inputs, f_name)
         self.db = None
 
     @staticmethod
-    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, constants: List[int] = []) -> 'InputOutputOracleLevelDB':
+    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], constants: List[int] = []) -> 'InputOutputOracleLevelDB':
         """
         Create a new empty lookup table with the given initial parameters, grammars, inputs
         and hash_mode.
 
         :param filename: filename of the table to create
         :param grammar: TritonGrammar object representing variables and operators
         :param inputs: list of inputs on which to perform evaluation
-        :param hash_mode: Hashing mode for keys
         :param constants: list of constants used
         :returns: InputOutputOracleLevelDB instance object
         """
         # TODO: If it exists deleting it ?
         db = plyvel.DB(str(filename), create_if_missing=True)
 
-        metas = dict(hash_mode=hash_mode.name, operators=[x.name for x in grammar.ops], constants=constants)
+        metas = dict(hash_mode="MD5", operators=[x.name for x in grammar.ops], constants=constants)
         db.put(META_KEY, json.dumps(metas).encode())
         db.put(VARS_KEY, json.dumps(grammar.vars_dict).encode())
         db.put(INPUTS_KEY, json.dumps(inputs).encode())
-        lkp = InputOutputOracleLevelDB(grammar=grammar, inputs=inputs, hash_mode=hash_mode, f_name=filename)
+        lkp = InputOutputOracleLevelDB(grammar=grammar, inputs=inputs, f_name=filename)
         lkp.db = db
         return lkp
 
     @staticmethod
     def load(file: Union[Path, str]) -> 'InputOutputOracleLevelDB':
         """
         Load the given lookup table and returns an instance object.
@@ -68,49 +66,44 @@
         """
         db = plyvel.DB(str(file))
         metas = json.loads(db.get(META_KEY))
         ops = [BvOp[x] for x in metas['operators']]
         vrs = list(json.loads(db.get(VARS_KEY)).items())
         inps = json.loads(db.get(INPUTS_KEY))
         grammar = TritonGrammar(vars=vrs, ops=ops)
-        lkp = InputOutputOracleLevelDB(grammar=grammar, inputs=inps, hash_mode=HashType[metas['hash_mode']], f_name=file)
+        lkp = InputOutputOracleLevelDB(grammar=grammar, inputs=inps, f_name=file)
         lkp.db = db
         return lkp
 
     def add_entry(self, hash: Hash, value: str) -> None:
         """
         Put the given hash and value in the leveldb trie.
 
         :param hash: already computed hash to add
         :param value: expression value to add in the table
         """
         self.db.put(hash, value.encode())
         self.db.put(SIZE_KEY, (str(int(self.db.get(SIZE_KEY))+1)).encode())
 
-    def add_entries(self, entries: List[Tuple[Hash, str]], calc_hash: bool = False, chunk_size: int = 10000, update_count: bool = True) -> None:
+    def add_entries(self, entries: List[Tuple[Hash, str]], chunk_size: int = 10000, update_count: bool = True) -> None:
         """
-        Add the given list of entries in the database. The boolean ``calc_hash`` indicates
-        whether hashes are already computed or not. If false the function should hash the
-        hash first.
+        Add the given list of entries in the database.
 
         :param entries: list of entries to add
-        :param calc_hash: whether or not hash should be performed on entries keys
         :param chunk_size: size of a chunk for bulk insert in DB
         :param update_count: whether or not to update the count of entries in DB
         :returns: None
         """
         count = len(entries)
 
-        def do_hash(x):
-            return x if not calc_hash else (hashlib.md5(bytes(x)).digest() if self.hash_mode == HashType.MD5 else self.hash)
-
         for step in range(0, count, chunk_size):
             with self.db.write_batch(sync=True) as wb:
                 for outs, s in entries[step:step+chunk_size]:
-                    wb.put(do_hash(outs), s.encode())
+                    h = self.hash(list(outs))  # compute hash (list convert ArTy to list)
+                    wb.put(h, s.encode())
         if update_count:
             cur_count = self.db.get(SIZE_KEY)
             new_count = count if cur_count is None else int(cur_count)+count
             self.db.put(SIZE_KEY, str(new_count).encode())
 
     def __iter__(self) -> Iterator[Tuple[Hash, str]]:
         """ Iterator of all the entries as an iterator of pair, hash, expression as string """
```

### Comparing `qsynthesis-0.1.2/qsynthesis/tables/lookuptablerest.py` & `qsynthesis-0.2.0/qsynthesis/tables/lookuptablerest.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 import binascii
 
 # third-party libs
 import requests
 
 # qsynthesis deps
 from qsynthesis.grammar import TritonGrammar
-from qsynthesis.tables.base import InputOutputOracle, HashType, Hash
-from qsynthesis.types import Input, Optional, List, Dict, Union, Tuple, Iterator
+from qsynthesis.tables.base import InputOutputOracle, Hash
+from qsynthesis.types import Input, Optional, List, Union, Tuple, Iterator
 
 
 class InputOutputOracleREST(InputOutputOracle):
     """
     REST-based lookup table. The table given in parameter is meant to be an IP
     address serving the API (that can be served with qsynthesis-table-manager runserver)
     """
 
-    def __init__(self, grammar: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, f_name: str = ""):
+    def __init__(self, grammar: TritonGrammar, inputs: List[Input], f_name: str = ""):
         """
         Constructor making a lookuptable from a grammar a set of inputs and an hash type.
 
         :param grammar: triton grammar
         :param inputs: List of inputs
         :param hash_mode: type of hash to be used as keys in tables
         :param f_name: file name of the table (when being loaded)
         """
-        super(InputOutputOracleREST, self).__init__(grammar, inputs, hash_mode, f_name)
+        super(InputOutputOracleREST, self).__init__(grammar, inputs, f_name)
         self.session = requests.Session()
         self._size = 0
 
     @staticmethod
-    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], hash_mode: HashType = HashType.RAW, constants: List[int] = []) -> 'InputOutputOracleREST':
+    def create(filename: Union[str, Path], grammar: TritonGrammar, inputs: List[Input], constants: List[int] = []) -> 'InputOutputOracleREST':
         """
         Such tables cannot be created as they are read-only databases.
         """
         raise RuntimeError("REST Lookup tables cannot be created only loaded")
 
     @staticmethod
     def load(file: Union[Path, str]) -> 'InputOutputOracleREST':
@@ -44,30 +44,30 @@
         the basic informations about the table (size, grammar, inputs etc..)
         and to create a completely transparent table.
         """
         res = requests.get(file)
         if res.status_code == 200:
             data = res.json()
             g = TritonGrammar.from_dict(data['grammar'])
-            lkp = InputOutputOracleREST(g, data['inputs'], HashType[data['hash_mode']], file)
+            lkp = InputOutputOracleREST(g, data['inputs'], file)
             lkp._size = data["size"]
             lkp.session.headers['Host'] = file
             lkp._name = file
             return lkp
         else:
             raise ConnectionAbortedError(f"Cannot reach remote server (code:{res.status_code})")
 
     def add_entry(self, hash: Hash, value: str):
         """
         Function not implemented at the moment. No new expressions can be
         submitted at the moment.
         """
         raise NotImplementedError("REST Lookup Table are read-only at the moment")
 
-    def add_entries(self, entries: List[Tuple[Hash, str]], calc_hash: bool = False, chunk_size: int = 10000) -> None:
+    def add_entries(self, entries: List[Tuple[Hash, str]], chunk_size: int = 10000) -> None:
         """
         Function not implemented at the moment. REST tables are read-only.
         """
         raise NotImplementedError("REST Lookup tables are read-only at the moment")
 
     def __iter__(self) -> Iterator[Tuple[Hash, str]]:
         """
@@ -90,8 +90,8 @@
         """
         hex_hash = binascii.hexlify(h).decode()
         res = self.session.get(str(self.name) + "/entry/" + hex_hash)
         if res.status_code == 200:
             data = res.json()
             return data['expression'] if data else None
         else:
-            raise ConnectionError("REST query did not suceeded correctly")
+            raise ConnectionError("REST query did not succeeded correctly")
```

### Comparing `qsynthesis-0.1.2/qsynthesis/tritonast.py` & `qsynthesis-0.2.0/qsynthesis/tritonast.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis/types.py` & `qsynthesis-0.2.0/qsynthesis/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 """Alias for :py:obj:`AstNode`, to abstract to Triton type"""
 
 SymVarMap = Dict[str, SymbolicVariable]
 """Dictionnary of symbolic variables names to theirs Triton object instance"""
 
 
 # Synthesis types
-Hash = Union[bytes, int, Tuple[int]]
-"""Hash abstract type used to performed lookup in tables. Given the HashType of the
-table a Hash value might be hashed before being used to perform the lookup."""
+Hash = bytes
+"""Hash abstract type used to performed lookup in tables. As now the only hash
+type supported is MD5 the underlying value is bytes."""
 
 Char = str
 """String of size one. Used to represent normalized variables names"""
 
 Input = Dict[Char, int]
 """An Input is a valuation of all inputs variables of an expression"""
```

### Comparing `qsynthesis-0.1.2/qsynthesis/utils/symexec.py` & `qsynthesis-0.2.0/qsynthesis/utils/symexec.py`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/qsynthesis.egg-info/PKG-INFO` & `qsynthesis-0.2.0/qsynthesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsynthesis
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python API to synthesize Triton AST's
 Home-page: https://github.com/quarkslab/qsynthesis
 Author: Robin David
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/qsynthesis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/qsynthesis/issues
 Project-URL: Source, https://github.com/quarkslab/qsynthesis
```

### Comparing `qsynthesis-0.1.2/qsynthesis.egg-info/SOURCES.txt` & `qsynthesis-0.2.0/qsynthesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsynthesis-0.1.2/setup.py` & `qsynthesis-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 assembly_deps = ["arybo", "llvmlite"]
 
 with open("README.md") as f:
     README = f.read()
 
 setup(
     name="qsynthesis",
-    version="0.1.2",
+    version="0.2.0",
     description="Python API to synthesize Triton AST's",
     long_description_content_type='text/markdown',
     long_description=README,
     packages=find_packages(),
     url="https://github.com/quarkslab/qsynthesis",
     project_urls={
         "Documentation": "https://quarkslab.github.io/qsynthesis/",
```

