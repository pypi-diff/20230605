# Comparing `tmp/sbtab-1.0.6.tar.gz` & `tmp/sbtab-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbtab-1.0.6.tar", last modified: Mon May 17 11:15:20 2021, max compression
+gzip compressed data, was "sbtab-1.0.7.tar", last modified: Mon Jun  5 07:38:56 2023, max compression
```

## Comparing `sbtab-1.0.6.tar` & `sbtab-1.0.7.tar`

### file list

```diff
@@ -1,45 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-17 11:15:20.000000 sbtab-1.0.6/
--rw-rw-r--   0 root         (0) root         (0)      107 2020-11-18 09:25:32.000000 sbtab-1.0.6/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      780 2021-05-17 11:14:29.000000 sbtab-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1352 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      562 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)      353 2018-10-05 14:26:28.000000 sbtab-1.0.6/README.rst
--rw-rw-r--   0 root         (0) root         (0)     1170 2020-11-18 09:15:52.000000 sbtab-1.0.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      205 2021-05-17 11:15:20.000000 sbtab-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2021-05-17 11:15:20.000000 sbtab-1.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab/
--rw-rw-r--   0 root         (0) root         (0)     5771 2018-10-25 07:40:01.000000 sbtab-1.0.6/sbtab/sbtab2html.py
--rwxrwxr-x   0 root         (0) root         (0)    49422 2021-05-17 11:14:57.000000 sbtab-1.0.6/sbtab/SBtab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab/__pycache__/
--rw-rw-r--   0 root         (0) root         (0)      501 2018-10-25 07:59:09.000000 sbtab-1.0.6/sbtab/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)    31812 2018-11-09 10:27:48.000000 sbtab-1.0.6/sbtab/__pycache__/SBtab.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)     4841 2018-10-25 07:59:09.000000 sbtab-1.0.6/sbtab/__pycache__/sbtab2html.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)    18686 2018-10-25 07:59:09.000000 sbtab-1.0.6/sbtab/__pycache__/sbml2sbtab.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)    33097 2018-10-25 07:59:09.000000 sbtab-1.0.6/sbtab/__pycache__/sbtab2sbml.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)    10563 2018-10-25 07:59:09.000000 sbtab-1.0.6/sbtab/__pycache__/validatorSBtab.cpython-35.pyc
--rw-rw-r--   0 root         (0) root         (0)     9643 2018-11-09 10:24:55.000000 sbtab-1.0.6/sbtab/__pycache__/misc.cpython-35.pyc
--rwxrwxr-x   0 root         (0) root         (0)    38566 2020-11-06 12:59:03.000000 sbtab-1.0.6/sbtab/sbml2sbtab.py
--rw-rw-r--   0 root         (0) root         (0)    27414 2020-11-10 14:25:17.000000 sbtab-1.0.6/sbtab/definitions.tsv
--rw-rw-r--   0 root         (0) root         (0)        6 2021-05-17 11:14:26.000000 sbtab-1.0.6/sbtab/VERSION
--rwxrwxr-x   0 root         (0) root         (0)    78105 2020-07-21 12:35:53.000000 sbtab-1.0.6/sbtab/sbtab2sbml.py
--rwxrwxr-x   0 root         (0) root         (0)    13859 2020-08-07 12:16:29.000000 sbtab-1.0.6/sbtab/validatorSBtab.py
--rw-rw-r--   0 root         (0) root         (0)      253 2018-10-25 07:50:18.000000 sbtab-1.0.6/sbtab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-17 11:15:20.000000 sbtab-1.0.6/sbtab/sbtab_examples/
--rw-rw-r--   0 root         (0) root         (0)      207 2019-11-25 09:51:36.000000 sbtab-1.0.6/sbtab/sbtab_examples/Feed-forward-loop_Relationship.tsv
--rw-rw-r--   0 root         (0) root         (0)    55262 2020-11-17 10:28:21.000000 sbtab-1.0.6/sbtab/sbtab_examples/ecoli_ccm_aerobic_ModelData.tsv
--rw-rw-r--   0 root         (0) root         (0)      284 2020-11-17 10:29:08.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Compartment.tsv
--rw-rw-r--   0 root         (0) root         (0)      433 2020-11-17 10:28:40.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Quantity-parameters.tsv
--rw-rw-r--   0 root         (0) root         (0)      306 2020-11-17 10:28:51.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Enzyme.tsv
--rw-rw-r--   0 root         (0) root         (0)      199 2020-11-17 10:26:25.000000 sbtab-1.0.6/sbtab/sbtab_examples/LacOperon_Regulator.tsv
--rw-rw-r--   0 root         (0) root         (0)     6894 2020-11-17 10:26:17.000000 sbtab-1.0.6/sbtab/sbtab_examples/SBtab_specification_example_tables.tsv
--rw-rw-r--   0 root         (0) root         (0)    50088 2020-11-17 10:23:00.000000 sbtab-1.0.6/sbtab/sbtab_examples/yeast_transcription_network_chang_2008.tsv
--rw-rw-r--   0 root         (0) root         (0)      437 2020-11-17 10:28:47.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Quantity-concentration.tsv
--rw-rw-r--   0 root         (0) root         (0)      259 2020-11-17 10:26:35.000000 sbtab-1.0.6/sbtab/sbtab_examples/LacOperon_Gene.tsv
--rw-rw-r--   0 root         (0) root         (0)      478 2020-11-17 10:28:32.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Reaction.tsv
--rw-rw-r--   0 root         (0) root         (0)      436 2020-11-17 10:28:57.000000 sbtab-1.0.6/sbtab/sbtab_examples/BIOMD0000000061_Compound.tsv
--rw-rw-r--   0 root         (0) root         (0)   210892 2020-11-17 10:27:03.000000 sbtab-1.0.6/sbtab/sbtab_examples/kegg_reactions_CC_ph7.0.tsv
--rwxrwxr-x   0 root         (0) root         (0)    16263 2021-05-11 07:24:06.000000 sbtab-1.0.6/sbtab/misc.py
+drwxrwxr-x   0 timo      (1000) timo      (1000)        0 2023-06-05 07:38:56.515597 sbtab-1.0.7/
+-rw-rw-r--   0 timo      (1000) timo      (1000)     1170 2023-06-05 07:29:55.000000 sbtab-1.0.7/LICENSE
+-rw-rw-r--   0 timo      (1000) timo      (1000)      107 2023-06-05 07:29:55.000000 sbtab-1.0.7/MANIFEST.in
+-rw-rw-r--   0 timo      (1000) timo      (1000)      573 2023-06-05 07:38:56.515597 sbtab-1.0.7/PKG-INFO
+-rwxrwxr-x   0 timo      (1000) timo      (1000)      353 2023-06-05 07:29:55.000000 sbtab-1.0.7/README.rst
+drwxrwxr-x   0 timo      (1000) timo      (1000)        0 2023-06-05 07:38:56.511597 sbtab-1.0.7/sbtab/
+-rwxrwxr-x   0 timo      (1000) timo      (1000)    49319 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/SBtab.py
+-rw-rw-r--   0 timo      (1000) timo      (1000)        6 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/VERSION
+-rw-rw-r--   0 timo      (1000) timo      (1000)      253 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/__init__.py
+-rw-rw-r--   0 timo      (1000) timo      (1000)    27414 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/definitions.tsv
+-rwxrwxr-x   0 timo      (1000) timo      (1000)    16263 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/misc.py
+-rwxrwxr-x   0 timo      (1000) timo      (1000)    38566 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbml2sbtab.py
+-rw-rw-r--   0 timo      (1000) timo      (1000)     8890 2023-06-05 07:38:14.000000 sbtab-1.0.7/sbtab/sbtab2html.py
+-rwxrwxr-x   0 timo      (1000) timo      (1000)    78105 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab2sbml.py
+drwxrwxr-x   0 timo      (1000) timo      (1000)        0 2023-06-05 07:38:56.515597 sbtab-1.0.7/sbtab/sbtab_examples/
+-rw-rw-r--   0 timo      (1000) timo      (1000)      284 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Compartment.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      436 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Compound.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      306 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Enzyme.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      437 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Quantity-concentration.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      433 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Quantity-parameters.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      478 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/BIOMD0000000061_Reaction.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      207 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/Feed-forward-loop_Relationship.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      259 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/LacOperon_Gene.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)      199 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/LacOperon_Regulator.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)     6894 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/SBtab_specification_example_tables.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)    55262 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/ecoli_ccm_aerobic_ModelData.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)   210892 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/kegg_reactions_CC_ph7.0.tsv
+-rw-rw-r--   0 timo      (1000) timo      (1000)    50088 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/sbtab_examples/yeast_transcription_network_chang_2008.tsv
+-rwxrwxr-x   0 timo      (1000) timo      (1000)    13859 2023-06-05 07:29:55.000000 sbtab-1.0.7/sbtab/validatorSBtab.py
+drwxrwxr-x   0 timo      (1000) timo      (1000)        0 2023-06-05 07:38:56.511597 sbtab-1.0.7/sbtab.egg-info/
+-rw-rw-r--   0 timo      (1000) timo      (1000)      573 2023-06-05 07:38:56.000000 sbtab-1.0.7/sbtab.egg-info/PKG-INFO
+-rw-rw-r--   0 timo      (1000) timo      (1000)     1053 2023-06-05 07:38:56.000000 sbtab-1.0.7/sbtab.egg-info/SOURCES.txt
+-rw-rw-r--   0 timo      (1000) timo      (1000)        1 2023-06-05 07:38:56.000000 sbtab-1.0.7/sbtab.egg-info/dependency_links.txt
+-rw-rw-r--   0 timo      (1000) timo      (1000)       76 2023-06-05 07:38:56.000000 sbtab-1.0.7/sbtab.egg-info/requires.txt
+-rw-rw-r--   0 timo      (1000) timo      (1000)        6 2023-06-05 07:38:56.000000 sbtab-1.0.7/sbtab.egg-info/top_level.txt
+-rw-rw-r--   0 timo      (1000) timo      (1000)      205 2023-06-05 07:38:56.515597 sbtab-1.0.7/setup.cfg
+-rw-rw-r--   0 timo      (1000) timo      (1000)      780 2023-06-05 07:31:30.000000 sbtab-1.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sbtab-1.0.6/setup.py` & `sbtab-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 Setup file for SBtab Python Modules.
 The SBtab modules can be integrated into existing workflows of Systems Biology.
 See: https://bitbucket.org/tlubitz/sbtab
 
 """
 from setuptools import setup,find_packages
 
-setup(name='sbtab',version='1.0.6',description='SBtab - Standardised Data Tables for Systems Biology',long_description='SBtab - Standardised Data Tables for Systems Biology',url='https://www.sbtab.net',author='Timo Lubitz',author_email='timo.lubitz@gmail.com',license='MIT',classifiers=['Development Status :: 4 - Beta','Intended Audience :: Developers', 'Topic :: Software Development', 'Programming Language :: Python :: 3.0'],keywords='modelling systems biology standard format data table',packages=find_packages(),python_requires='>=3.0',include_package_data=True)
+setup(name='sbtab',version='1.0.7',description='SBtab - Standardised Data Tables for Systems Biology',long_description='SBtab - Standardised Data Tables for Systems Biology',url='https://www.sbtab.net',author='Timo Lubitz',author_email='timo.lubitz@gmail.com',license='MIT',classifiers=['Development Status :: 4 - Beta','Intended Audience :: Developers', 'Topic :: Software Development', 'Programming Language :: Python :: 3.0'],keywords='modelling systems biology standard format data table',packages=find_packages(),python_requires='>=3.0',include_package_data=True)
```

### Comparing `sbtab-1.0.6/sbtab.egg-info/PKG-INFO` & `sbtab-1.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sbtab
-Version: 1.0.6
+Version: 1.0.7
 Summary: SBtab - Standardised Data Tables for Systems Biology
 Home-page: https://www.sbtab.net
 Author: Timo Lubitz
 Author-email: timo.lubitz@gmail.com
 License: MIT
-Description: SBtab - Standardised Data Tables for Systems Biology
 Keywords: modelling systems biology standard format data table
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.0
 Requires-Python: >=3.0
+License-File: LICENSE
+
+SBtab - Standardised Data Tables for Systems Biology
+
```

### Comparing `sbtab-1.0.6/LICENSE` & `sbtab-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/PKG-INFO` & `sbtab-1.0.7/sbtab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sbtab
-Version: 1.0.6
+Version: 1.0.7
 Summary: SBtab - Standardised Data Tables for Systems Biology
 Home-page: https://www.sbtab.net
 Author: Timo Lubitz
 Author-email: timo.lubitz@gmail.com
 License: MIT
-Description: SBtab - Standardised Data Tables for Systems Biology
 Keywords: modelling systems biology standard format data table
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.0
 Requires-Python: >=3.0
+License-File: LICENSE
+
+SBtab - Standardised Data Tables for Systems Biology
+
```

### Comparing `sbtab-1.0.6/sbtab/sbtab2html.py` & `sbtab-1.0.7/sbtab/sbtab2html.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,18 +4,105 @@
 
 Python script that converts SBtab file/s to HTML.
 """
 #!/usr/bin/env python
 import re
 import string
 import sys
