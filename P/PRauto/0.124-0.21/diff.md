# Comparing `tmp/PRauto-0.124.tar.gz` & `tmp/PRauto-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.124.tar", last modified: Fri Apr 21 01:42:33 2023, max compression
+gzip compressed data, was "PRauto-0.21.tar", last modified: Mon Jun  5 01:57:59 2023, max compression
```

## Comparing `PRauto-0.124.tar` & `PRauto-0.21.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.808723 PRauto-0.124/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.124/LICENSE
--rw-rw-rw-   0        0        0      349 2023-04-21 01:42:33.808723 PRauto-0.124/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.793723 PRauto-0.124/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-04-21 01:04:02.000000 PRauto-0.124/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.796723 PRauto-0.124/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.124/prauto/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-04-21 01:41:27.000000 PRauto-0.124/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.799724 PRauto-0.124/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.124/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.124/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.806753 PRauto-0.124/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.124/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-04-21 01:40:55.000000 PRauto-0.124/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.124/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2685 2023-04-20 06:05:57.000000 PRauto-0.124/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.124/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-21 01:42:33.809723 PRauto-0.124/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-04-21 01:42:18.000000 PRauto-0.124/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.636839 PRauto-0.21/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.21/LICENSE
+-rw-rw-rw-   0        0        0      348 2023-06-05 01:57:59.636839 PRauto-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.602530 PRauto-0.21/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 01:57:59.000000 PRauto-0.21/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2088 2023-04-21 03:50:22.000000 PRauto-0.21/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.606531 PRauto-0.21/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.21/prauto/__init__.py
+-rw-rw-rw-   0        0        0     3178 2023-06-02 04:51:18.000000 PRauto-0.21/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.614442 PRauto-0.21/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.21/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.21/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:57:59.633841 PRauto-0.21/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.21/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     3061 2023-06-02 01:56:52.000000 PRauto-0.21/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.21/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     5901 2023-06-02 02:00:27.000000 PRauto-0.21/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.21/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:57:59.637839 PRauto-0.21/setup.cfg
+-rw-rw-rw-   0        0        0     1249 2023-06-05 01:57:35.000000 PRauto-0.21/setup.py
```

### Comparing `PRauto-0.124/LICENSE` & `PRauto-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.124/README.md` & `PRauto-0.21/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,26 @@
+<<<<<<< HEAD
 PRauto is a Bioinformatic and Chemoinformatics tool
 that provides two main functionalities: Data Retrieval and Data Preprocessing.
+=======
+# PRauto
+ 
+#### PRauto is a automation tool that provides two main functionalities: [ Data Retrieval ] and [ Data Preprocessing ]                                                               in Bioinformatic and Chemoinformatics.
+_______________________________________________________________________________________________________________________________________
+### Install
+To install the PRauto, users can input the following command in the command-line interface:
+  
+```bash
+   pip install PRauto
+```
+If you have problems with PyMOL dependency, try:
+```bash
+   conda install -c conda-forge pymol-open-source
+```
+>>>>>>> 0eebdc859a4bed936fc1085306290e1db0273feb
 
 To use the Data Retrieval feature, users can input the command "python -m prauto" into the command-line interface. This tool allows users to retrieve the FASTA file of a target protein sequence via a search query in the UniProt API. Additionally, using the UniProt accession number, PRauto retrieves the PDB files of target protein from the RCSB PDB API and sdf files of ligands that interact with the target protein from the ChEMBL API.
 
 The output of this feature includes the target protein sequence in a FASTA file format, PDB files of the target protein structures, and sdf files of the ligands that interact with the target protein.
 
 To use the Data Preprocessing feature, users can input the command "python -m prauto.prepauto" into the command-line interface. This tool processes PDB files that are located in a single directory. It extracts only the chain(s) that correspond to the target protein and aligns them according to the reference PDB file. It also removes any unnecessary molecules that are not involved in the binding of the primary ligand. In a PSE PyMOL session, these unnecessary molecules are hidden rather than being removed.
```

### Comparing `PRauto-0.124/prauto/prepauto/__main__.py` & `PRauto-0.21/prauto/prepauto/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,27 +23,36 @@
                     pdb_start = int(line[14:18].strip())
                 except ValueError:
                     pdb_start = 0
                 try:
                     pdb_end = int(line[20:24].strip())
                 except ValueError:
                     pdb_end = 0
