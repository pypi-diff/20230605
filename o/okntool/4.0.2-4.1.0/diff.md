# Comparing `tmp/okntool-4.0.2.tar.gz` & `tmp/okntool-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-4.0.2.tar", last modified: Thu Jun  1 08:36:23 2023, max compression
+gzip compressed data, was "okntool-4.1.0.tar", last modified: Mon Jun  5 00:48:40 2023, max compression
```

## Comparing `okntool-4.0.2.tar` & `okntool-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.497352 okntool-4.0.2/
--rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.2/LICENSE
--rw-rw-rw-   0        0        0      555 2023-06-01 08:36:23.497352 okntool-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.489372 okntool-4.0.2/okntool/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.2/okntool/__init__.py
--rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.2/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0   102264 2023-06-01 08:35:44.000000 okntool-4.0.2/okntool/okntool.py
--rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.2/okntool/simpler_plot_config.json
-drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.496356 okntool-4.0.2/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 08:36:13.000000 okntool-4.0.2/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:36:23.497352 okntool-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-06-01 08:35:44.000000 okntool-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.316515 okntool-4.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-06-05 00:48:40.315518 okntool-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4138 2023-06-01 23:23:02.000000 okntool-4.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.307560 okntool-4.1.0/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.1.0/okntool/__init__.py
+-rw-rw-rw-   0        0        0     1257 2023-06-02 03:16:07.000000 okntool-4.1.0/okntool/indi_va_table_template.html
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.1.0/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0   108619 2023-06-05 00:42:34.000000 okntool-4.1.0/okntool/okntool.py
+-rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.1.0/okntool/simpler_plot_config.json
+-rw-rw-rw-   0        0        0     1889 2023-06-04 23:07:46.000000 okntool-4.1.0/okntool/sum_va_table_template.html
+drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.315518 okntool-4.1.0/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 00:48:22.000000 okntool-4.1.0/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 00:48:40.316515 okntool-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-06-05 00:00:56.000000 okntool-4.1.0/setup.py
```

### Comparing `okntool-4.0.2/LICENSE` & `okntool-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-4.0.2/PKG-INFO` & `okntool-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.2
+Version: 4.1.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.2/README.md` & `okntool-4.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # OKN TOOL PYTHON PACKAGE LIBRARY MANUAL
 ## Description
 This program will draw the graph image in the ABI eye research group web experience recording folder according to config file information and plot type input. 
 
-There are 4 types of plot which are:
+There are 5 types of plot which are:
 1.  **Trial** plot which represents sensor timestamp vs pupil displacement/movement graph for each trial.
 2.  **Summary** plot which is the combination of all trial plots with the same x and y axis scales.
 3.  **Staircase/progress** plot which is the graph image to visualize whether there is okn or not and the visual acuity etdrs calculation steps.
 4.  **Tidy** plot, the special plot for all trial protocol in which borders and boundaries are drawn in tidest format.
+5.  **Simpler** plot, the special plot for face detection and eye tracker related OKNs.
 
 ## Installation requirements and guide
 ### Anaconda
 To install this program, `Anaconda python distributing program` and `Anaconda Powershell Prompt` are needed.  
 If you do not have `Anaconda`, please use the following links to download and install:  
 Download link: https://www.anaconda.com/products/distribution  
 Installation guide link: https://docs.anaconda.com/anaconda/install/  
@@ -20,20 +21,20 @@
 In `Anaconda Powershell Prompt`:
 ```
 pip install okntool
 ```  
 ## Usage guide
 ### Example usage
 ```
-okntool -t "(plot_type)" -d "(directory to the folder)" -c "(directory to config file)"
+okntool -t "(plot_type)" -d "(directory to the folder)" -c "(directory to config file)" -r "(referenced csv)"
 ```
 plot_type: "trial", "summary" or "staircase"  
 If you are using "trial" plot type, please -d "(directory to trial folder)".  
 If you are using "summary" or "staircase" plot type, please -d "(directory to pim_recorded_folder/trials)".  
-**Note: please put `directory to pim recorded folder` and `directory to config file` into the string indication "(dir_input)".**  
+**-r** is only for "simpler" plot type.  
 
 There is a example folder under `development` folder.  
 If you want to test this program, you can clone this repository, install `okntool` and run the following command:  
 **For trial plot**
 ```
 okntool -t "trial" -d "development/example/trials/trials/trial-1-1_disk-condition-1-1"
 ```
@@ -49,23 +50,39 @@
 ```
 okntool -t "progress" -d "development/example/trials/trials"
 ```
 **For tidy plot**
 ```
 okntool -t "tidy" -d "development/example/trials/trials"
 ```
