# Comparing `tmp/BFEE2-2.3.2.tar.gz` & `tmp/BFEE2-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BFEE2-2.3.2.tar", last modified: Thu Feb  9 07:57:15 2023, max compression
+gzip compressed data, was "BFEE2-2.4.0.tar", last modified: Mon Jun  5 06:32:34 2023, max compression
```

## Comparing `BFEE2-2.3.2.tar` & `BFEE2-2.4.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.397421 BFEE2-2.3.2/
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.363313 BFEE2-2.3.2/BFEE2/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:56:19.000000 BFEE2-2.3.2/BFEE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.368499 BFEE2-2.3.2/BFEE2/commonTools/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/commonTools/__init__.py
--rw-rw-rw-   0        0        0     1450 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/commonTools/commonSlots.py
--rw-rw-rw-   0        0        0    11005 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/commonTools/fileParser.py
--rw-rw-rw-   0        0        0     5677 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/commonTools/ploter.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.369509 BFEE2-2.3.2/BFEE2/doc/
--rw-rw-rw-   0        0        0   143522 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/doc/Doc.pdf
--rw-rw-rw-   0        0        0        1 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/doc/__init__.py
--rw-rw-rw-   0        0        0    97821 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/gui.py
--rw-rw-rw-   0        0        0   129338 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/inputGenerator.py
--rw-rw-rw-   0        0        0    19724 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/postTreatment.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.389892 BFEE2-2.3.2/BFEE2/templates_gromacs/
--rw-rw-rw-   0        0        0      654 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/000.colvars.template
--rw-rw-rw-   0        0        0     1124 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/000.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/000.mdp.template
--rw-rw-rw-   0        0        0     1595 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/001.colvars.template
--rw-rw-rw-   0        0        0     1124 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/001.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/001.mdp.template
--rw-rw-rw-   0        0        0        2 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/001.readme.template
--rw-rw-rw-   0        0        0     2169 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/002.colvars.template
--rw-rw-rw-   0        0        0     1124 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/002.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/002.mdp.template
--rw-rw-rw-   0        0        0     2708 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/003.colvars.template
--rw-rw-rw-   0        0        0     1397 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/003.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/003.mdp.template
--rw-rw-rw-   0        0        0     3300 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/004.colvars.template
--rw-rw-rw-   0        0        0     1525 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/004.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/004.mdp.template
--rw-rw-rw-   0        0        0     3809 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/005.colvars.template
--rw-rw-rw-   0        0        0     1653 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/005.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/005.mdp.template
--rw-rw-rw-   0        0        0     4260 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/006.colvars.template
--rw-rw-rw-   0        0        0     1781 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/006.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/006.mdp.template
--rw-rw-rw-   0        0        0     4512 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007.colvars.template
--rw-rw-rw-   0        0        0     1909 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1497 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007.mdp.template
--rw-rw-rw-   0        0        0     3584 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007_eq.colvars.template
--rw-rw-rw-   0        0        0     3118 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1181 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/007_min.mdp.template
--rw-rw-rw-   0        0        0     1044 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/008.colvars.template
--rw-rw-rw-   0        0        0     1124 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/008.generate_tpr_sh.template
--rw-rw-rw-   0        0        0     1516 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/008.mdp.template
--rw-rw-rw-   0        0        0     1079 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template
--rw-rw-rw-   0        0        0    74395 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/BFEEGromacs.py
--rw-rw-rw-   0        0        0        0 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/__init__.py
--rw-rw-rw-   0        0        0      394 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_gromacs/find_min_max.awk
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.393418 BFEE2-2.3.2/BFEE2/templates_namd/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/__init__.py
--rw-rw-rw-   0        0        0    44058 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/configTemplate.py
--rw-rw-rw-   0        0        0     8601 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/fep.tcl
--rw-rw-rw-   0        0        0     4809 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/scriptTemplate.py
--rw-rw-rw-   0        0        0      302 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/solvate.tcl
--rw-rw-rw-   0        0        0      298 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/solvate_mem.tcl
--rw-rw-rw-   0        0        0    10591 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_namd/updateCenters.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.395426 BFEE2-2.3.2/BFEE2/templates_readme/
--rw-rw-rw-   0        0        0     1027 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt
--rw-rw-rw-   0        0        0      879 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt
--rw-rw-rw-   0        0        0     1492 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/templates_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.396426 BFEE2-2.3.2/BFEE2/third_party/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/third_party/__init__.py
--rw-rw-rw-   0        0        0    14767 2023-02-09 07:56:13.000000 BFEE2-2.3.2/BFEE2/third_party/py_bar.py
--rw-rw-rw-   0        0        0       22 2023-02-09 07:56:12.000000 BFEE2-2.3.2/BFEE2/version.py
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.366498 BFEE2-2.3.2/BFEE2.egg-info/
--rw-rw-rw-   0        0        0     5125 2023-02-09 07:57:15.000000 BFEE2-2.3.2/BFEE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2581 2023-02-09 07:57:15.000000 BFEE2-2.3.2/BFEE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 07:57:15.000000 BFEE2-2.3.2/BFEE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-02-09 07:57:15.000000 BFEE2-2.3.2/BFEE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-09 07:57:15.000000 BFEE2-2.3.2/BFEE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35349 2023-02-09 07:56:11.000000 BFEE2-2.3.2/LICENSE
--rw-rw-rw-   0        0        0     5125 2023-02-09 07:57:15.397421 BFEE2-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4659 2023-02-09 07:56:12.000000 BFEE2-2.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-09 07:57:15.396426 BFEE2-2.3.2/bin/
--rw-rw-rw-   0        0        0      468 2023-02-09 07:56:13.000000 BFEE2-2.3.2/bin/BFEE2Gui.py
--rw-rw-rw-   0        0        0      104 2023-02-09 07:56:12.000000 BFEE2-2.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      719 2023-02-09 07:57:15.399428 BFEE2-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-02-09 07:56:12.000000 BFEE2-2.3.2/setup.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/__init__.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/commonTools/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/__init__.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1450 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/commonSlots.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    11005 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/fileParser.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5677 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/ploter.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/doc/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)   143522 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/doc/Doc.pdf
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/doc/__init__.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    99397 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/gui.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)   130682 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/inputGenerator.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    20408 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/postTreatment.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.177026 BFEE2-2.4.0/BFEE2/templates_gromacs/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      654 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1595 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        2 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.readme.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2169 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2708 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1397 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3300 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1525 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3809 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1653 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4260 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1781 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4512 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1909 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1497 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3584 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3118 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1181 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_min.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1044 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.colvars.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.mdp.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1079 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    74395 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/BFEEGromacs.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/__init__.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      394 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/find_min_max.awk
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.177026 BFEE2-2.4.0/BFEE2/templates_namd/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/__init__.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    44797 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/configTemplate.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     8601 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/fep.tcl
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4809 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/scriptTemplate.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      302 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/solvate.tcl
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      298 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/solvate_mem.tcl
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    10591 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/updateCenters.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/BFEE2/templates_readme/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1027 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      879 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1492 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/__init__.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/BFEE2/third_party/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/third_party/__init__.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    14923 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/third_party/py_bar.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)       49 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/version.py
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2.egg-info/
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5059 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/PKG-INFO
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2581 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)       68 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/requires.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        6 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/top_level.txt
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    35349 2023-06-05 06:17:23.000000 BFEE2-2.4.0/LICENSE
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5059 2023-06-05 06:32:34.181026 BFEE2-2.4.0/PKG-INFO
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4659 2023-06-05 06:17:23.000000 BFEE2-2.4.0/README.md
+drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/bin/
+-rwxr-xr-x   0 chinfo    (1000) chinfo    (1000)      468 2023-06-05 06:17:23.000000 BFEE2-2.4.0/bin/BFEE2Gui.py
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      104 2023-06-05 06:17:23.000000 BFEE2-2.4.0/pyproject.toml
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      683 2023-06-05 06:32:34.181026 BFEE2-2.4.0/setup.cfg
+-rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      247 2023-06-05 06:17:23.000000 BFEE2-2.4.0/setup.py
```

### Comparing `BFEE2-2.3.2/BFEE2/commonTools/commonSlots.py` & `BFEE2-2.4.0/BFEE2/commonTools/commonSlots.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/commonTools/fileParser.py` & `BFEE2-2.4.0/BFEE2/commonTools/fileParser.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/commonTools/ploter.py` & `BFEE2-2.4.0/BFEE2/commonTools/ploter.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/doc/Doc.pdf` & `BFEE2-2.4.0/BFEE2/doc/Doc.pdf`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/gui.py` & `BFEE2-2.4.0/BFEE2/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
 import BFEE2.version
 from BFEE2 import doc
 
 __PROGRAM_NAME__ = f'BFEEstimator v{BFEE2.version.__VERSION__}'
+__NAMD_VERSION__ = f'v{BFEE2.version.__NAMD_VERSION__}'
 
 class mainSettings(QWidget):
     """settings in the menubar
        set pathes of third-party softwares (VMD, gmx and tleap)
     """
     
     def __init__(self):
@@ -427,14 +428,24 @@
         
         self.OPLSMixingRuleCheckbox = QCheckBox('OPLS mixing rules')
         self.OPLSMixingRuleCheckbox.setChecked(False)
         
         self.FFSettingsLayout.addWidget(self.OPLSMixingRuleCheckbox)
         self.FFSettings.setLayout(self.FFSettingsLayout)
 
+        # strategy settings
+        self.strategy = QGroupBox('Strategy settings')
+        self.strategyLayout = QHBoxLayout()
+
+        self.considerRMSDCVCheckbox = QCheckBox('Take into account RMSD CV')
+        self.considerRMSDCVCheckbox.setChecked(True)
+
+        self.strategyLayout.addWidget(self.considerRMSDCVCheckbox)
+        self.strategy.setLayout(self.strategyLayout)
+
         # membrane protein
         self.modeling = QGroupBox('Modeling (avaiable for CHARMM FF)')
         self.modelingLayout = QVBoxLayout()
 
         self.memProCheckbox = QCheckBox('Membrane protein')
         self.memProCheckbox.setChecked(False)
         
@@ -459,14 +470,15 @@
         self.alchemicalAdvancedSettingsButtonLayout.addWidget(self.alchemicalAdvancedSettingsOKButton)
         #self.alchemicalAdvancedSettingsButtonLayout.addWidget(self.alchemicalAdvancedSettingsCancelButton)
         
         self.mainLayout.addWidget(self.stratification)
         self.mainLayout.addWidget(self.doubleWide)
         self.mainLayout.addWidget(self.compatibility)
         self.mainLayout.addWidget(self.FFSettings)
+        self.mainLayout.addWidget(self.strategy)
         self.mainLayout.addWidget(self.minBeforeSample)
         self.mainLayout.addWidget(self.modeling)
         self.mainLayout.addLayout(self.alchemicalAdvancedSettingsButtonLayout)
         self.setLayout(self.mainLayout)
 
     def _initSingalsSlots(self):
         """initialize (connect) signals and slots for the alchemical advanced settings
@@ -479,15 +491,15 @@
        include the preTreatment, postTreatment and QuickPlot tab
        the preTreatment tab include NAMD and Gromacs tab
        the postTreatment tab include geometric and alchemical tab
     """
     
     def __init__(self):
         super().__init__()
-        
+
         self._initActions()
 
         self._initNAMDTab()
         self._initGromacsTab()
         self._initPreTreatmentTab()
         self._initQuickPlotTab()
 
@@ -505,14 +517,25 @@
         self.geometricAdvancedSettings = geometricAdvancedSettings()
 
         self.setGeometry(0,0,0,0)
         self.setWindowTitle(__PROGRAM_NAME__)    
         self.setWindowIcon(QIcon("BFEE2/icon/icon.png"))
         self.show()
 
+        self._showNAMDVersionWarning()
+
+    def _showNAMDVersionWarning(self):
+        ''' show a message box ask for the latest NAMD version '''
+        QMessageBox.warning(self, 
+                            'Warning', 
+                            f'\
+{__PROGRAM_NAME__} is fully compatible with NAMD {__NAMD_VERSION__}. \n\
+Please use the same or a later version of NAMD if you have any problem.\n'
+                        )
+
     def _initActions(self):
         ''' initialize actions for menubar '''
 
         # settings
         self.settingsAction = QAction('&Settings', self)
         self.settingsAction.setStatusTip('Set pathes for third-party softwares')
         self.settingsAction.triggered.connect(self._mainSettings())
@@ -1459,15 +1482,15 @@
             Show a QMessageBox for the result
 
         Args:
             unit (str): 'namd' or 'gromacs'
         """
         
         pTreat = postTreatment.postTreatment(
-            float(self.alchemicalPostTemperatureLineEdit.text()), unit, 'geometric')
+            float(self.alchemicalPostTemperatureLineEdit.text()), unit, 'alchemical')
         
         # alchemical outputs
         files = [
                     self.alchemicalForwardLineEdit1.text(), 
                     self.alchemicalBackwardLineEdit1.text(), 
                     self.alchemicalForwardLineEdit2.text(), 
                     self.alchemicalBackwardLineEdit2.text(), 
@@ -1495,36 +1518,40 @@
             return
         if self.alchemicalPostTypeBox.currentText() == 'FEP':
                 jobType = 'fep'
         elif self.alchemicalPostTypeBox.currentText() == 'BAR':
                 jobType = 'bar'
 
         # check inputs
-        for item in [
+        rigid_ligand = False
+        for index, item in enumerate([
                     self.alchemicalBackwardLineEdit1.text(), 
                     self.alchemicalBackwardLineEdit2.text(), 
                     self.alchemicalBackwardLineEdit3.text(), 
                     self.alchemicalBackwardLineEdit4.text()
-        ]:
-            if (not os.path.exists(item)) and item != '':
+        ]):
+            if (not os.path.exists(item)) and (index != 3):
                 QMessageBox.warning(self, 'Error', f'backward file {item} does not exist and is not empty!')
                 return
 
-        for item in [
+        for index, item in enumerate([
                     self.alchemicalForwardLineEdit1.text(), 
                     self.alchemicalForwardLineEdit2.text(), 
                     self.alchemicalForwardLineEdit3.text(), 
                     self.alchemicalForwardLineEdit4.text(), 
-        ]:
-            if not os.path.exists(item):
+        ]):
+            if (not os.path.exists(item)) and (index != 3):
                 QMessageBox.warning(self, 'Error', f'file {item} does not exist!')
                 return
+            elif (not os.path.exists(item)) and (index == 3):
+                QMessageBox.warning(self, 'Warning', f'Supposing dealing with a rigid ligand!')
+                rigid_ligand = True
 
         # calculate free energies
-        result, errors = pTreat.alchemicalBindingFreeEnergy(files, parameters, temperature, jobType)
+        result, errors = pTreat.alchemicalBindingFreeEnergy(files, parameters, temperature, jobType, rigid_ligand)
 
         QMessageBox.about(
             self,
             'Result',
             f'\
 Results:\n\
 ΔG(site,couple)   = {result[0]:.2f} ± {errors[0]:.2f} kcal/mol\n\
@@ -1663,18 +1690,15 @@
                             )
                             return
                     
                     if self.geometricAdvancedSettings.useGaWTMCheckbox.isChecked():
                         QMessageBox.warning(self, 'Error', 
                                 f'\
 The feature of using GaWTM-eABF as the workhorse engine is \
-experimental! Known issues:\n \
-The config files for extending GaWTM-eABF simulations \
-will do pre-equilibration again. This may cause some errors. \
-One can revise the config file manually to avoid it'
+experimental! Please always use the latest devel version of NAMD!\n'
                         )
 
                     try:
                         iGenerator.generateNAMDGeometricFiles(
                             path,
                             self.psfLineEdit.text(),
                             self.coorLineEdit.text(),
@@ -1764,14 +1788,15 @@
                             self.alchemicalAdvancedSettings.minBeforeSampleCheckbox.isChecked(),
                             self.alchemicalAdvancedSettings.memProCheckbox.isChecked(),
                             self.alchemicalAdvancedSettings.neutralizeLigOnlyCombobox.currentText(),
                             self.alchemicalAdvancedSettings.pinDownProCheckbox.isChecked(),
                             self.alchemicalAdvancedSettings.useOldCvCheckbox.isChecked(),
                             self.mainSettings.vmdLineEdit.text(),
                             self.alchemicalAdvancedSettings.OPLSMixingRuleCheckbox.isChecked(),
+                            self.alchemicalAdvancedSettings.considerRMSDCVCheckbox.isChecked()
                         )
                     except PermissionError:
                         QMessageBox.warning(
                                 self, 
                                 'Error', 
                                 f'\
 Cannot read input files due to the permission reason!\n\
@@ -1815,19 +1840,23 @@
 Unknown error! The error message is: \n\
 {e}\n'
                         )
                         return
 
             # gromacs
             if self.preTreatmentMainTabs.currentIndex() == 1:
-
+                
                 QMessageBox.warning(
-                    self, 'Warning', f'Any setting in "Advanced settings" is not supported \n\
-when using Gromacs-formatted files as inputs!'
-                )
+                    self, 'Warning', ('<ol>\
+                  <li>Any setting in "Advanced settings" is not supported\
+                      when using Gromacs-formatted files as inputs!</li>\
+                   <li>C-rescale pressure coupling (pcoupl) is used for all simulations, \
+                      GROMACS version >= 2021 with Colvars module is required. \
+                      You may need to download it from the \
+                      <a href=\'https://github.com/Colvars/colvars/\'>Colvars website</a>.</li></ol>'))
 
                 for item in [
                         self.topLineEdit.text(), 
                         self.gromacsPdbLineEdit.text(),
                         self.gromacsLigandOnlyPdbLineEdit.text(),
                         self.gromacsLigandOnlyTopLineEdit.text()
                     ]:
```

