# Comparing `tmp/rcsb.workflow-0.39.tar.gz` & `tmp/rcsb.workflow-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.workflow-0.39.tar", last modified: Tue May 23 16:05:39 2023, max compression
+gzip compressed data, was "rcsb.workflow-0.40.tar", last modified: Mon Jun  5 14:55:07 2023, max compression
```

## Comparing `rcsb.workflow-0.39.tar` & `rcsb.workflow-0.40.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/
--rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.295165 rcsb.workflow-0.39/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/chem/
--rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompFileWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompImageWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb/workflow/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28640 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/rcsb/workflow/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/rcsb.workflow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:05:38.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-23 16:05:39.000000 rcsb.workflow-0.39/rcsb.workflow.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-23 16:05:39.299165 rcsb.workflow-0.39/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-05-23 15:23:04.000000 rcsb.workflow-0.39/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2425 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.705616 rcsb.workflow-0.40/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/chem/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompFileWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompImageWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28750 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb.workflow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:55:06.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/setup.py
```

### Comparing `rcsb.workflow-0.39/HISTORY.txt` & `rcsb.workflow-0.40/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 26-Aug-2021 - V0.32 Update dependencies
 27-Jun-2022 - V0.33 Change the molBuildType value from "model-xyz" to "connection-table" in ChemCompImageWorkflow()
  9-Jan-2023 - V0.34 Configuration changes to support tox 4
  3-Mar-2023 - V0.35 Standardize args in ProteinTargetSequenceExecutionWorkflow
 14-Mar-2023 - V0.36 Generate CARD annotations instead of features during ProteinTargetSequenceExecutionWorkflow
 21-Mar-2023 - V0.37 Allow backing up Pharos-targets to stash
  5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
-22-May-2023 - V0.39 Add retries to tox task for MMseqs2 download
+22-May-2023 - V0.39 Add retries to tox task for MMseqs2 download
+ 1-Jun-2023 - V0.40 Don't back up resources to GitHub during cache update workflows
```

### Comparing `rcsb.workflow-0.39/LICENSE` & `rcsb.workflow-0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/PKG-INFO` & `rcsb.workflow-0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.39/README.md` & `rcsb.workflow-0.40/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompFileWorkflow.py` & `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompFileWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompImageWorkflow.py` & `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompImageWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py` & `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py` & `rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py` & `rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #  Updates:
 #  25-Jul-2021 add new StashableBase options for git backup
 #  29-Jul-2021 DrugBankProvider needs useCache=False to always rebuild
 #   3-Mar-2023 Fix error for missing taxonPath
 #  14-Mar-2023 Generate CARD annotations instead of CARD features
 #  21-Mar-2023 Allow backing up Pharos-targets to stash
 #   5-May-2023 Restore from stash if fromDbPharos and reloadPharos parameters are False
+#   1-Jun-2023 aae Don't back up resources to GitHub during cache update workflows
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
@@ -62,27 +63,27 @@
 
     def exportRCSBChemRefMapping(self):
         """Export RCSB chemical reference data identifier mapping data"""
         ok = False
         try:
             crmP = ChemRefMappingProvider(self.__cachePath, useCache=False)
             okF = crmP.fetchChemRefMapping(self.__cfgOb)
-            okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=True)
+            okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
             ok = okF and okB
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
     def exportRCSBLigandNeighborMapping(self):
         """Export RCSB ligand neighbor mapping data"""
         ok = False
         try:
             crmP = LigandNeighborMappingProvider(self.__cachePath, useCache=False)
             okF = crmP.fetchLigandNeighborMapping(self.__cfgOb)
-            okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=True)
+            okB = crmP.backup(self.__cfgOb, self.__configName, useStash=True, useGit=False)
             ok = okF and okB
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
     def exportRCSBProteinEntityFasta(self, resourceName="pdbprent"):
         """Export RCSB protein entity sequence data (FASTA, taxon mapping, and essential details)"""
@@ -176,15 +177,15 @@
             elif resourceName == "pharos":
                 user = self.__cfgOb.get("_MYSQL_DB_USER_NAME", sectionName=configName)
                 pw = self.__cfgOb.get("_MYSQL_DB_PASSWORD", sectionName=configName)
                 ptP = PharosTargetProvider(cachePath=self.__cachePath, useCache=useCache, reloadDb=reloadPharos, fromDb=fromDbPharos, mysqlUser=user, mysqlPassword=pw)
                 if ptP.testCache():
                     ok = ptP.exportProteinFasta(fastaPath, taxonPath, addTaxonomy=addTaxonomy)
                     if backupPharos:
