# Comparing `tmp/sequana_nanomerge-1.2.0.tar.gz` & `tmp/sequana_nanomerge-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_nanomerge-1.2.0.tar", last modified: Wed May 17 08:52:26 2023, max compression
+gzip compressed data, was "dist/sequana_nanomerge-1.3.0.tar", last modified: Mon Jun  5 10:06:44 2023, max compression
```

## Comparing `sequana_nanomerge-1.2.0.tar` & `sequana_nanomerge-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5520 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/dag.png
--rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/nanomerge.rules
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-17 08:52:26.000000 sequana_nanomerge-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-05-17 08:52:23.000000 sequana_nanomerge-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8443 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5812 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8443 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    14218 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/nanomerge.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-05 10:06:44.000000 sequana_nanomerge-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-06-05 10:06:40.000000 sequana_nanomerge-1.3.0/setup.py
```

### Comparing `sequana_nanomerge-1.2.0/PKG-INFO` & `sequana_nanomerge-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_nanomerge
-Version: 1.2.0
+Version: 1.3.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -59,20 +59,21 @@
         Usage
         ~~~~~
         
         ::
         
             sequana_nanomerge --help
         
-        If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY::
+        If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY so you will need to use a pattern
+        (--input-pattern) such as `*/*.gz`::
         
             sequana_nanomerge --input-directory DATAPATH/barcoded --samplesheet samplesheet.csv
                 --summary summary.txt --input-pattern '*/*fastq.gz'
         
-        otherwise all fastq files are in DATAPATH/::
+        otherwise all fastq files are in DATAPATH/ so the input pattern can just be `*.fastq.gz`::
         
             sequana_nanomerge --input-directory DATAPATH --samplesheet samplesheet.csv
                 --summary summary.txt --input-pattern '*fastq.gz'
         
         The --summary is optional and takes as input the output of albacore/guppy demultiplexing. usually a file called sequencing_summary.txt
         
         Note that the different between the two is the extra `*/` before the `*.fastq.gz` pattern since barcoded files are in individual subdirectories.
@@ -102,15 +103,15 @@
             ,main,A
         
         or just removed::
         
             project,sample
             main,A
         
-        Usage with apptainer::
+        Usage with apptainer:
         ~~~~~~~~~~~~~~~~~~~~~~~~~
         
         With apptainer, initiate the working directory as follows::
         
             sequana_nanomerge --use-apptainer
         
         Images are downloaded in the working directory but you can store then in a directory globally (e.g.)::
@@ -153,16 +154,19 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
-        1.2.0     * handle large promethium run by using find+cat instead of just cat
-                    to cope with very large number of input files.
+        1.3.0     * handle large promethium run by using a sub sample of the 
+                    sequencing summary file (--sample of pycoQC still loads the entire
+                    file in memory)
+        1.2.0     * handle large promethium run by using find+cat instead of just 
+                    cat to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
         1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
                   * Fix the pyco file paths, update requirements and doc
         1.0.0     Stable release ready for production
         0.0.1     **First release.**
         ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.2.0/README.rst` & `sequana_nanomerge-1.3.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -49,20 +49,21 @@
 Usage
 ~~~~~
 
 ::
 
     sequana_nanomerge --help
 
-If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY::
+If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY so you will need to use a pattern
+(--input-pattern) such as `*/*.gz`::
 
     sequana_nanomerge --input-directory DATAPATH/barcoded --samplesheet samplesheet.csv
         --summary summary.txt --input-pattern '*/*fastq.gz'
 
-otherwise all fastq files are in DATAPATH/::
+otherwise all fastq files are in DATAPATH/ so the input pattern can just be `*.fastq.gz`::
 
     sequana_nanomerge --input-directory DATAPATH --samplesheet samplesheet.csv
         --summary summary.txt --input-pattern '*fastq.gz'
 
 The --summary is optional and takes as input the output of albacore/guppy demultiplexing. usually a file called sequencing_summary.txt
 
 Note that the different between the two is the extra `*/` before the `*.fastq.gz` pattern since barcoded files are in individual subdirectories.
@@ -92,15 +93,15 @@
     ,main,A
 
 or just removed::
 
     project,sample
     main,A
 
-Usage with apptainer::
+Usage with apptainer:
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 With apptainer, initiate the working directory as follows::
 
     sequana_nanomerge --use-apptainer
 
 Images are downloaded in the working directory but you can store then in a directory globally (e.g.)::
@@ -143,16 +144,19 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
-1.2.0     * handle large promethium run by using find+cat instead of just cat
-            to cope with very large number of input files.
+1.3.0     * handle large promethium run by using a sub sample of the 
+            sequencing summary file (--sample of pycoQC still loads the entire
+            file in memory)
+1.2.0     * handle large promethium run by using find+cat instead of just 
+            cat to cope with very large number of input files.
 1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
             runs such as promethion
 1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
           * Fix the pyco file paths, update requirements and doc
 1.0.0     Stable release ready for production
 0.0.1     **First release.**
 ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/PKG-INFO` & `sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana-nanomerge
-Version: 1.2.0
+Version: 1.3.0
 Summary: Merge barcoded or non barcoded fastq files generated by Nanopore runs
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -59,20 +59,21 @@
         Usage
         ~~~~~
         
         ::
         
             sequana_nanomerge --help
         