+**For simpler plot**
+```
+okntool -t "simpler" -d "(folders which clip folders)"
+```
+or
+```
+okntool -t "simpler" -d "(folders which clip folders)" -c (simpler plot configuration) -r (referenced csv)
+```
+The **-c** and **-r** arguments are optional. The okntool has its own built-in config and default referenced csv location which is two folder back of input folder directory.
+i.e. If the input folder diectory is "(example/result/okn)", the default referenced csv location is "(example/protocol.simpler.csv)".  
+
 ### oknserver_graph_plot_config.json
 This is a built-in config file which contains the information how trial plot, summary plot and progress plot will be drawn.  
-Please read more details about them in TRIAL_PLOT_README.md, SUMMARY_PLOT_README.md and PROGRESS_PLOT_README.md.
-If you wanna change the parameters of config file, copy and paste the build-in config file into a different directory.
+Please read more details about them in TRIAL_PLOT_README.md, SUMMARY_PLOT_README.md, PROGRESS_PLOT_README.md and TIDY_PLOT_README.md.
+If you wanna change the parameters of config file, copy and paste the built-in config file into a different directory.
 After that modify the config file and run the okntool with optional argument `-c (directory to new config file)`.  
 ```
 okntool -t "(plot_type)" -d "(directory to the folder)" -c "(directory to new config file)"
 ```
 
+### simpler_plot_config.json
+This is a built-in config file which contains the information how simpler plot will be drawn.  
+Please read more details in SIMLER_PLOT_README.md.
+If you wanna change the parameters of config file, copy and paste the built-in config file into a different directory.
+
 ### To upgrade version  
 In `Anaconda Powershell Prompt`,
 ```
 pip install -U okntool
 ```
 or
 ```
```

### Comparing `okntool-4.0.2/okntool/oknserver_graph_plot_config.json` & `okntool-4.1.0/okntool/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.2/okntool/okntool.py` & `okntool-4.1.0/okntool/okntool.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     end_index = string_input.find(end_marker) + len(end_marker)
     output_string = os.path.join(string_input[start_index:end_index], "okn_detector_summary.csv")
     print(f"okn detector summary csv dir {output_string}")
     return output_string
 
 
 # This function is to draw a graph with slow phase and quick phase overlay from the given config info
-def draw_graph_with_overlay(input_dir, trial_plot_info_input, signal_dir_input):
+def draw_graph_with_overlay(input_dir, trial_plot_info_input, signal_dir_input, output_file_dir_input=None):
     title = trial_plot_info_input["title"]
     x_label = trial_plot_info_input["x_label"]
     y_label = trial_plot_info_input["y_label"]
     x_data_column_name = trial_plot_info_input["x_data_column_name"]
     y_data_column_name = trial_plot_info_input["y_data_column_name"]
     graph_line_color = trial_plot_info_input["graph_line_color"]
     graph_line_thickness = trial_plot_info_input["graph_line_thickness"]
@@ -87,14 +87,15 @@
     sp_column_name = trial_plot_info_input["sp_column_name"]
     qp_column_name = trial_plot_info_input["qp_column_name"]
     sp_line_color = trial_plot_info_input["sp_line_color"]
     sp_line_thickness = trial_plot_info_input["sp_line_thickness"]
     qp_line_color = trial_plot_info_input["qp_line_color"]
     qp_line_thickness = trial_plot_info_input["qp_line_thickness"]
     output_image_name = trial_plot_info_input["output_image_name"]
+
     file_to_open = open(input_dir)
     csv_reader = csv.reader(file_to_open)
     header_array = []
     rows = []
     count_one = 0
 
     for row in csv_reader:
@@ -200,14 +201,18 @@
         for marker_time in event_marker_info:
             plt.axvline(x=float(marker_time), color=graph_line_color,
                         linestyle=":",
                         linewidth=graph_line_thickness, label=f"{marker_time}")
     csv_name = os.path.basename(input_dir)
     output_dir = input_dir.replace(csv_name, "")
     display_output_dir = os.path.join(output_dir, output_image_name)
+    if output_file_dir_input:
+        display_output_dir = output_file_dir_input
+        output_image_name = os.path.basename(output_file_dir_input)
+        output_dir = os.path.join(output_file_dir_input, os.pardir)
     os.chdir(output_dir)
     plt.savefig(output_image_name)
     plt.close()
 
     print(f"Trial plot has been saved at:{display_output_dir}")
 
 
