# Comparing `tmp/vertica-sqlalchemy-dialect-0.0.2.tar.gz` & `tmp/vertica-sqlalchemy-dialect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.2.tar", last modified: Mon Jun  5 10:21:00 2023, max compression
+gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.3.tar", last modified: Mon Jun  5 10:28:58 2023, max compression
```

## Comparing `vertica-sqlalchemy-dialect-0.0.2.tar` & `vertica-sqlalchemy-dialect-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 10:21:00.136730 vertica-sqlalchemy-dialect-0.0.2/
--rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5754 2023-06-05 10:21:00.137732 vertica-sqlalchemy-dialect-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5407 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/README.rst
--rw-rw-rw-   0        0        0      211 2023-06-05 10:21:00.142736 vertica-sqlalchemy-dialect-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1916 2023-06-05 10:12:18.000000 vertica-sqlalchemy-dialect-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:21:00.012736 vertica-sqlalchemy-dialect-0.0.2/test/
--rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/test/test_core.py
--rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/test/test_integration.py
--rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/test/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:21:00.089735 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/
--rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/__init__.py
--rw-rw-rw-   0        0        0    68805 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/base.py
--rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/dialect_pyodbc.py
--rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/dialect_vertica_python.py
--rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/requirements.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:21:00.130732 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/
--rw-rw-rw-   0        0        0     5754 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-05 10:20:59.000000 vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.139608 vertica-sqlalchemy-dialect-0.0.3/
+-rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5742 2023-06-05 10:28:58.141609 vertica-sqlalchemy-dialect-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5395 2023-06-05 10:26:49.000000 vertica-sqlalchemy-dialect-0.0.3/README.rst
+-rw-rw-rw-   0        0        0      211 2023-06-05 10:28:58.145603 vertica-sqlalchemy-dialect-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1916 2023-06-05 10:28:52.000000 vertica-sqlalchemy-dialect-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.054604 vertica-sqlalchemy-dialect-0.0.3/test/
+-rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_core.py
+-rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_integration.py
+-rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.092608 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/
+-rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/__init__.py
+-rw-rw-rw-   0        0        0    68805 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/base.py
+-rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_pyodbc.py
+-rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_vertica_python.py
+-rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/requirements.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.134602 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/
+-rw-rw-rw-   0        0        0     5742 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/top_level.txt
```

### Comparing `vertica-sqlalchemy-dialect-0.0.2/LICENSE` & `vertica-sqlalchemy-dialect-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.2
+Version: 0.0.3
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
@@ -24,15 +24,15 @@
 Prerequisites
 -------------
 
 You will need the following softwares to run, build and test the dialect. Everything apart from Python and pip can be installed via pip itself.
 
 1. Python 3.x or higher
 2. pip 22 or higher
-3. SQLAlchemy > 1.3.24 and < 2.0
+3. SQLAlchemy 1.4.48
 4. vertica-python 1.1.1 or higher
 
 #####################################
 Vertica-Python
 #####################################
 
 `vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.2/README.rst` & `vertica-sqlalchemy-dialect-0.0.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -40,299 +40,299 @@
 00000270: 6869 6e67 2061 7061 7274 2066 726f 6d20  hing apart from 
 00000280: 5079 7468 6f6e 2061 6e64 2070 6970 2063  Python and pip c
 00000290: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
 000002a0: 7669 6120 7069 7020 6974 7365 6c66 2e0d  via pip itself..
 000002b0: 0a0d 0a31 2e20 5079 7468 6f6e 2033 2e78  ...1. Python 3.x
 000002c0: 206f 7220 6869 6768 6572 0d0a 322e 2070   or higher..2. p
 000002d0: 6970 2032 3220 6f72 2068 6967 6865 720d  ip 22 or higher.
-000002e0: 0a33 2e20 5351 4c41 6c63 6865 6d79 203e  .3. SQLAlchemy >
-000002f0: 2031 2e33 2e32 3420 616e 6420 3c20 322e   1.3.24 and < 2.
-00000300: 300d 0a34 2e20 7665 7274 6963 612d 7079  0..4. vertica-py
-00000310: 7468 6f6e 2031 2e31 2e31 206f 7220 6869  thon 1.1.1 or hi
-00000320: 6768 6572 0d0a 0d0a 2323 2323 2323 2323  gher....########
+000002e0: 0a33 2e20 5351 4c41 6c63 6865 6d79 2031  .3. SQLAlchemy 1
+000002f0: 2e34 2e34 380d 0a34 2e20 7665 7274 6963  .4.48..4. vertic
+00000300: 612d 7079 7468 6f6e 2031 2e31 2e31 206f  a-python 1.1.1 o
+00000310: 7220 6869 6768 6572 0d0a 0d0a 2323 2323  r higher....####
+00000320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000340: 2323 2323 2323 2323 2323 2323 230d 0a56  #############..V
-00000350: 6572 7469 6361 2d50 7974 686f 6e0d 0a23  ertica-Python..#
+00000340: 230d 0a56 6572 7469 6361 2d50 7974 686f  #..Vertica-Pytho
+00000350: 6e0d 0a23 2323 2323 2323 2323 2323 2323  n..#############
 00000360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000380: 2323 2323 0d0a 0d0a 6076 6572 7469 6361  ####....`vertica