-        If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY::
+        If you data is barcoded, they are usually in sub-directories barcoded/barcodeXY so you will need to use a pattern
+        (--input-pattern) such as `*/*.gz`::
         
             sequana_nanomerge --input-directory DATAPATH/barcoded --samplesheet samplesheet.csv
                 --summary summary.txt --input-pattern '*/*fastq.gz'
         
-        otherwise all fastq files are in DATAPATH/::
+        otherwise all fastq files are in DATAPATH/ so the input pattern can just be `*.fastq.gz`::
         
             sequana_nanomerge --input-directory DATAPATH --samplesheet samplesheet.csv
                 --summary summary.txt --input-pattern '*fastq.gz'
         
         The --summary is optional and takes as input the output of albacore/guppy demultiplexing. usually a file called sequencing_summary.txt
         
         Note that the different between the two is the extra `*/` before the `*.fastq.gz` pattern since barcoded files are in individual subdirectories.
@@ -102,15 +103,15 @@
             ,main,A
         
         or just removed::
         
             project,sample
             main,A
         
-        Usage with apptainer::
+        Usage with apptainer:
         ~~~~~~~~~~~~~~~~~~~~~~~~~
         
         With apptainer, initiate the working directory as follows::
         
             sequana_nanomerge --use-apptainer
         
         Images are downloaded in the working directory but you can store then in a directory globally (e.g.)::
@@ -153,16 +154,19 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
-        1.2.0     * handle large promethium run by using find+cat instead of just cat
-                    to cope with very large number of input files.
+        1.3.0     * handle large promethium run by using a sub sample of the 
+                    sequencing summary file (--sample of pycoQC still loads the entire
+                    file in memory)
+        1.2.0     * handle large promethium run by using find+cat instead of just 
+                    cat to cope with very large number of input files.
         1.1.0     * add subsample option and set to 1,000,000 reads to handle large 
                     runs such as promethion
         1.0.1     * CSV can now handle sample or samplename column name in samplesheet.
                   * Fix the pyco file paths, update requirements and doc
         1.0.0     Stable release ready for production
         0.0.1     **First release.**
         ========= ====================================================================
```

### Comparing `sequana_nanomerge-1.2.0/sequana_nanomerge.egg-info/SOURCES.txt` & `sequana_nanomerge-1.3.0/sequana_nanomerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/config.yaml` & `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -33,12 +33,17 @@
 apptainers:
   pycoqc: "https://zenodo.org/record/7746269/files/pycoqc_2.5.2.img"
   graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
 
 
 ###################################################################################
 #
-# subsample: If not None, N number of reads will be randomly selected instead of
-#     the entire dataset
 pycoqc:
-  subsample: 1000000
+  options: 
 
+
+##################################################################################
+# if number of reads is larger than **max_lines**, sub sample the summary by 
+# selection x **percent**
+#
+sub_sample_summary:
+  percentage: 100
```

### Comparing `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/nanomerge.rules` & `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/nanomerge.rules`

 * *Files 10% similar despite different names*

```diff
@@ -101,28 +101,42 @@
         barcode = samples.get_barcode_from_sample(wildcards.sample)
         return input_directory / barcode
     else:
         return input_directory
 
 
 if config["summary"]:
-    rule pyco:
+
+
+    rule sub_sample_summary:
         input:
             config['summary']
         output:
+            "sub_sample_summary/summary.txt"
+        params:
+            percentage=config['sub_sample_summary']['percentage'] / 100
+        shell:
+            """
+            head -n 1 {input} > {output} && tail -n +2 {input} | awk -v k={params.percentage} 'BEGIN {{ srand(); n = 0; }} {{ if (n < k * NR) {{ reservoir[n++] = $0; }} else {{ r = int(rand() * n); if (r < k * NR) {{ reservoir[r] = $0; }} }} }} END {{ for (i = 0; i < n; i++) {{ print reservoir[i]; }} }}' >> {output}
+            """
+
+    rule pyco:
+        input:
+            "sub_sample_summary/summary.txt"
+        output:
             "pyco/pyco.html"
         log:
             "pyco/pyco.log"
         params:
-            sample=config["pycoqc"]["subsample"]
+           options=config["pycoqc"]["options"]
         container:
             config["apptainers"]["pycoqc"]
         shell:
             """
-            pycoQC --summary_file {input} -o {output} --sample {params.sample} > {log} 2>&1
+            pycoQC --summary_file {input} -o {output} {params.options} > {log} 2>&1
             """
 
 
 rule merge:
     input:
         get_input_merge
     output:
```

### Comparing `sequana_nanomerge-1.2.0/sequana_pipelines/nanomerge/schema.yaml` & `sequana_nanomerge-1.3.0/sequana_pipelines/nanomerge/schema.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -19,16 +19,24 @@
         type: str
         required: True
 
     "apptainers":
         type: any
         required: true
 
+    "sub_sample_summary":
+      type: map
+      mapping:
+          "percentage":
+              type: int
+              range: {min: 1 ,  max: 100}
+
+
     "pycoqc":
         type: map
         mapping:
-          "subsample":
-            type: int
+          "options":
+            type: str
             required: False
```

### Comparing `sequana_nanomerge-1.2.0/setup.py` & `sequana_nanomerge-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # handle sequana git link
 with open("requirements.txt", encoding='utf-8') as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 1
-_MINOR               = 2
+_MINOR               = 3
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
```