### Comparing `BFEE2-2.3.2/BFEE2/inputGenerator.py` & `BFEE2-2.4.0/BFEE2/inputGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         doubleWide = False,
         minBeforeSample = False,
         membraneProtein = False,
         neutralizeLigOnly = 'NaCl',
         pinDownPro = True,
         useOldCv = True,
         vmdPath = '',
-        OPLSMixingRule = False
+        OPLSMixingRule = False,
+        considerRMSDCV = True
     ):
         """generate all the input files for NAMD alchemical simulation
 
         Args:
             path (str): the directory for generation of all the files
             topFile (str): the path of the topology (psf, parm) file
             coorFile (str): the path of the coordinate (pdb, rst7) file
@@ -84,23 +85,24 @@
             neutralizeLigOnly (str or None, optional): 'NaCl', 'KCl', 'CaCl2' or None.
                                                        neutralize the lig-only system using the salt.
                                                        Defaluts to NaCl.
             pinDownPro (bool, optional): whether pinning down the protien. Defaults to True.
             useOldCv (bool, optional): whether used old, custom-function-based cv. Defaults to True.
             vmdPath (str, optional): path to vmd. Defaults to ''.
             OPLSMixingRule (bool, optional): whether use the OPLS mixing rules. Defaults to False.
+            considerRMSDCV (bool, optional): Whether consider the RMSD CV. Default to True.
         """
 
         assert(len(stratification) == 4)
         assert(forceFieldType == 'charmm' or forceFieldType == 'amber')
 
         # determine the type of input top and coor file
         topType, coorType = self._determineFileType(topFile, coorFile)
 
-        self._makeDirectories(path, 'alchemical')
+        self._makeDirectories(path, 'alchemical', considerRMSDCV=considerRMSDCV)
         # after copying files
         # the coordinate file is converted to pdb
         self._copyFiles(
             path, topFile, topType, coorFile, coorType, forceFieldType, forceFieldFiles,
             selectionPro, selectionLig, selectionPro, '', '',
             'alchemical', membraneProtein, neutralizeLigOnly, vmdPath)
 