@@ -239,14 +244,15 @@
         x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, None,
                                                                                x_data_column_name, y_data_column_name,
                                                                                folder_array, x_axis_limit,
                                                                                y_axis_limit, mean_offset,
                                                                                axis_adjustment_types,
                                                                                axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        # If there is folder to be ignored, take out that folder name from the folder array
         if ignore_folder_array:
             folder_array = [folder for folder in folder_array if folder not in ignore_folder_array]
         for folder_name in folder_array:
             trial_id, disk_condition = str(folder_name).split("_", 1)
             data_dir_to_be_used = os.path.join(data_dir, folder_name, f"updated_{folder_name}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_data_column_name)
             y_array = get_data_array(data_dir_to_be_used, y_data_column_name)
@@ -268,14 +274,15 @@
         x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, None,
                                                                                x_data_column_name, y_data_column_name,
                                                                                folder_array, x_axis_limit,
                                                                                y_axis_limit, mean_offset,
                                                                                axis_adjustment_types,
                                                                                axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        # If there is folder to be ignored, take out that folder name from the folder array
         if ignore_folder_array:
             folder_array = [folder for folder in folder_array if folder not in ignore_folder_array]
         for folder_name in folder_array:
             trial_id, disk_condition = str(folder_name).split("_", 1)
             data_dir_to_be_used = os.path.join(data_dir, folder_name, f"updated_{folder_name}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_data_column_name)
             y_array = get_data_array(data_dir_to_be_used, y_data_column_name)
@@ -403,15 +410,15 @@
             qp_array[ind] = np.nan
 
     return sp_array, qp_array
 
 
 # The main function to plot the combined graph with plan array/plot info
 # If max graph in a row is "none", there is no limitation of graph number in a row
-def plot_combined_graph(folder_dir_input, summary_plot_info_input):
+def plot_combined_graph(folder_dir_input, summary_plot_info_input, output_file_dir_input=None):
     graph_line_color = summary_plot_info_input["graph_line_color"]
     graph_line_thickness = summary_plot_info_input["graph_line_thickness"]
     max_graph_in_a_row = summary_plot_info_input["max_graph_in_a_row"]
     image_scale = summary_plot_info_input["image_scale"]
 
     plot_data_array, auto_adjust_info = get_plot_info(folder_dir_input, summary_plot_info_input)
 
@@ -421,14 +428,19 @@
     y_adjust_limit = auto_adjust_info["y_adjust_limit"]
     y_lower_limit = y_adjust_limit["lower_limit"]
     y_upper_limit = y_adjust_limit["upper_limit"]
 
     output_image_name = summary_plot_info_input["output_image_name"]
     display_output_dir = os.path.join(folder_dir_input, output_image_name)
     gaze_csv_dir = str(folder_dir_input).replace(os.path.basename(folder_dir_input), "gaze.csv")
+    output_dir = folder_dir_input
+    if output_file_dir_input:
+        display_output_dir = output_file_dir_input
+        output_image_name = os.path.basename(output_file_dir_input)
+        output_dir = os.path.join(output_file_dir_input, os.pardir)
     print(f"Gaze csv dir:{gaze_csv_dir}")
 
     if type(max_graph_in_a_row) == str and str(max_graph_in_a_row).lower() == "none":
         final_plot_array = []
         for logmar_level in logmar_level_array:
             temp_logmar_info_array = []
 
@@ -475,15 +487,15 @@
                             axs_title = f"{trial_id}({logmar_level})"
                         plt.plot(x_array, y_array, color=graph_line_color, linewidth=graph_line_thickness)
                         plt.plot(x_array, sp_array, color=sp_line_color, linewidth=sp_line_thickness)
                         plt.plot(x_array, qp_array, color=qp_line_color, linewidth=qp_line_thickness)
                         plt.title(axs_title)
                         plt.xlabel(x_label)
                         plt.ylabel(y_label)
-                        os.chdir(folder_dir_input)
+                        os.chdir(output_dir)
                         plt.savefig(output_image_name)
                         plt.close()
                     else:
                         fig, axs = plt.subplots(final_row_length, final_column_length,
                                                 figsize=(final_column_length * image_scale,
                                                          final_row_length * image_scale))
                         for row_index, plot_info in enumerate(final_plot_array):
@@ -535,15 +547,15 @@
                                     axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                             # Hide x labels and tick labels for top plots and y ticks for right plots.
                             for ax in axs.flat:
                                 ax.label_outer()
 
                         plt.tight_layout()
-                        os.chdir(folder_dir_input)
+                        os.chdir(output_dir)
                         fig.savefig(output_image_name)
                         plt.close()
                 else:
                     fig, axs = plt.subplots(final_row_length, final_column_length,
                                             figsize=(final_column_length * image_scale,
                                                      final_row_length * image_scale))
                     for row_index, plot_info in enumerate(final_plot_array):
@@ -593,15 +605,15 @@
                                 axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                         # Hide x labels and tick labels for top plots and y ticks for right plots.
                         for ax in axs.flat:
                             ax.label_outer()
 
                     plt.tight_layout()
-                    os.chdir(folder_dir_input)
+                    os.chdir(output_dir)
                     fig.savefig(output_image_name)
                     plt.close()
             else:
                 if final_column_length <= 1:
                     fig, axs = plt.subplots(final_row_length, final_column_length,
                                             figsize=(final_column_length * image_scale,
                                                      final_row_length * image_scale))
@@ -666,15 +678,15 @@
                                 axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                         # Hide x labels and tick labels for top plots and y ticks for right plots.
                         for ax in axs.flat:
                             ax.label_outer()
 
                     plt.tight_layout()
-                    os.chdir(folder_dir_input)
+                    os.chdir(output_dir)
                     fig.savefig(output_image_name)
                     plt.close()
                 else:
                     fig, axs = plt.subplots(final_row_length, final_column_length,
                                             figsize=(final_column_length * image_scale,
                                                      final_row_length * image_scale))
 
@@ -723,15 +735,15 @@
                                 axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                         # Hide x labels and tick labels for top plots and y ticks for right plots.
                         for ax in axs.flat:
                             ax.label_outer()
 
                     plt.tight_layout()
-                    os.chdir(folder_dir_input)
+                    os.chdir(output_dir)
                     fig.savefig(output_image_name)
                     plt.close()
             print(f"Summary plot has been saved at:{display_output_dir}")
         else:
             print("There is nothing to plot")
     else:
         if int(max_graph_in_a_row) <= 0:
@@ -800,24 +812,24 @@
                             axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                     # Hide x labels and tick labels for top plots and y ticks for right plots.
                     for ax in axs.flat:
                         ax.label_outer()
 
                 plt.tight_layout()
-                os.chdir(folder_dir_input)
+                os.chdir(output_dir)
                 fig.savefig(f"okn_detector_summary.png")
                 plt.close()
                 print(f"Summary plot has been saved at:{display_output_dir}")
             else:
                 print("There is nothing to plot")
 
 
 # The main function to plot the combined tidy graph with plan array/plot info
-def draw_tidy_graph(folder_dir_input, tidy_plot_info_input):
+def draw_tidy_graph(folder_dir_input, tidy_plot_info_input, output_file_dir_input=None):
     graph_line_color = tidy_plot_info_input["graph_line_color"]
     graph_line_thickness = tidy_plot_info_input["graph_line_thickness"]
     x_label = tidy_plot_info_input["x_label"]
     x_label_x_position = tidy_plot_info_input["x_label_x_position"]
     x_label_y_position = tidy_plot_info_input["x_label_y_position"]
     x_label_alignment = tidy_plot_info_input["x_label_alignment"]
     x_label_rotation = tidy_plot_info_input["x_label_rotation"]
@@ -871,14 +883,19 @@
     x_upper_limit = x_adjust_limit["upper_limit"]
     y_adjust_limit = adjust_limit_info["y_adjust_limit"]
     y_lower_limit = y_adjust_limit["lower_limit"]
     y_upper_limit = y_adjust_limit["upper_limit"]
 
     output_image_name = tidy_plot_info_input["output_image_name"]
     display_output_dir = os.path.join(folder_dir_input, output_image_name)
+    output_dir = folder_dir_input
+    if output_file_dir_input:
+        display_output_dir = output_file_dir_input
+        output_image_name = os.path.basename(output_file_dir_input)
+        output_dir = os.path.join(output_file_dir_input, os.pardir)
 
     final_plot_array = []
     for logmar_level in logmar_level_array:
         temp_logmar_info_array = []
 
         for info in plot_info:
             if info["logmar"] == logmar_level:
@@ -1018,27 +1035,27 @@
                         lw=time_boundary_line_thickness,
                         zorder=1000, transform=fig.transFigure,
                         figure=fig
                     )
                     fig.patches.extend([main_boundary, time_notation_boundary])
                 else:
                     fig.patches.extend([main_boundary])
-                os.chdir(folder_dir_input)
+                os.chdir(output_dir)
                 fig.savefig(output_image_name)
                 plt.close()
             print(f"Tidy plot has been saved at:{display_output_dir}")
         else:
             print("There is only 1 logmar level in the given data.")
             print("Therefore, we cannot draw tidy graph. It needs at least 2 logmar level.")
     else:
         print("There is nothing to plot")
 
 
 # This function is to draw va testing progress graph from the given config info
-def draw_progress_graph(folder_dir_input, progress_plot_info_input):
+def draw_progress_graph(folder_dir_input, progress_plot_info_input, output_file_dir_input=None):
     x_label = progress_plot_info_input["x_label"]
     y_label = progress_plot_info_input["y_label"]
     x_data_column_name = progress_plot_info_input["x_data_column_name"]
     y_data_column_name = progress_plot_info_input["y_data_column_name"]
     okn_matlab_column_name = progress_plot_info_input["okn_matlab_column_name"]
     phase_column_name = progress_plot_info_input["phase_column_name"]
     final_logmar_column_name = progress_plot_info_input["final_logmar_column_name"]
@@ -1074,15 +1091,15 @@
     legend_icon_size = progress_plot_info_input["legend_icon_size"]
     line_style_equivalent = progress_plot_info_input["line_style_equivalent"]
 
     summary_csv_dir = os.path.join(folder_dir_input, summary_csv_name)
 
     trial_data_csv_dir = os.path.join(folder_dir_input, trial_summary_csv_name)
 
-    out_image_dir = os.path.join(folder_dir_input, output_image_name)
+    display_output_dir = os.path.join(folder_dir_input, output_image_name)
 
     file_to_open = open(summary_csv_dir)
     csv_reader = csv.reader(file_to_open)
     header_array = []
     rows = []
     count_one = 0
 
@@ -1186,19 +1203,24 @@
         legend_array.append(final_va_line)
     # legend_array = [okn_marker, non_okn_marker, final_va_line]
     legend = plt.legend(handles=legend_array, loc=legend_location, fontsize=legend_font_size, fancybox=True)
     frame = legend.get_frame()
     frame.set_facecolor(legend_background_color)
     frame.set_edgecolor(legend_edge_color)
     frame.set_alpha(1)
-    os.chdir(folder_dir_input)
-    plt.savefig(out_image_dir)
+    output_dir = folder_dir_input
+    if output_file_dir_input:
+        display_output_dir = output_file_dir_input
+        output_image_name = os.path.basename(output_file_dir_input)
+        output_dir = os.path.join(output_file_dir_input, os.pardir)
+    os.chdir(output_dir)
+    plt.savefig(output_image_name)
     # plt.show()
     plt.close()
-    print(f"Staircase/progress plot has been saved at:{out_image_dir}")
+    print(f"Staircase/progress plot has been saved at:{display_output_dir}")
 
 
 # This function is to produce x and y adjustment limits according the type of adjustment
 # Type comes into the function as int number and is converted into string to be used
 # to retrieve the string type from adjustment dictionary
 def get_adjust_limit(data_dir_input, csv_name, x_header_input, y_header_input, folder_array_input,
                      x_axis_limit_input, y_axis_limit_input, mean_offset_input,
@@ -1215,15 +1237,18 @@
     elif adjustment_type == "min_max_mean":
         x_lower_limit_array = []
         x_upper_limit_array = []
         y_lower_limit_array = []
         y_upper_limit_array = []
         for folder in folder_array_input:
             if not csv_name:
+                # Default csv name
                 csv_name = f"updated_{folder}.csv"
+            # Error handling for value error
+            # IF there is value error that that folder, its name will be put into the ignore_folder_array
             try:
                 data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
                 x_array = get_data_array(data_dir_to_be_used, x_header_input)
                 x_lower_limit_array.append(min(x_array))
                 x_upper_limit_array.append(max(x_array))
                 y_array = get_data_array(data_dir_to_be_used, y_header_input)
                 y_lower_limit_array.append(min(y_array))
@@ -1239,15 +1264,18 @@
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     elif adjustment_type == "mean_offset":
         x_lower_limit_array = []
         x_upper_limit_array = []
         for folder in folder_array_input:
             if not csv_name:
+                # Default csv name
                 csv_name = f"updated_{folder}.csv"
+            # Error handling for value error
+            # IF there is value error that that folder, its name will be put into the ignore_folder_array
             try:
                 data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
                 x_array = get_data_array(data_dir_to_be_used, x_header_input)
                 # print(data_dir_to_be_used)
                 x_lower_limit_array.append(min(x_array))
                 x_upper_limit_array.append(max(x_array))
                 y_array = get_data_array(data_dir_to_be_used, y_header_input)
@@ -1264,15 +1292,18 @@
     else:
         x_lower_limit_array = []
         x_upper_limit_array = []
         y_lower_limit_array = []
         y_upper_limit_array = []
         for folder in folder_array_input:
             if not csv_name:
+                # Default csv name
                 csv_name = f"updated_{folder}.csv"
+            # Error handling for value error
+            # IF there is value error that that folder, its name will be put into the ignore_folder_array
             try:
                 data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
                 x_array = get_data_array(data_dir_to_be_used, x_header_input)
                 x_lower_limit_array.append(min(x_array))
                 x_upper_limit_array.append(max(x_array))
                 y_array = get_data_array(data_dir_to_be_used, y_header_input)
                 y_lower_limit_array.append(min(y_array))
@@ -1430,15 +1461,15 @@
         with config_resources.path("okntool", config_name_input) as p:
             config_location = p
     else:
         config_location = None
     return config_location
 
 
-def draw_simpler_graph(folder_dir_input, config_input, referenced_csv_to_be_used):
+def draw_simpler_graph(folder_dir_input, config_input, referenced_csv_to_be_used, output_file_dir_input=None):
     graph_line_color = config_input["graph_line_color"]
     graph_line_thickness = config_input["graph_line_thickness"]
     x_label = config_input["x_label"]
     x_label_x_position = config_input["x_label_x_position"]
     x_label_y_position = config_input["x_label_y_position"]
     x_label_alignment = config_input["x_label_alignment"]
     x_label_rotation = config_input["x_label_rotation"]
@@ -1492,14 +1523,19 @@
     x_upper_limit = x_adjust_limit["upper_limit"]
     y_adjust_limit = adjust_limit_info["y_adjust_limit"]
     y_lower_limit = y_adjust_limit["lower_limit"]
     y_upper_limit = y_adjust_limit["upper_limit"]
 
     output_image_name = config_input["output_image_name"]
     display_output_dir = os.path.join(folder_dir_input, output_image_name)
+    output_dir = folder_dir_input
+    if output_file_dir_input:
+        display_output_dir = output_file_dir_input
+        output_image_name = os.path.basename(output_file_dir_input)
+        output_dir = os.path.join(output_file_dir_input, os.pardir)
 
     final_plot_array = []
     for logmar_level in logmar_level_array:
         temp_logmar_info_array = []
 
         for info in plot_info:
             if info["logmar"] == logmar_level:
@@ -1639,15 +1675,15 @@
                         lw=time_boundary_line_thickness,
                         zorder=1000, transform=fig.transFigure,
                         figure=fig
                     )
                     fig.patches.extend([main_boundary, time_notation_boundary])
                 else:
                     fig.patches.extend([main_boundary])
-                os.chdir(folder_dir_input)
+                os.chdir(output_dir)
                 fig.savefig(output_image_name)
                 plt.close()
             print(f"Simpler plot has been saved at:{display_output_dir}")
         else:
             print("There is only 1 logmar level in the given data.")
             print("Therefore, we cannot draw simpler graph. It needs at least 2 logmar level.")
     else:
@@ -1660,36 +1696,38 @@
     x_data_column_name = plot_info_input["x_data_column_name"]
     y_data_column_name = plot_info_input["y_data_column_name"]
     x_axis_limit = plot_info_input["x_axis_limit"]
     y_axis_limit = plot_info_input["y_axis_limit"]
     mean_offset = plot_info_input["mean_offset"]
     axis_adjustment_types = plot_info_input["axis_adjustment_types"]
     axis_adjustment_type_number = plot_info_input["axis_adjustment_type_number"]
-    signal_csv_folder_name = plot_info_input["signal_csv_folder_name"]
+    # signal_csv_folder_name = plot_info_input["signal_csv_folder_name"]
     signal_csv_name = plot_info_input["signal_csv_name"]
     sp_column_name = plot_info_input["sp_column_name"]
     qp_column_name = plot_info_input["qp_column_name"]
     sp_line_color = plot_info_input["sp_line_color"]
     sp_line_thickness = plot_info_input["sp_line_thickness"]
     qp_line_color = plot_info_input["qp_line_color"]
     qp_line_thickness = plot_info_input["qp_line_thickness"]
     info_array = get_info_array_for_simpler_plot(referenced_csv_dir_input, "logMAR", "filename")
+    # Get the folder away from info dictionary array in which index is 2
     folder_array = [info[2] for info in info_array]
     # print(folder_array)
 
     adjustment_type = axis_adjustment_types[str(axis_adjustment_type_number)]
     if adjustment_type == "mean_offset":
         plot_info_array = []
         x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, signal_csv_name,
                                                                                x_data_column_name, y_data_column_name,
                                                                                folder_array, x_axis_limit,
                                                                                y_axis_limit, mean_offset,
                                                                                axis_adjustment_types,
                                                                                axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        # If there is folder to be ignored, take out the info dictionary for that folder from info array
         if ignore_folder_array:
             info_array = [info for info in info_array if info[2] not in ignore_folder_array]
         for trial_id, logmar_level, folder_name in info_array:
             signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_name)
             x_array = get_data_array(signal_csv_dir, x_data_column_name)
             y_array = get_data_array(signal_csv_dir, y_data_column_name)
             y_mean = np.nanmean(y_array)
