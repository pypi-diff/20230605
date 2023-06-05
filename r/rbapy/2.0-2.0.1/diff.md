# Comparing `tmp/rbapy-2.0.tar.gz` & `tmp/rbapy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rbapy-2.0.tar", last modified: Tue Nov  8 15:40:36 2022, max compression
+gzip compressed data, was "dist/rbapy-2.0.1.tar", last modified: Mon Jun  5 14:37:44 2023, max compression
```

## Comparing `rbapy-2.0.tar` & `rbapy-2.0.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     6556 2022-11-08 15:40:36.000000 rbapy-2.0/PKG-INFO
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/sample_input/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2722 2022-09-06 11:29:00.000000 rbapy-2.0/sample_input/params.in
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/sample_input/data/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2022-09-06 11:29:00.000000 rbapy-2.0/sample_input/data/trnas.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2943 2022-09-06 11:29:00.000000 rbapy-2.0/sample_input/data/chaperones.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    22686 2022-09-06 11:29:00.000000 rbapy-2.0/sample_input/data/ribosome.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)  9168624 2022-09-06 11:29:00.000000 rbapy-2.0/sample_input/data/sample.xml
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/tests/
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/tests/utils/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4600 2022-09-06 11:29:00.000000 rbapy-2.0/tests/utils/test_inject_efficiencies.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      114 2022-09-06 11:29:00.000000 rbapy-2.0/tests/utils/efficiencies.tsv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    18474 2022-09-29 14:20:09.000000 rbapy-2.0/tests/test_tutorial.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2432 2022-11-08 14:48:35.000000 rbapy-2.0/tests/test_cli.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/docs/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   125020 2022-09-06 11:29:00.000000 rbapy-2.0/docs/Model_construction (RBApy.prerba).pdf
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    39066 2022-09-06 11:29:00.000000 rbapy-2.0/docs/xml_tutorial.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   227777 2022-09-06 11:29:00.000000 rbapy-2.0/docs/Model_computation (RBApy.core).pdf
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   163632 2022-09-06 11:29:00.000000 rbapy-2.0/docs/Parameter_estimation (RBApy.estim) - Text-S6.pdf
--rw-r--r--   0 oliverbodeit   (501) staff       (20)  5465542 2022-09-06 11:29:00.000000 rbapy-2.0/docs/XML_format (RBApy.xml).pdf
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/rba/
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/rba/core/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    10899 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/functions.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    11309 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/targets.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    13793 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/species.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    38261 2022-11-08 14:21:24.000000 rbapy-2.0/rba/core/solver.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      174 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/__init__.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7923 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/constraint_matrix.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2380 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/processes.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2214 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/density.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3101 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/constraint_blocks.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2960 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/parameters.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     5411 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/metabolism.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2833 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/enzymes.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      984 2022-09-06 11:29:00.000000 rbapy-2.0/rba/core/parameter_vector.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       20 2022-11-08 15:13:56.000000 rbapy-2.0/rba/_version.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/rba/estim/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3921 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/nonenz_per_compartment.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2618 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/prot_per_compartment.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    17016 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/utils.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      732 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/kapp.cfg
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3258 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/kapp.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1572 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/nonenz_per_compartment.cfg
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1325 2022-09-06 11:29:00.000000 rbapy-2.0/rba/estim/prot_per_compartment.cfg
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      587 2022-09-29 15:03:33.000000 rbapy-2.0/rba/__init__.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/rba/utils/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7807 2022-09-06 11:29:00.000000 rbapy-2.0/rba/utils/efficiencies.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     9724 2022-09-06 11:29:00.000000 rbapy-2.0/rba/utils/results.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      104 2022-09-06 11:29:00.000000 rbapy-2.0/rba/utils/__init__.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/rba/cli/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        0 2022-09-06 11:29:00.000000 rbapy-2.0/rba/cli/__init__.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2491 2022-11-08 14:21:24.000000 rbapy-2.0/rba/cli/solve_rba_model.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1022 2022-09-06 11:29:00.000000 rbapy-2.0/rba/cli/generate_rba_model.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/rba/xml/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    11610 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/targets.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      573 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/__init__.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    13880 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/processes.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     8072 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/common.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2655 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/density.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7669 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/parameters.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     6041 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/metabolism.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4220 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/enzymes.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     6557 2022-09-06 11:29:00.000000 rbapy-2.0/rba/xml/macromolecules.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7646 2022-09-29 14:20:09.000000 rbapy-2.0/rba/model.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/rba/prerba/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      990 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/enzyme.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    13855 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/model_builder.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    11897 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/sbml_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    10499 2022-09-27 22:28:33.000000 rbapy-2.0/rba/prerba/uniprot_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     9871 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/default_processes.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3718 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/fasta_parser.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      147 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/__init__.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      675 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/user_machinery.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2392 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/pipeline_parameters.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1926 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/macromolecule.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     8354 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/user_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4925 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/default_targets.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     8370 2022-09-27 22:28:27.000000 rbapy-2.0/rba/prerba/manual_annotation.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    13233 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/default_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3318 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/curation_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      901 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/protein_export.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4463 2022-09-28 13:02:09.000000 rbapy-2.0/rba/prerba/uniprot_importer.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     8427 2022-09-06 11:29:00.000000 rbapy-2.0/rba/prerba/protein_data.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      209 2022-09-29 15:04:48.000000 rbapy-2.0/rba/_authors.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     5103 2022-09-29 15:06:41.000000 rbapy-2.0/setup.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1218 2022-09-06 11:29:00.000000 rbapy-2.0/.gitignore
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/rbapy.egg-info/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     6556 2022-11-08 15:40:32.000000 rbapy-2.0/rbapy.egg-info/PKG-INFO
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2275 2022-11-08 15:40:33.000000 rbapy-2.0/rbapy.egg-info/SOURCES.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      119 2022-11-08 15:40:32.000000 rbapy-2.0/rbapy.egg-info/entry_points.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      367 2022-11-08 15:40:32.000000 rbapy-2.0/rbapy.egg-info/requires.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        4 2022-11-08 15:40:32.000000 rbapy-2.0/rbapy.egg-info/top_level.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        1 2022-11-08 15:40:32.000000 rbapy-2.0/rbapy.egg-info/dependency_links.txt
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/.github/
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:35.000000 rbapy-2.0/.github/workflows/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2566 2022-09-06 11:29:00.000000 rbapy-2.0/.github/workflows/ci.yml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       67 2022-11-08 15:40:36.000000 rbapy-2.0/setup.cfg
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     5067 2022-11-08 15:13:56.000000 rbapy-2.0/README.rst
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    35147 2022-09-06 11:29:00.000000 rbapy-2.0/LICENSE.txt
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/sample_input_small/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1454 2022-11-08 14:38:55.000000 rbapy-2.0/sample_input_small/params.in
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2022-11-08 15:40:36.000000 rbapy-2.0/sample_input_small/data/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2022-11-08 14:38:55.000000 rbapy-2.0/sample_input_small/data/trnas.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2956 2022-11-08 14:38:55.000000 rbapy-2.0/sample_input_small/data/chaperones.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2022-11-08 14:38:55.000000 rbapy-2.0/sample_input_small/data/sbml.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    23228 2022-11-08 14:38:55.000000 rbapy-2.0/sample_input_small/data/ribosome.fasta
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:44.000000 rbapy-2.0.1/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     6877 2023-06-05 14:37:44.000000 rbapy-2.0.1/PKG-INFO
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:43.000000 rbapy-2.0.1/sample_input/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2722 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input/params.in
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:43.000000 rbapy-2.0.1/sample_input/data/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2022-09-06 11:29:00.000000 rbapy-2.0.1/sample_input/data/trnas.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2943 2022-09-06 11:29:00.000000 rbapy-2.0.1/sample_input/data/chaperones.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    22686 2022-09-06 11:29:00.000000 rbapy-2.0.1/sample_input/data/ribosome.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)  9168624 2022-09-06 11:29:00.000000 rbapy-2.0.1/sample_input/data/sample.xml
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:44.000000 rbapy-2.0.1/tests/
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:44.000000 rbapy-2.0.1/tests/utils/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4600 2023-03-24 11:01:43.000000 rbapy-2.0.1/tests/utils/test_inject_efficiencies.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      114 2022-09-06 11:29:00.000000 rbapy-2.0.1/tests/utils/efficiencies.tsv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    18474 2023-03-24 11:01:43.000000 rbapy-2.0.1/tests/test_tutorial.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2432 2023-03-24 11:01:43.000000 rbapy-2.0.1/tests/test_cli.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:40.000000 rbapy-2.0.1/docs/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   125020 2022-09-06 11:29:00.000000 rbapy-2.0.1/docs/Model_construction (RBApy.prerba).pdf
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    39066 2022-09-06 11:29:00.000000 rbapy-2.0.1/docs/xml_tutorial.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   227777 2022-09-06 11:29:00.000000 rbapy-2.0.1/docs/Model_computation (RBApy.core).pdf
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   163632 2022-09-06 11:29:00.000000 rbapy-2.0.1/docs/Parameter_estimation (RBApy.estim) - Text-S6.pdf
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)  5465542 2023-03-24 11:01:43.000000 rbapy-2.0.1/docs/XML_format (RBApy.xml).pdf
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:40.000000 rbapy-2.0.1/rba/
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:41.000000 rbapy-2.0.1/rba/core/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    10899 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/functions.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    11309 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/core/targets.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    14046 2023-06-05 12:27:25.000000 rbapy-2.0.1/rba/core/species.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    38261 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/solver.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      174 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/core/__init__.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7923 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/constraint_matrix.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2380 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/core/processes.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2214 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/density.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3101 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/core/constraint_blocks.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2960 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/core/parameters.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     5411 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/metabolism.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2833 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/enzymes.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      984 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/core/parameter_vector.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       22 2023-06-05 14:34:42.000000 rbapy-2.0.1/rba/_version.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:41.000000 rbapy-2.0.1/rba/estim/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3921 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/estim/nonenz_per_compartment.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2618 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/estim/prot_per_compartment.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    17016 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/estim/utils.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      732 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/estim/kapp.cfg
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3258 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/estim/kapp.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1572 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/estim/nonenz_per_compartment.cfg
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1325 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/estim/prot_per_compartment.cfg
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      587 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/__init__.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:42.000000 rbapy-2.0.1/rba/utils/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7807 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/utils/efficiencies.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     9724 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/utils/results.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      104 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/utils/__init__.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:40.000000 rbapy-2.0.1/rba/cli/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        0 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/cli/__init__.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2491 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/cli/solve_rba_model.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1022 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/cli/generate_rba_model.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:43.000000 rbapy-2.0.1/rba/xml/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    11610 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/targets.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      573 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/__init__.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    13880 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/processes.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     8072 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/common.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2655 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/density.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7669 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/parameters.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     6041 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/metabolism.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4220 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/enzymes.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     6557 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/xml/macromolecules.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7646 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/model.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:42.000000 rbapy-2.0.1/rba/prerba/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      990 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/enzyme.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    13855 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/model_builder.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    11897 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/sbml_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    10499 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/uniprot_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     9871 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/default_processes.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3718 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/fasta_parser.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      147 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/__init__.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      675 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/user_machinery.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2392 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/pipeline_parameters.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1926 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/macromolecule.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     8354 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/user_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4925 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/default_targets.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     8370 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/manual_annotation.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    13233 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/default_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3356 2023-06-05 14:34:42.000000 rbapy-2.0.1/rba/prerba/curation_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      901 2022-09-06 11:29:00.000000 rbapy-2.0.1/rba/prerba/protein_export.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4463 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/uniprot_importer.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     8427 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/prerba/protein_data.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      209 2023-03-24 11:01:43.000000 rbapy-2.0.1/rba/_authors.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     5103 2023-03-24 11:01:43.000000 rbapy-2.0.1/setup.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1218 2022-09-06 11:29:00.000000 rbapy-2.0.1/.gitignore
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:43.000000 rbapy-2.0.1/rbapy.egg-info/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     6877 2023-06-05 14:37:32.000000 rbapy-2.0.1/rbapy.egg-info/PKG-INFO
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2275 2023-06-05 14:37:35.000000 rbapy-2.0.1/rbapy.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      119 2023-06-05 14:37:32.000000 rbapy-2.0.1/rbapy.egg-info/entry_points.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      367 2023-06-05 14:37:32.000000 rbapy-2.0.1/rbapy.egg-info/requires.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        4 2023-06-05 14:37:32.000000 rbapy-2.0.1/rbapy.egg-info/top_level.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        1 2023-06-05 14:37:32.000000 rbapy-2.0.1/rbapy.egg-info/dependency_links.txt
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:39.000000 rbapy-2.0.1/.github/
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:39.000000 rbapy-2.0.1/.github/workflows/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2566 2023-03-24 11:01:43.000000 rbapy-2.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       67 2023-06-05 14:37:44.000000 rbapy-2.0.1/setup.cfg
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     5386 2023-03-24 11:01:43.000000 rbapy-2.0.1/README.rst
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    35147 2022-09-06 11:29:00.000000 rbapy-2.0.1/LICENSE.txt
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:43.000000 rbapy-2.0.1/sample_input_small/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1454 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input_small/params.in
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-05 14:37:44.000000 rbapy-2.0.1/sample_input_small/data/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input_small/data/trnas.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2956 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input_small/data/chaperones.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input_small/data/sbml.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    23228 2023-03-24 11:01:43.000000 rbapy-2.0.1/sample_input_small/data/ribosome.fasta
```

### Comparing `rbapy-2.0/PKG-INFO` & `rbapy-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbapy
-Version: 2.0
+Version: 2.0.1
 Summary: Package for automated generation of bacterial Resource Balance Analysis (RBA) models and simulation of RBA models
 Home-page: https://sysbioinra.github.io/RBApy/
 Author: RBApy was conceived and implemented originally by INRAE (Stephan Fischer, Ana Bulovic, Anne Goelzer and Marc Dinh), and updated regularly by several contributors (Oliver Bodeit, Jonathan Karr, Michael Jahn)
 Author-email: anne.goelzer@inra.fr
 License: GPLv3
 Keywords: metabolism,Resource Balance Analysis,molecular biology,cell biology,biochemistry,systems biology,computational biology,mathematical modeling,numerical simulation
 Platform: UNKNOWN