+                try:
+                    uniprot_start = int(line[56:60].strip())
+                except ValueError:
+                    uniprot_start = 0
+                try:
+                    uniprot_end = int(line[63:67].strip())
+                except ValueError:
+                    uniprot_end = 0
                 db_accession = line[33:39].strip() or "NaN"
                 db_id = line[42:53].strip() or "NaN"
 
                 data_dict[key_count] = {"chain": chain, "pdb_start": pdb_start,
                                         "pdb_end": pdb_end, "db_accession": db_accession,
-                                        "db_id": db_id}
+                                        "db_id": db_id, "uniprot_start": uniprot_start, "uniprot_end": uniprot_end}
                 key_count += 1
     return data_dict
 
 
 def extract_target_chains(pdb_files, target_id, output_dir):
     parser = PDBParser(QUIET=True)
     remove_dict = {}
+    renumber_dict = {}
     for pdb_file in pdb_files:
         try:
             # Parse the PDB file
             structure = parser.get_structure("pdb", pdb_file)
             current_data = extract_dbref_data(pdb_file)
 
             target_chain = []
@@ -94,18 +103,38 @@
                     else:
                         remove_dict[key] = [{
                             "chain": current_data[keys]['chain'],
                             "db_id": current_data[keys]['db_id'],
                             "pdb_start": current_data[keys]['pdb_start'],
                             "pdb_end": current_data[keys]['pdb_end']
                         }]
+                else:
+                    key = os.path.basename(pdb_file)
+                    if key in renumber_dict:
+                        renumber_dict[key].append({
+                            "chain": current_data[keys]['chain'],
+                            "db_id": current_data[keys]['db_id'],
+                            "pdb_start": current_data[keys]['pdb_start'],
+                            "pdb_end": current_data[keys]['pdb_end'],
+                            "uniprot_start": current_data[keys]['uniprot_start'],
+                            "uniprot_end": current_data[keys]['uniprot_end']
+                        })
+                    else:
+                        renumber_dict[key] = [{
+                            "chain": current_data[keys]['chain'],
+                            "db_id": current_data[keys]['db_id'],
+                            "pdb_start": current_data[keys]['pdb_start'],
+                            "pdb_end": current_data[keys]['pdb_end'],
+                            "uniprot_start": current_data[keys]['uniprot_start'],
+                            "uniprot_end": current_data[keys]['uniprot_end']
+                        }]
         except Exception as e:
             print(f"Failed to extract chains from {pdb_file}: {e}")
 
-    return remove_dict
+    return remove_dict, renumber_dict
 
 
 # 'ER0', #Tetramethyloctadecanoate
 # 'OLA', #Oleic acid
 # 'OLB', #(2S)-2,3-dihydroxypropyl (9Z)-octadec-9-enoate
 # 'OLC', #1-Oleoyl-R-glycerol
 # 'PEG', #2-(2-hydroxyethyloxy)ethanol
@@ -134,113 +163,119 @@
 # 'SBT', #Butanol
 # '1BO', #Butanol
 # 'PGO', #1,2-Propanediol
 # 'BU1', #1,4-Butanediol
 # 'CCN', #Acetonitrile
 # 'DMF', #Dimethylformamide
 # 'PLM', #Palmitic acid
+# 'J40',
 
 remove_list = ['ER0', 'OLA', 'OLB', 'OLC', 'PEG', '1PE', 'HEX', 'SO4', 'OCT', 'MYS', 'D12', 'TRD', 'EDT', 'D10', 'GOL',
                'PGE', '8K6', 'PE4', 'STE', 'UND', 'EDO', 'DMS', 'ACN', 'IPA', 'MOH', 'EOH', 'POL', 'SBT', '1BO', 'PGO',
-               'BU1', 'DMF', 'PLM']
+               'BU1', 'DMF', 'PLM', 'J40']
 
 
-def align_and_save_all_pdb_files(directory, ref_pdb_file, ligand_name, ligand_range, remove_dict):
+def align_and_save_all_pdb_files(directory, ref_pdb_file, ligand_name, ligand_range, remove_dict, renumber_dict):
     # Create a new directory for aligned pdb files
     parent_dir = os.path.dirname(directory)
     new_dir_name = os.path.join(parent_dir, f"{os.path.basename(directory)}_aligned")
     os.makedirs(new_dir_name, exist_ok=True)