@@ -1709,14 +1747,15 @@
         x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, signal_csv_name,
                                                                                x_data_column_name, y_data_column_name,
                                                                                folder_array, x_axis_limit,
                                                                                y_axis_limit, mean_offset,
                                                                                axis_adjustment_types,
                                                                                axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        # If there is folder to be ignored, take out the info dictionary for that folder from info array
         if ignore_folder_array:
             info_array = [info for info in info_array if info[2] not in ignore_folder_array]
         for trial_id, logmar_level, folder_name in info_array:
             signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_name)
             x_array = get_data_array(signal_csv_dir, x_data_column_name)
             y_array = get_data_array(signal_csv_dir, y_data_column_name)
             sp_array, qp_array = get_sp_and_qp_array(signal_csv_dir, sp_column_name, qp_column_name,
@@ -1757,42 +1796,61 @@
         folder_name = raw_file_name[raw_file_name.find("./") + 2:raw_file_name.find(".mp4")]
         trial_id = folder_name[folder_name.find("trial-"):folder_name.find("-disks")]
         output_array.append([trial_id, logmar_level, folder_name])
 
     return output_array
 
 
+def check_image_file_name(file_name_input, ending_array_input):
+    return True if any([end in file_name_input for end in ending_array_input]) else False
+
+
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='4.0.2'),
+    parser.add_argument('--version', action='version', version='4.1.0'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
                         help="trial, summary, (staircase or progress), tidy or simpler", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
                         help="config file to be used", metavar="config location")
     parser.add_argument("-r", dest="referenced_csv", required=False, default=sys.stdin,
-                        help="csv file to be referenced", metavar="referenced csv location")
+                        help="referenced csv file to be referenced", metavar="referenced csv")
+    parser.add_argument("-o", dest="output", required=False, default=sys.stdin,
+                        help="output directory and file name", metavar="output")
 
     args = parser.parse_args()
     directory_input = str(args.directory_input)
     type_input = str(args.plot_type)
     config_file_location = str(args.config_dir)
     referenced_csv_dir = str(args.referenced_csv)