@@ -30,16 +30,16 @@
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 RBApy
 ==============================
 
-RBApy is a open-source Python package for automated generation of bacterial Resource Balance Analysis (RBA) models.
-RBA models have been developed for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain). You can find these models here: https://github.com/SysBioInra/Bacterial-RBA-models.
+RBApy is a open-source Python package for the automated generation of bacterial Resource Balance Analysis (RBA) models (https://rba.inrae.fr).
+Existing RBA models for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain) can be found here: https://github.com/SysBioInra/Bacterial-RBA-models.
 
 For a complete documentation on RBApy installation and usage, please visit the website:
 https://sysbioinra.github.io/RBApy/
 
 
 Installation
 -------------
@@ -49,33 +49,33 @@
 1. Optionally, install the CPLEX linear programming solver.
 
 2. Install this package from PyPI:
     ```
     pip install rbapy
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
+    Optionally, also install CPLEX by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
 
     ```
     pip install rbapy[cplex]
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
+    Optionally, also install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
     
     ```
     pip install rbapy[swiglpk]
     ```
 
-    Optionally, install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
+    Optionally, also install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
 
     ```
     pip install rbapy[gurobi]
     ```
 
-More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/.
+More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/installation.html.
 
 Remark on usage
 ---------------
 
 When using RBApy in own Python code, it must be imported as: rba
 
     ```
@@ -83,15 +83,15 @@
     ```
     
 Running
 -------
 
 For more detailed instructions on usage, please refer to the RBApy website https://sysbioinra.github.io/RBApy/.
 
