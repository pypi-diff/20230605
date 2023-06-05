# Comparing `tmp/vMedNLP-1.0.0-py38-none-any.whl.zip` & `tmp/vMedNLP-1.0.1-py38-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12525 bytes, number of entries: 7
--rw-------  2.0 unx      139 b- defN 23-May-17 13:57 vMedNLP/__init__.pyc
--rw-------  2.0 unx    19050 b- defN 23-May-17 13:57 vMedNLP/medToolkit.pyc
--rw-------  2.0 unx     3013 b- defN 23-May-17 13:57 vMedNLP/models.pyc
--rw-------  2.0 unx     9145 b- defN 23-May-17 13:57 vMedNLP-1.0.0.dist-info/METADATA
--rw-------  2.0 unx       82 b- defN 23-May-17 13:57 vMedNLP-1.0.0.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 23-May-17 13:57 vMedNLP-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      528 b- defN 23-May-17 13:57 vMedNLP-1.0.0.dist-info/RECORD
-7 files, 31965 bytes uncompressed, 11595 bytes compressed:  63.7%
+Zip file size: 13745 bytes, number of entries: 7
+-rw-------  2.0 unx      139 b- defN 23-Jun-05 02:39 vMedNLP/__init__.pyc
+-rw-------  2.0 unx    19050 b- defN 23-Jun-05 02:39 vMedNLP/medToolkit.pyc
+-rw-------  2.0 unx     3013 b- defN 23-Jun-05 02:39 vMedNLP/models.pyc
+-rw-------  2.0 unx    13070 b- defN 23-Jun-05 02:39 vMedNLP-1.0.1.dist-info/METADATA
+-rw-------  2.0 unx       82 b- defN 23-Jun-05 02:39 vMedNLP-1.0.1.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 23-Jun-05 02:39 vMedNLP-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      529 b- defN 23-Jun-05 02:39 vMedNLP-1.0.1.dist-info/RECORD
+7 files, 35891 bytes uncompressed, 12815 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: vMedNLP/medToolkit.pyc
 Comment: 
 
 Filename: vMedNLP/models.pyc
 Comment: 
 
-Filename: vMedNLP-1.0.0.dist-info/METADATA
+Filename: vMedNLP-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: vMedNLP-1.0.0.dist-info/WHEEL
+Filename: vMedNLP-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: vMedNLP-1.0.0.dist-info/top_level.txt
+Filename: vMedNLP-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vMedNLP-1.0.0.dist-info/RECORD
+Filename: vMedNLP-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vMedNLP/medToolkit.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 17 09:56:48 2023 UTC, .py size: 26760 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1152,20 +1152,20 @@
 000047f0: 6465 6e74 6966 795f 6469 636f 6d4e 290a  dentify_dicomN).
 00004800: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
 00004810: 8b00 0000 727f 0000 0072 a200 0000 7219  ....r....r....r.
 00004820: 0000 0072 4600 0000 72a3 0000 0072 a400  ...rF...r....r..
 00004830: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
 00004840: 0072 1800 0000 7287 0000 0044 0200 0073  .r....r....D...s
 00004850: 0c00 0000 0802 080a 0e15 080a 0808 0818  ................
-00004860: 7287 0000 0029 35da 0c74 7261 6e73 666f  r....)5..transfo
+00004860: 7287 0000 0029 355a 0c74 7261 6e73 666f  r....)5Z.transfo
 00004870: 726d 6572 7372 0200 0000 7203 0000 0072  rmersr....r....r
 00004880: 0400 0000 7205 0000 0072 0600 0000 726d  ....r....r....rm
 00004890: 0000 0072 5700 0000 da02 6f73 7269 0000  ...rW.....osri..
 000048a0: 00da 0670 616e 6461 73da 0270 6472 0700  ...pandas..pdr..
-000048b0: 0000 da08 7363 6973 7061 6379 5a15 7363  ....scispacyZ.sc
+000048b0: 0000 5a08 7363 6973 7061 6379 5a15 7363  ..Z.scispacyZ.sc
 000048c0: 6973 7061 6379 2e61 6262 7265 7669 6174  ispacy.abbreviat
 000048d0: 696f 6e72 0800 0000 5a10 7363 6973 7061  ionr....Z.scispa
 000048e0: 6379 2e6c 696e 6b69 6e67 7209 0000 0072  cy.linkingr....r
 000048f0: 3800 0000 da04 6a6f 696e da07 6469 726e  8.....join..dirn
 00004900: 616d 65da 085f 5f66 696c 655f 5f5a 0844  ame..__file__Z.D
 00004910: 6174 615f 6469 725a 0a73 7061 6379 315f  ata_dirZ.spacy1_
 00004920: 6469 7272 6b00 0000 722c 0000 0072 2d00  dirrk...r,...r-.
```

