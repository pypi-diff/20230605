# Comparing `tmp/ablang-0.2.2.tar.gz` & `tmp/ablang-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablang-0.2.2.tar", last modified: Fri Mar 25 18:30:19 2022, max compression
+gzip compressed data, was "ablang-0.2.3.tar", last modified: Mon Jun  5 10:01:49 2023, max compression
```

## Comparing `ablang-0.2.2.tar` & `ablang-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 18:30:19.138969 ablang-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-03-25 18:30:09.000000 ablang-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4879 2022-03-25 18:30:19.138969 ablang-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-03-25 18:30:09.000000 ablang-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 18:30:19.134969 ablang-0.2.2/ablang/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)     5690 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/encoderblocks.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/extra_fns.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    12122 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-03-25 18:30:09.000000 ablang-0.2.2/ablang/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 18:30:19.138969 ablang-0.2.2/ablang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4879 2022-03-25 18:30:18.000000 ablang-0.2.2/ablang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-03-25 18:30:19.000000 ablang-0.2.2/ablang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-25 18:30:18.000000 ablang-0.2.2/ablang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-03-25 18:30:18.000000 ablang-0.2.2/ablang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-25 18:30:18.000000 ablang-0.2.2/ablang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-25 18:30:19.138969 ablang-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-03-25 18:30:09.000000 ablang-0.2.2/setup.py
+drwx------   0 olsen    (10273) rstudent (30003)        0 2023-06-05 10:01:49.326259 ablang-0.2.3/
+-rw-------   0 olsen    (10273) rstudent (30003)     1528 2021-11-14 21:37:49.000000 ablang-0.2.3/LICENSE
+-rw-------   0 olsen    (10273) rstudent (30003)     5025 2023-06-05 10:01:49.325259 ablang-0.2.3/PKG-INFO
+-rw-------   0 olsen    (10273) rstudent (30003)     4751 2022-03-25 18:44:23.000000 ablang-0.2.3/README.md
+drwx------   0 olsen    (10273) rstudent (30003)        0 2023-06-05 10:01:49.325259 ablang-0.2.3/ablang/
+-rw-------   0 olsen    (10273) rstudent (30003)      111 2021-11-15 20:44:31.000000 ablang-0.2.3/ablang/__init__.py
+-rw-------   0 olsen    (10273) rstudent (30003)     1395 2021-03-24 12:28:34.000000 ablang-0.2.3/ablang/embedding.py
+-rw-------   0 olsen    (10273) rstudent (30003)     5690 2021-11-14 21:51:46.000000 ablang-0.2.3/ablang/encoderblocks.py
+-rw-------   0 olsen    (10273) rstudent (30003)      749 2021-03-24 12:28:34.000000 ablang-0.2.3/ablang/extra_fns.py
+-rw-------   0 olsen    (10273) rstudent (30003)     3329 2021-11-14 21:51:49.000000 ablang-0.2.3/ablang/model.py
+-rw-------   0 olsen    (10273) rstudent (30003)    12215 2023-06-05 09:52:53.000000 ablang-0.2.3/ablang/pretrained.py
+-rw-------   0 olsen    (10273) rstudent (30003)     1789 2023-06-05 09:54:14.000000 ablang-0.2.3/ablang/tokenizers.py
+drwx------   0 olsen    (10273) rstudent (30003)        0 2023-06-05 10:01:49.325259 ablang-0.2.3/ablang.egg-info/
+-rw-------   0 olsen    (10273) rstudent (30003)     5025 2023-06-05 10:01:49.000000 ablang-0.2.3/ablang.egg-info/PKG-INFO
+-rw-------   0 olsen    (10273) rstudent (30003)      316 2023-06-05 10:01:49.000000 ablang-0.2.3/ablang.egg-info/SOURCES.txt
+-rw-------   0 olsen    (10273) rstudent (30003)        1 2023-06-05 10:01:49.000000 ablang-0.2.3/ablang.egg-info/dependency_links.txt
+-rw-------   0 olsen    (10273) rstudent (30003)       40 2023-06-05 10:01:49.000000 ablang-0.2.3/ablang.egg-info/requires.txt
+-rw-------   0 olsen    (10273) rstudent (30003)        7 2023-06-05 10:01:49.000000 ablang-0.2.3/ablang.egg-info/top_level.txt
+-rw-------   0 olsen    (10273) rstudent (30003)       38 2023-06-05 10:01:49.326259 ablang-0.2.3/setup.cfg
+-rw-------   0 olsen    (10273) rstudent (30003)      679 2023-06-05 09:55:04.000000 ablang-0.2.3/setup.py
```

### Comparing `ablang-0.2.2/LICENSE` & `ablang-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ablang-0.2.2/PKG-INFO` & `ablang-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,122 @@
 Metadata-Version: 2.1
 Name: ablang