-Put the SBML file containing the GSMM of your organism of interest in the `input` directory and fill in the
+Put the SBML file containing the Genome Size Metabolic Model (GSMM) of your organism of interest in the `input` directory and fill in the
 parameter file `input/params.in`. Then open a console at the root
 of the repository and run:
 
 
 ```
 python generate_rba_model.py input/params.in
 ```
@@ -109,22 +109,22 @@
 Warning: for the first run, the script will download and parse Uniprot data
 as best it can. Unfortunately, numerous values cannot be parsed properly and
 are replaced with default values. The script will generate many helper files
 to replace these default values with hand-curated values. You should fill in
 these helper files and rerun the script to obtain more relevant output
 (see instructions below).
 
-If rbapy was installed properly, there also exists command-line interface called by:
+If rbapy has been installed properly, there also exists command-line interface called by:
 
 
 ```
 generate-rba-model path/to/params.in
 ```
 
-Once the RBA model was generated, you can solve it using:
+Once the RBA model has been generated, you can solve it using:
 
 
 ```
 python solve_rba_model.py path/to/model
 ```
 
 where the path points to the directory containing the XML files defining
@@ -160,15 +160,15 @@
 
 Fischer S. , Bulovic A. , Goelzer A. , Bodeit, O., Dinh M.
 
 
 Citation
 ---------------
 