+    output_dir = str(args.output)
     config_dir_exist = False
     config_input = False if "_io.TextIOWrapper" in config_file_location else True
     referenced_csv_input = False if "_io.TextIOWrapper" in referenced_csv_dir else True
+    output_dir_input = False if "_io.TextIOWrapper" in output_dir else True
+    image_file_ending_array = ['.png', '.jpg', '.jpeg', '.tiff', '.bmp', '.gif']
+    output_file_name = None
+    if output_dir_input:
+        output_folder = os.path.join(output_dir, os.pardir)
+        output_folder_exist = os.path.isdir(output_folder)
+        if output_folder_exist:
+            output_file_name = os.path.basename(output_dir)
+    else:
+        output_folder_exist = False
     # config_name_dict = {}
     # config_name_dict["trial"] = "oknserver_graph_plot_config.json"
     # config_name_dict["summary"] = "oknserver_graph_plot_config.json"
     # config_name_dict["staircase"] = "oknserver_graph_plot_config.json"
     # config_name_dict["progress"] = "oknserver_graph_plot_config.json"
     # config_name_dict["tidy"] = "oknserver_graph_plot_config.json"
     # config_name_dict["simpler"] = "simpler_plot_config.json"
+
+    # Dictionary to retrieve the name of config file according the type
     config_name_dict = {"trial": "oknserver_graph_plot_config.json", "summary": "oknserver_graph_plot_config.json",
                         "staircase": "oknserver_graph_plot_config.json", "progress": "oknserver_graph_plot_config.json",
                         "tidy": "oknserver_graph_plot_config.json", "simpler": "simpler_plot_config.json"}
 
     config_name = config_name_dict[type_input]
 
     # print(config_file_location)