-00000390: 2d70 7974 686f 6e20 0d0a 3c68 7474 7073  -python ..<https
-000003a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7665  ://github.com/ve
-000003b0: 7274 6963 612f 7665 7274 6963 612d 7079  rtica/vertica-py
-000003c0: 7468 6f6e 3e60 5f20 6973 206e 6565 6465  thon>`_ is neede
-000003d0: 6420 746f 2075 7365 2074 6865 2056 6572  d to use the Ver
-000003e0: 7469 6361 2d53 514c 416c 6368 656d 792d  tica-SQLAlchemy-
-000003f0: 4469 616c 6563 742e 2054 6865 2063 6f6e  Dialect. The con
-00000400: 6e65 6374 6f72 2064 6f65 7320 6e6f 7420  nector does not 
-00000410: 6e65 6564 2074 6f20 6265 2069 6e73 7461  need to be insta
-00000420: 6c6c 6564 2061 7320 7468 6520 6469 616c  lled as the dial
-00000430: 6563 7420 696e 7374 616c 6c61 7469 6f6e  ect installation
-00000440: 2074 616b 6573 2063 6172 6520 6f66 2069   takes care of i
-00000450: 742e 0d0a 0d0a 4e6f 7465 3a20 5765 2072  t.....Note: We r
-00000460: 6563 6f6d 6d65 6e64 2075 7369 6e67 2074  ecommend using t
-00000470: 6865 2076 6572 7469 6361 2d70 7974 686f  he vertica-pytho
-00000480: 6e20 636f 6e6e 6563 746f 722e 2048 6f77  n connector. How
-00000490: 6576 6572 2c20 7468 6520 6469 616c 6563  ever, the dialec
-000004a0: 7420 616c 736f 2061 6c6c 6f77 7320 636f  t also allows co
-000004b0: 6e6e 6563 7469 6e67 2075 7369 6e67 2060  nnecting using `
-000004c0: 7079 6f64 6263 203c 6874 7470 733a 2f2f  pyodbc <https://
-000004d0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000004e0: 2f70 796f 6462 632f 3e60 5f2e 204d 6f72  /pyodbc/>`_. Mor
-000004f0: 6520 696e 7374 7275 6374 696f 6e73 2061  e instructions a
-00000500: 7265 2061 7420 7468 6520 656e 6420 6f66  re at the end of
-00000510: 2074 6869 7320 5245 4144 4d45 2e0d 0a0d   this README....
-00000520: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000540: 2d2d 2d2d 2d2d 0d0a 496e 7374 616c 6c69  ------..Installi
-00000550: 6e67 2056 6572 7469 6361 2053 514c 416c  ng Vertica SQLAl
-00000560: 6368 656d 7920 4469 616c 6563 740d 0a2d  chemy Dialect..-
+00000370: 2323 2323 2323 2323 0d0a 0d0a 6076 6572  ########....`ver
+00000380: 7469 6361 2d70 7974 686f 6e20 0d0a 3c68  tica-python ..<h
+00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003a0: 6d2f 7665 7274 6963 612f 7665 7274 6963  m/vertica/vertic
+000003b0: 612d 7079 7468 6f6e 3e60 5f20 6973 206e  a-python>`_ is n
+000003c0: 6565 6465 6420 746f 2075 7365 2074 6865  eeded to use the
+000003d0: 2056 6572 7469 6361 2d53 514c 416c 6368   Vertica-SQLAlch
+000003e0: 656d 792d 4469 616c 6563 742e 2054 6865  emy-Dialect. The
+000003f0: 2063 6f6e 6e65 6374 6f72 2064 6f65 7320   connector does 
+00000400: 6e6f 7420 6e65 6564 2074 6f20 6265 2069  not need to be i
+00000410: 6e73 7461 6c6c 6564 2061 7320 7468 6520  nstalled as the 
+00000420: 6469 616c 6563 7420 696e 7374 616c 6c61  dialect installa
+00000430: 7469 6f6e 2074 616b 6573 2063 6172 6520  tion takes care 
+00000440: 6f66 2069 742e 0d0a 0d0a 4e6f 7465 3a20  of it.....Note: 
+00000450: 5765 2072 6563 6f6d 6d65 6e64 2075 7369  We recommend usi
+00000460: 6e67 2074 6865 2076 6572 7469 6361 2d70  ng the vertica-p
+00000470: 7974 686f 6e20 636f 6e6e 6563 746f 722e  ython connector.
+00000480: 2048 6f77 6576 6572 2c20 7468 6520 6469   However, the di
+00000490: 616c 6563 7420 616c 736f 2061 6c6c 6f77  alect also allow
+000004a0: 7320 636f 6e6e 6563 7469 6e67 2075 7369  s connecting usi
+000004b0: 6e67 2060 7079 6f64 6263 203c 6874 7470  ng `pyodbc <http
+000004c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000004d0: 6a65 6374 2f70 796f 6462 632f 3e60 5f2e  ject/pyodbc/>`_.
+000004e0: 204d 6f72 6520 696e 7374 7275 6374 696f   More instructio
+000004f0: 6e73 2061 7265 2061 7420 7468 6520 656e  ns are at the en
+00000500: 6420 6f66 2074 6869 7320 5245 4144 4d45  d of this README
+00000510: 2e0d 0a0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .....-----------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 496e 7374  ----------..Inst
+00000540: 616c 6c69 6e67 2056 6572 7469 6361 2053  alling Vertica S
+00000550: 514c 416c 6368 656d 7920 4469 616c 6563  QLAlchemy Dialec
+00000560: 740d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  t..-------------
 00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2d 2d2d 0d0a 0d0a 5468 6520 5665 7274  ----....The Vert
-000005a0: 6963 6120 5351 4c41 6c63 6865 6d79 2070  ica SQLAlchemy p
-000005b0: 6163 6b61 6765 2063 616e 2062 6520 696e  ackage can be in
-000005c0: 7374 616c 6c65 6420 6672 6f6d 2074 6865  stalled from the
-000005d0: 2070 7562 6c69 6320 5079 5049 2072 6570   public PyPI rep
-000005e0: 6f73 6974 6f72 7920 7573 696e 6720 6070  ository using `p
-000005f0: 6970 603a 200d 0a3a 3a0d 0a0d 0a20 2020  ip`: ..::....   
-00000600: 2070 6970 2069 6e73 7461 6c6c 202d 2d75   pip install --u
-00000610: 7067 7261 6465 2076 6572 7469 6361 2d73  pgrade vertica-s
-00000620: 716c 616c 6368 656d 792d 6469 616c 6563  qlalchemy-dialec
-00000630: 740d 0a0d 0a0d 0a60 7069 7060 2061 7574  t......`pip` aut
-00000640: 6f6d 6174 6963 616c 6c79 2069 6e73 7461  omatically insta
-00000650: 6c6c 7320 616c 6c20 7265 7175 6972 6564  lls all required
-00000660: 206d 6f64 756c 6573 2c20 696e 636c 7564   modules, includ
-00000670: 696e 6720 7665 7274 6963 612d 7079 7468  ing vertica-pyth
-00000680: 6f6e 2e0d 0a0d 0a46 6f72 206d 6f72 6520  on.....For more 
-00000690: 696e 666f 726d 6174 696f 6e20 6f6e 2069  information on i
-000006a0: 6e73 7461 6c6c 6174 696f 6e20 616e 6420  nstallation and 
-000006b0: 7661 6c69 6461 7469 6f6e 2063 6865 636b  validation check
-000006c0: 206f 7572 2067 6974 6875 6220 7061 6765   our github page
-000006d0: 2e0d 0a0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .....-----------
-000006e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 5061  ------------..Pa
-000006f0: 7261 6d65 7465 7273 2061 6e64 2042 6568  rameters and Beh
-00000700: 6176 696f 720d 0a2d 2d2d 2d2d 2d2d 2d2d  avior..---------
-00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
-00000720: 0d0a 4173 206d 7563 6820 6173 2070 6f73  ..As much as pos
-00000730: 7369 626c 652c 2056 6572 7469 6361 2053  sible, Vertica S
-00000740: 514c 416c 6368 656d 7920 7072 6f76 6964  QLAlchemy provid
-00000750: 6573 2063 6f6d 7061 7469 626c 6520 6675  es compatible fu
-00000760: 6e63 7469 6f6e 616c 6974 7920 666f 7220  nctionality for 
-00000770: 5351 4c41 6c63 6865 6d79 2061 7070 6c69  SQLAlchemy appli
-00000780: 6361 7469 6f6e 732e 200d 0a46 6f72 2069  cations. ..For i
-00000790: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7573  nformation on us
-000007a0: 696e 6720 5351 4c41 6c63 6865 6d79 2c20  ing SQLAlchemy, 
-000007b0: 7365 6520 7468 6520 6053 514c 416c 6368  see the `SQLAlch
-000007c0: 656d 7920 646f 6375 6d65 6e74 6174 696f  emy documentatio
-000007d0: 6e0d 0a3c 6874 7470 3a2f 2f64 6f63 732e  n..<http://docs.
-000007e0: 7371 6c61 6c63 6865 6d79 2e6f 7267 2f65  sqlalchemy.org/e
-000007f0: 6e2f 6c61 7465 7374 2f3e 605f 2e0d 0a0d  n/latest/>`_....
-00000800: 0a4e 6f74 653a 2043 7572 7265 6e74 2073  .Note: Current s
-00000810: 7461 7465 206f 6620 7468 6520 6469 616c  tate of the dial
-00000820: 6563 7420 6f6e 6c79 2073 7570 706f 7274  ect only support
-00000830: 7320 6d65 7461 6461 7461 2066 756e 6374  s metadata funct
-00000840: 696f 6e73 2e20 4974 2069 7320 7374 696c  ions. It is stil
-00000850: 6c20 756e 6465 7220 6465 7665 6c6f 706d  l under developm
-00000860: 656e 742e 200d 0a0d 0a48 6f77 6576 6572  ent. ....However
-00000870: 2c20 5665 7274 6963 6120 5351 4c41 6c63  , Vertica SQLAlc
-00000880: 6865 6d79 2061 6c73 6f20 7072 6f76 6964  hemy also provid
-00000890: 6573 2073 7065 6369 6669 6320 7061 7261  es specific para
-000008a0: 6d65 7465 7273 2061 6e64 2062 6568 6176  meters and behav
-000008b0: 696f 722c 2077 6869 6368 2061 7265 2064  ior, which are d
-000008c0: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
-000008d0: 666f 6c6c 6f77 696e 6720 7365 6374 696f  following sectio
-000008e0: 6e73 2e0d 0a0d 0a23 2323 2323 2323 2323  ns.....#########
-000008f0: 2323 2323 2323 2323 2323 2323 0d0a 436f  ############..Co
-00000900: 6e6e 6563 7469 6f6e 2050 6172 616d 6574  nnection Paramet
-00000910: 6572 730d 0a23 2323 2323 2323 2323 2323  ers..###########
-00000920: 2323 2323 2323 2323 2323 0d0a 0d0a 5665  ##########....Ve
-00000930: 7274 6963 6120 5351 4c41 6c63 6865 6d79  rtica SQLAlchemy
-00000940: 2044 6961 6c65 6374 2075 7365 7320 7468   Dialect uses th
-00000950: 6520 666f 6c6c 6f77 696e 6720 7379 6e74  e following synt
-00000960: 6178 2066 6f72 2074 6865 2063 6f6e 6e65  ax for the conne
-00000970: 6374 696f 6e20 7374 7269 6e67 2075 7365  ction string use
-00000980: 6420 746f 2063 6f6e 6e65 6374 2074 6f20  d to connect to 
-00000990: 5665 7274 6963 6120 616e 6420 696e 6974  Vertica and init
-000009a0: 6961 7465 2061 2073 6573 7369 6f6e 3a0d  iate a session:.
-000009b0: 0a3a 3a0d 0a0d 0a20 2020 2027 7665 7274  .::....    'vert
-000009c0: 6963 612b 7665 7274 6963 615f 7079 7468  ica+vertica_pyth
-000009d0: 6f6e 3a2f 2f3c 7573 6572 3e3a 3c70 6173  on://<user>:<pas
-000009e0: 7377 6f72 643e 403c 686f 7374 5f6e 616d  sword>@<host_nam
-000009f0: 653e 2f3c 6461 7461 6261 7365 5f6e 616d  e>/<database_nam
-00000a00: 653e 270d 0a0d 0a0d 0a57 6865 7265 3a0d  e>'......Where:.
-00000a10: 0a0d 0a2d 2060 3c75 7365 723e 6020 6973  ...- `<user>` is
-00000a20: 2074 6865 206c 6f67 696e 206e 616d 6520   the login name 
-00000a30: 666f 7220 796f 7572 2056 6572 7469 6361  for your Vertica
-00000a40: 2075 7365 722e 0d0a 2d20 603c 7061 7373   user...- `<pass
-00000a50: 776f 7264 3e60 2069 7320 7468 6520 7061  word>` is the pa
-00000a60: 7373 776f 7264 2066 6f72 2079 6f75 7220  ssword for your 
-00000a70: 5665 7274 6963 6120 7573 6572 2e0d 0a2d  Vertica user...-
-00000a80: 2060 3c68 6f73 745f 6e61 6d65 3e60 2069   `<host_name>` i
-00000a90: 7320 7468 6520 4950 2f46 5144 4e20 6f66  s the IP/FQDN of
-00000aa0: 2079 6f75 7220 5665 7274 6963 6120 486f   your Vertica Ho
-00000ab0: 7374 2e0d 0a2d 2060 3c64 6174 6162 6173  st...- `<databas
-00000ac0: 655f 6e61 6d65 3e60 2069 7320 7468 6520  e_name>` is the 
-00000ad0: 6e61 6d65 206f 6620 796f 7572 2056 6572  name of your Ver
-00000ae0: 7469 6361 2044 6174 6162 6173 652e 0d0a  tica Database...
-00000af0: 0d0a 0d0a 596f 7520 6361 6e20 6f70 7469  ....You can opti
-00000b00: 6f6e 616c 6c79 2073 7065 6369 6679 2074  onally specify t
-00000b10: 6865 2069 6e69 7469 616c 2064 6174 6162  he initial datab
-00000b20: 6173 6520 616e 6420 7363 6865 6d61 2066  ase and schema f
-00000b30: 6f72 2074 6865 2056 6572 7469 6361 2073  or the Vertica s
-00000b40: 6573 7369 6f6e 2062 7920 696e 636c 7564  ession by includ
-00000b50: 696e 6720 7468 656d 2061 7420 7468 6520  ing them at the 
-00000b60: 656e 6420 6f66 2074 6865 2063 6f6e 6e65  end of the conne
-00000b70: 6374 696f 6e20 7374 7269 6e67 2c20 7365  ction string, se
-00000b80: 7061 7261 7465 6420 6279 2060 2f60 2e20  parated by `/`. 
-00000b90: 596f 7520 6361 6e20 616c 736f 2073 7065  You can also spe
-00000ba0: 6369 6679 206f 7468 6572 2073 7570 706f  cify other suppo
-00000bb0: 7274 6564 2070 6172 616d 6574 6572 7320  rted parameters 
-00000bc0: 6279 2076 6572 7469 6361 2d70 7974 686f  by vertica-pytho
-00000bd0: 6e20 6174 2074 6865 2065 6e64 206f 6620  n at the end of 
-00000be0: 7468 6520 636f 6e6e 6563 7469 6f6e 2073  the connection s
-00000bf0: 7472 696e 673a 0d0a 3a3a 0d0a 0d0a 2020  tring:..::....  
-00000c00: 2020 2776 6572 7469 6361 2b76 6572 7469    'vertica+verti
-00000c10: 6361 5f70 7974 686f 6e3a 2f2f 3c75 7365  ca_python://<use
-00000c20: 723e 3a3c 7061 7373 776f 7264 3e40 3c68  r>:<password>@<h
-00000c30: 6f73 745f 6e61 6d65 3e2f 3c64 6174 6162  ost_name>/<datab
-00000c40: 6173 655f 6e61 6d65 3e3f 7365 7373 696f  ase_name>?sessio
-00000c50: 6e5f 6c61 6265 6c3d 7371 6c61 6c63 6865  n_label=sqlalche
-00000c60: 6d79 2663 6f6e 6e65 6374 696f 6e5f 6c6f  my&connection_lo
-00000c70: 6164 5f62 616c 616e 6365 3d31 270d 0a0d  ad_balance=1'...
-00000c80: 0a46 6f72 206d 6f72 6520 696e 666f 726d  .For more inform
-00000c90: 6174 696f 6e2c 2063 6865 636b 206f 7574  ation, check out
-00000ca0: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
-00000cb0: 606f 7074 696f 6e73 203c 6874 7470 733a  `options <https:
-00000cc0: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6572  //github.com/ver
-00000cd0: 7469 6361 2f76 6572 7469 6361 2d70 7974  tica/vertica-pyt
-00000ce0: 686f 6e23 7365 742d 7072 6f70 6572 7469  hon#set-properti
-00000cf0: 6573 2d77 6974 682d 636f 6e6e 6563 7469  es-with-connecti
-00000d00: 6f6e 2d73 7472 696e 673e 605f 206f 6620  on-string>`_ of 
-00000d10: 7665 7274 6963 612d 7079 7468 6f6e 2e0d  vertica-python..
-00000d20: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
-00000d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d40: 230d 0a4f 7065 6e69 6e67 2061 6e64 2043  #..Opening and C
-00000d50: 6c6f 7369 6e67 2043 6f6e 6e65 6374 696f  losing Connectio
-00000d60: 6e0d 0a23 2323 2323 2323 2323 2323 2323  n..#############
-00000d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d80: 230d 0a0d 0a4f 7065 6e20 6120 636f 6e6e  #....Open a conn
-00000d90: 6563 7469 6f6e 2062 7920 6578 6563 7574  ection by execut
-00000da0: 696e 6720 6065 6e67 696e 652e 636f 6e6e  ing `engine.conn
-00000db0: 6563 7428 2960 3b20 6176 6f69 6420 7573  ect()`; avoid us
-00000dc0: 696e 6720 6065 6e67 696e 652e 6578 6563  ing `engine.exec
-00000dd0: 7574 6528 2960 2e20 4d61 6b65 2063 6572  ute()`. Make cer
-00000de0: 7461 696e 2074 6f20 636c 6f73 6520 7468  tain to close th
-00000df0: 6520 636f 6e6e 6563 7469 6f6e 2062 7920  e connection by 
-00000e00: 6578 6563 7574 696e 6720 6063 6f6e 6e65  executing `conne
-00000e10: 6374 696f 6e2e 636c 6f73 6528 2960 2062  ction.close()` b
-00000e20: 6566 6f72 650d 0a60 656e 6769 6e65 2e64  efore..`engine.d
-00000e30: 6973 706f 7365 2829 603b 206f 7468 6572  ispose()`; other
-00000e40: 7769 7365 2c20 7468 6520 5079 7468 6f6e  wise, the Python
-00000e50: 2047 6172 6261 6765 2063 6f6c 6c65 6374   Garbage collect
-00000e60: 6f72 2072 656d 6f76 6573 2074 6865 2072  or removes the r
-00000e70: 6573 6f75 7263 6573 2072 6571 7569 7265  esources require
-00000e80: 6420 746f 2063 6f6d 6d75 6e69 6361 7465  d to communicate
-00000e90: 2077 6974 6820 5665 7274 6963 612c 2070   with Vertica, p
-00000ea0: 7265 7665 6e74 696e 6720 7468 6520 5079  reventing the Py
-00000eb0: 7468 6f6e 2063 6f6e 6e65 6374 6f72 2066  thon connector f
-00000ec0: 726f 6d20 636c 6f73 696e 6720 7468 6520  rom closing the 
-00000ed0: 7365 7373 696f 6e20 7072 6f70 6572 6c79  session properly
-00000ee0: 2e0d 0a0d 0a3a 3a0d 0a0d 0a20 2020 2065  .....::....    e
-00000ef0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-00000f00: 6e67 696e 6528 2e2e 2e29 0d0a 2020 2020  ngine(...)..    
-00000f10: 636f 6e6e 6563 7469 6f6e 203d 2065 6e67  connection = eng
-00000f20: 696e 652e 636f 6e6e 6563 7428 290d 0a20  ine.connect().. 
-00000f30: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00000f40: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
-00000f50: 7574 6528 3c53 514c 3e29 0d0a 2020 2020  ute(<SQL>)..    
-00000f60: 6669 6e61 6c6c 793a 0d0a 2020 2020 2020  finally:..      
-00000f70: 2020 636f 6e6e 6563 7469 6f6e 2e63 6c6f    connection.clo
-00000f80: 7365 2829 0d0a 2020 2020 2020 2020 656e  se()..        en
-00000f90: 6769 6e65 2e64 6973 706f 7365 2829 0d0a  gine.dispose()..
-00000fa0: 0d0a 0d0a 2a2a 5573 696e 6720 7079 6f64  ....**Using pyod
-00000fb0: 6263 2069 6e73 7465 6164 206f 6620 7665  bc instead of ve
-00000fc0: 7274 6963 612d 7079 7468 6f6e 2a2a 0d0a  rtica-python**..
-00000fd0: 0d0a 596f 7520 6d61 7920 7573 6520 7079  ..You may use py
-00000fe0: 6f64 6263 2069 6e73 7465 6164 206f 6620  odbc instead of 
-00000ff0: 7665 7274 6963 612d 7079 7468 6f6e 2066  vertica-python f
-00001000: 6f72 2074 6865 2063 6f6e 6e65 6374 696f  or the connectio
-00001010: 6e2e 0d0a 0d0a 2a43 7265 6174 6520 6120  n.....*Create a 
-00001020: 5665 7274 6963 6120 4453 4e2a 200d 0a0d  Vertica DSN* ...
-00001030: 0a0d 0a59 6f75 2077 696c 6c20 6e65 6564  ...You will need
-00001040: 2074 6f20 6861 7665 2061 2056 6572 7469   to have a Verti
-00001050: 6361 204f 4442 4320 6472 6976 6572 2069  ca ODBC driver i
-00001060: 6e73 7461 6c6c 6564 2066 726f 6d20 6056  nstalled from `V
-00001070: 6572 7469 6361 2d43 6c69 656e 742d 4472  ertica-Client-Dr
-00001080: 6976 6572 7320 3c68 7474 7073 3a2f 2f77  ivers <https://w
-00001090: 7777 2e76 6572 7469 6361 2e63 6f6d 2f64  ww.vertica.com/d
-000010a0: 6f77 6e6c 6f61 642f 7665 7274 6963 612f  ownload/vertica/
-000010b0: 636c 6965 6e74 2d64 7269 7665 7273 2f3e  client-drivers/>
-000010c0: 605f 2e20 466f 7220 7374 6570 7320 746f  `_. For steps to
-000010d0: 2069 6e73 7461 6c6c 204f 4442 4320 666f   install ODBC fo
-000010e0: 7220 5665 7274 6963 612c 2066 6f6c 6c6f  r Vertica, follo
-000010f0: 7720 6f66 6669 6369 616c 2060 5665 7274  w official `Vert
-00001100: 6963 6120 446f 6373 203c 6874 7470 733a  ica Docs <https:
-00001110: 2f2f 7777 772e 7665 7274 6963 612e 636f  //www.vertica.co
-00001120: 6d2f 646f 6373 2f31 322e 302e 782f 4854  m/docs/12.0.x/HT
-00001130: 4d4c 2f43 6f6e 7465 6e74 2f41 7574 686f  ML/Content/Autho
-00001140: 7269 6e67 2f43 6f6e 6e65 6374 696e 6754  ring/ConnectingT
-00001150: 6f56 6572 7469 6361 2f43 6c69 656e 744f  oVertica/ClientO
-00001160: 4442 432f 496e 7374 616c 6c69 6e67 4f44  DBC/InstallingOD
-00001170: 4243 2e68 746d 3e60 5f2e 0d0a 0d0a 466f  BC.htm>`_.....Fo
-00001180: 7220 6578 616d 706c 652c 2079 6f75 2077  r example, you w
-00001190: 696c 6c20 6e65 6564 2074 6f20 636f 6e66  ill need to conf
-000011a0: 6967 7572 6520 7468 6573 6520 6669 6c65  igure these file
-000011b0: 7320 7769 7468 2079 6f75 7220 6372 6564  s with your cred
-000011c0: 656e 7469 616c 733a 0d0a 0d0a 602f 6574  entials:....`/et
-000011d0: 632f 7665 7274 6963 612e 696e 6960 0d0a  c/vertica.ini`..
-000011e0: 3a3a 0d0a 0d0a 2020 2020 5b44 7269 7665  ::....    [Drive
-000011f0: 725d 0d0a 2020 2020 4572 726f 724d 6573  r]..    ErrorMes
-00001200: 7361 6765 7350 6174 6820 3d20 2f6f 7074  sagesPath = /opt
-00001210: 2f76 6572 7469 6361 2f6c 6962 3634 2f0d  /vertica/lib64/.
-00001220: 0a20 2020 204f 4442 4349 6e73 744c 6962  .    ODBCInstLib
-00001230: 203d 202f 7573 722f 6c69 622f 7838 365f   = /usr/lib/x86_
-00001240: 3634 2d6c 696e 7578 2d67 6e75 2f6c 6962  64-linux-gnu/lib
-00001250: 6f64 6263 696e 7374 2e73 6f0d 0a20 2020  odbcinst.so..   
-00001260: 2044 7269 7665 724d 616e 6167 6572 456e   DriverManagerEn
-00001270: 636f 6469 6e67 3d55 5446 2d31 360d 0a0d  coding=UTF-16...
-00001280: 0a0d 0a60 7e2f 2e6f 6462 632e 696e 6960  ...`~/.odbc.ini`
-00001290: 0d0a 3a3a 0d0a 0d0a 2020 2020 5b4f 4442  ..::....    [ODB
-000012a0: 4320 4461 7461 2053 6f75 7263 6573 5d0d  C Data Sources].
-000012b0: 0a20 2020 2076 6572 7469 6361 203d 2022  .    vertica = "
-000012c0: 4d79 2044 6174 6162 6173 6522 0d0a 0d0a  My Database"....
-000012d0: 2020 2020 5b76 6572 7469 6361 6473 6e5d      [verticadsn]
-000012e0: 0d0a 2020 2020 4465 7363 7269 7074 696f  ..    Descriptio
-000012f0: 6e20 3d20 4d79 2044 6174 6162 6173 650d  n = My Database.
-00001300: 0a20 2020 2044 7269 7665 7220 3d20 2f6f  .    Driver = /o
-00001310: 7074 2f76 6572 7469 6361 2f6c 6962 3634  pt/vertica/lib64
-00001320: 2f6c 6962 7665 7274 6963 616f 6462 632e  /libverticaodbc.
-00001330: 736f 0d0a 2020 2020 4461 7461 6261 7365  so..    Database
-00001340: 203d 2064 6f63 6b65 720d 0a20 2020 2053   = docker..    S
-00001350: 6572 7665 726e 616d 6520 3d20 3132 372e  ervername = 127.
-00001360: 302e 302e 310d 0a20 2020 2055 4944 203d  0.0.1..    UID =
-00001370: 2064 6261 646d 696e 0d0a 2020 2020 5057   dbadmin..    PW
-00001380: 4420 3d0d 0a0d 0a0d 0a0d 0a54 6865 6e20  D =........Then 
-00001390: 7573 6520 7468 6520 5665 7274 6963 6120  use the Vertica 
-000013a0: 4453 4e20 696e 2061 2066 696c 6520 6c69  DSN in a file li
-000013b0: 6b65 2073 6f3a 0d0a 3a3a 0d0a 0d0a 2020  ke so:..::....  
-000013c0: 2020 6672 6f6d 2073 716c 616c 6368 656d    from sqlalchem
-000013d0: 7920 696d 706f 7274 2063 7265 6174 655f  y import create_
-000013e0: 656e 6769 6e65 0d0a 0d0a 2020 2020 656e  engine....    en
-000013f0: 6769 6e65 203d 2073 612e 6372 6561 7465  gine = sa.create
-00001400: 5f65 6e67 696e 6528 2776 6572 7469 6361  _engine('vertica
-00001410: 2b70 796f 6462 633a 2f2f 4076 6572 7469  +pyodbc://@verti
-00001420: 6361 6473 6e27 290d 0a20 2020 2074 7279  cadsn')..    try
-00001430: 3a0d 0a20 2020 2020 2020 2072 6573 203d  :..        res =
-00001440: 2065 6e67 696e 652e 636f 6e6e 6563 7428   engine.connect(
-00001450: 292e 7363 616c 6172 2827 7365 6c65 6374  ).scalar('select
-00001460: 2076 6572 7369 6f6e 2829 3b27 290d 0a20   version();').. 
-00001470: 2020 2020 2020 2070 7269 6e74 2872 6573         print(res
-00001480: 290d 0a20 2020 2066 696e 616c 6c79 3a0d  )..    finally:.
-00001490: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-000014a0: 696f 6e2e 636c 6f73 6528 290d 0a20 2020  ion.close()..   
-000014b0: 2020 2020 2065 6e67 696e 652e 6469 7370       engine.disp
-000014c0: 6f73 6528 290d 0a0d 0a54 6869 7320 7368  ose()....This sh
-000014d0: 6f75 6c64 2064 6973 706c 6179 2074 6865  ould display the
-000014e0: 2056 6572 7469 6361 2076 6572 7369 6f6e   Vertica version
-000014f0: 2069 6e66 6f3a 2022 5665 7274 6963 6120   info: "Vertica 
-00001500: 416e 616c 7974 6963 2044 6174 6162 6173  Analytic Databas
-00001510: 6520 7631 322e 302e 302d 3022 2e0d 0a    e v12.0.0-0"...
+00000580: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5468 6520  --------....The 
+00000590: 5665 7274 6963 6120 5351 4c41 6c63 6865  Vertica SQLAlche
+000005a0: 6d79 2070 6163 6b61 6765 2063 616e 2062  my package can b
+000005b0: 6520 696e 7374 616c 6c65 6420 6672 6f6d  e installed from
+000005c0: 2074 6865 2070 7562 6c69 6320 5079 5049   the public PyPI
+000005d0: 2072 6570 6f73 6974 6f72 7920 7573 696e   repository usin
+000005e0: 6720 6070 6970 603a 200d 0a3a 3a0d 0a0d  g `pip`: ..::...
+000005f0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000600: 202d 2d75 7067 7261 6465 2076 6572 7469   --upgrade verti
+00000610: 6361 2d73 716c 616c 6368 656d 792d 6469  ca-sqlalchemy-di
+00000620: 616c 6563 740d 0a0d 0a0d 0a60 7069 7060  alect......`pip`
+00000630: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
+00000640: 6e73 7461 6c6c 7320 616c 6c20 7265 7175  nstalls all requ
+00000650: 6972 6564 206d 6f64 756c 6573 2c20 696e  ired modules, in
+00000660: 636c 7564 696e 6720 7665 7274 6963 612d  cluding vertica-
+00000670: 7079 7468 6f6e 2e0d 0a0d 0a46 6f72 206d  python.....For m
+00000680: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+00000690: 6f6e 2069 6e73 7461 6c6c 6174 696f 6e20  on installation 
+000006a0: 616e 6420 7661 6c69 6461 7469 6f6e 2063  and validation c
+000006b0: 6865 636b 206f 7572 2067 6974 6875 6220  heck our github 
+000006c0: 7061 6765 2e0d 0a0d 0a2d 2d2d 2d2d 2d2d  page.....-------
+000006d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006e0: 0d0a 5061 7261 6d65 7465 7273 2061 6e64  ..Parameters and
+000006f0: 2042 6568 6176 696f 720d 0a2d 2d2d 2d2d   Behavior..-----
+00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000710: 2d2d 0d0a 0d0a 4173 206d 7563 6820 6173  --....As much as
+00000720: 2070 6f73 7369 626c 652c 2056 6572 7469   possible, Verti
+00000730: 6361 2053 514c 416c 6368 656d 7920 7072  ca SQLAlchemy pr
+00000740: 6f76 6964 6573 2063 6f6d 7061 7469 626c  ovides compatibl
+00000750: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
+00000760: 666f 7220 5351 4c41 6c63 6865 6d79 2061  for SQLAlchemy a
+00000770: 7070 6c69 6361 7469 6f6e 732e 200d 0a46  pplications. ..F
+00000780: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
+00000790: 6e20 7573 696e 6720 5351 4c41 6c63 6865  n using SQLAlche
+000007a0: 6d79 2c20 7365 6520 7468 6520 6053 514c  my, see the `SQL
+000007b0: 416c 6368 656d 7920 646f 6375 6d65 6e74  Alchemy document
+000007c0: 6174 696f 6e0d 0a3c 6874 7470 3a2f 2f64  ation..<http://d
+000007d0: 6f63 732e 7371 6c61 6c63 6865 6d79 2e6f  ocs.sqlalchemy.o
+000007e0: 7267 2f65 6e2f 6c61 7465 7374 2f3e 605f  rg/en/latest/>`_
+000007f0: 2e0d 0a0d 0a4e 6f74 653a 2043 7572 7265  .....Note: Curre
+00000800: 6e74 2073 7461 7465 206f 6620 7468 6520  nt state of the 
+00000810: 6469 616c 6563 7420 6f6e 6c79 2073 7570  dialect only sup
+00000820: 706f 7274 7320 6d65 7461 6461 7461 2066  ports metadata f
+00000830: 756e 6374 696f 6e73 2e20 4974 2069 7320  unctions. It is 
+00000840: 7374 696c 6c20 756e 6465 7220 6465 7665  still under deve
+00000850: 6c6f 706d 656e 742e 200d 0a0d 0a48 6f77  lopment. ....How
+00000860: 6576 6572 2c20 5665 7274 6963 6120 5351  ever, Vertica SQ
+00000870: 4c41 6c63 6865 6d79 2061 6c73 6f20 7072  LAlchemy also pr
+00000880: 6f76 6964 6573 2073 7065 6369 6669 6320  ovides specific 
+00000890: 7061 7261 6d65 7465 7273 2061 6e64 2062  parameters and b
+000008a0: 6568 6176 696f 722c 2077 6869 6368 2061  ehavior, which a
+000008b0: 7265 2064 6573 6372 6962 6564 2069 6e20  re described in 
+000008c0: 7468 6520 666f 6c6c 6f77 696e 6720 7365  the following se
+000008d0: 6374 696f 6e73 2e0d 0a0d 0a23 2323 2323  ctions.....#####
+000008e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008f0: 0d0a 436f 6e6e 6563 7469 6f6e 2050 6172  ..Connection Par
+00000900: 616d 6574 6572 730d 0a23 2323 2323 2323  ameters..#######
+00000910: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00000920: 0d0a 5665 7274 6963 6120 5351 4c41 6c63  ..Vertica SQLAlc
+00000930: 6865 6d79 2044 6961 6c65 6374 2075 7365  hemy Dialect use
+00000940: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+00000950: 7379 6e74 6178 2066 6f72 2074 6865 2063  syntax for the c
+00000960: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
+00000970: 2075 7365 6420 746f 2063 6f6e 6e65 6374   used to connect
+00000980: 2074 6f20 5665 7274 6963 6120 616e 6420   to Vertica and 
+00000990: 696e 6974 6961 7465 2061 2073 6573 7369  initiate a sessi
+000009a0: 6f6e 3a0d 0a3a 3a0d 0a0d 0a20 2020 2027  on:..::....    '
+000009b0: 7665 7274 6963 612b 7665 7274 6963 615f  vertica+vertica_
+000009c0: 7079 7468 6f6e 3a2f 2f3c 7573 6572 3e3a  python://<user>:
+000009d0: 3c70 6173 7377 6f72 643e 403c 686f 7374  <password>@<host
+000009e0: 5f6e 616d 653e 2f3c 6461 7461 6261 7365  _name>/<database
+000009f0: 5f6e 616d 653e 270d 0a0d 0a0d 0a57 6865  _name>'......Whe
+00000a00: 7265 3a0d 0a0d 0a2d 2060 3c75 7365 723e  re:....- `<user>
+00000a10: 6020 6973 2074 6865 206c 6f67 696e 206e  ` is the login n
+00000a20: 616d 6520 666f 7220 796f 7572 2056 6572  ame for your Ver
+00000a30: 7469 6361 2075 7365 722e 0d0a 2d20 603c  tica user...- `<
+00000a40: 7061 7373 776f 7264 3e60 2069 7320 7468  password>` is th
+00000a50: 6520 7061 7373 776f 7264 2066 6f72 2079  e password for y
+00000a60: 6f75 7220 5665 7274 6963 6120 7573 6572  our Vertica user
+00000a70: 2e0d 0a2d 2060 3c68 6f73 745f 6e61 6d65  ...- `<host_name
+00000a80: 3e60 2069 7320 7468 6520 4950 2f46 5144  >` is the IP/FQD
+00000a90: 4e20 6f66 2079 6f75 7220 5665 7274 6963  N of your Vertic
+00000aa0: 6120 486f 7374 2e0d 0a2d 2060 3c64 6174  a Host...- `<dat
+00000ab0: 6162 6173 655f 6e61 6d65 3e60 2069 7320  abase_name>` is 
+00000ac0: 7468 6520 6e61 6d65 206f 6620 796f 7572  the name of your
+00000ad0: 2056 6572 7469 6361 2044 6174 6162 6173   Vertica Databas
+00000ae0: 652e 0d0a 0d0a 0d0a 596f 7520 6361 6e20  e.......You can 
+00000af0: 6f70 7469 6f6e 616c 6c79 2073 7065 6369  optionally speci
+00000b00: 6679 2074 6865 2069 6e69 7469 616c 2064  fy the initial d
+00000b10: 6174 6162 6173 6520 616e 6420 7363 6865  atabase and sche
+00000b20: 6d61 2066 6f72 2074 6865 2056 6572 7469  ma for the Verti
+00000b30: 6361 2073 6573 7369 6f6e 2062 7920 696e  ca session by in
+00000b40: 636c 7564 696e 6720 7468 656d 2061 7420  cluding them at 
+00000b50: 7468 6520 656e 6420 6f66 2074 6865 2063  the end of the c
+00000b60: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
+00000b70: 2c20 7365 7061 7261 7465 6420 6279 2060  , separated by `
+00000b80: 2f60 2e20 596f 7520 6361 6e20 616c 736f  /`. You can also
+00000b90: 2073 7065 6369 6679 206f 7468 6572 2073   specify other s
+00000ba0: 7570 706f 7274 6564 2070 6172 616d 6574  upported paramet
+00000bb0: 6572 7320 6279 2076 6572 7469 6361 2d70  ers by vertica-p
+00000bc0: 7974 686f 6e20 6174 2074 6865 2065 6e64  ython at the end
+00000bd0: 206f 6620 7468 6520 636f 6e6e 6563 7469   of the connecti
+00000be0: 6f6e 2073 7472 696e 673a 0d0a 3a3a 0d0a  on string:..::..
+00000bf0: 0d0a 2020 2020 2776 6572 7469 6361 2b76  ..    'vertica+v
+00000c00: 6572 7469 6361 5f70 7974 686f 6e3a 2f2f  ertica_python://
+00000c10: 3c75 7365 723e 3a3c 7061 7373 776f 7264  <user>:<password
+00000c20: 3e40 3c68 6f73 745f 6e61 6d65 3e2f 3c64  >@<host_name>/<d
+00000c30: 6174 6162 6173 655f 6e61 6d65 3e3f 7365  atabase_name>?se
+00000c40: 7373 696f 6e5f 6c61 6265 6c3d 7371 6c61  ssion_label=sqla
+00000c50: 6c63 6865 6d79 2663 6f6e 6e65 6374 696f  lchemy&connectio
+00000c60: 6e5f 6c6f 6164 5f62 616c 616e 6365 3d31  n_load_balance=1
+00000c70: 270d 0a0d 0a46 6f72 206d 6f72 6520 696e  '....For more in
+00000c80: 666f 726d 6174 696f 6e2c 2063 6865 636b  formation, check
+00000c90: 206f 7574 2074 6865 2063 6f6e 6e65 6374   out the connect
+00000ca0: 696f 6e20 606f 7074 696f 6e73 203c 6874  ion `options <ht
+00000cb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000cc0: 2f76 6572 7469 6361 2f76 6572 7469 6361  /vertica/vertica
+00000cd0: 2d70 7974 686f 6e23 7365 742d 7072 6f70  -python#set-prop
+00000ce0: 6572 7469 6573 2d77 6974 682d 636f 6e6e  erties-with-conn
+00000cf0: 6563 7469 6f6e 2d73 7472 696e 673e 605f  ection-string>`_
+00000d00: 206f 6620 7665 7274 6963 612d 7079 7468   of vertica-pyth
+00000d10: 6f6e 2e0d 0a0d 0a23 2323 2323 2323 2323  on.....#########
+00000d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000d30: 2323 2323 230d 0a4f 7065 6e69 6e67 2061  #####..Opening a
+00000d40: 6e64 2043 6c6f 7369 6e67 2043 6f6e 6e65  nd Closing Conne
+00000d50: 6374 696f 6e0d 0a23 2323 2323 2323 2323  ction..#########
+00000d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000d70: 2323 2323 230d 0a0d 0a4f 7065 6e20 6120  #####....Open a 
+00000d80: 636f 6e6e 6563 7469 6f6e 2062 7920 6578  connection by ex
+00000d90: 6563 7574 696e 6720 6065 6e67 696e 652e  ecuting `engine.
+00000da0: 636f 6e6e 6563 7428 2960 3b20 6176 6f69  connect()`; avoi
+00000db0: 6420 7573 696e 6720 6065 6e67 696e 652e  d using `engine.
+00000dc0: 6578 6563 7574 6528 2960 2e20 4d61 6b65  execute()`. Make
+00000dd0: 2063 6572 7461 696e 2074 6f20 636c 6f73   certain to clos
+00000de0: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
+00000df0: 2062 7920 6578 6563 7574 696e 6720 6063   by executing `c
+00000e00: 6f6e 6e65 6374 696f 6e2e 636c 6f73 6528  onnection.close(
+00000e10: 2960 2062 6566 6f72 650d 0a60 656e 6769  )` before..`engi
+00000e20: 6e65 2e64 6973 706f 7365 2829 603b 206f  ne.dispose()`; o
+00000e30: 7468 6572 7769 7365 2c20 7468 6520 5079  therwise, the Py
+00000e40: 7468 6f6e 2047 6172 6261 6765 2063 6f6c  thon Garbage col
+00000e50: 6c65 6374 6f72 2072 656d 6f76 6573 2074  lector removes t
+00000e60: 6865 2072 6573 6f75 7263 6573 2072 6571  he resources req
+00000e70: 7569 7265 6420 746f 2063 6f6d 6d75 6e69  uired to communi
+00000e80: 6361 7465 2077 6974 6820 5665 7274 6963  cate with Vertic
+00000e90: 612c 2070 7265 7665 6e74 696e 6720 7468  a, preventing th
+00000ea0: 6520 5079 7468 6f6e 2063 6f6e 6e65 6374  e Python connect
+00000eb0: 6f72 2066 726f 6d20 636c 6f73 696e 6720  or from closing 
+00000ec0: 7468 6520 7365 7373 696f 6e20 7072 6f70  the session prop
+00000ed0: 6572 6c79 2e0d 0a0d 0a3a 3a0d 0a0d 0a20  erly.....::.... 
+00000ee0: 2020 2065 6e67 696e 6520 3d20 6372 6561     engine = crea
+00000ef0: 7465 5f65 6e67 696e 6528 2e2e 2e29 0d0a  te_engine(...)..
+00000f00: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
+00000f10: 2065 6e67 696e 652e 636f 6e6e 6563 7428   engine.connect(
+00000f20: 290d 0a20 2020 2074 7279 3a0d 0a20 2020  )..    try:..   
+00000f30: 2020 2020 2063 6f6e 6e65 6374 696f 6e2e       connection.
+00000f40: 6578 6563 7574 6528 3c53 514c 3e29 0d0a  execute(<SQL>)..
+00000f50: 2020 2020 6669 6e61 6c6c 793a 0d0a 2020      finally:..  
+00000f60: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+00000f70: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
+00000f80: 2020 656e 6769 6e65 2e64 6973 706f 7365    engine.dispose
+00000f90: 2829 0d0a 0d0a 0d0a 2a2a 5573 696e 6720  ()......**Using 
+00000fa0: 7079 6f64 6263 2069 6e73 7465 6164 206f  pyodbc instead o
+00000fb0: 6620 7665 7274 6963 612d 7079 7468 6f6e  f vertica-python
+00000fc0: 2a2a 0d0a 0d0a 596f 7520 6d61 7920 7573  **....You may us
+00000fd0: 6520 7079 6f64 6263 2069 6e73 7465 6164  e pyodbc instead
+00000fe0: 206f 6620 7665 7274 6963 612d 7079 7468   of vertica-pyth
+00000ff0: 6f6e 2066 6f72 2074 6865 2063 6f6e 6e65  on for the conne
+00001000: 6374 696f 6e2e 0d0a 0d0a 2a43 7265 6174  ction.....*Creat
+00001010: 6520 6120 5665 7274 6963 6120 4453 4e2a  e a Vertica DSN*
+00001020: 200d 0a0d 0a0d 0a59 6f75 2077 696c 6c20   ......You will 
+00001030: 6e65 6564 2074 6f20 6861 7665 2061 2056  need to have a V
+00001040: 6572 7469 6361 204f 4442 4320 6472 6976  ertica ODBC driv
+00001050: 6572 2069 6e73 7461 6c6c 6564 2066 726f  er installed fro
+00001060: 6d20 6056 6572 7469 6361 2d43 6c69 656e  m `Vertica-Clien
+00001070: 742d 4472 6976 6572 7320 3c68 7474 7073  t-Drivers <https
+00001080: 3a2f 2f77 7777 2e76 6572 7469 6361 2e63  ://www.vertica.c
+00001090: 6f6d 2f64 6f77 6e6c 6f61 642f 7665 7274  om/download/vert
+000010a0: 6963 612f 636c 6965 6e74 2d64 7269 7665  ica/client-drive
+000010b0: 7273 2f3e 605f 2e20 466f 7220 7374 6570  rs/>`_. For step
+000010c0: 7320 746f 2069 6e73 7461 6c6c 204f 4442  s to install ODB
+000010d0: 4320 666f 7220 5665 7274 6963 612c 2066  C for Vertica, f
+000010e0: 6f6c 6c6f 7720 6f66 6669 6369 616c 2060  ollow official `
+000010f0: 5665 7274 6963 6120 446f 6373 203c 6874  Vertica Docs <ht
+00001100: 7470 733a 2f2f 7777 772e 7665 7274 6963  tps://www.vertic
+00001110: 612e 636f 6d2f 646f 6373 2f31 322e 302e  a.com/docs/12.0.
+00001120: 782f 4854 4d4c 2f43 6f6e 7465 6e74 2f41  x/HTML/Content/A
+00001130: 7574 686f 7269 6e67 2f43 6f6e 6e65 6374  uthoring/Connect
+00001140: 696e 6754 6f56 6572 7469 6361 2f43 6c69  ingToVertica/Cli
+00001150: 656e 744f 4442 432f 496e 7374 616c 6c69  entODBC/Installi
+00001160: 6e67 4f44 4243 2e68 746d 3e60 5f2e 0d0a  ngODBC.htm>`_...
+00001170: 0d0a 466f 7220 6578 616d 706c 652c 2079  ..For example, y
+00001180: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
+00001190: 636f 6e66 6967 7572 6520 7468 6573 6520  configure these 
+000011a0: 6669 6c65 7320 7769 7468 2079 6f75 7220  files with your 
+000011b0: 6372 6564 656e 7469 616c 733a 0d0a 0d0a  credentials:....
+000011c0: 602f 6574 632f 7665 7274 6963 612e 696e  `/etc/vertica.in
+000011d0: 6960 0d0a 3a3a 0d0a 0d0a 2020 2020 5b44  i`..::....    [D
+000011e0: 7269 7665 725d 0d0a 2020 2020 4572 726f  river]..    Erro
+000011f0: 724d 6573 7361 6765 7350 6174 6820 3d20  rMessagesPath = 
+00001200: 2f6f 7074 2f76 6572 7469 6361 2f6c 6962  /opt/vertica/lib
+00001210: 3634 2f0d 0a20 2020 204f 4442 4349 6e73  64/..    ODBCIns
+00001220: 744c 6962 203d 202f 7573 722f 6c69 622f  tLib = /usr/lib/
+00001230: 7838 365f 3634 2d6c 696e 7578 2d67 6e75  x86_64-linux-gnu
+00001240: 2f6c 6962 6f64 6263 696e 7374 2e73 6f0d  /libodbcinst.so.
+00001250: 0a20 2020 2044 7269 7665 724d 616e 6167  .    DriverManag
+00001260: 6572 456e 636f 6469 6e67 3d55 5446 2d31  erEncoding=UTF-1
+00001270: 360d 0a0d 0a0d 0a60 7e2f 2e6f 6462 632e  6......`~/.odbc.
+00001280: 696e 6960 0d0a 3a3a 0d0a 0d0a 2020 2020  ini`..::....    
+00001290: 5b4f 4442 4320 4461 7461 2053 6f75 7263  [ODBC Data Sourc
+000012a0: 6573 5d0d 0a20 2020 2076 6572 7469 6361  es]..    vertica
+000012b0: 203d 2022 4d79 2044 6174 6162 6173 6522   = "My Database"
+000012c0: 0d0a 0d0a 2020 2020 5b76 6572 7469 6361  ....    [vertica
+000012d0: 6473 6e5d 0d0a 2020 2020 4465 7363 7269  dsn]..    Descri
+000012e0: 7074 696f 6e20 3d20 4d79 2044 6174 6162  ption = My Datab
+000012f0: 6173 650d 0a20 2020 2044 7269 7665 7220  ase..    Driver 
+00001300: 3d20 2f6f 7074 2f76 6572 7469 6361 2f6c  = /opt/vertica/l
+00001310: 6962 3634 2f6c 6962 7665 7274 6963 616f  ib64/libverticao
+00001320: 6462 632e 736f 0d0a 2020 2020 4461 7461  dbc.so..    Data
+00001330: 6261 7365 203d 2064 6f63 6b65 720d 0a20  base = docker.. 
+00001340: 2020 2053 6572 7665 726e 616d 6520 3d20     Servername = 
+00001350: 3132 372e 302e 302e 310d 0a20 2020 2055  127.0.0.1..    U
+00001360: 4944 203d 2064 6261 646d 696e 0d0a 2020  ID = dbadmin..  
+00001370: 2020 5057 4420 3d0d 0a0d 0a0d 0a0d 0a54    PWD =........T
+00001380: 6865 6e20 7573 6520 7468 6520 5665 7274  hen use the Vert
+00001390: 6963 6120 4453 4e20 696e 2061 2066 696c  ica DSN in a fil
+000013a0: 6520 6c69 6b65 2073 6f3a 0d0a 3a3a 0d0a  e like so:..::..
+000013b0: 0d0a 2020 2020 6672 6f6d 2073 716c 616c  ..    from sqlal
+000013c0: 6368 656d 7920 696d 706f 7274 2063 7265  chemy import cre
+000013d0: 6174 655f 656e 6769 6e65 0d0a 0d0a 2020  ate_engine....  
+000013e0: 2020 656e 6769 6e65 203d 2073 612e 6372    engine = sa.cr
+000013f0: 6561 7465 5f65 6e67 696e 6528 2776 6572  eate_engine('ver
+00001400: 7469 6361 2b70 796f 6462 633a 2f2f 4076  tica+pyodbc://@v
+00001410: 6572 7469 6361 6473 6e27 290d 0a20 2020  erticadsn')..   
+00001420: 2074 7279 3a0d 0a20 2020 2020 2020 2072   try:..        r
+00001430: 6573 203d 2065 6e67 696e 652e 636f 6e6e  es = engine.conn
+00001440: 6563 7428 292e 7363 616c 6172 2827 7365  ect().scalar('se
+00001450: 6c65 6374 2076 6572 7369 6f6e 2829 3b27  lect version();'
+00001460: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00001470: 2872 6573 290d 0a20 2020 2066 696e 616c  (res)..    final
+00001480: 6c79 3a0d 0a20 2020 2020 2020 2063 6f6e  ly:..        con
+00001490: 6e65 6374 696f 6e2e 636c 6f73 6528 290d  nection.close().
+000014a0: 0a20 2020 2020 2020 2065 6e67 696e 652e  .        engine.
+000014b0: 6469 7370 6f73 6528 290d 0a0d 0a54 6869  dispose()....Thi
+000014c0: 7320 7368 6f75 6c64 2064 6973 706c 6179  s should display
+000014d0: 2074 6865 2056 6572 7469 6361 2076 6572   the Vertica ver
+000014e0: 7369 6f6e 2069 6e66 6f3a 2022 5665 7274  sion info: "Vert
+000014f0: 6963 6120 416e 616c 7974 6963 2044 6174  ica Analytic Dat
+00001500: 6162 6173 6520 7631 322e 302e 302d 3022  abase v12.0.0-0"
+00001510: 2e0d 0a                                  ...
```