-    new_session_dir = os.path.join(new_dir_name, f"{os.path.basename(directory)}_pse")
-    os.makedirs(new_session_dir, exist_ok=True)
 
     # Start PyMOL and load the reference pdb file
     pymol.finish_launching()
     time.sleep(1)  # wait for PyMOL to fully load
     pymol.cmd.load(ref_pdb_file, 'ref')
-    distance_cutoff = 5.0
+    distance_cutoff = 3.0
+    save = 1
 
     # Loop through all pdb files in the directory
     for pdb_file in os.listdir(directory):
         if pdb_file.endswith(".pdb"):
 
             # Load the pdb file
             pymol.cmd.load(os.path.join(directory, pdb_file), pdb_file[:-4])
-
             name_for_dict = '_'.join(pdb_file.split('_')[:2]) + '.pdb'
 
             try:
                 for data in remove_dict[name_for_dict]:
                     rm_chain = data['chain']
                     rm_start = data['pdb_start']
                     rm_end = data['pdb_end']
+                    if (rm_start - rm_end) > 0:
+                        print(f'Wrong DBREF data: {pdb_file} , Check resi {rm_start}-{rm_end}')
+                        save = 0
                     pymol.cmd.remove(f"(chain {rm_chain} and resi {rm_start}-{rm_end})")
                     print(f"{pdb_file}, resi{rm_start}-{rm_end} has been removed")
 
-            except : pass
+            except: pass
+
+            try:
+                for data in renumber_dict[name_for_dict]:
+                    rn_chain = data['chain']
+                    rn_start = data['pdb_start']
+                    rn_end = data['pdb_end']
+                    un_start = data['uniprot_start']
+                    un_end = data['uniprot_end']
+                    minus = rn_start - un_start
+                    plus = rn_start - un_start
+
+                    if rn_start != un_start or rn_end != un_end:
+                        pymol.cmd.select('selection', f'chain {rn_chain} and resi {rn_start}-{rn_end}')
+                        pymol.cmd.alter('selection', f'resi=str(int(resi)-{minus})')
+                        pymol.cmd.select('selection2',
+                                         f'resi {un_start}-{un_end} and chain "" and polymer.protein and resn ""')
+                        pymol.cmd.alter('selection2', f'resi=str(int(resi)+{plus})')
+
+                        print(f"{pdb_file}, resi{rn_start}-{rn_end} has been renumbered")
+
+            except:
+                print(pdb_file, 'renumber error')
+                pass
 
             # Align the pdb file to the reference pdb file
             pymol.cmd.align(pdb_file[:-4], 'ref')
 
             pymol.cmd.origin('ref')
             pymol.cmd.zoom("all", 0.8)
-
-            # Hide unnecessary parts and save sessions
-            pymol.cmd.select("main_ligand", f"resn {ligand_name}")
-            pymol.cmd.select("main_organic", f"bymolecule(main_ligand expand {ligand_range})")
-            pymol.cmd.hide("everything", "organic and not main_organic")
-
-            pymol.cmd.select("nearby_solvent", f"solvent within {distance_cutoff} of main_organic")
-            pymol.cmd.hide('everything', 'solvent and not nearby_solvent')
-
-            pymol.cmd.select("target", "polymer.protein")
-            pymol.cmd.select("main_inorganic", f"inorganic within {distance_cutoff} of target")
-            pymol.cmd.select("not_nearby_inorganic", f"inorganic and not main_inorganic")
-            pymol.cmd.hide("everything", "not_nearby_inorganic")
-
-            for mol in remove_list:
-                pymol.cmd.hide("everything", f"resn {mol}")
-
-            new_session_name = f"{pdb_file[:-4]}_aligned.pse"
-            pymol.cmd.save(os.path.join(new_session_dir, new_session_name), pdb_file[:-4])
-            pymol.cmd.sync()  # wait for the save command to complete
-
+            #
             # Remove the organic and solvent
             pymol.cmd.select("main_ligand", f"resn {ligand_name}")
             pymol.cmd.select("main_organic", f"bymolecule(main_ligand expand {ligand_range})")
             pymol.cmd.remove('organic and not main_organic')
             #
             pymol.cmd.select("nearby_solvent", f"solvent within {distance_cutoff} of main_organic")
             pymol.cmd.remove('solvent and not nearby_solvent')
             #
             # Remove the inorganic
             pymol.cmd.select("target", "polymer.protein")
             pymol.cmd.select("main_inorganic", f"inorganic within {distance_cutoff} of target")
             pymol.cmd.select("not_nearby_inorganic", f"inorganic and not main_inorganic")
             pymol.cmd.remove("not_nearby_inorganic")