@@ -1839,63 +1897,122 @@
         if plot_config_info is not None:
             print(f"{config_name} is found.")
         else:
             print(f"Essential config file:{config_name} is missing.")
     else:
         plot_config_info = None
 
+    if output_dir_input:
+        if output_folder_exist:
+            print("Output file location input is found and output folder exists.")
+        else:
+            print("Output file location input is found but output folder does not exist.")
+            print("Therefore, default output location will be used.")
+    else:
+        print("There is no output file location input.")
+        print("Therefore, default output location will be used.")
+
     if config_dir_exist and dir_exist and plot_config_info is not None:
         if type_input == "trial":
             # Retrieve trial plot info from config
             trial_plot_info = plot_config_info["trial_plot"]
 
             csv_name = f"updated_{os.path.basename(directory_input)}.csv"
             print(f"csv name {csv_name}")
             updated_csv_dir = os.path.join(directory_input, csv_name)
             print(f"update csv dir {updated_csv_dir}")
             signal_csv_folder_name = trial_plot_info["signal_csv_folder_name"]
             signal_csv_name = trial_plot_info["signal_csv_name"]
             signal_csv_dir = os.path.join(directory_input, signal_csv_folder_name, signal_csv_name)
             print(f"signal csv dir {signal_csv_dir}")