-                        okB = ptP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                        okB = ptP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                         logger.info("%r targets backup status (%r)", resourceName, okB)
                 elif not (reloadPharos or fromDbPharos):
                     ptP.restore(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
                     if ptP.testCache():
                         ok = ptP.exportProteinFasta(fastaPath, taxonPath, addTaxonomy=addTaxonomy)
             elif resourceName == "sabdab":
                 stP = SAbDabTargetProvider(cachePath=self.__cachePath, useCache=False)
@@ -336,27 +337,27 @@
             okB = True
             resultPath = self.__getFilteredSearchResultPath(resourceName, referenceResourceName)
             #
             if resourceName == "sabdab":
                 fP = SAbDabTargetFeatureProvider(cachePath=self.__cachePath, useCache=True)
                 ok = fP.buildFeatureList(resultPath)
                 if backup:
-                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r features backup status (%r)", resourceName, okB)
             elif resourceName == "card":
                 fP = CARDTargetAnnotationProvider(cachePath=self.__cachePath, useCache=True)
                 ok = fP.buildAnnotationList(resultPath, useTaxonomy=useTaxonomy)
                 if backup:
-                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r annotations backup status (%r)", resourceName, okB)
             elif resourceName == "imgt":
                 fP = IMGTTargetFeatureProvider(cachePath=self.__cachePath, useCache=True)
                 ok = fP.buildFeatureList(useCache=True)
                 if backup:
-                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = fP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r features backup status (%r)", resourceName, okB)
             return ok & okB
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
     def buildActivityData(self, referenceResourceName, resourceNameList=None, backup=False, remotePrefix=None, maxTargets=None):
@@ -403,28 +404,28 @@
                 except Exception:
                     pass
                 targetIdList = aP.getTargetIdList(resultPath)
                 targetIdList = targetIdList[:maxTargets] if maxTargets else targetIdList
                 ok = aP.fetchTargetActivityDataMulti(targetIdList, skip="tried", chunkSize=50, numProc=6)
                 #
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r activity backup status (%r)", resourceName, okB)
             elif resourceName == "pharos":
                 aP = PharosTargetActivityProvider(cachePath=self.__cachePath, useCache=True)
                 ok = aP.fetchTargetActivityData()
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r activity data backup status (%r)", resourceName, okB)
                 #
                 chemblIdList = aP.fetchCompoundIdentifiers()
                 phP = PharosProvider(cachePath=self.__cachePath, useCache=False)
                 phP.load(chemblIdList, "identifiers", fmt="json", indent=0)
                 if backup:
-                    okC = phP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okC = phP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r identifier backup status (%r)", resourceName, okC)
 
             return ok and okB and okC
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
 
@@ -468,29 +469,29 @@
             resultPath = self.__getFilteredSearchResultPath(resourceName, referenceResourceName)
             #
             if resourceName == "chembl":
                 aP = ChEMBLTargetCofactorProvider(cachePath=self.__cachePath, useCache=True)
                 ok = aP.buildCofactorList(resultPath, crmpObj=crmpObj, lnmpObj=lnmpObj, maxActivity=maxActivity)
                 #
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r cofactor backup status (%r)", resourceName, okB)
 
             elif resourceName == "pharos":
                 aP = PharosTargetCofactorProvider(cachePath=self.__cachePath, useCache=True, useStash=True, useGit=True)
                 ok = aP.buildCofactorList(resultPath, crmpObj=crmpObj, lnmpObj=lnmpObj, maxActivity=maxActivity)
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useGit=True)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r cofactor data backup status (%r)", resourceName, okB)
 
             elif resourceName == "drugbank":
                 aP = DrugBankTargetCofactorProvider(cachePath=self.__cachePath, useCache=True)
                 ok = aP.buildCofactorList(resultPath, crmpObj=crmpObj, lnmpObj=lnmpObj)
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=False)
                     logger.info("%r cofactor data backup status (%r)", resourceName, okB)
 
             return ok & okB
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return False
```

### Comparing `rcsb.workflow-0.39/rcsb.workflow.egg-info/PKG-INFO` & `rcsb.workflow-0.40/rcsb.workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.39/rcsb.workflow.egg-info/SOURCES.txt` & `rcsb.workflow-0.40/rcsb.workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.39/setup.py` & `rcsb.workflow-0.40/setup.py`

 * *Files identical despite different names*