@@ -108,18 +110,19 @@
         relativeFFPath = []
         for item in forceFieldFiles:
             _, name = os.path.split(item)
             relativeFFPath.append(f'../{name}')
         
         self._generateAlchemicalNAMDConfig(
             path, forceFieldType, relativeFFPath, temperature, stratification, doubleWide, minBeforeSample,
-            membraneProtein, OPLSMixingRule=OPLSMixingRule
+            membraneProtein, OPLSMixingRule=OPLSMixingRule, considerRMSDCV=considerRMSDCV
         )
         self._generateAlchemicalColvarsConfig(
-            path, topType, 'pdb', selectionPro, selectionLig, selectionPro, stratification, pinDownPro, useOldCv
+            path, topType, 'pdb', selectionPro, selectionLig, selectionPro, stratification, pinDownPro, useOldCv,
+            considerRMSDCV=considerRMSDCV
         )
 
     def generateNAMDGeometricFiles(
         self,
         path,
         topFile,
         coorFile,
@@ -171,15 +174,15 @@
             pinDownPro (bool, optional): whether pinning down the protien. Defaults to True.
             useOldCv (bool, optional): whether used old, custom-function-based cv. Defaults to True.
             parallelRuns (int, optional): generate files for duplicate runs. Defaults to 1.
             vmdPath (str, optional): path to vmd. Defaults to ''.
             reflectingBoundary (bool, optional): Whether use reflecting boundaries, requires setBoundary on. Default to False.
             MDEngine (str, optional): namd or gromacs. Default to namd.
             OPLSMixingRule (bool, optional): whether use the OPLS mixing rules. Defaults to False.
-            considerRMSDCV (bool, optional): Whethre consider the RMSD CV. Default to True.
+            considerRMSDCV (bool, optional): Whether consider the RMSD CV. Default to True.
             GaWTM (bool, optional): Whether performing GaWTM-eABF simulations. Default to False
         """ 
 
         assert(len(stratification) == 8)
         assert(forceFieldType == 'charmm' or forceFieldType == 'amber')
 
         if selectionRef == '':
@@ -237,15 +240,15 @@
         pdbFile, 
         pdbFileFormat,
         ligandOnlyTopFile, 
         ligandOnlyPdbFile,
         ligandOnlyPdbFileFormat,
         selectionPro,
         selectionLig,
-        selectionSol='resname TIP3* or resname SPC* or resname HOH or resname WAT',
+        selectionSol='resname TIP3* or resname SPC* or resname HOH or resname WAT or resname SOL',
         temperature=300.0
     ):
         """generate all the input files for Gromacs Geometric simulation
            This function is based on BFEEGromacs.py
            contributed by Haochuan Chen (yjcoshc_at_mail.nankai.edu.cn)
            
         Args:
@@ -374,22 +377,25 @@
             os.mkdir(f'{path}/BFEE/004_EulerPsi/output')
             os.mkdir(f'{path}/BFEE/005_PolarTheta/output')
             os.mkdir(f'{path}/BFEE/006_PolarPhi/output')
             os.mkdir(f'{path}/BFEE/007_r/output')
             
 
         if jobType == 'alchemical':
+            if considerRMSDCV:
+                os.mkdir(f'{path}/BFEE/004_RestraintUnbound')
+                os.mkdir(f'{path}/BFEE/004_RestraintUnbound/output')
+
             os.mkdir(f'{path}/BFEE/001_MoleculeBound')
             os.mkdir(f'{path}/BFEE/002_RestraintBound')
             os.mkdir(f'{path}/BFEE/003_MoleculeUnbound')
-            os.mkdir(f'{path}/BFEE/004_RestraintUnbound')
             os.mkdir(f'{path}/BFEE/001_MoleculeBound/output')
             os.mkdir(f'{path}/BFEE/002_RestraintBound/output')
             os.mkdir(f'{path}/BFEE/003_MoleculeUnbound/output')
-            os.mkdir(f'{path}/BFEE/004_RestraintUnbound/output')
+            
 
 
     def _copyFiles(
         self, 
         path, 
         topFile, 
         topType, 
@@ -833,15 +839,16 @@
         forceFieldType,
         forceFields,
         temperature,
         stratification = [1,1,1,1],
         doubleWide = False,
         minBeforeSample = False,
         membraneProtein = False,
-        OPLSMixingRule = False
+        OPLSMixingRule = False,
+        considerRMSDCV = True
     ):
         """generate NAMD config fils for the alchemical route
 
         Args:
             path (str): the directory for generation of all the files
             forceFieldType (str): 'charmm' or 'amber'
             forceFields (list of str): list of CHARMM force field files
@@ -851,14 +858,15 @@
             doubleWide (bool, optional): whether double-wide simulations are carried out. 
                                          Defaults to False.
             minBeforeSample (bool, optional): minimization before sampling in each FEP window. 
                                               Defaults to False.
             membraneProtein (bool, optional): whether simulating a membrane protein. 
                                               Defaults to False.
             OPLSMixingRule (bool, optional): whether use the OPLS mixing rules. Defaults to False.
+            considerRMSDCV (bool, optional): Whethre consider the RMSD CV. Default to True.
         """
 
         if forceFieldType == 'charmm':
             topType = 'psf'
         elif forceFieldType == 'amber':
             topType = 'parm7'
         coorType = 'pdb'
@@ -946,88 +954,95 @@
                 self.cTemplate.namdConfigTemplate(
                     forceFieldType, forceFields, f'../complex.{topType}', f'../complex.pdb',
                     f'../000_eq/output/eq.coor', f'../000_eq/output/eq.vel', f'../000_eq/output/eq.xsc', '',
                     'output/ti_backward', temperature, f'{500000*(stratification[1]+1)}', 'colvars_backward.in', 
                     '', membraneProtein=membraneProtein, OPLSMixingRule=OPLSMixingRule
                 )
             )
-
+            
         # 003_MoleculeUnbound
+        if considerRMSDCV:
+            step3ColvarsConfig = 'colvars.in'
+        else:
+            step3ColvarsConfig = ''
         with open(f'{path}/BFEE/003_MoleculeUnbound/003.2_fep_forward.conf', 'w') as namdConfig:
             namdConfig.write(
                 self.cTemplate.namdConfigTemplate(
                     forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
                     f'output/fep_backward.coor', f'output/fep_backward.vel', 
                     f'output/fep_backward.xsc', '',
-                    'output/fep_forward', temperature, 0, 'colvars.in', '', '', '../fep_ligandOnly.pdb', 
+                    'output/fep_forward', temperature, 0, step3ColvarsConfig, '', '', '../fep_ligandOnly.pdb', 
                     stratification[2], True, False, minBeforeSample, OPLSMixingRule=OPLSMixingRule
                 )
             )
         with open(f'{path}/BFEE/003_MoleculeUnbound/003.1_fep_backward.conf', 'w') as namdConfig:
             namdConfig.write(
                 self.cTemplate.namdConfigTemplate(
                     forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
                     f'../000_eq/output/eq_ligandOnly.coor', f'../000_eq/output/eq_ligandOnly.vel', 
                     f'../000_eq/output/eq_ligandOnly.xsc', '',
-                    'output/fep_backward', temperature, 0, 'colvars.in', '', '', '../fep_ligandOnly.pdb', 
+                    'output/fep_backward', temperature, 0, step3ColvarsConfig, '', '', '../fep_ligandOnly.pdb', 
                     stratification[2], False, False, minBeforeSample, OPLSMixingRule=OPLSMixingRule
                 )
             )
 
         if doubleWide:
             with open(f'{path}/BFEE/003_MoleculeUnbound/003_fep_doubleWide.conf', 'w') as namdConfig:
                 namdConfig.write(
                     self.cTemplate.namdConfigTemplate(
                         forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
                         f'../000_eq/output/eq_ligandOnly.coor', f'../000_eq/output/eq_ligandOnly.vel', 
                         f'../000_eq/output/eq_ligandOnly.xsc', '',
-                        'output/fep_doubleWide', temperature, 0, 'colvars.in', '', '', '../fep_ligandOnly.pdb', 
+                        'output/fep_doubleWide', temperature, 0, step3ColvarsConfig, '', '', '../fep_ligandOnly.pdb', 
                         stratification[2], False, True, OPLSMixingRule=OPLSMixingRule
                     )
                 )
 
-        # 004_RestraintUnbound
-        with open(f'{path}/BFEE/004_RestraintUnbound/004.2_ti_forward.conf', 'w') as namdConfig:
-            namdConfig.write(
-                self.cTemplate.namdConfigTemplate(
-                    forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
-                    f'output/ti_backward.coor', f'output/ti_backward.vel', 
-                    f'output/ti_backward.xsc', '',
-                    'output/ti_forward', temperature, f'{500000*(stratification[3]+1)}', 'colvars_forward.in', 
-                    '', OPLSMixingRule=OPLSMixingRule
+
+        if considerRMSDCV:
+            # 004_RestraintUnbound
+            with open(f'{path}/BFEE/004_RestraintUnbound/004.2_ti_forward.conf', 'w') as namdConfig:
+                namdConfig.write(
+                    self.cTemplate.namdConfigTemplate(
+                        forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
+                        f'output/ti_backward.coor', f'output/ti_backward.vel', 
+                        f'output/ti_backward.xsc', '',
+                        'output/ti_forward', temperature, f'{500000*(stratification[3]+1)}', 'colvars_forward.in', 
+                        '', OPLSMixingRule=OPLSMixingRule
+                    )
                 )
-            )
-        with open(f'{path}/BFEE/004_RestraintUnbound/004.1_ti_backward.conf', 'w') as namdConfig:
-            namdConfig.write(
-                self.cTemplate.namdConfigTemplate(
-                    forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
-                    f'../000_eq/output/eq_ligandOnly.coor', f'../000_eq/output/eq_ligandOnly.vel', 
-                    f'../000_eq/output/eq_ligandOnly.xsc', '',
-                    'output/ti_backward', temperature, f'{500000*(stratification[3]+1)}', 'colvars_backward.in', 
-                    '', OPLSMixingRule=OPLSMixingRule
+            with open(f'{path}/BFEE/004_RestraintUnbound/004.1_ti_backward.conf', 'w') as namdConfig:
+                namdConfig.write(
+                    self.cTemplate.namdConfigTemplate(
+                        forceFieldType, forceFields, f'../ligandOnly.{topType}', f'../ligandOnly.pdb',
+                        f'../000_eq/output/eq_ligandOnly.coor', f'../000_eq/output/eq_ligandOnly.vel', 
+                        f'../000_eq/output/eq_ligandOnly.xsc', '',
+                        'output/ti_backward', temperature, f'{500000*(stratification[3]+1)}', 'colvars_backward.in', 
+                        '', OPLSMixingRule=OPLSMixingRule
+                    )
                 )
-            )
 
     def _generateAlchemicalColvarsConfig(
         self, path, topType, coorType, selectionPro, selectionLig, selectionRef, 
-        stratification=[1,1,1,1], pinDownPro=True, useOldCv=True
+        stratification=[1,1,1,1], pinDownPro=True, useOldCv=True, considerRMSDCV=True
     ):
         """generate Colvars config fils for geometric route
 
         Args:
             path (str): the directory for generation of all the files
             topType (str): the type (psf, parm) of the topology file
             coorType (str): the type (pdb, rst) of the topology file
             selectionPro (str): MDAnalysis-style selection of the protein
             selectionLig (str): MDAnalysis-style selection of the ligand
             selectionRef (str): MDAnalysis-style selection of the reference group for pulling simulation
             stratification (list of int, 4, optional): number of windows for each simulation. 
                                                        Defaults to [1,1,1,1].
             pinDownPro (bool, optinal): Whether pinning down the protein. Defaults to True.
             useOldCv (bool, optional): whether used old, custom-function-based cv. Defaults to True.
+            considerRMSDCV (bool, optional): Whethre consider the RMSD CV. Default to True.
         """
 
         assert(len(stratification) == 4)
 
         # read the original topology and coordinate file
         fParser = fileParser.fileParser(f'{path}/BFEE/complex.{topType}', f'{path}/BFEE/complex.{coorType}')
         center = fParser.measureCenter(selectionPro)
@@ -1112,29 +1127,31 @@
             )
             colvarsConfig.write(
                 self.cTemplate.cvRMSDTemplate(
                     False, '', '', '../ligandOnly.xyz',
                     extendedLagrangian = False
                 )
             )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
-            )
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
+                )
 
         # 001_MoleculeBound
         with open(f'{path}/BFEE/001_MoleculeBound/colvars.in', 'w') as colvarsConfig:
             colvarsConfig.write(
                 self.cTemplate.cvHeadTemplate('../complex.ndx')
             )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../complex.xyz',