-            #
-            #
+            # #
+            # #
             for mol in remove_list:
                 pymol.cmd.remove(f"resn {mol}")
 
             # Save the aligned pdb file with a new name
             new_file_name = f"{pdb_file[:-4]}_aligned.pdb"
-            pymol.cmd.save(os.path.join(new_dir_name, new_file_name), pdb_file[:-4])
+            if save != 0:
+                pymol.cmd.save(os.path.join(new_dir_name, new_file_name), pdb_file[:-4])
+            else: save = 1
             pymol.cmd.sync()  # wait for the save command to complete
 
             # Delete the loaded pdb file to free up memory
             pymol.cmd.delete(pdb_file[:-4])
 
     # Delete the reference pdb file to free up memory
     pymol.cmd.delete('ref')
 
     # Quit PyMOL
     pymol.cmd.quit()
 
 
-
 if __name__ == "__main__":
     print('Step 1: Extract target chains'+'\n' * 6)
     # Select a directory using a file dialog
     dir_path = filedialog.askdirectory(title='Select a directory to work with')
     ref_pdb_file = filedialog.askopenfilename(title='Select the file you want to use as the reference',initialdir=dir_path)
 
     # Parse the reference PDB file
@@ -258,28 +293,30 @@
 
     # Create a directory to store the output files containing the separated chains
     output_dir = os.path.join(dir_path, f"{target_id}_target_chains")
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     # Extract the chains from the input PDB files that match the molecules in the reference PDB file
-    remove_dict= extract_target_chains(pdb_files, target_id, output_dir)
+    remove_dict, renumber_dict = extract_target_chains(pdb_files, target_id, output_dir)
     print('remove_dict: ',remove_dict)
     print('\n' * 7)
     print('###########  Target chains extraction Complete  ###########'+'\n' * 2)
     print('Step 2: Start preprocessing with pymol'+'\n' * 8)
     align_ref = filedialog.askopenfilename(title='Select the file you want to use as the align criteria',initialdir=output_dir)
 
     with open(os.path.join(align_ref), 'r') as f:
         ligand_menu = []
         for line in f:
+            if line.startswith('HETNAM'):
+                print(line)
             if line.startswith('HETATM'):
                 ligand_menu.append(line[17:20].replace(' ', ''))
         print(list(set(ligand_menu)))
 
     ligand_name = input("Enter ligand name: ")
     print('\n' * 1)
     ligand_range = input("Range around the ligand you do not want to delete(Å): ")
     print('\n' * 7)
-    align_and_save_all_pdb_files(output_dir, align_ref, ligand_name,ligand_range,remove_dict)
+    align_and_save_all_pdb_files(output_dir, align_ref, ligand_name, ligand_range, remove_dict, renumber_dict)
     print('\n' * 7)
     print('########### PDB Preprocessing Complete  ###########' + '\n' * 2)
```

### Comparing `PRauto-0.124/prauto/retriever/get_fasta.py` & `PRauto-0.21/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.124/prauto/retriever/get_pdb.py` & `PRauto-0.21/prauto/retriever/get_pdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def extract_accessions(fasta_file_path):
     with open(fasta_file_path, "r") as f:
         fasta_seq = f.readlines()
     uniprot_accessions = []
     for line in fasta_seq:
-        if line.startswith('>'):
+        if line.startswith('>sp'):
             uniprot_accessions.append(line.split('|')[1])
     return list(set(uniprot_accessions))
 
 
 def search_pdb_by_accession(accession):
     """Search the RCSB PDB API for protein structures by gene name and return a list of PDB IDs"""
     search_url = 'https://search.rcsb.org/rcsbsearch/v2/query?json={search-request}'
```

### Comparing `PRauto-0.124/setup.py` & `PRauto-0.21/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.124',
+        version = '0.21',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