-If you wish to cite this work, please refer to `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
+If you use RBApy for scientific publications, please cite Bulović A., Fischer S., Dinh M., Golib F., Liebermeister W., Poirier C., Tournier L., Klipp E., Fromion V., Goelzer A. (2019), "Automated generation of bacterial resource allocation models", Metabolic Engineering 55 (2019) 12–22. `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
 
 
 License
 -------
 
 Copyright (c) 2018 INRAE - MaIAGE - France.
```

### Comparing `rbapy-2.0/sample_input/params.in` & `rbapy-2.0.1/sample_input/params.in`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input/data/trnas.fasta` & `rbapy-2.0.1/sample_input/data/trnas.fasta`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input/data/chaperones.fasta` & `rbapy-2.0.1/sample_input/data/chaperones.fasta`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input/data/ribosome.fasta` & `rbapy-2.0.1/sample_input/data/ribosome.fasta`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input/data/sample.xml` & `rbapy-2.0.1/sample_input/data/sample.xml`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/tests/utils/test_inject_efficiencies.py` & `rbapy-2.0.1/tests/utils/test_inject_efficiencies.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/tests/test_tutorial.py` & `rbapy-2.0.1/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/tests/test_cli.py` & `rbapy-2.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/docs/Model_construction (RBApy.prerba).pdf` & `rbapy-2.0.1/docs/Model_construction (RBApy.prerba).pdf`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/docs/xml_tutorial.ipynb` & `rbapy-2.0.1/docs/xml_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/docs/Model_computation (RBApy.core).pdf` & `rbapy-2.0.1/docs/Model_computation (RBApy.core).pdf`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/docs/Parameter_estimation (RBApy.estim) - Text-S6.pdf` & `rbapy-2.0.1/docs/Parameter_estimation (RBApy.estim) - Text-S6.pdf`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/docs/XML_format (RBApy.xml).pdf` & `rbapy-2.0.1/docs/XML_format (RBApy.xml).pdf`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/functions.py` & `rbapy-2.0.1/rba/core/functions.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/targets.py` & `rbapy-2.0.1/rba/core/targets.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/species.py` & `rbapy-2.0.1/rba/core/species.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,20 @@
                 )
     # aggregate matrices across sets
     production_metabolites = [s.production for s in (proteins, rnas, dna)]
     production_cost = [s.production_cost for s in (proteins, rnas, dna)]
     degradation_metabolites = [s.degradation for s in (proteins, rnas, dna)]
     degradation_cost = [s.degradation_cost for s in (proteins, rnas, dna)]
     weight = [s.weight for s in (proteins, rnas, dna)]
+    #print('hstack')
+    #print(type(proteins.production))
+    #print(proteins.production)
+    #print(hstack([s.production for s in (proteins,rnas, dna)]))
+    #print(hstack([s.production_cost for s in (proteins,rnas, dna)]))
+    #print('------------')
     return (hstack(production_metabolites), hstack(production_cost),
             hstack(degradation_metabolites), hstack(degradation_cost),
             hstack(weight))
 
 
 class MacromoleculeSet(object):
     """Macromolecule information."""
```