-            draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir)
+            if output_folder_exist:
+                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                if file_name_valid:
+                    draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir, output_dir)
+                else:
+                    print("Invalid image file name")
+                    return
+            else:
+                draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir)
         elif type_input == "summary":
             # Retrieve summary plot info from config
             summary_plot_info = plot_config_info["summary_plot"]
 
-            plot_combined_graph(directory_input, summary_plot_info)
+            if output_folder_exist:
+                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                if file_name_valid:
+                    plot_combined_graph(directory_input, summary_plot_info, output_dir)
+                else:
+                    print("Invalid image file name")
+                    return
+            else:
+                plot_combined_graph(directory_input, summary_plot_info)
         elif type_input == "staircase" or type_input == "progress":
             # Retrieve progress plot info from config
             progress_plot_info = plot_config_info["progress_plot"]
 
-            draw_progress_graph(directory_input, progress_plot_info)
+            if output_folder_exist:
+                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                if file_name_valid:
+                    draw_progress_graph(directory_input, progress_plot_info, output_dir)
+                else:
+                    print("Invalid image file name")
+                    return
+            else:
+                draw_progress_graph(directory_input, progress_plot_info)
         elif type_input == "tidy":
             # Retrieve progress plot info from config
             tidy_plot_info = plot_config_info["tidy_plot"]
 