-                    extendedLagrangian = False
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../complex.xyz',
+                        extendedLagrangian = False
+                    )
                 )
-            )
             colvarsConfig.write(
                 self.cTemplate.cvAngleTemplate(
                     False, 0, 0, 'eulerTheta', '../complex.xyz', useOldCv,
                     extendedLagrangian = False
                 )
             )
             colvarsConfig.write(
@@ -1162,17 +1179,18 @@
                 )
             )
             colvarsConfig.write(
                 self.cTemplate.cvRTemplate(
                     False, 0, 0, extendedLagrangian = False
                 )
             )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
-            )
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
+                )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerTheta', 0.1, 0)
             )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerPhi', 0.1, 0)
             )
             colvarsConfig.write(
@@ -1193,20 +1211,21 @@
                 )
 
         # 002_RestraintBound
         with open(f'{path}/BFEE/002_RestraintBound/colvars_forward.in', 'w') as colvarsConfig:
             colvarsConfig.write(
                 self.cTemplate.cvHeadTemplate('../complex.ndx')
             )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../complex.xyz',
-                    extendedLagrangian = False
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../complex.xyz',
+                        extendedLagrangian = False
+                    )
                 )
-            )
             colvarsConfig.write(
                 self.cTemplate.cvAngleTemplate(
                     False, 0, 0, 'eulerTheta', '../complex.xyz', useOldCv,
                     extendedLagrangian = False
                 )
             )
             colvarsConfig.write(
@@ -1234,17 +1253,18 @@
                 )
             )
             colvarsConfig.write(
                 self.cTemplate.cvRTemplate(
                     False, 0, 0, extendedLagrangian = False
                 )
             )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[1], True, 10)
-            )
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[1], True, 10)
+                )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerTheta', 0, 0, stratification[1], True, 0.1)
             )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerPhi', 0, 0, stratification[1], True, 0.1)
             )
             colvarsConfig.write(
@@ -1263,19 +1283,20 @@
                 colvarsConfig.write(
                     self.cTemplate.cvProteinTemplate(center, '../complex.xyz')
                 )
         with open(f'{path}/BFEE/002_RestraintBound/colvars_backward.in', 'w') as colvarsConfig:
             colvarsConfig.write(
                 self.cTemplate.cvHeadTemplate('../complex.ndx')
             )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../complex.xyz', extendedLagrangian = False
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../complex.xyz', extendedLagrangian = False
+                    )
                 )
-            )
             colvarsConfig.write(
                 self.cTemplate.cvAngleTemplate(
                     False, 0, 0, 'eulerTheta', '../complex.xyz', useOldCv,
                     extendedLagrangian = False
                 )
             )
             colvarsConfig.write(
@@ -1303,17 +1324,18 @@
                 )
             )
             colvarsConfig.write(
                 self.cTemplate.cvRTemplate(
                     False, 0, 0, extendedLagrangian = False
                 )
             )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[1], False, 10)
-            )
+            if considerRMSDCV:
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[1], False, 10)
+                )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerTheta', 0, 0, stratification[1], False, 0.1)
             )
             colvarsConfig.write(
                 self.cTemplate.cvHarmonicTemplate('eulerPhi', 0, 0, stratification[1], False, 0.1)
             )
             colvarsConfig.write(
@@ -1329,56 +1351,57 @@
                 self.cTemplate.cvHarmonicTemplate('r', 0, distance, stratification[1], False, 10)
             )
             if pinDownPro:
                 colvarsConfig.write(
                     self.cTemplate.cvProteinTemplate(center, '../complex.xyz')
                 )
 
-        # 003_MoleculeUnbound
-        with open(f'{path}/BFEE/003_MoleculeUnbound/colvars.in', 'w') as colvarsConfig:
-            colvarsConfig.write(
-                self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../ligandOnly.xyz',
-                    extendedLagrangian = False
+        if considerRMSDCV:
+            # 003_MoleculeUnbound
+            with open(f'{path}/BFEE/003_MoleculeUnbound/colvars.in', 'w') as colvarsConfig:
+                colvarsConfig.write(
+                    self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
+                )
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../ligandOnly.xyz',
+                        extendedLagrangian = False
+                    )
+                )
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
                 )
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 10, 0)
-            )
 
-        # 004_RestraintUnbound
-        with open(f'{path}/BFEE/004_RestraintUnbound/colvars_forward.in', 'w') as colvarsConfig:
-            colvarsConfig.write(
-                self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../ligandOnly.xyz',
-                    extendedLagrangian = False
+            # 004_RestraintUnbound
+            with open(f'{path}/BFEE/004_RestraintUnbound/colvars_forward.in', 'w') as colvarsConfig:
+                colvarsConfig.write(
+                    self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
                 )
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[3], True, 10)
-            )
-        with open(f'{path}/BFEE/004_RestraintUnbound/colvars_backward.in', 'w') as colvarsConfig:
-            colvarsConfig.write(
-                self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvRMSDTemplate(
-                    False, '', '', '../ligandOnly.xyz',
-                    extendedLagrangian = False
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../ligandOnly.xyz',
+                        extendedLagrangian = False
+                    )
+                )
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[3], True, 10)
+                )
+            with open(f'{path}/BFEE/004_RestraintUnbound/colvars_backward.in', 'w') as colvarsConfig:
+                colvarsConfig.write(
+                    self.cTemplate.cvHeadTemplate('../ligandOnly.ndx')
+                )
+                colvarsConfig.write(
+                    self.cTemplate.cvRMSDTemplate(
+                        False, '', '', '../ligandOnly.xyz',
+                        extendedLagrangian = False
+                    )
+                )
+                colvarsConfig.write(
+                    self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[3], False, 10)
                 )