### Comparing `rbapy-2.0/rba/core/solver.py` & `rbapy-2.0.1/rba/core/solver.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/constraint_matrix.py` & `rbapy-2.0.1/rba/core/constraint_matrix.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/processes.py` & `rbapy-2.0.1/rba/core/processes.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/density.py` & `rbapy-2.0.1/rba/core/density.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/constraint_blocks.py` & `rbapy-2.0.1/rba/core/constraint_blocks.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/parameters.py` & `rbapy-2.0.1/rba/core/parameters.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/metabolism.py` & `rbapy-2.0.1/rba/core/metabolism.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/enzymes.py` & `rbapy-2.0.1/rba/core/enzymes.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/core/parameter_vector.py` & `rbapy-2.0.1/rba/core/parameter_vector.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/nonenz_per_compartment.py` & `rbapy-2.0.1/rba/estim/nonenz_per_compartment.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/prot_per_compartment.py` & `rbapy-2.0.1/rba/estim/prot_per_compartment.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/utils.py` & `rbapy-2.0.1/rba/estim/utils.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/kapp.cfg` & `rbapy-2.0.1/rba/estim/kapp.cfg`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/kapp.py` & `rbapy-2.0.1/rba/estim/kapp.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/nonenz_per_compartment.cfg` & `rbapy-2.0.1/rba/estim/nonenz_per_compartment.cfg`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/estim/prot_per_compartment.cfg` & `rbapy-2.0.1/rba/estim/prot_per_compartment.cfg`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/__init__.py` & `rbapy-2.0.1/rba/__init__.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/utils/efficiencies.py` & `rbapy-2.0.1/rba/utils/efficiencies.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/utils/results.py` & `rbapy-2.0.1/rba/utils/results.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/cli/solve_rba_model.py` & `rbapy-2.0.1/rba/cli/solve_rba_model.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/cli/generate_rba_model.py` & `rbapy-2.0.1/rba/cli/generate_rba_model.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/targets.py` & `rbapy-2.0.1/rba/xml/targets.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/__init__.py` & `rbapy-2.0.1/rba/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/processes.py` & `rbapy-2.0.1/rba/xml/processes.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/common.py` & `rbapy-2.0.1/rba/xml/common.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/density.py` & `rbapy-2.0.1/rba/xml/density.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/parameters.py` & `rbapy-2.0.1/rba/xml/parameters.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/metabolism.py` & `rbapy-2.0.1/rba/xml/metabolism.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/enzymes.py` & `rbapy-2.0.1/rba/xml/enzymes.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/xml/macromolecules.py` & `rbapy-2.0.1/rba/xml/macromolecules.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/model.py` & `rbapy-2.0.1/rba/model.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/enzyme.py` & `rbapy-2.0.1/rba/prerba/enzyme.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/model_builder.py` & `rbapy-2.0.1/rba/prerba/model_builder.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/sbml_data.py` & `rbapy-2.0.1/rba/prerba/sbml_data.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/uniprot_data.py` & `rbapy-2.0.1/rba/prerba/uniprot_data.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/default_processes.py` & `rbapy-2.0.1/rba/prerba/default_processes.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/fasta_parser.py` & `rbapy-2.0.1/rba/prerba/fasta_parser.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/user_machinery.py` & `rbapy-2.0.1/rba/prerba/user_machinery.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/pipeline_parameters.py` & `rbapy-2.0.1/rba/prerba/pipeline_parameters.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/macromolecule.py` & `rbapy-2.0.1/rba/prerba/macromolecule.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/user_data.py` & `rbapy-2.0.1/rba/prerba/user_data.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/default_targets.py` & `rbapy-2.0.1/rba/prerba/default_targets.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/manual_annotation.py` & `rbapy-2.0.1/rba/prerba/manual_annotation.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/default_data.py` & `rbapy-2.0.1/rba/prerba/default_data.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/curation_data.py` & `rbapy-2.0.1/rba/prerba/curation_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         ----------
         rows : list of lists/tuples
             Set of rows to add to current data. The length of each row
             has to match the number of columns.
 
         """
         new_rows = pandas.DataFrame(rows, columns=self.data.columns)
-        self.data = self.data.append(new_rows)
+        self.data = pandas.concat([self.data, new_rows], axis=0,ignore_index=True)  
         self._data_added = True
 
     def add_row(self, row):
         """
         Add single row to data.
 
         Parameters
