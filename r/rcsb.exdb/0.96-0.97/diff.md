# Comparing `tmp/rcsb.exdb-0.96.tar.gz` & `tmp/rcsb.exdb-0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.exdb-0.96.tar", last modified: Thu Apr 13 21:42:14 2023, max compression
+gzip compressed data, was "rcsb.exdb-0.97.tar", last modified: Mon Jun  5 14:33:10 2023, max compression
```

## Comparing `rcsb.exdb-0.96.tar` & `rcsb.exdb-0.97.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/
--rw-r--r--   0 vsts      (1001) docker     (122)     7244 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/exdb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/exdb/branch/
--rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/BranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/GlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/citation/
--rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/cli/ExDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/entry/
--rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/entry/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/entry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.507021 rcsb.exdb-0.96/rcsb/exdb/seq/
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/AnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/PolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/TaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/UniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/UniProtExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9677 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/fixturePdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testAnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testBranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5268 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testTaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3557 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testTreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtExtractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/tree/
--rw-r--r--   0 vsts      (1001) docker     (122)    11987 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tree/TreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tree/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectValidator.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)     2486 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10714 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/ExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2736 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/GlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10388 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/PubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb.exdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 21:14:08.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7326 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/exdb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb/exdb/branch/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/BranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/GlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/branch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/citation/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/CitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/cli/ExDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.563758 rcsb.exdb-0.97/rcsb/exdb/entry/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/entry/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/entry/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.567757 rcsb.exdb-0.97/rcsb/exdb/seq/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/AnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/PolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/TaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/UniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/UniProtExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9677 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/fixturePdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testAnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testBranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testCitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5268 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testTaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3557 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testTreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtExtractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/tree/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11987 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tree/TreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/tree/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/ObjectValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/rcsb/exdb/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2570 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10714 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/ExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2820 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/GlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10473 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/PubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/rcsb/exdb/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:33:10.559757 rcsb.exdb-0.97/rcsb.exdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:05:52.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-05 14:33:10.000000 rcsb.exdb-0.97/rcsb.exdb.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-05 14:33:10.575757 rcsb.exdb-0.97/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-06-05 13:59:25.000000 rcsb.exdb-0.97/setup.py
```

### Comparing `rcsb.exdb-0.96/HISTORY.txt` & `rcsb.exdb-0.97/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,8 +85,9 @@
                   Fix test case in testObjectExtractor;
                   Switch fixturePdbxLoader to use remote HTTP loading for Azure tests instead of local mock/sandbox paths
 25-May-2022 V0.92 Add error checking for SIFTS data loading in ReferenceSequenceAnnotationProvider and ReferenceSequenceAssignmentProvider
  9-Jan-2023 V0.93 Configuration changes to support tox 4
  9-Mar-2023 V0.94 Update ExDbWorkflow to make use of multiple processors for 'upd_ref_seq' operation;
                   Lower refChunkSize to 10 for requests to UniProt API
 13-Mar-2023 V0.95 Updates to PubChem workflow to use multiprocess count, disable git stash testing, remove obsolete entries from test data
-12-Apr-2023 V0.96 Add CARD ontology data to tree builder
+12-Apr-2023 V0.96 Add CARD ontology data to tree builder
+ 1-Jun-2023 V0.97 Don't back up resources to GitHub during cache update workflows
```

### Comparing `rcsb.exdb-0.96/LICENSE` & `rcsb.exdb-0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/PKG-INFO` & `rcsb.exdb-0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.96
+Version: 0.97
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.96/README.md` & `rcsb.exdb-0.97/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/branch/BranchedEntityExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/branch/BranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/branch/GlycanProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/branch/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/branch/GlycanUtils.py` & `rcsb.exdb-0.97/rcsb/exdb/branch/GlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefEtlWorker.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefMappingProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/ChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemDataCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemEtlWrapper.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemIndexCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/chemref/PubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/citation/CitationAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/citation/CitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/citation/CitationExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/citation/CitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/citation/CitationUtils.py` & `rcsb.exdb-0.97/rcsb/exdb/citation/CitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/cli/ExDbExec.py` & `rcsb.exdb-0.97/rcsb/exdb/cli/ExDbExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/entry/EntryInfoProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/entry/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/AnnotationExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/AnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/LigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/PolymerEntityExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/PolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/TaxonomyExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/TaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/UniProtCoreEtlWorker.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/UniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/seq/UniProtExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/seq/UniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/fixturePdbxLoader.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/fixturePdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testAnnotationExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testAnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testBranchedEntityExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testBranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefLoader.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefMappingProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationUtils.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testCitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testEntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testExDbWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanUtils.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testGlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testLigandNeighborMappingProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testLigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectTransformer.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectUpdater.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testPolymerEntityExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testPolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemDataCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWrapper.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemIndexCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testPubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testTaxonomyExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testTaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testTreeNodeListWorker.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testTreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtCoreEtlWorker.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/tests/testUniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/tree/TreeNodeListWorker.py` & `rcsb.exdb-0.97/rcsb/exdb/tree/TreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectExtractor.py` & `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectTransformer.py` & `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectUpdater.py` & `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectValidator.py` & `rcsb.exdb-0.97/rcsb/exdb/utils/ObjectValidator.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/wf/EntryInfoEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/wf/EntryInfoEtlWorkflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 # File: EntryInfoEtlWorkflow.py
 # Date: 22-Sep-2021  jdw
 #
 #  Workflow wrapper  --  Entry-level annotations extracted from ExDB
 #
 #  Updates:
+#   1-Jun-2023 aae Don't back up resources to GitHub during cache update workflows
 #
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
@@ -55,15 +56,15 @@
         """
         try:
             ok = False
             eiP = EntryInfoProvider(cachePath=self.__cachePath, useCache=True)
             eiP.update(self.__cfgOb, fmt="json", indent=3)
             #
             if backup:
-                ok = eiP.backup(self.__cfgOb, self.__configName, self.__stashRemotePrefix, useGit=True, useStash=True)
+                ok = eiP.backup(self.__cfgOb, self.__configName, self.__stashRemotePrefix, useGit=False, useStash=True)
                 logger.info("Backup entry-level annotations (%r)", ok)
             else:
                 ok = True
 
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         #
```

### Comparing `rcsb.exdb-0.96/rcsb/exdb/wf/ExDbWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/wf/ExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/rcsb/exdb/wf/GlycanEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/wf/GlycanEtlWorkflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 # File: GlycanEtlWorkflow.py
 # Date: 30-Jun-2021  jdw
 #
 #  Workflow wrapper  --  Glycan ETL utilities
 #
 #  Updates:
+#   1-Jun-2023 aae Don't back up resources to GitHub during cache update workflows
 #
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
@@ -60,15 +61,15 @@
             logger.info("Restore glycan matched identifiers status (%r)", ok)
 
             ok1 = gP.update(self.__cfgOb, fmt="json", indent=3)
             riD = gP.getIdentifiers()
             logger.info("Matched glycan identifiers (%d)", len(riD))
             #
             if backup:
-                ok2 = gP.backup(self.__cfgOb, self.__configName, self.__stashRemotePrefix, useGit=True, useStash=True)
+                ok2 = gP.backup(self.__cfgOb, self.__configName, self.__stashRemotePrefix, useGit=False, useStash=True)
                 logger.info("Backup matched glycan identifiers (%r)", ok2)
             else:
                 ok2 = True
 
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         #
```

### Comparing `rcsb.exdb-0.96/rcsb/exdb/wf/PubChemEtlWorkflow.py` & `rcsb.exdb-0.97/rcsb/exdb/wf/PubChemEtlWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # File: PubChemEtlWorkflow.py
 # Date: 28-Jul-2020  jdw
 #
 #  Workflow wrapper  --  PubChem ETL utilities
 #
 #  Updates:
 #  13-Mar-2023 aae Updates to use multiprocess count, disable git stash testing
+#   1-Jun-2023 aae Don't back up resources to GitHub during cache update workflows
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
@@ -164,15 +165,15 @@
             birdUrlTarget = kwargs.get("birdUrlTarget", None)
             ccFileNamePrefix = kwargs.get("ccFileNamePrefix", "cc-full")
             numProcChemComp = kwargs.get("numProcChemComp", 8)
             numProc = kwargs.get("numProc", 2)
             rebuildChemIndices = kwargs.get("rebuildChemIndices", True)
             exportPath = kwargs.get("exportPath", None)
             useStash = kwargs.get("useStash", True)
-            useGit = kwargs.get("useGit", True)
+            useGit = kwargs.get("useGit", False)
             #
             pcewP = PubChemEtlWrapper(self.__cfgOb, self.__cachePath, stashRemotePrefix=self.__stashRemotePrefix)
             ok1 = pcewP.updateIndex(
                 ccUrlTarget=ccUrlTarget,
                 birdUrlTarget=birdUrlTarget,
                 ccFileNamePrefix=ccFileNamePrefix,
                 exportPath=exportPath,
@@ -203,15 +204,15 @@
             (bool): True for success or False otherwise
         """
         try:
             ok1 = ok2 = ok3 = ok4 = ok5 = ok6 = False
             #  --
             numProc = kwargs.get("numProc", 2)
             useStash = kwargs.get("useStash", True)
-            useGit = kwargs.get("useGit", True)
+            useGit = kwargs.get("useGit", False)
             #
             pcewP = PubChemEtlWrapper(self.__cfgOb, self.__cachePath, stashRemotePrefix=self.__stashRemotePrefix)
             ok1 = pcewP.updateMatchedData(numProc=numProc)
             ok2 = pcewP.dump(contentType="data")
             if useGit or useStash:
                 ok3 = pcewP.toStash(contentType="data", useStash=useStash, useGit=useGit)
             else:
```

### Comparing `rcsb.exdb-0.96/rcsb.exdb.egg-info/PKG-INFO` & `rcsb.exdb-0.97/rcsb.exdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.96
+Version: 0.97
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.96/rcsb.exdb.egg-info/SOURCES.txt` & `rcsb.exdb-0.97/rcsb.exdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.96/setup.py` & `rcsb.exdb-0.97/setup.py`

 * *Files identical despite different names*