-            )
-            colvarsConfig.write(
-                self.cTemplate.cvHarmonicTemplate('RMSD', 0, 0, stratification[3], False, 10)
-            )
 
     def _generateGeometricNAMDConfig(
         self,
         path,
         forceFieldType,
         forceFields,
         temperature,
```

### Comparing `BFEE2-2.3.2/BFEE2/postTreatment.py` & `BFEE2-2.4.0/BFEE2/postTreatment.py`

 * *Files 3% similar despite different names*

```diff
@@ -327,44 +327,50 @@
         if Lambda[0] > Lambda[1]:
             Lambda.reverse()
             dA_dLambda.reverse()
                 
         return np.array((Lambda, np.cumsum(dA_dLambda)))
 
         
-    def _tiLogFile(self, filePath):
+    def _tiLogFile(self, filePath, rigidLigand = False):
         """parse a ti log file and return the lambda-free energy relationship
 
         Args:
             filePath (str): path of the fepout file
+            rigidLigand (bool): whether dealing with a rigid ligand. Default to False.
         
         Returns:
             tuple (2D np.array): lambda-free energy relationship
         """
         
         Lambda = []
         dA_dLambda = []
 
+        if rigidLigand:
+            numCVs = 6
+        else:
+            numCVs = 7
+
         with open(filePath, 'r', encoding='utf-8') as fepoutFile:
             for line in fepoutFile.readlines():
                 if not ('dA/dLambda' in line):
                     continue
                 splitedLine = line.strip().split()
                 Lambda.append(float(splitedLine[4]))
                 dA_dLambda.append(float(splitedLine[6]))
                 
         # seven CVs in total with the same Lambda in the step 2
         if Lambda[0] == Lambda[1]:
             correctedLambda = []
             correctedDA_dLambda = []
             
-            for i in range(0, len(Lambda), 7):
+            for i in range(0, len(Lambda), numCVs):
                 correctedLambda.append(Lambda[i])
                 totalDA_dLambda = 0
-                for j in range(7):
+                for j in range(numCVs):
                     totalDA_dLambda += dA_dLambda[i+j]
                 correctedDA_dLambda.append(totalDA_dLambda)
             
             Lambda = correctedLambda
             dA_dLambda = correctedDA_dLambda
         
         if Lambda[0] > Lambda[1]:
@@ -372,30 +378,31 @@
             dA_dLambda.reverse()
 
         for i in range(1, len(Lambda)):
             dA_dLambda[i] = (Lambda[i] - Lambda[i-1]) * dA_dLambda[i]
         
         return np.array((Lambda, np.cumsum(dA_dLambda)))
 
-    def _alchemicalFepoutFile(self, filePath, fileType = 'fepout'):
+    def _alchemicalFepoutFile(self, filePath, fileType = 'fepout', rigidLigand = False):
         """parse a fepout/log file and return the total free energy change
 
         Args:
             filePath (str): path of the fepout file
             fileType (str): 'fepout' (decouping atoms) or 'log' (decoupling restraints). Defaults to 'fepout'.
+            rigidLigand (bool): whether dealing with a rigid ligand. Default to False.
 
         Returns:
             float: free-energy change
         """
         
         if fileType == 'fepout':
             _, freeEnergyProfile = self._fepoutFile(filePath)
 
         if fileType == 'log':
-            _, freeEnergyProfile = self._tiLogFile(filePath)
+            _, freeEnergyProfile = self._tiLogFile(filePath, rigidLigand)
 
         return freeEnergyProfile[-1]
     
     def alchemicalFreeEnergy(self, forwardFilePath, backwardFilePath = '', temperature = 300, jobType = 'fep'):
         """ parse a pair of fepout file, or a single double-wide file using the py_bar library
 
         Args:
@@ -417,44 +424,49 @@
             result = analyzer.FEP_free_energy()
 
         freeEnergy = np.sum(result[1])
         error = np.sqrt(np.sum(np.power(result[2], 2)))
         
         return freeEnergy, error
 
-    def alchemicalBindingFreeEnergy(self, filePathes, parameters, temperature = 300, jobType = 'fep'):
-        """calculate binding free energy for geometric route
+    def alchemicalBindingFreeEnergy(self, filePathes, parameters, temperature = 300, jobType = 'fep', rigidLigand = False):
+        """calculate binding free energy for alchemical route
 
         Args:
             filePathes (list of strings, 8): pathes of alchemical output files
                                              (step1-forward, step1-backward, step2-forward ...)
             parameters (np.array, floats, 9): (eulerTheta, polarTheta, r, forceConstant1, FC2, FC3, FC4, FC5, FC6)
             temperature (float): temperature of the simulation
             jobType (str, optional): Type of the post-treatment method. 'fep' or 'bar'. 
                                       Defaults to 'fep'.
+            rigidLigand (bool): whether dealing with a rigid ligand. Default to False.
 
         Returns:
             tuple:
                 np.array, float, 6: (contributions for step1, 2, 3, 4, bulk restraining contribution, free energy)
                 np.array, float, 6: errors corresponding each contribution
         """
 
         assert len(parameters) == 9
         assert len(filePathes) == 8
 
+        rigid_ligand = False
+        if (filePathes[6] == ''):
+            rigid_ligand = True
+
         # get free energies from fep outputs
         freeEnergies = []
         for i in range(len(filePathes)):
             if filePathes[i] != '':
                 if (i // 2) % 2 == 0:
                     # just a dirty solution
                     freeEnergies.append(None)
                     #freeEnergies.append(self._alchemicalFepoutFile(filePathes[i], 'fepout'))
                 else:
-                    freeEnergies.append(self._alchemicalFepoutFile(filePathes[i], 'log'))
+                    freeEnergies.append(self._alchemicalFepoutFile(filePathes[i], 'log', rigidLigand))
             else:
                 # backward file can be empty
                 freeEnergies.append(None)
 
         contributions = np.zeros(6)
         errors = np.zeros(6)
         
@@ -466,20 +478,24 @@
         else:
             contributions[1] = -freeEnergies[2]
             errors[1] = 99999
             
         contributions[2], errors[2] = self.alchemicalFreeEnergy(filePathes[4], filePathes[5], temperature, jobType)
         contributions[2] = -contributions[2]
 
-        if freeEnergies[7] is not None:
-            contributions[3] = (freeEnergies[6] + freeEnergies[7]) / 2
-            errors[3] = abs((freeEnergies[6] - freeEnergies[7]) / 1.414)
+        if not rigid_ligand:
+            if freeEnergies[7] is not None:
+                contributions[3] = (freeEnergies[6] + freeEnergies[7]) / 2
+                errors[3] = abs((freeEnergies[6] - freeEnergies[7]) / 1.414)
+            else:
+                contributions[3] = freeEnergies[6]
+                errors[3] = 99999
         else:
-            contributions[3] = freeEnergies[6]
-            errors[3] = 99999
+            contributions[3] = 0
+            errors[3] = 0
 
         contributions[4] = self._alchemicalRestraintContributionBulk(*parameters)
         errors[4] = 0
 
         contributions[5] = contributions[0] + contributions[1] + contributions[2] + contributions[3] + contributions[4]
         errors[5] = math.sqrt(errors[0]**2 + errors[1]**2 +errors[2]**2 + errors[3]**2 + errors[4]**2)
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/000.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/000.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/000.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/000.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/000.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/000.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/001.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/001.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/001.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/001.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/001.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/001.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/002.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/002.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/002.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/002.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/002.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/002.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/003.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/003.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/003.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/003.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/003.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/003.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/004.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/004.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/004.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/004.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/004.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/004.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/005.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/005.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/005.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/005.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/005.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/005.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/006.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/006.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/006.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/006.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/006.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/006.mdp.template`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
 ;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/008.mdp.template`

 * *Files 10% similar despite different names*

```diff
@@ -41,29 +41,30 @@
 rvdw                = 1.2
 rvdw-switch         = 1.0
 DispCorr            = no
 
 ;Bonds (for minimization)
 constraint-algorithm    = LINCS
 constraints             = h-bonds
-continuation            = no
+continuation            = yes
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
-pcoupl              = berendsen
+;Pressure coupling
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
 tcoupl              = v-rescale
 tc-grps             = System
 tau_t               = 0.1
 ref_t               = $temperature
 
 ;Velocity generation
-gen-vel             = yes
+gen-vel             = no
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007_eq.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/007_min.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007_min.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/008.colvars.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/008.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/008.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/008.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/008.mdp.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/007.mdp.template`

 * *Files 17% similar despite different names*

```diff
@@ -41,30 +41,29 @@
 rvdw                = 1.2
 rvdw-switch         = 1.0
 DispCorr            = no
 
 ;Bonds (for minimization)
 constraint-algorithm    = LINCS
 constraints             = h-bonds
-continuation            = yes
+continuation            = no
 morse                   = no
 
 ;Implicit solvent
 implicit-solvent    = no
 
 ;Pressure coupling
-;Pressure coupling
-pcoupl              = berendsen
+pcoupl              = C-rescale
 pcoupltype          = Isotropic
 nstpcouple          = -1
 tau-p               = 2
 compressibility     = 4.5e-5
 ref-p               = $pressure
 
 ;Temperature coupling
 tcoupl              = v-rescale
 tc-grps             = System
 tau_t               = 0.1
 ref_t               = $temperature
 
 ;Velocity generation
-gen-vel             = no
+gen-vel             = yes
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template` & `BFEE2-2.4.0/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_gromacs/BFEEGromacs.py` & `BFEE2-2.4.0/BFEE2/templates_gromacs/BFEEGromacs.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_namd/configTemplate.py` & `BFEE2-2.4.0/BFEE2/templates_namd/configTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,16 @@
         if cvFile != '':
             configString += f'\
 colvars    on                                   \n'
             if not GaWTM:
                 configString += f'\
 colvarsConfig    {cvFile}                       \n'
 
-            if CVRestartFile != '':
-                configString += f'\
+                if CVRestartFile != '':
+                    configString += f'\
 colvarsInput     {CVRestartFile}                \n'
 
 
         if cvDefinitionFile != '':
             configString += f'\
 source     {cvDefinitionFile}                   \n'
 
@@ -207,33 +207,48 @@
             if not GaWTM:
                 configString += f'\
 run    {numSteps}                               \n'
             else:
                 configString += f'\
 accelMD                         on                     \n\
 accelMDG                        on                     \n\
+accelMDdihe                     on                     \n\
+accelMDOutFreq                  1000                   \n\
+accelMDGSigma0D                 6.0                    \n'
+                if CVRestartFile == '':
+                     # new GaMD-WTM-eABF simulation
+                     configString += f'\
 accelMDGcMDSteps                500000                 \n\
 accelMDGcMDPrepSteps            100000                 \n\
 accelMDGEquiPrepSteps           100000                 \n\
 accelMDGEquiSteps               500000                 \n\
-accelMDdihe                     on                     \n\
-accelMDOutFreq                  1000                   \n\
-accelMDGSigma0D                 6.0                    \n\
 for {{set stage 0}} {{$stage < 2}} {{incr stage}} {{   \n\
     if {{$stage == 0}} {{                              \n\
         puts "Probing the GaMD parameters..."          \n\
         cv configfile {cvFile}                         \n\
         run norepeat 1000000                           \n\
     }} elseif {{$stage == 1}} {{                       \n\
         puts "Starting eABF + GaMD..."                 \n\
         cv reset                                       \n\
         cv configfile {cvFile + ".amd"}                \n\
         run norepeat   {numSteps}                      \n\
     }}                                                 \n\
 }}                                                     \n'
+                else:
+                     configString += f'\
+accelMDGcMDSteps                0                      \n\
+accelMDGcMDPrepSteps            0                      \n\
+accelMDGEquiPrepSteps           0                      \n\
+accelMDGEquiSteps               0                      \n\
+accelMDGRestart                 on                     \n\
+accelMDGRestartFile             {CVRestartFile}.gamd   \n\
+colvarsConfig                   {cvFile + ".amd"}      \n\
+colvarsInput                    {CVRestartFile}        \n\
+run norepeat   {numSteps}                              \n'
+
         else:
             # currently the alchemical route is somewhat hard-coded
             # this will be improved in the future
             configString += f'\
 source ../fep.tcl                                  \n\
 alch on                                         \n\
 alchType FEP                                    \n\
@@ -846,17 +861,17 @@
             str: head of colvars file
         """
         
         string = f'\
 colvarsTrajFrequency      5000             \n\
 colvarsRestartFrequency   5000            \n\
 indexFile                 {indexFile}      \n'
-        if reweightAMD:
-            string += f'\
-smp                       off              \n'
+#        if reweightAMD:
+#            string += f'\
+#smp                       off              \n'
         return string
 
     def cvHarmonicWallsTemplate(self, cv, lowerWall, upperWall, unit = 'namd'):
         ''' template of harmonic wall bias
         
         Args:
             cv (str): name of the colvars
```

### Comparing `BFEE2-2.3.2/BFEE2/templates_namd/fep.tcl` & `BFEE2-2.4.0/BFEE2/templates_namd/fep.tcl`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_namd/scriptTemplate.py` & `BFEE2-2.4.0/BFEE2/templates_namd/scriptTemplate.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_namd/updateCenters.py` & `BFEE2-2.4.0/BFEE2/templates_namd/updateCenters.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt` & `BFEE2-2.4.0/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt` & `BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt` & `BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/BFEE2/third_party/py_bar.py` & `BFEE2-2.4.0/BFEE2/third_party/py_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,14 @@
         Returns:
             Tuple[List[Tuple[float, float]], List[Tuple[NDArray, NDArray]]]: recording the boundary and 
                                                                              deltaU of each window of
                                                                              bidirectional simulations 
         """
         
         return self._windows, self._deltaU_data
-    
-                
 
 class FEPAnalyzer:
     """ Analyze FEP simulations
     """
     
     def __init__(
         self, 
@@ -233,15 +231,15 @@
             errors.append((forward_free_energy + backward_free_energy) / np.sqrt(2))
         return self._windows, free_energies, errors
     
     def BAR_free_energy(
         self, 
         tolerance: float = 1e-6,
         block_size: int = 20,
-        n_bootstrap: int = 20
+        n_bootstrap: int = 20,
     ) -> Tuple[List[Tuple[float, float]], List[NDArray], List[NDArray]]:
         """ Calculate and return the free-energy change using the BAR estimator
         
         Args:
             tolerance (float): tolerance of the SCF. Default to 1e-6.
             block_size (int): the size of the block in block bootstrap. Default to 10.
             n_bootstrap (int): number of bootstrap samples. Default to 20.
@@ -251,14 +249,15 @@
         """
         
         free_energies = []
         errors = []
         for i in range(len(self._windows)):
             dA = self._BAR_estimator(self._deltaU_data[i], tolerance)
             err = self._BAR_error_estimator(self._deltaU_data[i], tolerance, block_size, n_bootstrap)
+            
             free_energies.append(dA)
             errors.append(err)
         return self._windows, free_energies, errors
     
     def _BAR_estimator(self, deltaU: Tuple[NDArray, NDArray], tolerance: float = 1e-6) -> float:
         """ Estimate the free energy of a window using the BAR estimator
 
@@ -310,27 +309,25 @@
         forward_size = len(deltaU[0])
         backward_size = len(deltaU[1])
         bootstrap_samples = int(np.max((forward_size, backward_size)) / block_size)
         
         if bootstrap_samples < 1:
             raise RuntimeError('Error! block_size larger than sample size!')
         
-        # bootstrap
-        estimates = []
+        # block bootstrap
+        estimates = np.zeros(n_bootstrap)
+
         for i in range(n_bootstrap):
-            forward_bootstrap = []
-            for j in np.random.randint(0, forward_size - block_size - 1, bootstrap_samples):
-                for k in range(block_size):
-                    forward_bootstrap.append(j + k)
+            forward_bootstrap = np.zeros(bootstrap_samples * block_size, dtype=int)
+            for idx, j in enumerate(np.random.randint(0, forward_size - block_size - 1, bootstrap_samples)):
+                forward_bootstrap[idx*block_size:idx*block_size+block_size] = j + np.arange(block_size)
                     
-            backward_bootstrap = []
-            for j in np.random.randint(0, backward_size - block_size - 1, bootstrap_samples):
-                for k in range(block_size):
-                    backward_bootstrap.append(j + k)
+            backward_bootstrap = np.zeros(bootstrap_samples * block_size, dtype=int)
+            for idx, j in enumerate(np.random.randint(0, backward_size - block_size - 1, bootstrap_samples)):
+                backward_bootstrap[idx*block_size:idx*block_size+block_size] = j + np.arange(block_size)
             
-            estimates.append(
-                self._BAR_estimator(
-                    (deltaU[0][forward_bootstrap], deltaU[1][backward_bootstrap]),
-                    tolerance
-                )
-            )
+            estimates[i] = self._BAR_estimator(
+                            (deltaU[0][forward_bootstrap], deltaU[1][backward_bootstrap]),
+                            tolerance
+                        )
+
         return np.std(estimates)
```

### Comparing `BFEE2-2.3.2/BFEE2.egg-info/PKG-INFO` & `BFEE2-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,52 @@
-Metadata-Version: 2.1
-Name: BFEE2
-Version: 2.3.2
-Summary: Binding Free Energy Estimator 2
-Home-page: https://github.com/fhh2626/BFEE2
-Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
-Author-email: wscai@nankai.edu.cn
-Maintainer: Haohao Fu
-Maintainer-email: fhh2626@mail.nankai.edu.cn
-License: GPLv3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Binding Free Energy Estimator 2
-[![DOI](https://zenodo.org/badge/322234705.svg)](https://zenodo.org/badge/latestdoi/322234705)
-
-Binding free energy estimator (BFEE) is a python-based software that automates absolute binding free energy calculations through either the alchemical or geometric route by molecular dynamics simulations.<br>
-
-## Theoretical backgrounds
-The degrees of freedom of the protein-ligand (or host-guest) system are described by a series of geometric variables (or collective variables), as firstly described by the [Karplus group](https://pubs.acs.org/doi/abs/10.1021/jp0217839). In BFEE, a generalized, best-fit-rotation-based geometric variables are used, making it in principle available to any protein-ligand complex. See [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791) for introduction of these variables.<br>
-
-In the [geometric route](https://pubs.acs.org/doi/10.1021/ct3008099), the degrees of freedom is investigated one by one, through one-dimensional free-energy calculations. In BFEE, [WTM-eABF](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) is used, while other importance-sampling algorithms such as [plain eABF](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.6b00447) are also acceptable.
-The [alchemical route](https://pubs.acs.org/doi/10.1021/ct3008099) is a variants of the [double decoupling method (DDM)](https://www.sciencedirect.com/science/article/pii/S0006349597787563). A thermodynamic cycle, in which the ligand and the geometric restraints are decoupled independently to guarantee the convergence of the simulations.<br>
-[这里](http://sioc-journal.cn/Jwk_hxxb/CN/10.6023/A20100489)是标准结合自由能计算方法的中文介绍.<br>
-
-## Features
-Generates all the input files for absolute binding free energy calculations;<br>
-Perform post-treatment automatedly;<br>
-Support NAMD (alchemical and geometric route) and Gromacs (geometric route) as molecular dynamics engines;<br>
-Support many file formats for the input complex structure (PSF/PDB/PRM, PRM7/RST7, TOP/PDB);<br>
-...<br>
-
-## Requirements
-Python 3.6+, PySide 2, numpy, scipy, matplotlib, parmed and MDAnalysis.<br>
-[NAMD 3.0 or later](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=NAMD) / [Colvars patched Gromacs](https://github.com/Colvars/colvars).<br>
-**Note: BFEE2 uses cutting-edge features of NAMD and Colvars. We highly suggest the end-user download the devel branch of NAMD from [here](https://gitlab.com/tcbgUIUC/namd/-/tree/devel) and patch it with [Colvars](https://github.com/Colvars/colvars) to prevent possible problems.**
-
-## Installation
-We suggest to install BFEE2 through conda. It will be safe if conda is install in a new environment<br>
-```
-conda create --name bfee   (optional)
-conda activate bfee        (optional)
-conda install -c conda-forge BFEE2
-```
-
-## Usage
-Simply run BFEE2Gui.py in terminal or PowerShell. One may need to use the absolute path on MS Windows.<br>
-A step-by-step tutorial is provided [here](https://www.nature.com/articles/s41596-021-00676-1).<br>
-
-## Citations
-When possible, please consider mentioning [Fu et al. Nat. Protoc. 2022, doi:10.1038/s41596-021-00676-1](https://www.nature.com/articles/s41596-021-00676-1#citeas) when BFEE2 is used in your project.
-
-
-Additional references:<br>
-BFEE2: [Fu et al. J. Chem. Inf. Model. 2021, 61, 2116–2123](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c00269)<br>
-Alchemical and geometric routes [Gumbart et al. J. Chem. Theory Comput. 2013, 9, 794–802](https://pubs.acs.org/doi/abs/10.1021/ct3008099)<br>
-WTM-eABF: [Fu et al. Acc. Chem. Res. 2019, 52, 3254–3264](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) and [Fu et al. J. Phys. Chem. Lett. 2018, 9, 4738–4745](https://pubs.acs.org/doi/abs/10.1021/acs.jpclett.8b01994)<br>
-Collective variables: [Fu et al. J. Chem. Theory Comput. 2017, 13, 5173–5178](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791)<br>
-Colvars module: [Fiorin et al. Mol. Phys. 2013 111, 3345-3362](https://www.tandfonline.com/doi/full/10.1080/00268976.2013.813594)<br>
-"Mother" of all restraint-based binding free-energy calculations: [Hermans et al. Isr. J. Chem. 1986, 27, 225–227](https://onlinelibrary.wiley.com/doi/abs/10.1002/ijch.198600032)<br>
-
-## Contact us
-Technique issues: Haohao Fu (fhh2626@mail.nankai.edu.cn) and Haochuan Chen (yjcoshc@mail.nankai.edu.cn)<br>
-
-This software is under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) license. For more information about the copyright of BFEE, contact the corresponding authors of the aforementioned papers (wscai@nankai.edu.cn, Christophe.Chipot@univ-lorraine.fr).
+# Binding Free Energy Estimator 2
+[![DOI](https://zenodo.org/badge/322234705.svg)](https://zenodo.org/badge/latestdoi/322234705)
+
+Binding free energy estimator (BFEE) is a python-based software that automates absolute binding free energy calculations through either the alchemical or geometric route by molecular dynamics simulations.<br>
+
+## Theoretical backgrounds
+The degrees of freedom of the protein-ligand (or host-guest) system are described by a series of geometric variables (or collective variables), as firstly described by the [Karplus group](https://pubs.acs.org/doi/abs/10.1021/jp0217839). In BFEE, a generalized, best-fit-rotation-based geometric variables are used, making it in principle available to any protein-ligand complex. See [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791) for introduction of these variables.<br>
+
+In the [geometric route](https://pubs.acs.org/doi/10.1021/ct3008099), the degrees of freedom is investigated one by one, through one-dimensional free-energy calculations. In BFEE, [WTM-eABF](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) is used, while other importance-sampling algorithms such as [plain eABF](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.6b00447) are also acceptable.
+The [alchemical route](https://pubs.acs.org/doi/10.1021/ct3008099) is a variants of the [double decoupling method (DDM)](https://www.sciencedirect.com/science/article/pii/S0006349597787563). A thermodynamic cycle, in which the ligand and the geometric restraints are decoupled independently to guarantee the convergence of the simulations.<br>
+[这里](http://sioc-journal.cn/Jwk_hxxb/CN/10.6023/A20100489)是标准结合自由能计算方法的中文介绍.<br>
+
+## Features
+Generates all the input files for absolute binding free energy calculations;<br>
+Perform post-treatment automatedly;<br>
+Support NAMD (alchemical and geometric route) and Gromacs (geometric route) as molecular dynamics engines;<br>
+Support many file formats for the input complex structure (PSF/PDB/PRM, PRM7/RST7, TOP/PDB);<br>
+...<br>
+
+## Requirements
+Python 3.6+, PySide 2, numpy, scipy, matplotlib, parmed and MDAnalysis.<br>
+[NAMD 3.0 or later](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=NAMD) / [Colvars patched Gromacs](https://github.com/Colvars/colvars).<br>
+**Note: BFEE2 uses cutting-edge features of NAMD and Colvars. We highly suggest the end-user download the devel branch of NAMD from [here](https://gitlab.com/tcbgUIUC/namd/-/tree/devel) and patch it with [Colvars](https://github.com/Colvars/colvars) to prevent possible problems.**
+
+## Installation
+We suggest to install BFEE2 through conda. It will be safe if conda is install in a new environment<br>
+```
+conda create --name bfee   (optional)
+conda activate bfee        (optional)
+conda install -c conda-forge BFEE2
+```
+
+## Usage
+Simply run BFEE2Gui.py in terminal or PowerShell. One may need to use the absolute path on MS Windows.<br>
+A step-by-step tutorial is provided [here](https://www.nature.com/articles/s41596-021-00676-1).<br>
+
+## Citations
+When possible, please consider mentioning [Fu et al. Nat. Protoc. 2022, doi:10.1038/s41596-021-00676-1](https://www.nature.com/articles/s41596-021-00676-1#citeas) when BFEE2 is used in your project.
+
+
+Additional references:<br>
+BFEE2: [Fu et al. J. Chem. Inf. Model. 2021, 61, 2116–2123](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c00269)<br>
+Alchemical and geometric routes [Gumbart et al. J. Chem. Theory Comput. 2013, 9, 794–802](https://pubs.acs.org/doi/abs/10.1021/ct3008099)<br>
+WTM-eABF: [Fu et al. Acc. Chem. Res. 2019, 52, 3254–3264](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) and [Fu et al. J. Phys. Chem. Lett. 2018, 9, 4738–4745](https://pubs.acs.org/doi/abs/10.1021/acs.jpclett.8b01994)<br>
+Collective variables: [Fu et al. J. Chem. Theory Comput. 2017, 13, 5173–5178](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791)<br>
+Colvars module: [Fiorin et al. Mol. Phys. 2013 111, 3345-3362](https://www.tandfonline.com/doi/full/10.1080/00268976.2013.813594)<br>
+"Mother" of all restraint-based binding free-energy calculations: [Hermans et al. Isr. J. Chem. 1986, 27, 225–227](https://onlinelibrary.wiley.com/doi/abs/10.1002/ijch.198600032)<br>
+
+## Contact us
+Technique issues: Haohao Fu (fhh2626@mail.nankai.edu.cn) and Haochuan Chen (yjcoshc@mail.nankai.edu.cn)<br>
+
+This software is under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) license. For more information about the copyright of BFEE, contact the corresponding authors of the aforementioned papers (wscai@nankai.edu.cn, Christophe.Chipot@univ-lorraine.fr).
```

### Comparing `BFEE2-2.3.2/BFEE2.egg-info/SOURCES.txt` & `BFEE2-2.4.0/BFEE2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/LICENSE` & `BFEE2-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BFEE2-2.3.2/PKG-INFO` & `BFEE2-2.4.0/BFEE2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: BFEE2
-Version: 2.3.2
-Summary: Binding Free Energy Estimator 2
-Home-page: https://github.com/fhh2626/BFEE2
-Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
-Author-email: wscai@nankai.edu.cn
-Maintainer: Haohao Fu
-Maintainer-email: fhh2626@mail.nankai.edu.cn
-License: GPLv3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Binding Free Energy Estimator 2
-[![DOI](https://zenodo.org/badge/322234705.svg)](https://zenodo.org/badge/latestdoi/322234705)
-
-Binding free energy estimator (BFEE) is a python-based software that automates absolute binding free energy calculations through either the alchemical or geometric route by molecular dynamics simulations.<br>
-
-## Theoretical backgrounds
-The degrees of freedom of the protein-ligand (or host-guest) system are described by a series of geometric variables (or collective variables), as firstly described by the [Karplus group](https://pubs.acs.org/doi/abs/10.1021/jp0217839). In BFEE, a generalized, best-fit-rotation-based geometric variables are used, making it in principle available to any protein-ligand complex. See [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791) for introduction of these variables.<br>
-
-In the [geometric route](https://pubs.acs.org/doi/10.1021/ct3008099), the degrees of freedom is investigated one by one, through one-dimensional free-energy calculations. In BFEE, [WTM-eABF](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) is used, while other importance-sampling algorithms such as [plain eABF](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.6b00447) are also acceptable.
-The [alchemical route](https://pubs.acs.org/doi/10.1021/ct3008099) is a variants of the [double decoupling method (DDM)](https://www.sciencedirect.com/science/article/pii/S0006349597787563). A thermodynamic cycle, in which the ligand and the geometric restraints are decoupled independently to guarantee the convergence of the simulations.<br>
-[这里](http://sioc-journal.cn/Jwk_hxxb/CN/10.6023/A20100489)是标准结合自由能计算方法的中文介绍.<br>
-
-## Features
-Generates all the input files for absolute binding free energy calculations;<br>
-Perform post-treatment automatedly;<br>
-Support NAMD (alchemical and geometric route) and Gromacs (geometric route) as molecular dynamics engines;<br>
-Support many file formats for the input complex structure (PSF/PDB/PRM, PRM7/RST7, TOP/PDB);<br>
-...<br>
-
-## Requirements
-Python 3.6+, PySide 2, numpy, scipy, matplotlib, parmed and MDAnalysis.<br>
-[NAMD 3.0 or later](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=NAMD) / [Colvars patched Gromacs](https://github.com/Colvars/colvars).<br>
-**Note: BFEE2 uses cutting-edge features of NAMD and Colvars. We highly suggest the end-user download the devel branch of NAMD from [here](https://gitlab.com/tcbgUIUC/namd/-/tree/devel) and patch it with [Colvars](https://github.com/Colvars/colvars) to prevent possible problems.**
-
-## Installation
-We suggest to install BFEE2 through conda. It will be safe if conda is install in a new environment<br>
-```
-conda create --name bfee   (optional)
-conda activate bfee        (optional)
-conda install -c conda-forge BFEE2
-```
-
-## Usage
-Simply run BFEE2Gui.py in terminal or PowerShell. One may need to use the absolute path on MS Windows.<br>
-A step-by-step tutorial is provided [here](https://www.nature.com/articles/s41596-021-00676-1).<br>
-
-## Citations
-When possible, please consider mentioning [Fu et al. Nat. Protoc. 2022, doi:10.1038/s41596-021-00676-1](https://www.nature.com/articles/s41596-021-00676-1#citeas) when BFEE2 is used in your project.
-
-
-Additional references:<br>
-BFEE2: [Fu et al. J. Chem. Inf. Model. 2021, 61, 2116–2123](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c00269)<br>
-Alchemical and geometric routes [Gumbart et al. J. Chem. Theory Comput. 2013, 9, 794–802](https://pubs.acs.org/doi/abs/10.1021/ct3008099)<br>
-WTM-eABF: [Fu et al. Acc. Chem. Res. 2019, 52, 3254–3264](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) and [Fu et al. J. Phys. Chem. Lett. 2018, 9, 4738–4745](https://pubs.acs.org/doi/abs/10.1021/acs.jpclett.8b01994)<br>
-Collective variables: [Fu et al. J. Chem. Theory Comput. 2017, 13, 5173–5178](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791)<br>
-Colvars module: [Fiorin et al. Mol. Phys. 2013 111, 3345-3362](https://www.tandfonline.com/doi/full/10.1080/00268976.2013.813594)<br>
-"Mother" of all restraint-based binding free-energy calculations: [Hermans et al. Isr. J. Chem. 1986, 27, 225–227](https://onlinelibrary.wiley.com/doi/abs/10.1002/ijch.198600032)<br>
-
-## Contact us
-Technique issues: Haohao Fu (fhh2626@mail.nankai.edu.cn) and Haochuan Chen (yjcoshc@mail.nankai.edu.cn)<br>
-
-This software is under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) license. For more information about the copyright of BFEE, contact the corresponding authors of the aforementioned papers (wscai@nankai.edu.cn, Christophe.Chipot@univ-lorraine.fr).
+Metadata-Version: 2.1
+Name: BFEE2
+Version: 2.4.0
+Summary: Binding Free Energy Estimator 2
+Home-page: https://github.com/fhh2626/BFEE2
+Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
+Author-email: wscai@nankai.edu.cn
+Maintainer: Haohao Fu
+Maintainer-email: fhh2626@mail.nankai.edu.cn
+License: GPLv3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Binding Free Energy Estimator 2
+[![DOI](https://zenodo.org/badge/322234705.svg)](https://zenodo.org/badge/latestdoi/322234705)
+
+Binding free energy estimator (BFEE) is a python-based software that automates absolute binding free energy calculations through either the alchemical or geometric route by molecular dynamics simulations.<br>
+
+## Theoretical backgrounds
+The degrees of freedom of the protein-ligand (or host-guest) system are described by a series of geometric variables (or collective variables), as firstly described by the [Karplus group](https://pubs.acs.org/doi/abs/10.1021/jp0217839). In BFEE, a generalized, best-fit-rotation-based geometric variables are used, making it in principle available to any protein-ligand complex. See [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791) for introduction of these variables.<br>
+
+In the [geometric route](https://pubs.acs.org/doi/10.1021/ct3008099), the degrees of freedom is investigated one by one, through one-dimensional free-energy calculations. In BFEE, [WTM-eABF](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) is used, while other importance-sampling algorithms such as [plain eABF](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.6b00447) are also acceptable.
+The [alchemical route](https://pubs.acs.org/doi/10.1021/ct3008099) is a variants of the [double decoupling method (DDM)](https://www.sciencedirect.com/science/article/pii/S0006349597787563). A thermodynamic cycle, in which the ligand and the geometric restraints are decoupled independently to guarantee the convergence of the simulations.<br>
+[这里](http://sioc-journal.cn/Jwk_hxxb/CN/10.6023/A20100489)是标准结合自由能计算方法的中文介绍.<br>
+
+## Features
+Generates all the input files for absolute binding free energy calculations;<br>
+Perform post-treatment automatedly;<br>
+Support NAMD (alchemical and geometric route) and Gromacs (geometric route) as molecular dynamics engines;<br>
+Support many file formats for the input complex structure (PSF/PDB/PRM, PRM7/RST7, TOP/PDB);<br>
+...<br>
+
+## Requirements
+Python 3.6+, PySide 2, numpy, scipy, matplotlib, parmed and MDAnalysis.<br>
+[NAMD 3.0 or later](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=NAMD) / [Colvars patched Gromacs](https://github.com/Colvars/colvars).<br>
+**Note: BFEE2 uses cutting-edge features of NAMD and Colvars. We highly suggest the end-user download the devel branch of NAMD from [here](https://gitlab.com/tcbgUIUC/namd/-/tree/devel) and patch it with [Colvars](https://github.com/Colvars/colvars) to prevent possible problems.**
+
+## Installation
+We suggest to install BFEE2 through conda. It will be safe if conda is install in a new environment<br>
+```
+conda create --name bfee   (optional)
+conda activate bfee        (optional)
+conda install -c conda-forge BFEE2
+```
+
+## Usage
+Simply run BFEE2Gui.py in terminal or PowerShell. One may need to use the absolute path on MS Windows.<br>
+A step-by-step tutorial is provided [here](https://www.nature.com/articles/s41596-021-00676-1).<br>
+
+## Citations
+When possible, please consider mentioning [Fu et al. Nat. Protoc. 2022, doi:10.1038/s41596-021-00676-1](https://www.nature.com/articles/s41596-021-00676-1#citeas) when BFEE2 is used in your project.
+
+
+Additional references:<br>
+BFEE2: [Fu et al. J. Chem. Inf. Model. 2021, 61, 2116–2123](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c00269)<br>
+Alchemical and geometric routes [Gumbart et al. J. Chem. Theory Comput. 2013, 9, 794–802](https://pubs.acs.org/doi/abs/10.1021/ct3008099)<br>
+WTM-eABF: [Fu et al. Acc. Chem. Res. 2019, 52, 3254–3264](https://pubs.acs.org/doi/abs/10.1021/acs.accounts.9b00473) and [Fu et al. J. Phys. Chem. Lett. 2018, 9, 4738–4745](https://pubs.acs.org/doi/abs/10.1021/acs.jpclett.8b01994)<br>
+Collective variables: [Fu et al. J. Chem. Theory Comput. 2017, 13, 5173–5178](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791)<br>
+Colvars module: [Fiorin et al. Mol. Phys. 2013 111, 3345-3362](https://www.tandfonline.com/doi/full/10.1080/00268976.2013.813594)<br>
+"Mother" of all restraint-based binding free-energy calculations: [Hermans et al. Isr. J. Chem. 1986, 27, 225–227](https://onlinelibrary.wiley.com/doi/abs/10.1002/ijch.198600032)<br>
+
+## Contact us
+Technique issues: Haohao Fu (fhh2626@mail.nankai.edu.cn) and Haochuan Chen (yjcoshc@mail.nankai.edu.cn)<br>
+
+This software is under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) license. For more information about the copyright of BFEE, contact the corresponding authors of the aforementioned papers (wscai@nankai.edu.cn, Christophe.Chipot@univ-lorraine.fr).
```

### Comparing `BFEE2-2.3.2/README.md` & `BFEE2-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: BFEE2
+Version: 2.4.0
+Summary: Binding Free Energy Estimator 2
+Home-page: https://github.com/fhh2626/BFEE2
+Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
+Author-email: wscai@nankai.edu.cn
+Maintainer: Haohao Fu
+Maintainer-email: fhh2626@mail.nankai.edu.cn
+License: GPLv3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Binding Free Energy Estimator 2
 [![DOI](https://zenodo.org/badge/322234705.svg)](https://zenodo.org/badge/latestdoi/322234705)
 
 Binding free energy estimator (BFEE) is a python-based software that automates absolute binding free energy calculations through either the alchemical or geometric route by molecular dynamics simulations.<br>
 
 ## Theoretical backgrounds
 The degrees of freedom of the protein-ligand (or host-guest) system are described by a series of geometric variables (or collective variables), as firstly described by the [Karplus group](https://pubs.acs.org/doi/abs/10.1021/jp0217839). In BFEE, a generalized, best-fit-rotation-based geometric variables are used, making it in principle available to any protein-ligand complex. See [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.7b00791) for introduction of these variables.<br>
```

### Comparing `BFEE2-2.3.2/setup.cfg` & `BFEE2-2.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2042 4645 4532 0d0a 6175 7468 6f72   = BFEE2..author
-00000020: 203d 2048 616f 6861 6f20 4675 2c20 4861   = Haohao Fu, Ha
-00000030: 6f63 6875 616e 2043 6865 6e2c 2057 656e  ochuan Chen, Wen
-00000040: 7368 656e 6720 4361 6920 616e 6420 4368  sheng Cai and Ch
-00000050: 7269 7320 4368 6970 6f74 0d0a 6175 7468  ris Chipot..auth
-00000060: 6f72 5f65 6d61 696c 203d 2077 7363 6169  or_email = wscai
-00000070: 406e 616e 6b61 692e 6564 752e 636e 0d0a  @nankai.edu.cn..
-00000080: 6d61 696e 7461 696e 6572 203d 2048 616f  maintainer = Hao
-00000090: 6861 6f20 4675 0d0a 6d61 696e 7461 696e  hao Fu..maintain
-000000a0: 6572 5f65 6d61 696c 203d 2066 6868 3236  er_email = fhh26
-000000b0: 3236 406d 6169 6c2e 6e61 6e6b 6169 2e65  26@mail.nankai.e
-000000c0: 6475 2e63 6e0d 0a75 726c 203d 2068 7474  du.cn..url = htt
-000000d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000e0: 6668 6832 3632 362f 4246 4545 320d 0a6c  fhh2626/BFEE2..l
-000000f0: 6963 656e 7365 203d 2047 504c 7633 0d0a  icense = GPLv3..
-00000100: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
-00000110: 0d0a 094c 4943 454e 5345 0d0a 6465 7363  ...LICENSE..desc
-00000120: 7269 7074 696f 6e20 3d20 4269 6e64 696e  ription = Bindin
-00000130: 6720 4672 6565 2045 6e65 7267 7920 4573  g Free Energy Es
-00000140: 7469 6d61 746f 7220 320d 0a6c 6f6e 675f  timator 2..long_
-00000150: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000160: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000170: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000180: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000190: 6578 742f 6d61 726b 646f 776e 0d0a 0d0a  ext/markdown....
-000001a0: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-000001b0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000001c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001d0: 3d33 2e36 0d0a 7363 7269 7074 7320 3d20  =3.6..scripts = 
-000001e0: 0d0a 0962 696e 2f42 4645 4532 4775 692e  ...bin/BFEE2Gui.
-000001f0: 7079 0d0a 696e 7374 616c 6c5f 7265 7175  py..install_requ
-00000200: 6972 6573 203d 200d 0a09 7365 7475 7074  ires = ...setupt
-00000210: 6f6f 6c73 0d0a 0970 7973 6964 6532 0d0a  ools...pyside2..
-00000220: 0961 7070 6469 7273 0d0a 094d 4441 6e61  .appdirs...MDAna
-00000230: 6c79 7369 730d 0a09 6d61 7470 6c6f 746c  lysis...matplotl
-00000240: 6962 0d0a 096e 756d 7079 0d0a 0973 6369  ib...numpy...sci
-00000250: 7079 0d0a 0970 6172 6d65 640d 0a0d 0a5b  py...parmed....[
-00000260: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-00000270: 6461 7461 5d0d 0a2a 203d 202a 2e74 656d  data]..* = *.tem
-00000280: 706c 6174 652c 202a 2e74 636c 2c20 2a2e  plate, *.tcl, *.
-00000290: 6177 6b2c 202a 2e70 6466 2c20 2a2e 7478  awk, *.pdf, *.tx
-000002a0: 740d 0a0d 0a5b 6567 675f 696e 666f 5d0d  t....[egg_info].
-000002b0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000002c0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 4246 4545 320a 6175 7468 6f72 203d  = BFEE2.author =
+00000020: 2048 616f 6861 6f20 4675 2c20 4861 6f63   Haohao Fu, Haoc
+00000030: 6875 616e 2043 6865 6e2c 2057 656e 7368  huan Chen, Wensh
+00000040: 656e 6720 4361 6920 616e 6420 4368 7269  eng Cai and Chri
+00000050: 7320 4368 6970 6f74 0a61 7574 686f 725f  s Chipot.author_
+00000060: 656d 6169 6c20 3d20 7773 6361 6940 6e61  email = wscai@na
+00000070: 6e6b 6169 2e65 6475 2e63 6e0a 6d61 696e  nkai.edu.cn.main
+00000080: 7461 696e 6572 203d 2048 616f 6861 6f20  tainer = Haohao 
+00000090: 4675 0a6d 6169 6e74 6169 6e65 725f 656d  Fu.maintainer_em
+000000a0: 6169 6c20 3d20 6668 6832 3632 3640 6d61  ail = fhh2626@ma
+000000b0: 696c 2e6e 616e 6b61 692e 6564 752e 636e  il.nankai.edu.cn
+000000c0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+000000d0: 6974 6875 622e 636f 6d2f 6668 6832 3632  ithub.com/fhh262
+000000e0: 362f 4246 4545 320a 6c69 6365 6e73 6520  6/BFEE2.license 
+000000f0: 3d20 4750 4c76 330a 6c69 6365 6e73 655f  = GPLv3.license_
+00000100: 6669 6c65 7320 3d20 0a09 4c49 4345 4e53  files = ..LICENS
+00000110: 450a 6465 7363 7269 7074 696f 6e20 3d20  E.description = 
+00000120: 4269 6e64 696e 6720 4672 6565 2045 6e65  Binding Free Ene
+00000130: 7267 7920 4573 7469 6d61 746f 7220 320a  rgy Estimator 2.
+00000140: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000150: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000160: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
+00000170: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000180: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000190: 0a0a 5b6f 7074 696f 6e73 5d0a 7061 636b  ..[options].pack
+000001a0: 6167 6573 203d 2066 696e 643a 0a70 7974  ages = find:.pyt
+000001b0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000001c0: 3d33 2e36 0a73 6372 6970 7473 203d 200a  =3.6.scripts = .
+000001d0: 0962 696e 2f42 4645 4532 4775 692e 7079  .bin/BFEE2Gui.py
+000001e0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000001f0: 7320 3d20 0a09 7365 7475 7074 6f6f 6c73  s = ..setuptools
+00000200: 0a09 7079 7369 6465 320a 0961 7070 6469  ..pyside2..appdi
+00000210: 7273 0a09 4d44 416e 616c 7973 6973 0a09  rs..MDAnalysis..
+00000220: 6d61 7470 6c6f 746c 6962 0a09 6e75 6d70  matplotlib..nump
+00000230: 790a 0973 6369 7079 0a09 7061 726d 6564  y..scipy..parmed
+00000240: 0a0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000250: 6765 5f64 6174 615d 0a2a 203d 202a 2e74  ge_data].* = *.t
+00000260: 656d 706c 6174 652c 202a 2e74 636c 2c20  emplate, *.tcl, 
+00000270: 2a2e 6177 6b2c 202a 2e70 6466 2c20 2a2e  *.awk, *.pdf, *.
+00000280: 7478 740a 0a5b 6567 675f 696e 666f 5d0a  txt..[egg_info].
+00000290: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
+000002a0: 5f64 6174 6520 3d20 300a 0a              _date = 0..
```

