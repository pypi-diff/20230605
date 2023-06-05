# Comparing `tmp/phc-ingestion-0.3.30.tar.gz` & `tmp/phc-ingestion-0.3.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.30.tar", last modified: Fri Jun  2 17:59:01 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.31.tar", last modified: Mon Jun  5 11:16:54 2023, max compression
```

## Comparing `phc-ingestion-0.3.30.tar` & `phc-ingestion-0.3.31.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2924 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2214 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     7359 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3675 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5503 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2222 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.30/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3030 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2214 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     7359 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3652 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5664 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2222 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-05 11:16:31.651489 phc-ingestion-0.3.31/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-05 11:16:31.655489 phc-ingestion-0.3.31/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.31/PKG-INFO
```

### Comparing `phc-ingestion-0.3.30/ingestion/caris/process.py` & `phc-ingestion-0.3.31/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.31/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.31/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.31/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.31/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/json.py` & `phc-ingestion-0.3.31/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.31/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.31/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.31/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.31/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/foundation/process.py` & `phc-ingestion-0.3.31/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.31/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.31/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.31/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.31/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/process.py` & `phc-ingestion-0.3.31/ingestion/nextgen/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,18 +69,21 @@
     with open(manifest_path_name, "w") as file:
         yaml = YAML()
         yaml.dump(manifest, file)
 
     # Hard-code genome reference for nextgen
     genome_reference = "GRCh38"
 
-    return {
+    nextgen_metadata = {
         "manifest_path_name": manifest_path_name,
         "cnv_path_name": cnv_path_name,
         "cnv_genome_reference": genome_reference,
-        "structural_path_name": structural_path_name,
-        "structural_genome_reference": genome_reference,
         "somatic_vcf_meta_data": somatic_vcf_meta_data,
         "somatic_genome_reference": genome_reference,
         "germline_vcf_meta_data": germline_vcf_meta_data,
         "germline_genome_reference": genome_reference,
     }
+    if structural_path_name:
+        nextgen_metadata["structural_path_name"] = structural_path_name
+        nextgen_metadata["structural_genome_reference"] = genome_reference
+
+    return nextgen_metadata
```

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.31/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.31/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.31/ingestion/nextgen/util/process_structural.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
     if not variants:
         log.info(f"No structural variants found in {sv_in_file}")
         return None
 
     structural_variant_rows = []
     for variant in variants:
-        print(variant)
         working_variant = variant.strip().split("\t")
 
         chromosome1 = f"chr{working_variant[0]}"
         start_position1 = working_variant[1]
 
         if working_variant[4] in ["<DEL>", "<DUP:TANDEM>"]:
             end_position1 = working_variant[7].split(";")[0].split("=")[1]
```

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.31/ingestion/nextgen/util/process_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.pruned_info = self.info[0]
         self.pruned_frmt = ":".join(list(frmt_smpl_dict.keys()))
         self.pruned_smpl = ":".join(list(frmt_smpl_dict.values()))
 
 
 def transform_vcf(vcf_in_file: str, headers: list, variants: list, sequence_type: str, log: Logger):
     log.info(f"Performing file transformations on {vcf_in_file}")
+    approved_chr_list = ["chr" + str(i) for i in range(1, 23)] + ["chrX", "chrY", "chrM"]
     vcf_out = []
 
     for header in headers:
         # Add AF/INFO and DP/FORMAT to header if somatic (already in germline headers)
         if "#CHROM" in header and sequence_type == "somatic":
             vcf_out.append(
                 '##INFO=<ID=AF,Number=A,Type=Float,Description="Allele frequency, for each ALT allele, in the same order as listed">'
@@ -74,14 +75,16 @@
 
     for var in variants:
         split_var = var.split("\t")
         if len(split_var) != 10:
             raise RuntimeError(
                 f"Variant does not contain correct number of fields. Should be 10 when {len(split_var)} were detected: {var}"
             )
+        if split_var[0] not in approved_chr_list:
+            continue
 
         chr_pos = f"{split_var[0]} {split_var[1]}"
         info_string = split_var[7]
         # Ignore structural variants
         if "SVTYPE" in info_string:
             continue
```

### Comparing `phc-ingestion-0.3.30/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.31/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.31/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.31/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.31/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.31/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.30/pyproject.toml` & `phc-ingestion-0.3.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.30"
+version = "0.3.31"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