```

### Comparing `rbapy-2.0/rba/prerba/protein_export.py` & `rbapy-2.0.1/rba/prerba/protein_export.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/uniprot_importer.py` & `rbapy-2.0.1/rba/prerba/uniprot_importer.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rba/prerba/protein_data.py` & `rbapy-2.0.1/rba/prerba/protein_data.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/setup.py` & `rbapy-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/.gitignore` & `rbapy-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/rbapy.egg-info/PKG-INFO` & `rbapy-2.0.1/rbapy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbapy
-Version: 2.0
+Version: 2.0.1
 Summary: Package for automated generation of bacterial Resource Balance Analysis (RBA) models and simulation of RBA models
 Home-page: https://sysbioinra.github.io/RBApy/
 Author: RBApy was conceived and implemented originally by INRAE (Stephan Fischer, Ana Bulovic, Anne Goelzer and Marc Dinh), and updated regularly by several contributors (Oliver Bodeit, Jonathan Karr, Michael Jahn)
 Author-email: anne.goelzer@inra.fr
 License: GPLv3
 Keywords: metabolism,Resource Balance Analysis,molecular biology,cell biology,biochemistry,systems biology,computational biology,mathematical modeling,numerical simulation
 Platform: UNKNOWN
@@ -30,16 +30,16 @@
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 RBApy
 ==============================
 