-            draw_tidy_graph(directory_input, tidy_plot_info)
+            if output_folder_exist:
+                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                if file_name_valid:
+                    draw_tidy_graph(directory_input, tidy_plot_info, output_dir)
+                else:
+                    print("Invalid image file name")
+                    return
+            else:
+                draw_tidy_graph(directory_input, tidy_plot_info)
         elif type_input == "simpler":
-            # Retrieve progress plot info from config
+            # Retrieve simpler plot info from config
             simpler_plot_info = plot_config_info["simpler_plot"]
             if referenced_csv_input:
-                draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
+                if output_folder_exist:
+                    file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                    if file_name_valid:
+                        draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir, output_dir)
+                    else:
+                        print("Invalid image file name")
+                        return
+                else:
+                    draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
             else:
                 print("There is no referenced csv input in the commandline.")
                 try:
                     referenced_csv_name = simpler_plot_info["summary_csv_name"]
                 except KeyError:
                     print("There is no referenced csv info in the config.")
                     referenced_csv_name = "protocol.simpler.csv"
                     print(f"Therefore using default name => {referenced_csv_name} as default referenced csv")
+                # os.path.abspath(os.path.join(directory_input, os.pardir)) == retrieve the parent path
                 one_folder_back_dir = os.path.abspath(os.path.join(directory_input, os.pardir))
                 two_folder_back_dir = os.path.abspath(os.path.join(one_folder_back_dir, os.pardir))
                 referenced_csv_dir = os.path.join(two_folder_back_dir, referenced_csv_name)
                 referenced_csv_dir_exist = os.path.isfile(referenced_csv_dir)
                 if referenced_csv_dir_exist:
                     print(f"Default referenced csv location:{referenced_csv_dir} is found.")
                     print("Start plotting simpler plot...")
-                    draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
+                    if output_folder_exist:
+                        file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                        if file_name_valid:
+                            draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir, output_dir)
+                        else:
+                            print("Invalid image file name")
+                            return
+                    else:
+                        draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
                 else:
                     print(f"Default referenced csv location:{referenced_csv_dir} cannot be found.")
         else:
             print("wrong plot type or invalid plot type.")
     else:
         return
```

### Comparing `okntool-4.0.2/okntool/simpler_plot_config.json` & `okntool-4.1.0/okntool/simpler_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.2/okntool.egg-info/PKG-INFO` & `okntool-4.1.0/okntool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.2
+Version: 4.1.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.2/setup.py` & `okntool-4.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='4.0.2',
+    version='4.1.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
     packages=find_packages(),
     include_package_data=True,
-    package_data={'': ['oknserver_graph_plot_config.json', 'simpler_plot_config.json']},
+    package_data={'': ['oknserver_graph_plot_config.json',
+                       'simpler_plot_config.json',
+                       'indi_va_table_template.html',
+                       'sum_va_table_template.html']},
     entry_points={
         'console_scripts': [
             'okntool = okntool.okntool:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