-Version: 0.2.2
+Version: 0.2.3
 Summary: AbLang: A language model for antibodies.
-Home-page: UNKNOWN
 Maintainer: Tobias Hegelund Olsen
 Maintainer-email: tobias.olsen@stats.ox.ac.uk
 License: BSD 3-clause license
-Description: 
-        ---
-        
-        <div align="center">    
-         
-        # AbLang: A language model for antibodies  
-        
-        [![DOI:10.1101/2022.01.20.477061](http://img.shields.io/badge/DOI-10.1101/2022.01.20.477061-B31B1B.svg)](https://doi.org/10.1101/2022.01.20.477061)
-        
-        </div>
-        
-        
-        General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Language models require vast numbers of sequences for training and antibodies are one of the few protein types for which such volumes of data exist, for example in the Observed Antibody Space (OAS) database. Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with BCR-seq data, as seen with over 40% of OAS sequences missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
-        
-        -----------
-        
-        # Install AbLang
-        
-        AbLang is freely available and can be installed with pip.
-        
-        ~~~.sh
-            pip install ablang
-        ~~~
-        
-        or directly from github.
-        
-        ~~~.sh
-            pip install -U git+https://github.com/oxpig/AbLang.git
-        ~~~
-        
-        ----------
-        
-        # AbLang use cases
-        
-        **A Jupyter notebook** showing the different use cases of AbLang can be found [here](https://github.com/TobiasHeOl/AbLang/tree/main/examples). 
-        
-        
-        Currently, AbLang can be used to generate three different representations/encodings for antibody sequences. 
-        
-        1. **Res-codings:** These encodings are 768 values for each residue, useful for residue specific predictions.
-        
-        2. **Seq-codings:** These encodings are 768 values for each sequence, useful for sequence specific predictions. The same length of encodings for each sequence, means these encodings also removes the need to align antibody sequences.
-        
-        3. **Res-likelihoods:** These encodings are the likelihoods of each amino acid at each position in a given antibody sequence, useful for exploring possible mutations.
-        
-        These representations can be used for a plethora of antibody design applications. As an example, we have used the res-likelihoods from AbLang to restore missing residues in antibody sequences due either to sequencing errors, such as ambiguous bases, or the limitations of the sequencing techniques used.
-        
-        
-        ## Antibody sequence restoration
-        
-        Restoration of antibody sequences can be done using the "restore" mode as seen below.
-        
-        ```{r, engine='python', count_lines}
-        import ablang
-        
-        heavy_ablang = ablang.pretrained("heavy") # Use "light" if you are working with light chains
-        heavy_ablang.freeze()
-        
-        
-        seqs = [
-            'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
-            '*************PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL*****',
-        ]
-        
-        heavy_ablang(seqs, mode='restore')
-        
-        ```
-        
-        The output of the above is seen below.
-        
-        ```console
-        array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
-               'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
-              dtype='<U121')
-        ```
-        -----
-        
-        ### Citation   
-        ```
-        @article{Olsen2022,
-          title={AbLang: An antibody language model for completing antibody sequences},
-          author={Tobias H. Olsen, Iain H. Moal and Charlotte M. Deane},
-          journal={bioRxiv},
-          doi={https://doi.org/10.1101/2022.01.20.477061},
-          year={2022}
-        }
-        ```  
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+---
+
+<div align="center">    
+ 
+# AbLang: A language model for antibodies  
+
+[![DOI:10.1101/2022.01.20.477061](http://img.shields.io/badge/DOI-10.1101/2022.01.20.477061-B31B1B.svg)](https://doi.org/10.1101/2022.01.20.477061)
+
+</div>
+
+
+**Motivation:** General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Antibodies are one of the few protein types where the volume of sequence data needed for such language models is available, for example in the Observed Antibody Space (OAS) database. 
+
+**Results:** Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with B-cell receptor repertoire sequencing, for example over 40% of OAS sequences are missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
+
+-----------
+
+# Install AbLang
+
+AbLang is freely available and can be installed with pip.
+
+~~~.sh
+    pip install ablang
+~~~
+
+or directly from github.
+
+~~~.sh
+    pip install -U git+https://github.com/oxpig/AbLang.git
+~~~
+
+----------
+
+# AbLang use cases
+
+**A Jupyter notebook** showing the different use cases of AbLang can be found [here](https://github.com/TobiasHeOl/AbLang/tree/main/examples). 
+
+
+Currently, AbLang can be used to generate three different representations/encodings for antibody sequences. 
+
+1. **Res-codings:** These encodings are 768 values for each residue, useful for residue specific predictions.
+
+2. **Seq-codings:** These encodings are 768 values for each sequence, useful for sequence specific predictions. The same length of encodings for each sequence, means these encodings also removes the need to align antibody sequences.
+
+3. **Res-likelihoods:** These encodings are the likelihoods of each amino acid at each position in a given antibody sequence, useful for exploring possible mutations.
+
+These representations can be used for a plethora of antibody design applications. As an example, we have used the res-likelihoods from AbLang to restore missing residues in antibody sequences due either to sequencing errors, such as ambiguous bases, or the limitations of the sequencing techniques used.
+
+
+## Antibody sequence restoration
+
+Restoration of antibody sequences can be done using the "restore" mode as seen below.
+
+```{r, engine='python', count_lines}
+import ablang
+
+heavy_ablang = ablang.pretrained("heavy") # Use "light" if you are working with light chains
+heavy_ablang.freeze()
+
+
+seqs = [
+    'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+    '*************PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL*****',
+]
+
+heavy_ablang(seqs, mode='restore')
+
+```
+
+The output of the above is seen below.
+
+```console
+array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+       'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
+      dtype='<U121')
+```
+-----
+
+For restoration of an unknown number of missing residues at the ends of antibody sequences, the "align" parameter can be set to True.
+
+```{r, engine='python', count_lines}
+seqs = [
+    'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+    'PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL',
+]
+
+heavy_ablang(seqs, mode='restore', align=True)
+
+```
+
+The output of the above is seen below.
+
+```console
+array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+       'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
+      dtype='<U121')
+```
+-----
+
+
+
+### Citation   
+```
+@article{Olsen2022,
+  title={AbLang: An antibody language model for completing antibody sequences},
+  author={Tobias H. Olsen, Iain H. Moal and Charlotte M. Deane},
+  journal={bioRxiv},
+  doi={https://doi.org/10.1101/2022.01.20.477061},
+  year={2022}
+}
+```
```

### Comparing `ablang-0.2.2/README.md` & `ablang-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 # AbLang: A language model for antibodies  
 
 [![DOI:10.1101/2022.01.20.477061](http://img.shields.io/badge/DOI-10.1101/2022.01.20.477061-B31B1B.svg)](https://doi.org/10.1101/2022.01.20.477061)
 
 </div>
 
 
-General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Language models require vast numbers of sequences for training and antibodies are one of the few protein types for which such volumes of data exist, for example in the Observed Antibody Space (OAS) database. Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with BCR-seq data, as seen with over 40% of OAS sequences missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
+**Motivation:** General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Antibodies are one of the few protein types where the volume of sequence data needed for such language models is available, for example in the Observed Antibody Space (OAS) database. 
+
+**Results:** Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with B-cell receptor repertoire sequencing, for example over 40% of OAS sequences are missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
 
 -----------
 
 # Install AbLang
 
 AbLang is freely available and can be installed with pip.
 
@@ -71,14 +73,37 @@
 ```console
 array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
        'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
       dtype='<U121')
 ```
 -----
 
+For restoration of an unknown number of missing residues at the ends of antibody sequences, the "align" parameter can be set to True.
+
+```{r, engine='python', count_lines}
+seqs = [
+    'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+    'PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL',
+]
+
+heavy_ablang(seqs, mode='restore', align=True)
+
+```
+
+The output of the above is seen below.
+
+```console
+array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+       'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
+      dtype='<U121')
+```
+-----
+
+
+
 ### Citation   
 ```
 @article{Olsen2022,
   title={AbLang: An antibody language model for completing antibody sequences},
   author={Tobias H. Olsen, Iain H. Moal and Charlotte M. Deane},
   journal={bioRxiv},
   doi={https://doi.org/10.1101/2022.01.20.477061},
```

### Comparing `ablang-0.2.2/ablang/embedding.py` & `ablang-0.2.3/ablang/embedding.py`

 * *Files identical despite different names*

### Comparing `ablang-0.2.2/ablang/encoderblocks.py` & `ablang-0.2.3/ablang/encoderblocks.py`

 * *Files identical despite different names*

### Comparing `ablang-0.2.2/ablang/extra_fns.py` & `ablang-0.2.3/ablang/extra_fns.py`

 * *Files identical despite different names*

### Comparing `ablang-0.2.2/ablang/model.py` & `ablang-0.2.3/ablang/model.py`

 * *Files identical despite different names*

### Comparing `ablang-0.2.2/ablang/pretrained.py` & `ablang-0.2.3/ablang/pretrained.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             # Download model and save to specific place - if already downloaded do not download again
             model_folder = os.path.join(os.path.dirname(__file__), "model-weights-{}".format(chain))
             os.makedirs(model_folder, exist_ok = True)
             
             if not os.path.isfile(os.path.join(model_folder, "amodel.pt")):
                 print("Downloading model ...")
                 
-                url = "http://opig.stats.ox.ac.uk/website/data/downloads/ablang-{}.tar.gz".format(chain)
+                url = "https://opig.stats.ox.ac.uk/data/downloads/ablang-{}.tar.gz".format(chain)
                 tmp_file = os.path.join(model_folder, "tmp.tar.gz")
 
                 with open(tmp_file,'wb') as f: f.write(requests.get(url).content)
                 
                 subprocess.run(["tar", "-zxvf", tmp_file, "-C", model_folder], check = True) 
                 
                 os.remove(tmp_file)
@@ -203,15 +203,19 @@
             return residue_output
         
     def sequence_aligning(self, seqs):
         
         import pandas as pd
         import anarci
 
-        anarci_out = anarci.run_anarci(pd.DataFrame(seqs).reset_index().values.tolist(), ncpu=self.ncpu, scheme='imgt') #, allowed_species=['human', 'mouse']
+        anarci_out = anarci.run_anarci(
+            pd.DataFrame([seq.replace('*', 'X') for seq in seqs]).reset_index().values.tolist(), 
+            ncpu=self.ncpu, 
+            scheme='imgt'
+        ) #, allowed_species=['human', 'mouse']
         anarci_data = pd.DataFrame([str(anarci[0][0]) if anarci else 'ANARCI_error' for anarci in anarci_out[1]], columns=['anarci']).astype('<U90')
 
         seqs = anarci_data.apply(lambda x: get_sequences_from_anarci(x.anarci, 
                                                                      self.max_position, 
                                                                      self.spread), axis=1, result_type='expand').to_numpy().reshape(-1)
         
         return seqs
@@ -339,15 +343,15 @@
     end_position = int(re.search(r'\d+', out_anarci[::-1]).group()[::-1])
     # Fixes ANARCI error of poor numbering of the CDR1 region
     start_position = int(re.search(r'\d+,\s\'.\'\),\s\'[^-]+\'\),\s\(\(\d+,\s\'.\'\),\s\'[^-]+\'\),\s\(\(\d+,\s\'.\'\),\s\'[^-]+\'\),\s\(\(\d+,\s\'.\'\),\s\'[^-]+',
                                    out_anarci).group().split(',')[0]) - 1
     
     sequence = "".join(re.findall(r"(?i)[A-Z*]", "".join(re.findall(r'\),\s\'[A-Z*]', out_anarci))))
 
-    sequence_j = ''.join(sequence).replace('-','') + '*'*(max_position-int(end_position))
+    sequence_j = ''.join(sequence).replace('-','').replace('X','*') + '*'*(max_position-int(end_position))
     
     numba_list = List.empty_list(unicode_type)
 
     spread_seqs = np.array(get_spread_sequences(sequence_j, spread, start_position, numba_list))
 
     return spread_seqs
```

### Comparing `ablang-0.2.2/ablang/tokenizers.py` & `ablang-0.2.3/ablang/tokenizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,23 @@
     def set_vocabs(self, vocab_dir):
         with open(vocab_dir, encoding="utf-8") as vocab_handle:
             self.vocab_to_token=json.load(vocab_handle)
             
         self.vocab_to_aa = {v: k for k, v in self.vocab_to_token.items()}
      
     def encode(self, sequence, device='cpu'):
-        
-        encoded = [self.vocab_to_token["<"]]+[self.vocab_to_token[resn] for resn in sequence]+[self.vocab_to_token[">"]]
+        try:
+            encoded = [self.vocab_to_token["<"]]+[self.vocab_to_token[resn] for resn in sequence]+[self.vocab_to_token[">"]]
+        except KeyError as e:
+            
+            wrong_aa = e.args
+            
+            e.args = (f"Following character(s) not accepted in sequences: {wrong_aa}. \
+Please only use amino acids (MRHKDESTNQCGPAVIFYWL) or the mask token (*).",)
+            raise 
         
         return torch.tensor(encoded, dtype=torch.long, device=device)
         # Start and Stop token should probably not be added here, but instead earlier
     
     def decode(self, seqtokens):
         
         if torch.is_tensor(seqtokens): seqtokens = seqtokens.cpu().numpy()
```

### Comparing `ablang-0.2.2/ablang.egg-info/PKG-INFO` & `ablang-0.2.3/ablang.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,122 @@
 Metadata-Version: 2.1
 Name: ablang
-Version: 0.2.2
+Version: 0.2.3
 Summary: AbLang: A language model for antibodies.
-Home-page: UNKNOWN
 Maintainer: Tobias Hegelund Olsen
 Maintainer-email: tobias.olsen@stats.ox.ac.uk
 License: BSD 3-clause license
-Description: 
-        ---
-        
-        <div align="center">    
-         
-        # AbLang: A language model for antibodies  
-        
-        [![DOI:10.1101/2022.01.20.477061](http://img.shields.io/badge/DOI-10.1101/2022.01.20.477061-B31B1B.svg)](https://doi.org/10.1101/2022.01.20.477061)
-        
-        </div>
-        
-        
-        General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Language models require vast numbers of sequences for training and antibodies are one of the few protein types for which such volumes of data exist, for example in the Observed Antibody Space (OAS) database. Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with BCR-seq data, as seen with over 40% of OAS sequences missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
-        
-        -----------
-        
-        # Install AbLang
-        
-        AbLang is freely available and can be installed with pip.
-        
-        ~~~.sh
-            pip install ablang
-        ~~~
-        
-        or directly from github.
-        
-        ~~~.sh
-            pip install -U git+https://github.com/oxpig/AbLang.git
-        ~~~
-        
-        ----------
-        
-        # AbLang use cases
-        
-        **A Jupyter notebook** showing the different use cases of AbLang can be found [here](https://github.com/TobiasHeOl/AbLang/tree/main/examples). 
-        
-        
-        Currently, AbLang can be used to generate three different representations/encodings for antibody sequences. 
-        
-        1. **Res-codings:** These encodings are 768 values for each residue, useful for residue specific predictions.
-        
-        2. **Seq-codings:** These encodings are 768 values for each sequence, useful for sequence specific predictions. The same length of encodings for each sequence, means these encodings also removes the need to align antibody sequences.
-        
-        3. **Res-likelihoods:** These encodings are the likelihoods of each amino acid at each position in a given antibody sequence, useful for exploring possible mutations.
-        
-        These representations can be used for a plethora of antibody design applications. As an example, we have used the res-likelihoods from AbLang to restore missing residues in antibody sequences due either to sequencing errors, such as ambiguous bases, or the limitations of the sequencing techniques used.
-        
-        
-        ## Antibody sequence restoration
-        
-        Restoration of antibody sequences can be done using the "restore" mode as seen below.
-        
-        ```{r, engine='python', count_lines}
-        import ablang
-        
-        heavy_ablang = ablang.pretrained("heavy") # Use "light" if you are working with light chains
-        heavy_ablang.freeze()
-        
-        
-        seqs = [
-            'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
-            '*************PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL*****',
-        ]
-        
-        heavy_ablang(seqs, mode='restore')
-        
-        ```
-        
-        The output of the above is seen below.
-        
-        ```console
-        array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
-               'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
-              dtype='<U121')
-        ```
-        -----
-        
-        ### Citation   
-        ```
-        @article{Olsen2022,
-          title={AbLang: An antibody language model for completing antibody sequences},
-          author={Tobias H. Olsen, Iain H. Moal and Charlotte M. Deane},
-          journal={bioRxiv},
-          doi={https://doi.org/10.1101/2022.01.20.477061},
-          year={2022}
-        }
-        ```  
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+---
+
+<div align="center">    
+ 
+# AbLang: A language model for antibodies  
+
+[![DOI:10.1101/2022.01.20.477061](http://img.shields.io/badge/DOI-10.1101/2022.01.20.477061-B31B1B.svg)](https://doi.org/10.1101/2022.01.20.477061)
+
+</div>
+
+
+**Motivation:** General protein language models have been shown to summarise the semantics of protein sequences into representations that are useful for state-of-the-art predictive methods. However, for antibody specific problems, such as restoring residues lost due to sequencing errors, a model trained solely on antibodies may be more powerful. Antibodies are one of the few protein types where the volume of sequence data needed for such language models is available, for example in the Observed Antibody Space (OAS) database. 
+
+**Results:** Here, we introduce AbLang, a language model trained on the antibody sequences in the OAS database. We demonstrate the power of AbLang by using it to restore missing residues in antibody sequence data, a key issue with B-cell receptor repertoire sequencing, for example over 40% of OAS sequences are missing the first 15 amino acids. AbLang restores the missing residues of antibody sequences better than using IMGT germlines or the general protein language model ESM-1b. Further, AbLang does not require knowledge of the germline of the antibody and is seven times faster than ESM-1b.
+
+-----------
+
+# Install AbLang
+
+AbLang is freely available and can be installed with pip.
+
+~~~.sh
+    pip install ablang
+~~~
+
+or directly from github.
+
+~~~.sh
+    pip install -U git+https://github.com/oxpig/AbLang.git
+~~~
+
+----------
+
+# AbLang use cases
+
+**A Jupyter notebook** showing the different use cases of AbLang can be found [here](https://github.com/TobiasHeOl/AbLang/tree/main/examples). 
+
+
+Currently, AbLang can be used to generate three different representations/encodings for antibody sequences. 
+
+1. **Res-codings:** These encodings are 768 values for each residue, useful for residue specific predictions.
+
+2. **Seq-codings:** These encodings are 768 values for each sequence, useful for sequence specific predictions. The same length of encodings for each sequence, means these encodings also removes the need to align antibody sequences.
+
+3. **Res-likelihoods:** These encodings are the likelihoods of each amino acid at each position in a given antibody sequence, useful for exploring possible mutations.
+
+These representations can be used for a plethora of antibody design applications. As an example, we have used the res-likelihoods from AbLang to restore missing residues in antibody sequences due either to sequencing errors, such as ambiguous bases, or the limitations of the sequencing techniques used.
+
+
+## Antibody sequence restoration
+
+Restoration of antibody sequences can be done using the "restore" mode as seen below.
+
+```{r, engine='python', count_lines}
+import ablang
+
+heavy_ablang = ablang.pretrained("heavy") # Use "light" if you are working with light chains
+heavy_ablang.freeze()
+
+
+seqs = [
+    'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+    '*************PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL*****',
+]
+
+heavy_ablang(seqs, mode='restore')
+
+```
+
+The output of the above is seen below.
+
+```console
+array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+       'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
+      dtype='<U121')
+```
+-----
+
+For restoration of an unknown number of missing residues at the ends of antibody sequences, the "align" parameter can be set to True.
+
+```{r, engine='python', count_lines}
+seqs = [
+    'EV*LVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+    'PGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNK*YADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTL',
+]
+
+heavy_ablang(seqs, mode='restore', align=True)
+
+```
+
+The output of the above is seen below.
+
+```console
+array(['EVQLVESGPGLVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS',
+       'QVQLVESGGGVVQPGKSLRLSCVASGFTFSGYGMHWVRQAPGKGLEWIALIIYDESNKYYADSVKGRFTISRDNSKNTLYLQMSSLRAEDTAVFYCAKVKFYDPTAPNDYWGQGTLVTVSS'],
+      dtype='<U121')
+```
+-----
+
+
+
+### Citation   
+```
+@article{Olsen2022,
+  title={AbLang: An antibody language model for completing antibody sequences},
+  author={Tobias H. Olsen, Iain H. Moal and Charlotte M. Deane},
+  journal={bioRxiv},
+  doi={https://doi.org/10.1101/2022.01.20.477061},
+  year={2022}
+}
+```
```

### Comparing `ablang-0.2.2/setup.py` & `ablang-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
     
 setup(
     name='ablang',
-    version='0.2.2',
+    version='0.2.3',
     description='AbLang: A language model for antibodies.',
     license='BSD 3-clause license',
     maintainer='Tobias Hegelund Olsen',
     long_description=long_description,
     long_description_content_type='text/markdown',
     maintainer_email='tobias.olsen@stats.ox.ac.uk',
     include_package_data=True,
     packages=find_packages(include=('ablang', 'ablang.*')),
     install_requires=[
-        'numpy',
-        'numba',
         'requests',
         'fairseq',
         'torch>=1.6',
+        'numpy',
+        'numba',
     ],
 )
```