-RBApy is a open-source Python package for automated generation of bacterial Resource Balance Analysis (RBA) models.
-RBA models have been developed for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain). You can find these models here: https://github.com/SysBioInra/Bacterial-RBA-models.
+RBApy is a open-source Python package for the automated generation of bacterial Resource Balance Analysis (RBA) models (https://rba.inrae.fr).
+Existing RBA models for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain) can be found here: https://github.com/SysBioInra/Bacterial-RBA-models.
 
 For a complete documentation on RBApy installation and usage, please visit the website:
 https://sysbioinra.github.io/RBApy/
 
 
 Installation
 -------------
@@ -49,33 +49,33 @@
 1. Optionally, install the CPLEX linear programming solver.
 
 2. Install this package from PyPI:
     ```
     pip install rbapy
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
+    Optionally, also install CPLEX by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
 
     ```
     pip install rbapy[cplex]
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
+    Optionally, also install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
     
     ```
     pip install rbapy[swiglpk]
     ```
 
-    Optionally, install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
+    Optionally, also install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
 
     ```
     pip install rbapy[gurobi]
     ```
 
-More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/.
+More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/installation.html.
 
 Remark on usage
 ---------------
 
 When using RBApy in own Python code, it must be imported as: rba
 
     ```
@@ -83,15 +83,15 @@
     ```
     
 Running
 -------
 
 For more detailed instructions on usage, please refer to the RBApy website https://sysbioinra.github.io/RBApy/.
 
-Put the SBML file containing the GSMM of your organism of interest in the `input` directory and fill in the
+Put the SBML file containing the Genome Size Metabolic Model (GSMM) of your organism of interest in the `input` directory and fill in the
 parameter file `input/params.in`. Then open a console at the root
 of the repository and run:
 
 
 ```
 python generate_rba_model.py input/params.in
 ```
@@ -109,22 +109,22 @@
 Warning: for the first run, the script will download and parse Uniprot data
 as best it can. Unfortunately, numerous values cannot be parsed properly and
 are replaced with default values. The script will generate many helper files
 to replace these default values with hand-curated values. You should fill in
 these helper files and rerun the script to obtain more relevant output
 (see instructions below).
 
-If rbapy was installed properly, there also exists command-line interface called by:
+If rbapy has been installed properly, there also exists command-line interface called by:
 
 
 ```
 generate-rba-model path/to/params.in
 ```
 
-Once the RBA model was generated, you can solve it using:
+Once the RBA model has been generated, you can solve it using:
 
 
 ```
 python solve_rba_model.py path/to/model
 ```
 
 where the path points to the directory containing the XML files defining
@@ -160,15 +160,15 @@
 
 Fischer S. , Bulovic A. , Goelzer A. , Bodeit, O., Dinh M.
 
 
 Citation
 ---------------
 
-If you wish to cite this work, please refer to `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
+If you use RBApy for scientific publications, please cite Bulović A., Fischer S., Dinh M., Golib F., Liebermeister W., Poirier C., Tournier L., Klipp E., Fromion V., Goelzer A. (2019), "Automated generation of bacterial resource allocation models", Metabolic Engineering 55 (2019) 12–22. `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
 
 
 License
 -------
 
 Copyright (c) 2018 INRAE - MaIAGE - France.
```

### Comparing `rbapy-2.0/rbapy.egg-info/SOURCES.txt` & `rbapy-2.0.1/rbapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/.github/workflows/ci.yml` & `rbapy-2.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/README.rst` & `rbapy-2.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RBApy
 ==============================
 