### Comparing `vertica-sqlalchemy-dialect-0.0.2/setup.py` & `vertica-sqlalchemy-dialect-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from setuptools import setup
 
 with open("README.rst", "r") as f:
     description = f.read()
 
 
-version_info = (0, 0, 2)
+version_info = (0, 0, 3)
 
 version = '.'.join(map(str, version_info))
 
 setup(
     name='vertica-sqlalchemy-dialect',
     version=version,
     description='Official Vertica dialect for SQLalchemy',
```

### Comparing `vertica-sqlalchemy-dialect-0.0.2/test/test_core.py` & `vertica-sqlalchemy-dialect-0.0.3/test/test_core.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/test/test_integration.py` & `vertica-sqlalchemy-dialect-0.0.3/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/test/test_suite.py` & `vertica-sqlalchemy-dialect-0.0.3/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/base.py` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/base.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/dialect_pyodbc.py` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_pyodbc.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/dialect_vertica_python.py` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_vertica_python.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect/requirements.py` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/requirements.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.2
+Version: 0.0.3
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
@@ -24,15 +24,15 @@
 Prerequisites
 -------------
 
 You will need the following softwares to run, build and test the dialect. Everything apart from Python and pip can be installed via pip itself.
 
 1. Python 3.x or higher
 2. pip 22 or higher
-3. SQLAlchemy > 1.3.24 and < 2.0
+3. SQLAlchemy 1.4.48
 4. vertica-python 1.1.1 or higher
 
 #####################################
 Vertica-Python
 #####################################
 
 `vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.2/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt` & `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

