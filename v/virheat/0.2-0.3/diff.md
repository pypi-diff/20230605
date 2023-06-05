# Comparing `tmp/virheat-0.2.tar.gz` & `tmp/virheat-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virheat-0.2.tar", last modified: Tue May 23 14:27:02 2023, max compression
+gzip compressed data, was "virheat-0.3.tar", last modified: Mon Jun  5 16:52:41 2023, max compression
```

## Comparing `virheat-0.2.tar` & `virheat-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-23 14:27:02.112931 virheat-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-23 14:26:44.000000 virheat-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:27:02.112931 virheat-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-23 14:26:44.000000 virheat-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 14:26:44.000000 virheat-0.2/virheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 14:26:44.000000 virheat-0.2/virheat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-23 14:26:44.000000 virheat-0.2/virheat/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:27:01.000000 virheat-0.2/virheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 16:52:41.322300 virheat-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 16:52:20.000000 virheat-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:52:41.322300 virheat-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 16:52:20.000000 virheat-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.318300 virheat-0.3/virheat/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 16:52:20.000000 virheat-0.3/virheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 16:52:20.000000 virheat-0.3/virheat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-05 16:52:20.000000 virheat-0.3/virheat/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/virheat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/virheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/top_level.txt
```

### Comparing `virheat-0.2/PKG-INFO` & `virheat-0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.2
+Version: 0.3
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 [![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
 [![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
 [![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+[![pypi version](https://static.pepy.tech/badge/virheat)](https://pypi.org/project/virheat/)
 
-[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+![Logo](./virheat.png)
 
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
+![Example](./example_data/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
@@ -81,17 +82,12 @@
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
 
 You need to either provide the length of your reference genome or if you want to get the sequence annotation you will need to provide the gff3 file.
 
-## Planned features
-
-- Clustering
-- Interactive mode
-
 ---
 
 **Important disclaimer:**
 *The code is under the GPLv3 licence. The code is WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.*
```

### Comparing `virheat-0.2/README.md` & `virheat-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
 [![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
 [![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+[![pypi version](https://static.pepy.tech/badge/virheat)](https://pypi.org/project/virheat/)
 
-[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+![Logo](./virheat.png)
 
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
+![Example](./example_data/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
@@ -69,17 +70,12 @@
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
 
 You need to either provide the length of your reference genome or if you want to get the sequence annotation you will need to provide the gff3 file.
 
-## Planned features
-
-- Clustering
-- Interactive mode
-
 ---
 
 **Important disclaimer:**
 *The code is under the GPLv3 licence. The code is WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.*
```

### Comparing `virheat-0.2/setup.py` & `virheat-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `virheat-0.2/virheat/command.py` & `virheat-0.3/virheat/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 contains the main workflow of virHEAT
 """
-
 # BUILT-INS
 import os
 import sys
+import math
 import argparse
 
 # LIB
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from matplotlib import colors
 from matplotlib import colormaps
@@ -99,55 +99,59 @@
     frequency_array = data_prep.create_freq_array(unique_mutations, frequency_lists)
     if args.delete:
         frequency_array = data_prep.delete_common_mutations(frequency_array, unique_mutations)
 
     # define relative locations of all items in the plot
     n_samples = len(frequency_array)
     n_mutations = len(frequency_array[0])
-    genome_y_location = n_samples/4
+    if n_samples < 4:
+        genome_y_location = 2
+    else:
+        genome_y_location = math.log2(n_samples)
 
     # gff3 data extraction
     if args.gff3_path is not None and args.genome_length is not None:
         sys.exit("\033[31m\033[1mERROR:\033[0m Do not provide the -g and -l argument simultaneously!")
     elif args.gff3_path is not None:
         gff3_info, gff3_ref_name = data_prep.parse_gff3(args.gff3_path)
         # issue a warning if #CHROM and gff3 do not match
         if gff3_ref_name not in reference_name and reference_name not in gff3_ref_name:
             print("\033[31m\033[WARNING:\033[0m gff3 reference does not match the vcf reference!")
         genome_end = data_prep.get_genome_end(gff3_info)
         genes_with_mutations, n_tracks = data_prep.create_track_dict(unique_mutations, gff3_info)
         # define space for the genome vis tracks
-        min_y_location = genome_y_location + genome_y_location/4 * (n_tracks+2)
+        min_y_location = genome_y_location + genome_y_location/2 * (n_tracks+1)
     elif args.genome_length is not None:
         genome_end = args.genome_length
         min_y_location = genome_y_location
     else:
         sys.exit("\033[31m\033[1mERROR:\033[0m Provide either a gff3 file (-g) or the length (-l) of the genome which you used for mapping")
 
     # define size of the plot
     y_size = (n_mutations)*0.4
     x_size = y_size*(n_samples+min_y_location)/n_mutations
-    x_size = x_size-x_size*1/6  # compensate of heatmap annotation
+    x_size = x_size-x_size*0.15  # compensate of heatmap annotation
 
     # ini the fig
     fig, ax = plt.subplots(figsize=[y_size, x_size])
 
     # plot all elements
     cmap_cells = cm.ScalarMappable(norm=colors.Normalize(0, 1), cmap=colormaps["gist_heat_r"])
     plotting.create_heatmap(ax, frequency_array, cmap_cells)
     mutation_set = plotting.create_genome_vis(ax, genome_y_location, n_mutations, unique_mutations, genome_end)
     if args.gff3_path is not None:
         # distinct colors for the genes
-        cmap_genes = plt.get_cmap("tab20")
+        cmap_genes = plt.get_cmap('tab20', len(genes_with_mutations))
         colors_genes = [cmap_genes(i) for i in range(len(genes_with_mutations))]
         # plot gene track
         plotting.create_gene_vis(ax, genes_with_mutations, n_mutations, y_size, n_tracks, genome_end, min_y_location, genome_y_location, colors_genes)
     plotting.create_axis(ax, n_mutations, min_y_location, n_samples, file_names, genome_end, genome_y_location, unique_mutations, reference_name)
-    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples)
+    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples, n_mutations)
     plotting.create_mutation_legend(mutation_set, min_y_location, n_samples)
 
     # create output folder
     if not os.path.exists(args.input[1]):
         os.makedirs(args.input[1])
 
     # save fig
     fig.savefig(os.path.join(args.input[1], "virHEAT_plot.pdf"), bbox_inches="tight")
+
```

### Comparing `virheat-0.2/virheat/scripts/data_prep.py` & `virheat-0.3/virheat/scripts/data_prep.py`

 * *Files identical despite different names*

### Comparing `virheat-0.2/virheat/scripts/plotting.py` & `virheat-0.3/virheat/scripts/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         }
     mutation_set = set()
     # define coordinates
     y_min = -genome_y_location
     y_max = -genome_y_location+genome_y_location/2
 
     # create blank rectangle for genome vis
-    # ax.add_patch(patches.Rectangle((0,y_min),n_mutations,y_max - y_min, alpha=1, edgecolor=None, facecolor="lightgrey"))
     ax.add_patch(
         patches.FancyBboxPatch(
                             (0, y_min), n_mutations, y_max - y_min,
                             boxstyle="round,pad=-0.0040,rounding_size=0.03",
                             ec="none", fc="lightgrey"
                         )
     )
@@ -63,33 +62,39 @@
         coordinates = [(x_start, 0), (x_start+1, 0), (mutation_x_location, y_max)]
         ax.add_patch(patches.Polygon(coordinates, facecolor=mutation_color, alpha=0.5))
         x_start += 1
 
     return mutation_set
 
 
-def create_colorbar(threshold, cmap, min_y_location, n_samples):
+def create_colorbar(threshold, cmap, min_y_location, n_samples, n_mutations):
     """
     creates a custom colorbar and annotates the threshold
     """
-    ticks = [0, 0.2, 0.4, 0.6, 0.8, 1]
-    labels = [0, 0.2, 0.4, 0.6, 0.8, 1]
-
-    if threshold+0.1 in ticks or threshold-0.1 in ticks:
-        rounded_threshold = threshold
+    if n_samples >= 8:
+        ticks = [0, 0.2, 0.4, 0.6, 0.8, 1]
+        labels = [0, 0.2, 0.4, 0.6, 0.8, 1]
+        if threshold + 0.1 in ticks or threshold - 0.1 in ticks:
+            rounded_threshold = threshold
+        else:
+            rounded_threshold = round(threshold * 5) / 5
     else:
-        rounded_threshold = round(threshold*5)/5
+        ticks = [0, 0.5, 1]
+        labels = [0, 0.5, 1]
+        if threshold + 0.25 in ticks or threshold - 0.25 in ticks:
+            rounded_threshold = threshold
+        else:
+            rounded_threshold = round(threshold * 2) / 2
 
     if rounded_threshold in ticks:
         ticks.remove(rounded_threshold)
         labels.remove(rounded_threshold)
     ticks.append(threshold)
     labels.append(f"threshold\n={threshold}")
-
-    cbar = plt.colorbar(cmap, label="variant frequency", pad=0, shrink=n_samples/(min_y_location+n_samples), anchor=(0.1, 1))
+    cbar = plt.colorbar(cmap, label="variant frequency", pad=0, shrink=n_samples/(min_y_location+n_samples), anchor=(0.1, 1), aspect=15)
     cbar.set_ticks(ticks)
     cbar.set_ticklabels(labels)
 
 
 def create_mutation_legend(mutation_set, min_y_location, n_samples):
     """
     create a legend for the mutation type
@@ -111,16 +116,22 @@
     create the axis of the plot
     """
 
     # define plot limits
     ax.set_xlim(0, n_mutations)
     ax.set_ylim(-min_y_location, n_samples)
     # define new ticks depending on the genome size
-    xtick_dis = round(genome_end/6, -int(math.log10(genome_end/6))+1)
-    xtick_labels = [0, xtick_dis, xtick_dis*2, xtick_dis*3, xtick_dis*4, xtick_dis*5, genome_end]
+    if n_mutations >= 20:
+        xtick_dis = round(genome_end/6, -int(math.log10(genome_end / 6)) + 1)
+        xtick_labels = [0, xtick_dis, xtick_dis*2, xtick_dis*3, xtick_dis*4, xtick_dis*5, genome_end]
+    elif n_mutations >= 10:
+        xtick_dis = round(genome_end / 3, -int(math.log10(genome_end / 3)) + 1)
+        xtick_labels = [0, xtick_dis, xtick_dis * 2, genome_end]
+    else:
+        xtick_labels = [0, genome_end]
     xtick_labels = [int(tick) for tick in xtick_labels]
     # get the correct location of the genome pos on the axis
     xticks = [n_mutations/genome_end*tick for tick in xtick_labels]
     # set new ticks and change spines/yaxis
     ax.set_xticks(xticks, xtick_labels)
     # set y axis labels
     y_ticks = [idx+0.5 for idx in range(0, len(file_names))]
@@ -148,22 +159,22 @@
     create the vis for the gene
     """
 
     gene_annotations = []
     mult_factor = n_mutations/genome_end
 
     for idx, gene in enumerate(genes_with_mutations):
-        start = (mult_factor*genes_with_mutations[gene][0][0], -min_y_location+(n_tracks-genes_with_mutations[gene][1])*genome_y_location/4-genome_y_location/4)
+        start = (mult_factor*genes_with_mutations[gene][0][0], -min_y_location+(n_tracks-genes_with_mutations[gene][1])*genome_y_location/2-genome_y_location/2)
         stop = mult_factor*genes_with_mutations[gene][0][1]
         height = genome_y_location/2
         ax.add_patch(
             patches.FancyBboxPatch(
                                 start, stop-start[0], height,
                                 boxstyle="round,pad=-0.0040,rounding_size=0.03",
                                 ec="black", fc=colors_genes[idx]
                             )
         )
         # define text pos for gene description inside or below the gene box, depending if it fits within
         if stop-start[0] > n_mutations/(y_size*8)*len(gene):
             gene_annotations.append(ax.text(start[0]+(stop-start[0])/2, start[1]+height/2, gene, ha="center", va="center"))
         else:
-            gene_annotations.append(ax.text(start[0]+(stop-start[0])/2, start[1]-height/4, gene, ha="center", va="center"))
+            gene_annotations.append(ax.text(start[0]+(stop-start[0])/2, start[1]-height/4, gene, rotation=40, rotation_mode="anchor", ha="right", va="bottom"))
```

### Comparing `virheat-0.2/virheat.egg-info/PKG-INFO` & `virheat-0.3/virheat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.2
+Version: 0.3
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 [![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
 [![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
 [![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
 [![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+[![pypi version](https://static.pepy.tech/badge/virheat)](https://pypi.org/project/virheat/)
 
-[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+![Logo](./virheat.png)
 
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
+![Example](./example_data/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
@@ -81,17 +82,12 @@
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
 
 You need to either provide the length of your reference genome or if you want to get the sequence annotation you will need to provide the gff3 file.
 
-## Planned features
-
-- Clustering
-- Interactive mode
-
 ---
 
 **Important disclaimer:**
 *The code is under the GPLv3 licence. The code is WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.*
```