-RBApy is a open-source Python package for automated generation of bacterial Resource Balance Analysis (RBA) models.
-RBA models have been developed for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain). You can find these models here: https://github.com/SysBioInra/Bacterial-RBA-models.
+RBApy is a open-source Python package for the automated generation of bacterial Resource Balance Analysis (RBA) models (https://rba.inrae.fr).
+Existing RBA models for *Bacillus subtilis 168* (wild type), *Escherichia coli K-12* (wild type) and CO2-fixing *Escherichia coli K-12* (an engineered strain) can be found here: https://github.com/SysBioInra/Bacterial-RBA-models.
 
 For a complete documentation on RBApy installation and usage, please visit the website:
 https://sysbioinra.github.io/RBApy/
 
 
 Installation
 -------------
@@ -16,33 +16,33 @@
 1. Optionally, install the CPLEX linear programming solver.
 
 2. Install this package from PyPI:
     ```
     pip install rbapy
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
+    Optionally, also install CPLEX by installing RBApy with the ``cplex`` option. Note, this requires a CPLEX license.:
 
     ```
     pip install rbapy[cplex]
     ```
 
-    Optionally, install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
+    Optionally, also install GLPK by installing RBApy with the ``swiglpk`` option. Note, this requires ``libglpk-dev``.:
     
     ```
     pip install rbapy[swiglpk]
     ```
 
-    Optionally, install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
+    Optionally, also install Gurobi by installing RBApy with the ``gurobi`` option. Note, this requires a Gurobi license.:
 
     ```
     pip install rbapy[gurobi]
     ```
 
-More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/.
+More information about how to install RBApy is available at https://sysbioinra.github.io/RBApy/installation.html.
 
 Remark on usage
 ---------------
 
 When using RBApy in own Python code, it must be imported as: rba
 
     ```
@@ -50,15 +50,15 @@
     ```
     
 Running
 -------
 
 For more detailed instructions on usage, please refer to the RBApy website https://sysbioinra.github.io/RBApy/.
 
-Put the SBML file containing the GSMM of your organism of interest in the `input` directory and fill in the
+Put the SBML file containing the Genome Size Metabolic Model (GSMM) of your organism of interest in the `input` directory and fill in the
 parameter file `input/params.in`. Then open a console at the root
 of the repository and run:
 
 
 ```
 python generate_rba_model.py input/params.in
 ```
@@ -76,22 +76,22 @@
 Warning: for the first run, the script will download and parse Uniprot data
 as best it can. Unfortunately, numerous values cannot be parsed properly and
 are replaced with default values. The script will generate many helper files
 to replace these default values with hand-curated values. You should fill in
 these helper files and rerun the script to obtain more relevant output
 (see instructions below).
 
-If rbapy was installed properly, there also exists command-line interface called by:
+If rbapy has been installed properly, there also exists command-line interface called by:
 
 
 ```
 generate-rba-model path/to/params.in
 ```
 
-Once the RBA model was generated, you can solve it using:
+Once the RBA model has been generated, you can solve it using:
 
 
 ```
 python solve_rba_model.py path/to/model
 ```
 
 where the path points to the directory containing the XML files defining
@@ -127,15 +127,15 @@
 
 Fischer S. , Bulovic A. , Goelzer A. , Bodeit, O., Dinh M.
 
 
 Citation
 ---------------
 
-If you wish to cite this work, please refer to `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
+If you use RBApy for scientific publications, please cite Bulović A., Fischer S., Dinh M., Golib F., Liebermeister W., Poirier C., Tournier L., Klipp E., Fromion V., Goelzer A. (2019), "Automated generation of bacterial resource allocation models", Metabolic Engineering 55 (2019) 12–22. `https://doi.org/10.1016/j.ymben.2019.06.001 <https://doi.org/10.1016/j.ymben.2019.06.001>`_.
 
 
 License
 -------
 
 Copyright (c) 2018 INRAE - MaIAGE - France.
```

### Comparing `rbapy-2.0/LICENSE.txt` & `rbapy-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input_small/params.in` & `rbapy-2.0.1/sample_input_small/params.in`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input_small/data/trnas.fasta` & `rbapy-2.0.1/sample_input_small/data/trnas.fasta`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input_small/data/chaperones.fasta` & `rbapy-2.0.1/sample_input_small/data/chaperones.fasta`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input_small/data/sbml.xml` & `rbapy-2.0.1/sample_input_small/data/sbml.xml`

 * *Files identical despite different names*

### Comparing `rbapy-2.0/sample_input_small/data/ribosome.fasta` & `rbapy-2.0.1/sample_input_small/data/ribosome.fasta`

 * *Files identical despite different names*