+import os
 from . import misc
+from . import SBtab
+
+
 
 urns = ["obo.chebi","kegg.compound","kegg.reaction","obo.go","obo.sgd","biomodels.sbo","ec-code","kegg.orthology","uniprot"]
 
+class SBtabError(Exception):
+    '''
+    Base class for errors in the SBtab class.
+    '''
+    def __init__(self, message):
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
+
+def write_html(sbtab, name, template, links, pageheader, definitions_file, show_table_text=True, show_units=False):
+    '''
+    calls the sbtab_to_html function and writes the HTML to disk
+    '''
+    html = misc.sbtab_to_html(sbtab, mode='standalone',template=template, put_links = links, title_string=pageheader, show_header_row=False, show_table_name=True, show_table_text=show_table_text, show_units=show_units, definitions_file = definitions_file)
+    h = open(name, 'w')
+    h.write(html)
+    h.close()
+
+
+def sbtab2html_wrapper(sbtab, multiple, output, template, links, pageheader, definitions_file=None, show_table_text=True, show_units=False):
+    '''
+    commandline wrapper for sbtab_to_html function
+    '''
+
+    # open and create SBtab
+    try:
+        f = open(sbtab, 'r').read()
+    except:
+        raise SBtabError('SBtab file %s could not be found.' % sbtab)
+    
+    # count given tabs and prepare file name w/o path
+    tab_amount = misc.count_tabs(f)
+    if '/' in sbtab:
+        name_pre = sbtab.split('/')[-1:]
+    else:
+        name_pre = sbtab
+
+    # count given tabs and prepare file name w/o path
+    if output is not None:
+        outfile_dir, outfile_file = os.path.split(output)
+        if len(outfile_dir)==0:
+            outfile_dir = '.'
+        elif not os.path.exists(outfile_dir):
+            os.mkdir(outfile_dir)
+        outfile_file=os.path.splitext(outfile_file)[0]
+        name_pre[0] = outfile_file
+    else:
+        outfile_dir = '.'
+
+    file_basename = os.path.splitext(name_pre[0])[0]
+
+    if tab_amount > 1:
+        multiple = True
+
+    if multiple:
+        try:
+            sbtab_doc = SBtab.SBtabDocument('sbtab_doc_prelim', f, sbtab, definitions_file = definitions_file)
+            for tab in sbtab_doc.sbtabs:
+                if len(file_basename):
+                    name = outfile_dir + '/' + file_basename + '_' + tab.table_id + '.html'
+                else:
+                    name = outfile_dir + '/' + tab.table_id + '.html'
+                try:
+                    write_html(tab, name, template, links, pageheader, definitions_file, show_table_text, show_units)
+                except:
+                    raise SBtabError('The HTML file %s could not be created.' % name)
+        except:
+            raise SBtabError('The multiple HTML files could not be created.')
+    else:
+        try:
+            if tab_amount > 1:
+                sbtab = SBtab.SBtabDocument('sbtab_doc_prelim', f, sbtab)
+                name = outfile_dir + '/' + file_basename + '_' + sbtab.table_id + '.html'
+            else:
+                sbtab = SBtab.SBtabTable(f, sbtab)
+                name = outfile_dir + '/' + file_basename + '.html'
+            write_html(sbtab, name, template, links, pageheader, definitions_file, show_table_text, show_units)
+        except:
+            raise SBtabError('The HTML file could not be created.')
+
+
 def csv2html(sbtab_file,file_name,definition_file=None,sbtype=None):
     '''
     Generates html view out of csv file.
 
     Parameters
     ----------
     sbtab_file : str
```

### Comparing `sbtab-1.0.6/sbtab/SBtab.py` & `sbtab-1.0.7/sbtab/SBtab.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
 
         Returns: str
             The SBtab table in form of a string.
         '''
         table_string = [self.header_row]
         table_string.append('\t'.join(self.columns))
         for row in self.value_rows:
-            row = '\t'.join(str(p) for p in row)
+            row = '\t'.join(row)
             table_string.append(row)
             
         return '\n'.join(table_string)
     
     def change_attribute(self, attribute, value):
         '''
         Changes the value of an SBtab attribute.
@@ -849,30 +849,29 @@
         # Overwrite old table data
         self.columns = trans_columns
         self.columns_dict = trans_columns_dict
         self.value_rows = trans_value_rows
 
         return True
     
-    def to_data_frame(self, rba=False):
+    def to_data_frame(self):
         '''
         Exports SBtab table object as pandas dataframe.
 
         Returns: pandas.DataFrame
             SBtab table object as pandas dataframe.
         '''
         try:
             import pandas as pd
-            rows = self.value_rows
+            rows = self._get_rows()
             n_cols = max(map(len, rows))
-            if rba: column_names = list(map(lambda s: s, self.columns))
-            else: column_names = list(map(lambda s: s[1:], self.columns))
+            column_names = list(map(lambda s: s[1:], self.columns))
             while len(column_names) < n_cols:
                 column_names += ['Col%d' % len(column_names)]
-            df = pd.DataFrame(data=self.value_rows, columns=column_names)
+            df = pd.DataFrame(data=self._get_rows(), columns=column_names)
             return df
         except:
             raise SBtabError('Pandas dataframe could not be built.')
 
     @staticmethod
     def from_data_frame(
         df,
```

### Comparing `sbtab-1.0.6/sbtab/sbml2sbtab.py` & `sbtab-1.0.7/sbtab/sbml2sbtab.py`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/definitions.tsv` & `sbtab-1.0.7/sbtab/definitions.tsv`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/sbtab2sbml.py` & `sbtab-1.0.7/sbtab/sbtab2sbml.py`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/validatorSBtab.py` & `sbtab-1.0.7/sbtab/validatorSBtab.py`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/sbtab_examples/ecoli_ccm_aerobic_ModelData.tsv` & `sbtab-1.0.7/sbtab/sbtab_examples/ecoli_ccm_aerobic_ModelData.tsv`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/sbtab_examples/SBtab_specification_example_tables.tsv` & `sbtab-1.0.7/sbtab/sbtab_examples/SBtab_specification_example_tables.tsv`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/sbtab_examples/yeast_transcription_network_chang_2008.tsv` & `sbtab-1.0.7/sbtab/sbtab_examples/yeast_transcription_network_chang_2008.tsv`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/sbtab_examples/kegg_reactions_CC_ph7.0.tsv` & `sbtab-1.0.7/sbtab/sbtab_examples/kegg_reactions_CC_ph7.0.tsv`

 * *Files identical despite different names*

### Comparing `sbtab-1.0.6/sbtab/misc.py` & `sbtab-1.0.7/sbtab/misc.py`

 * *Files identical despite different names*

