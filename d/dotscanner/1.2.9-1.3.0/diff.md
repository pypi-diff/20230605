# Comparing `tmp/dotscanner-1.2.9.tar.gz` & `tmp/dotscanner-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.2.9.tar", last modified: Sun Oct 30 13:50:51 2022, max compression
+gzip compressed data, was "dist/dotscanner-1.3.0.tar", last modified: Mon Jun  5 03:16:55 2023, max compression
```

## Comparing `dotscanner-1.2.9.tar` & `dotscanner-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.899818 dotscanner-1.2.9/
--rw-r--r--   0 holly      (501) staff       (20)    13890 2022-10-30 13:50:51.899591 dotscanner-1.2.9/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    11824 2022-10-30 11:35:44.000000 dotscanner-1.2.9/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.893289 dotscanner-1.2.9/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2183 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)     8425 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5306 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     3291 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)     8582 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     4098 2022-10-30 13:47:00.000000 dotscanner-1.2.9/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.896602 dotscanner-1.2.9/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5240 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1879 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3477 2022-10-30 13:03:04.000000 dotscanner-1.2.9/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5145 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    14800 2022-10-30 13:28:42.000000 dotscanner-1.2.9/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    10626 2022-10-30 13:35:09.000000 dotscanner-1.2.9/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3135 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.894608 dotscanner-1.2.9/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13890 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      898 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       57 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.897293 dotscanner-1.2.9/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     5629 2022-10-30 13:38:35.000000 dotscanner-1.2.9/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    10355 2022-10-30 13:38:26.000000 dotscanner-1.2.9/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2022-10-30 13:50:51.899916 dotscanner-1.2.9/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1460 2022-10-30 11:35:44.000000 dotscanner-1.2.9/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.899166 dotscanner-1.2.9/tests/
--rw-r--r--   0 holly      (501) staff       (20)      554 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3857 2022-10-30 12:55:59.000000 dotscanner-1.2.9/tests/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5098 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     1690 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)     4802 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     9963 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     2155 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.392806 dotscanner-1.3.0/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.0/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13274 2023-06-05 03:16:55.392655 dotscanner-1.3.0/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12617 2023-06-05 03:13:05.000000 dotscanner-1.3.0/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.387288 dotscanner-1.3.0/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3552 2023-06-05 02:53:53.000000 dotscanner-1.3.0/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     9355 2023-06-05 02:34:51.000000 dotscanner-1.3.0/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6128 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10494 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     5321 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.389727 dotscanner-1.3.0/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3343 2023-06-05 02:53:52.000000 dotscanner-1.3.0/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5569 2023-06-05 02:53:50.000000 dotscanner-1.3.0/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16340 2023-06-05 02:53:51.000000 dotscanner-1.3.0/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    14995 2023-06-05 02:53:52.000000 dotscanner-1.3.0/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-05 02:53:49.000000 dotscanner-1.3.0/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.388224 dotscanner-1.3.0/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13274 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1000 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-05 03:16:55.000000 dotscanner-1.3.0/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.390485 dotscanner-1.3.0/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6218 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.0/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-05 03:16:55.392863 dotscanner-1.3.0/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-05 03:16:55.000000 dotscanner-1.3.0/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.391579 dotscanner-1.3.0/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5572 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     4068 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-05 03:16:55.392401 dotscanner-1.3.0/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      471 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)      962 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4000 2023-06-05 02:53:50.000000 dotscanner-1.3.0/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8414 2023-06-05 02:24:39.000000 dotscanner-1.3.0/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.2.9/PKG-INFO` & `dotscanner-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,193 +1,199 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.2.9
+Version: 1.3.0
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
-Description: # Dot Scanner
-        > Software designed for analysis of microscope imaging data
-        
-        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
-        
-        Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
-        
-        ## Getting Started
-        
-        ### Dependencies
-        
-        [Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
-        
-        ### Installation
-        
-        To install Dot Scanner, open a terminal window and run the following command:
-        
-        ```
-        pip install dotscanner
-        ```
-        
-        *(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
-        
-        ### Running the Software
-        
-        To launch the main graphical user interface (GUI), run the following command:
-        
-        ```
-        dotscanner
-        ```
-        
-        Some demo images are included in the `images/demo/` folder, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
-        
-        ## The Configurations Window
-        The first window displayed in the GUI is the Configurations Window:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
-        
-        If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the `images/demo/` folder can be downloaded to try this out for oneself):
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
-        
-        If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
-        
-        The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
-        
-        If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
-        
-        If **Lifetime** is selected, some additional options will appear:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
-        
-        ### Descriptions of Configuration Options
-        
-        #### Save figures
-        Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
-        
-        #### Blob size
-        This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
-        
-        #### Dot size
-        Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
-        
-        #### Thresholds
-        There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
-        1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
-        2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
-        3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
-        
-        ### Descriptions of Configuration Options for the Lifetime Program
-        
-        #### Start image
-        This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
-        
-        #### Skips allowed
-        This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
-              
-        #### Remove edge frames
-        This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
-        
-        #### Edit defaults
-        This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
-        
-        Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
-        
-        ## The Threshold Adjustment Window
-        This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
-        
-        From top to bottom, these button groups perform the following actions:
-        
-        #### View
-        These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
-        
-        #### Contrast
-        These buttons adjust the contrast of the image.
-        
-        #### Dots
-        These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
-        
-        #### Blobs
-        These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
-        
-        #### Edit
-        This button changes the left button bar view to display some manual threshold adjustment options:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
-        
-        *(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
-        
-        #### Reset
-        This button resets the adjusted thresholds back to the default values.
-        
-        #### Skip
-        This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
-        
-        ## The Region Selector Window
-        Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
-        
-        This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
-        
-        Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
-        
-        ## Authors
-        
-        Holly Allen (holly.allen@colorado.edu)
-        
-        Brian Davis
-        
-        ## Release History
-        
-        * 1.2.9
-             * Bug fixes
-        * 1.2.0
-             * Added options for editing the configuration file
-             * Added startup processes to check the configuration file for errors
-        * 1.1.0
-             * Migrated the remaining portions of the app from a terminal interface to a GUI
-        * 1.0.0
-             * Initial Release
-        
-        ## License
-        
-        This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
-        
-        ## Development
-        
-        To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
-        
-        ```
-        python -m dotscanner
-        ```
-        
-        *(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
-        
-        ### Testing
-        
-        Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
-        
-        ```
-        python -m unittest
-        ```
-        
-        *(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
-        
-        ### Bug Reports and Feature Requests
-        
-        To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
-        
-        ## Citations
-        
-        When using this program on data used in published works, please cite:
-        
-        Allen, H., Davis, B., Patel, J., & Gu, Y. 2022 (in prep.)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dot Scanner
+> Software designed for analysis of microscope imaging data
+
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
+
+Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
+
+## Getting Started
+
+### Dependencies
+
+[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
+
+### Installation
+
+To install Dot Scanner, open a terminal window and run the following command:
+
+```
+pip install dotscanner
+```
+
+*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+
+### Running the Software
+
+To launch the main graphical user interface (GUI), run the following command:
+
+```
+dotscanner
+```
+
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+
+## The Configurations Window
+The first window displayed in the GUI is the Configurations Window:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
+
+If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
+![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
+
+If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
+
+The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
+
+If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
+
+If **Lifetime** is selected, some additional options will appear:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
+
+### Descriptions of Configuration Options
+
+#### Save figures
+Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
+
+#### Blob size
+This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
+
+#### Dot size
+Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
+
+#### Thresholds
+There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
+1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
+2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
+3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
+
+#### Edit defaults
+This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
+
+#### Use previous analysis
+This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+
+Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
+
+### Descriptions of Configuration Options for the Lifetime Program
+
+#### Start image
+This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
+
+#### Skips allowed
+This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
+      
+#### Remove edge frames
+This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
+
+## The Threshold Adjustment Window
+This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
+
+From top to bottom, these button groups perform the following actions:
+
+#### View
+These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
+
+#### Contrast
+These buttons adjust the contrast of the image.
+
+#### Dots
+These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
+
+#### Blobs
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
+
+#### Edit
+This button changes the left button bar view to display some manual threshold and size adjustment options:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
+
+*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+
+#### Reset
+This button resets the adjusted thresholds back to the default values.
+
+#### Skip
+This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
+
+## The Region Selector Window
+Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
+
+This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
+
+Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
+
+*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+
+## Authors
+
+Holly Allen (holly.allen@colorado.edu)
+
+Brian Davis
+
+## Release History
+
+* 1.3.0
+     * Added option to re-analyze data without redrawing regions
+     * Added particle displacement tracking during lifetime measurement
+     * Added histogram output for lifetimes measurements
+* 1.2.0
+     * Added options for editing the configuration file
+     * Added startup processes to check the configuration file for errors
+* 1.1.0
+     * Migrated the remaining portions of the app from a terminal interface to a GUI
+* 1.0.0
+     * Initial Release
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
+
+## Development
+
+To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
+
+```
+python -m dotscanner
+```
+
+*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+
+### Testing
+
+Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
+
+```
+python -m unittest
+```
+
+*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+
+### Bug Reports and Feature Requests
+
+To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
+
+## Citations
+
+When using this program on data used in published works, please cite:
+
+Allen, H., Davis, B., Patel, J., & Gu, Y. 2023 (in prep.)
```

### Comparing `dotscanner-1.2.9/README.md` & `dotscanner-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
 To launch the main graphical user interface (GUI), run the following command:
 
 ```
 dotscanner
 ```
 
-Some demo images are included in the `images/demo/` folder, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
 
 ## The Configurations Window
 The first window displayed in the GUI is the Configurations Window:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
 
-If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the `images/demo/` folder can be downloaded to try this out for oneself):
+If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
 
 If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
 
 The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
 
 If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
@@ -61,30 +61,33 @@
 
 #### Thresholds
 There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
 1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
+#### Edit defaults
+This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
+
+#### Use previous analysis
+This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+
+Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
+
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
 This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
 
 #### Skips allowed
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
       
 #### Remove edge frames
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
-#### Edit defaults
-This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
-
-Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
-
 ## The Threshold Adjustment Window
 This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
@@ -93,21 +96,21 @@
 #### Contrast
 These buttons adjust the contrast of the image.
 
 #### Dots
 These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
 
 #### Blobs
-These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
 
 #### Edit
-This button changes the left button bar view to display some manual threshold adjustment options:
+This button changes the left button bar view to display some manual threshold and size adjustment options:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
 
-*(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
 
 #### Reset
 This button resets the adjusted thresholds back to the default values.
 
 #### Skip
 This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
 
@@ -115,24 +118,28 @@
 Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
 
 This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
 
 Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
 
+*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+
 ## Authors
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.2.9
-     * Bug fixes
+* 1.3.0
+     * Added option to re-analyze data without redrawing regions
+     * Added particle displacement tracking during lifetime measurement
+     * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
      * Added startup processes to check the configuration file for errors
 * 1.1.0
      * Migrated the remaining portions of the app from a terminal interface to a GUI
 * 1.0.0
      * Initial Release
@@ -165,8 +172,8 @@
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
 
 ## Citations
 
 When using this program on data used in published works, please cite:
 
-Allen, H., Davis, B., Patel, J., & Gu, Y. 2022 (in prep.)
+Allen, H., Davis, B., Patel, J., & Gu, Y. 2023 (in prep.)
```

### Comparing `dotscanner-1.2.9/dotscanner/dataprocessing.py` & `dotscanner-1.3.0/dotscanner/dataprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,67 @@
 	maxElement = float("-inf")
 	for index, element in enumerate(array):
 		if element > maxElement:
 			maxElement = element
 			maxIndex = index
 	return maxIndex
 
+def getClosestCoordWithinRadius(y, x, coordMap, radius):
+	if coordExists(y, x, coordMap):
+		return y, x
+	
+	yStart, xStart = y, x
+	visited = {(yStart, xStart)}
+	queue = []
+	
+	for stepSize in range(1, radius + 1):
+		boundaries = getBoundaries(yStart, xStart, stepSize)
+		addCentralNeighbors(yStart, xStart, queue, stepSize, radius)
+		while queue:
+			coordToDirectionMap = queue.pop(0)
+			coord, direction = coordToDirectionMap.popitem()
+			y, x = coord
+			if coordExists(y, x, coordMap):
+				return coord
+			visited.add(coord)
+			addNeighbors(y, x, queue, direction, visited, boundaries)
+
+def getBoundaries(yStart, xStart, stepSize):
+	return {
+		"top": yStart - stepSize,
+		"bottom": yStart + stepSize,
+		"left": xStart - stepSize,
+		"right": xStart + stepSize
+	}
+
+def addCentralNeighbors(y, x, queue, stepSize, radius):
+	if stepSize <= radius:
+		queue.append({(y, x - stepSize): "vertical"})
+		queue.append({(y, x + stepSize): "vertical"})
+		queue.append({(y - stepSize, x): "horizontal"})
+		queue.append({(y + stepSize, x): "horizontal"})
+
+def addNeighbors(y, x, queue, direction, visited, boundaries):
+	if direction == "horizontal":
+		addHorizontalNeighbors(y, x, queue, visited, boundaries)
+	else:
+		addVerticalNeighbors(y, x, queue, visited, boundaries)
+
+def addHorizontalNeighbors(y, x, queue, visited, boundaries):
+	if x - 1 >= boundaries["left"] and (y, x - 1) not in visited:
+		queue.append({(y, x - 1): "horizontal"})
+	if x + 1 <= boundaries["right"] and (y, x + 1) not in visited:
+		queue.append({(y, x + 1): "horizontal"})
+
+def addVerticalNeighbors(y, x, queue, visited, boundaries):
+	if y - 1 >= boundaries["top"] and (y - 1, x) not in visited:
+		queue.append({(y - 1, x): "vertical"})
+	if y + 1 <= boundaries["bottom"] and (y + 1, x) not in visited:
+		queue.append({(y + 1, x): "vertical"})
+
 def getCoordPairsFromCoordMap(coordMap):
 	coordList = []
 	for y, xSet in coordMap.items():
 		for x in xSet:
 			coordList.append([x, y]) # For use with set_offsets(), which expects (x, y) coords
 	return coordList
 
@@ -69,15 +122,15 @@
 	path = matplotlib.path.Path(polygonVertices)
 	flattenedMask = path.contains_points(points)
 	mask = flattenedMask.reshape(len(data), len(data[0]))
 	coordsInPolygon = np.argwhere(mask)
 	return coordsInPolygon
 
 def getCoordMapsWithinPolygon(data, sums, lowerDotThresh, upperDotThresh, lowerBlobThresh, dotSize, 
-								polygonCoordMap, xMin, xMax, yMin, yMax):
+	polygonCoordMap, xMin, xMax, yMin, yMax):
 	dotCoords = {}
 	blobCoords = {}
 	for y in range(yMin, yMax + 1):
 		if y in polygonCoordMap:
 			for x in range(xMin, xMax + 1):
 				if x in polygonCoordMap[y]:
 					if sums[y][x] > lowerDotThresh:
@@ -89,15 +142,15 @@
 							else:
 								addCoordinate(y, x, dotCoords)
 	return dotCoords, blobCoords
 
 def getData(directory, filename):
 	image = Image.open(directory + filename)
 	data = np.array(image)
-	subtractedData = data - np.mean(image)
+	subtractedData = data - np.median(image)
 	return subtractedData
 
 def getFullDataSquareSum(data):
 	sums = np.zeros_like(data)
 
 	sums[:len(data)-1, :len(data[0]) - 1] += data[1:,             1:               ]
 	sums[:len(data)-1, :                ] += data[1:,             :                ]
```

### Comparing `dotscanner-1.2.9/dotscanner/strings.py` & `dotscanner-1.3.0/dotscanner/strings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,118 @@
 import settings.config as cfg
 
+class ProgramType:
+	DENSITY = "Density"
+	LIFETIME = "Lifetime"
+
 configurationsWindowTitle = "Dot Scanner - Configurations"
 
 defaultConfigurationsEditorWindowTitle = "Dot Scanner - Default Configurations"
 
-densityOutputFileHeader = f"# filename | density (per sq {'pix' if cfg.SCALE is None else 'um'}) | \
-error | lowerDotThreshScale | upperDotThreshScale | lowerBlobThreshScale | blobSize | dotSize | \
-polygon vertices (x, y)\n"
+def outputFileTopHeader(programType):
+	return f"\
+# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
+# Generated output file for {programType.lower()} measurement\n#"
+
+densityOutputFileHeader = f"{outputFileTopHeader(ProgramType.DENSITY)}\n\
+# The data columns are organized as follows:\n\
+# filename | number of dots | number of pixels surveyed | \
+density (per sq {'pix' if cfg.SCALE is None else 'um'}) | error | lowerDotThreshScale | \
+upperDotThreshScale | lowerBlobThreshScale | blobSize | dotSize | lowerContrast | upperContrast | \
+polygon vertices (x, y)\n#\n"
 
-fileNumberingException = "Filenames must contain sequentially-ordered numbers to calculate \
-lifetimes."
+fileNumberingException = "Filenames must contain sequentially-ordered numbers with no gaps and \
+have valid file extensions to calculate lifetimes."
 
 fileNumberingWarning = "WARNING: Filenames must contain sequentially-ordered numbers to calculate \
 lifetimes."
 
 filepathException = "Filepath must point to a file or directory."
 
 invalidPolygonWarning = "\nNo valid, enclosed polygon drawn. No measurements made."
 
+invalidDotAndBlobSizeEdit = "\nInvalid input. Previous dot and blob size values will be retained."
+
 invalidThresholdEdit = "\nInvalid input. Previous threshold values will be retained."
 
 lifetimeSingleFileException = "Lifetimes must be calculated using a directory of images, \
 not a single image."
 
 lifetimeSingleFileWarning = "WARNING: Lifetimes must be calculated using a directory of images, \
 not a single image."
 
 lowerBlobThreshScaleWarning = "\nWARNING: Lower blob threshold scale set below 1.0, which means \
 blobs can be dimmer than the brightest dots, which shouldn't happen. Setting to 1.0."
 
 maxContrastWarning = "\nWARNING: Max contrast reached. Previous contrast values will be retained."
 
-noFilesException = "No files selected. Check the values of 'FILEPATH' and 'START_IMAGE' in the \
-configurations file."
+noFilesException = "No valid files selected. Does the folder you've selected contain files with \
+valid file extensions (e.g., .tiff)? Subfolders within the selected folder will not be scanned for \
+files. Check the values of 'FILEPATH' and 'START_IMAGE' in the configurations file."
 
 programNameException = "Invalid program name selected in configurations file."
 
 regionSelectorWindowTitle = "Dot Scanner - Region Selection (click the plot to add polygon \
 vertices)"
 
 startImageDirectoryWarning = "WARNING: Start image must be in the same directory as the other \
 lifetime files."
 
 thresholdAdjusterWindowTitle = "Dot Scanner - Threshold Adjustment"
 
 tooFewFramesException = "There are not enough images to get meaningful lifetimes."
 
-unitsInconsistentException = f"Inconsistent units with other measurements already recorded in \
-{cfg.DENSITY_OUTPUT_FILENAME}. To record measurements in units of per sq pix, set SCALE to None \
-in configurations file. Otherwise, set the scale to the scale that was selected for the previous \
-measurements."
-
 upperDotThreshScaleWarning = "\nWARNING: Upper dot threshold scale set below lower dot threshold \
 scale. Previous threshold values will be retained."
 
 windowSizeWarning = "\nWARNING: The current window height is smaller than 550 pixels, potentially \
 resulting in some buttons not being visible. However, the Return key will still allow confirmation \
 in each window, and the Escape key will allow for skipping files, when the option is available."
 
 def alreadyMeasuredNotification(filename):
 	return f"\nFile {filename} already measured in {cfg.DENSITY_OUTPUT_FILENAME} file. Skipping."
 
-def densityOutput(filename, density, error, thresholds, dotSize, blobSize, polygon):
+def densityOutput(filename, dotTotal, surveyedArea, density, error, microscopeImage, userSettings):
+	thresholds = microscopeImage.thresholds
+	polygon = microscopeImage.polygon
+	dotSize = userSettings.dotSize
+	blobSize = userSettings.blobSize
+	lowerContrast = userSettings.lowerContrast
+	upperContrast = userSettings.upperContrast
+	
 	verticesStringList = []
 	for vertex in polygon[:-1]:
 		y, x = vertex
 		verticesStringList.append(f"({x}, {y})")
 	verticesString = ", ".join(verticesStringList)
 	
-	return f"{filename} {density} {error} {thresholds[0]} {thresholds[1]} {thresholds[2]} \
-{blobSize} {dotSize} {verticesString}\n"
+	return f"{filename} {dotTotal} {surveyedArea} {density} {error} {thresholds[0]} \
+{thresholds[1]} {thresholds[2]} {blobSize} {dotSize} {lowerContrast} {upperContrast} \
+{verticesString}\n"
 
 def fileSkippedNotification(filename):
 	return f"\nFile {filename} skipped"
 
-def lifetimeOutputFileHeader(polygon, userSettings):
+def lifetimeOutputFileHeader(microscopeImage, userSettings):
 	verticesStringList = []
-	for vertex in polygon[:-1]:
+	for vertex in microscopeImage.polygon[:-1]:
 		y, x = vertex
 		verticesStringList.append(f"({x}, {y})")
 	verticesString = ", ".join(verticesStringList)
 	
 	thresholdsStringList = []
-	for threshold in userSettings.thresholds:
+	for threshold in microscopeImage.thresholds:
 		thresholdsStringList.append(str(threshold))
 	thresholdsString = ", ".join(thresholdsStringList)
 	
-	return f"# Polygon vertices (x, y): {verticesString}\n\
+	return f"{outputFileTopHeader(ProgramType.LIFETIME)}\n\
+# Polygon vertices (x, y): {verticesString}\n\
 # Threshold scales: {thresholdsString}\n\
+# Contrast settings: {userSettings.lowerContrast}, {userSettings.upperContrast}\n\
 # Dot size: {userSettings.dotSize} | Blob size: {userSettings.blobSize} | Remove edge frames: \
-{userSettings.removeEdgeFrames} | Skips allowed: {userSettings.skipsAllowed}\n\
-#\n# x | y | lifetime | starting image\n"
+{userSettings.removeEdgeFrames} | Save figures: {userSettings.saveFigures} | Skips allowed: \
+{userSettings.skipsAllowed}{getLifetimeStartImageHeaderText(userSettings.startImage)}\n#\n\
+# The data columns are organized as follows:\n\
+# x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
+
+def getLifetimeStartImageHeaderText(startImage):
+	return f" | Start image: {startImage.split('/')[-1]}" if startImage != "" else ""
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.0/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,43 +15,43 @@
 		else:
 			self.filepath = os.path.dirname(self.userSettings.filepath)
 		
 		self.filepathFrame = tk.Frame(self.window)
 		
 		self.labelFilepath = tk.Label(self.window, text="Default filepath:")
 		self.labelSelectedPath = tk.Label(self.window, text="No default filepath selected", 
-											bg="white", fg="lightgray")
+			bg="white", fg="lightgray")
 		self.labelSaved = tk.Label(self.window, text=" Saved!", fg="green")
 		self.showFilepath()
 		
 		self.labelFilepath.pack(in_=self.filepathFrame, side=tk.LEFT)
 		self.labelSelectedPath.pack(in_=self.filepathFrame, side=tk.LEFT)
 		
 		self.navigation = tk.Frame(self.window)
 
 		self.buttonSelectFolder = tk.Button(self.window, text="Browse...", 
-											command=self.browseFolders)
+			command=self.browseFolders)
 		self.buttonClearDefaultPath = tk.Button(self.window, text="Clear", fg="red", 
-											command=self.clearDefaultPath)
+			command=self.clearDefaultPath)
 		self.buttonSaveDefaultPath = tk.Button(self.window, text="Save", fg="blue", 
-											command=self.saveDefaultPath)
+			command=self.saveDefaultPath)
 		
 		self.buttonSelectFolder.pack(in_=self.navigation, side=tk.LEFT)
 		self.buttonClearDefaultPath.pack(in_=self.navigation, side=tk.LEFT)
 		self.buttonSaveDefaultPath.pack(in_=self.navigation, side=tk.LEFT)
 		
 		self.spacer = tk.Label(self.window, text=" ")
 		
 		self.configFileButtons = tk.Frame(self.window)
 		
 		self.configFileLabel = tk.Label(self.window, text="Config file:")
 		self.buttonEdit = tk.Button(self.window, text="Edit...", 
-									command=cm.showEditConfigFileDialog)
+			command=cm.showEditConfigFileDialog)
 		self.buttonReset = tk.Button(self.window, text="Reset", fg="red", 
-									command=cm.showResetConfigFileDialog)
+			command=cm.showResetConfigFileDialog)
 		
 		self.configFileLabel.pack(in_=self.configFileButtons, side=tk.LEFT)
 		self.buttonEdit.pack(in_=self.configFileButtons, side=tk.LEFT)
 		self.buttonReset.pack(in_=self.configFileButtons, side=tk.LEFT)
 				
 		self.filepathFrame.pack()
 		self.navigation.pack()
@@ -61,15 +61,15 @@
 		self.window.bind("<q>", self.quitWithQKey)
 		self.window.bind("<w>", self.closeWindowWithWKey)
 		
 		self.window.mainloop()
 
 	def browseFolders(self):
 		chosenFolder = filedialog.askdirectory(initialdir=self.filepath, 
-												title="Select a default starting folder")
+			title="Select a default starting folder")
 		if chosenFolder not in ["", " ", "/"]:
 			self.filepath = chosenFolder
 			displayedFolder = chosenFolder
 			if len(chosenFolder) > 50:
 				displayedFolder = "..." + chosenFolder[-50:]
 			self.labelSelectedPath.configure(text=displayedFolder, bg="white", fg="black")
 		self.unshowSavedText()
@@ -105,15 +105,15 @@
 		self.userSettings.filepath = self.filepath
 		self.userSettings.showFilepath()
 		self.userSettings.checkForWarning()
 	
 	def showFilepath(self):
 		if self.filepath in ["", " ", "/"]:
 			self.labelSelectedPath.configure(text="No default filepath selected", fg="lightgray", 
-												bg="white")
+				bg="white")
 		else:
 			displayedFilepath = self.filepath
 			if len(displayedFilepath) > 50:
 				displayedFilepath = "..." + displayedFilepath[-50:]
 			self.labelSelectedPath.configure(text=displayedFilepath, bg="white", fg="black")
 	
 	def showSavedText(self):
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.0/dotscanner/ui/DialogWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 		self.messageText = tk.Label(self.window, text=message)
 		
 		self.spacer2 = tk.Label(self.window, text=" ")
 		
 		self.buttonsFrame = tk.Frame(self.window)
 		
 		self.positiveButton = tk.Button(self.window, text=positiveButtonText, 
-										fg=positiveButtonColor, command=positiveButtonAction)
+			fg=positiveButtonColor, command=positiveButtonAction)
 		
 		if negativeButtonAction is None:
 			self.negativeButton = tk.Button(self.window, text=negativeButtonText, 
-											command=self.window.destroy)
+				command=self.window.destroy)
 			self.window.bind("<Escape>", self.closeWindowWithEscapeKey)
 		else:
 			self.negativeButton = tk.Button(self.window, text=negativeButtonText, 
-											command=negativeButtonAction)
+				command=negativeButtonAction)
 		
 		self.negativeButton.pack(in_=self.buttonsFrame, side=tk.LEFT)
 		self.positiveButton.pack(in_=self.buttonsFrame, side=tk.LEFT)
 		
 		self.spacer.pack()
 		self.messageText.pack()
 		self.spacer2.pack()
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.0/dotscanner/ui/MicroscopeImage.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 
 class MicroscopeImage:
 	def __init__(self, directory, filename, userSettings):
 		self.memoizedCoords = {}
 		self.polygon = [] # Vertices of the region selected for analysis (mutated by other classes)
 		self.skipped = False # Whether the image should be skipped (mutated by other classes)
 		
-		self.dotSize = userSettings.dotSize
-		self.blobSize = userSettings.blobSize
-		self.saveFigures = userSettings.saveFigures
-		self.startImage = userSettings.startImage
-		self.skipsAllowed = userSettings.skipsAllowed
-		self.removeEdgeFrames = userSettings.removeEdgeFrames
-		
+		self.userSettings = userSettings
 		self.thresholds = userSettings.thresholds
 		self.lowerDotThreshScale = self.thresholds[0]
 		self.upperDotThreshScale = self.thresholds[1]
 		self.lowerBlobThreshScale = self.thresholds[2]
 		
 		self.data = dp.getData(directory, filename)
 		self.sums = dp.getFullDataSquareSum(self.data)
@@ -39,21 +33,23 @@
 			print(strings.upperDotThreshScaleWarning)
 			return
 		self.upperDotThreshScale = value
 		self.updateThresholds()
 		self.dotCoords, self.blobCoords = self.getCoords()
 	
 	def getCoords(self):
-		if self.thresholds in self.memoizedCoords:
-			dotCoords, blobCoords = self.memoizedCoords[self.thresholds]
+		combination = (self.thresholds, (self.userSettings.dotSize, self.userSettings.blobSize))
+		if combination in self.memoizedCoords:
+			dotCoords, blobCoords = self.memoizedCoords[combination]
 		else:
 			dotCoords, blobCoords = dp.getCoords(self.data, self.sums, self.thresholds, 
-													self.dotSize)
-			dp.cleanDotCoords(self.data, dotCoords, blobCoords, self.blobSize, self.dotSize)
-			self.memoizedCoords[self.thresholds] = (dotCoords, blobCoords)
+				self.userSettings.dotSize)
+			dp.cleanDotCoords(self.data, dotCoords, blobCoords, self.userSettings.blobSize, 
+				self.userSettings.dotSize)
+			self.memoizedCoords[combination] = (dotCoords, blobCoords)
 		return dotCoords, blobCoords
 	
 	def increaseLowerDotThreshScale(self):
 		value = self.lowerDotThreshScale + cfg.THRESHOLD_DELTA
 		value = round(value, 1)
 		if value > self.upperDotThreshScale:
 			print(strings.upperDotThreshScaleWarning)
@@ -86,8 +82,8 @@
 		self.upperDotThreshScale = newUpperDotThreshScale
 		self.lowerBlobThreshScale = newLowerBlobThreshScale
 		
 		self.updateThresholds()
 	
 	def updateThresholds(self):
 		self.thresholds = (self.lowerDotThreshScale, self.upperDotThreshScale, 
-							self.lowerBlobThreshScale)
+			self.lowerBlobThreshScale)
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.0/dotscanner/ui/RegionSelector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 import dotscanner.dataprocessing as dp
 import dotscanner.strings as strings
 import dotscanner.ui.window as ui
 import matplotlib
+
 matplotlib.use("TkAgg")
+
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import tkinter as tk
 
 class RegionSelector:
-	def __init__(self, image, userSettings, skipButton=True):
+	def __init__(self, microscopeImage, userSettings, skipButton=True):
 		ui.setupWindow()
 		
-		self.xList = []
-		self.yList = []
-		
-		self.image = image
-		self.dotSize = userSettings.dotSize
-		self.blobSize = userSettings.blobSize
-		self.data = image.data
+		if userSettings.reanalysis:
+			if userSettings.polygon is None:
+				raise Exception(strings.invalidPolygonWarning)
+			self.xList, self.yList = userSettings.polygon
+			self.drawingBlocked = True
+		
+		else:
+			self.xList, self.yList = [], []
+			self.drawingBlocked = False
 		
+		self.image = microscopeImage
 		self.window = ui.createPlotWindow(strings.regionSelectorWindowTitle)
 		
-		self.figure, self.axes, _, self.dotScatter, self.blobScatter = ui.createPlots(self.data, 
-																					userSettings)
+		self.figure, self.axes, _, self.dotScatter, self.blobScatter = ui.createPlots(
+			self.image.data, userSettings)
 		
 		self.clickMarkerBackdrop = self.axes.scatter([None], [None], s=100, marker='x', color="k", 
-														linewidth=4)
-		self.underLine, = self.axes.plot([None], [None], linestyle="-", color="k", linewidth=5)
-		self.line, = self.axes.plot([None], [None], linestyle="-", color="C1", linewidth=1.5)
+			linewidth=4)
+		self.underLine, = self.axes.plot(
+			self.xList+[self.xList[0]] if userSettings.reanalysis else [None], 
+			self.yList+[self.yList[0]] if userSettings.reanalysis else [None], 
+			linestyle="-", color="k", linewidth=5)
+		self.line, = self.axes.plot(
+			self.xList+[self.xList[0]] if userSettings.reanalysis else [None], 
+			self.yList+[self.yList[0]] if userSettings.reanalysis else [None], 
+			linestyle="-", color="C1", linewidth=1.5)
 		self.dottedLine, = self.axes.plot([None], [None], linestyle=":", color="C1", linewidth=1.5)
 		self.clickMarker = self.axes.scatter([None], [None], s=100, marker='x', color="C1", 
-												linewidth=1.5)
+			linewidth=1.5)
 		
 		self.connectId = self.line.figure.canvas.mpl_connect("button_press_event", self)
 		
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		
 		self.canvas = FigureCanvasTkAgg(self.figure, master=self.window)
 		self.canvas.draw()
 		
 		self.buttonBar = tk.Frame(self.window)
 		self.buttonBar.pack(side=tk.LEFT, expand=False)
 		self.canvas.get_tk_widget().pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
@@ -51,30 +62,30 @@
 		
 		self.spacer = tk.Label(self.window, text="    ---------    ", fg="lightgray")
 		self.spacer.pack(in_=self.buttonBar, side=tk.TOP)
 		
 		if skipButton:
 			self.window.bind("<Escape>", self.skipWithEscapeKey)
 			self.skipButton = tk.Button(self.window, text="Skip", command=self.skip, 
-										fg="darkgoldenrod")
+				fg="darkgoldenrod")
 			self.skipButton.pack(in_=self.buttonBar, side=tk.TOP)
 		
 		self.doneButton = tk.Button(self.window, text="Done", command=self.finish, fg="blue", 
-									font=tk.font.Font(weight="bold"))
+			font=tk.font.Font(weight="bold"))
 		self.doneButton.pack(in_=self.buttonBar, side=tk.TOP)
 		
 		self.window.protocol("WM_DELETE_WINDOW", quit)
 		self.window.bind("<q>", self.quitWithQKey)
 		self.window.bind("<Return>", self.finishWithReturnKey)
 		self.window.bind("<BackSpace>", self.resetWithDeleteKey)
 		
 		self.window.mainloop()
 
 	def __call__(self, event):
-		if event.inaxes != self.line.axes:
+		if event.inaxes != self.line.axes or self.drawingBlocked:
 			return
 		self.drawLine(event)
 		self.drawclickMarker(event)
 	
 	def drawclickMarker(self, event):
 		self.clickMarkerBackdrop.set_offsets([event.xdata, event.ydata])
 		self.clickMarker.set_offsets([event.xdata, event.ydata])
@@ -85,15 +96,15 @@
 		self.xList.append(event.xdata)
 		self.yList.append(event.ydata)
 		self.underLine.set_data(self.xList, self.yList)
 		self.line.set_data(self.xList, self.yList)
 		if len(self.xList) > 2:
 			self.underLine.set_data([self.xList + [self.xList[0]], self.yList + [self.yList[0]]])
 			self.dottedLine.set_data([[self.xList[0], self.xList[-1]], [self.yList[0], 
-										self.yList[-1]]])
+				self.yList[-1]]])
 		self.underLine.figure.canvas.draw_idle()
 		self.line.figure.canvas.draw_idle()
 	
 	def finish(self):
 		if len(self.xList) > 2: # If a valid enclosed polygon was drawn
 			self.xList.append(self.xList[0]) # Enclose the polygon to the beginning vertex
 			self.yList.append(self.yList[0])
@@ -110,14 +121,15 @@
 	def finishWithReturnKey(self, event):
 		self.finish()
 	
 	def quitWithQKey(self, event):
 		quit()
 		
 	def reset(self):
+		self.drawingBlocked = False
 		self.xList = []
 		self.yList = []
 		self.line.set_data(self.xList, self.yList)
 		self.underLine.set_data(self.xList, self.yList)
 		self.dottedLine.set_data(self.xList, self.yList)
 		self.underLine.figure.canvas.draw_idle()
 		self.line.figure.canvas.draw_idle()
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.0/dotscanner/ui/ThresholdAdjuster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import dotscanner.dataprocessing as dp
 import dotscanner.strings as strings
 import dotscanner.ui.window as ui
 import matplotlib
+
 matplotlib.use("TkAgg")
+
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import numpy as np
 import tkinter as tk
 
 class ThresholdAdjuster:
-	def __init__(self, image, userSettings, skipButton=True):
-		ui.setupWindow()
-		
+	def __init__(self, microscopeImage, userSettings, skipButton=True, drawUi=True):
 		self.index = 0
 		self.skipButtonExists = skipButton
 		
-		
-		self.image = image
+		self.image = microscopeImage
+		self.userSettings = userSettings
 		self.dotSize = userSettings.dotSize
 		self.blobSize = userSettings.blobSize
 		self.defaultThresholds = userSettings.thresholds
-		self.userSettings = userSettings
-		self.data = image.data
 		
 		self.xBounds = [
-			(0,                     len(self.data[0]) - 1),
-			(0,                     len(self.data[0]) / 2),
-			(len(self.data[0]) / 2, len(self.data[0]) - 1),
-			(0,                     len(self.data[0]) / 2),
-			(len(self.data[0]) / 2, len(self.data[0]) - 1),
+			(0,                           len(self.image.data[0]) - 1),
+			(0,                           len(self.image.data[0]) / 2),
+			(len(self.image.data[0]) / 2, len(self.image.data[0]) - 1),
+			(0,                           len(self.image.data[0]) / 2),
+			(len(self.image.data[0]) / 2, len(self.image.data[0]) - 1),
 		]
 
 		self.yBounds = [
-			(0,                     len(self.data) - 1),
-			(len(self.data) / 2,    len(self.data) - 1),
-			(len(self.data) / 2,    len(self.data) - 1),
-			(0,                     len(self.data) / 2),
-			(0,                     len(self.data) / 2),
+			(0,                           len(self.image.data) - 1),
+			(len(self.image.data) / 2,    len(self.image.data) - 1),
+			(len(self.image.data) / 2,    len(self.image.data) - 1),
+			(0,                           len(self.image.data) / 2),
+			(0,                           len(self.image.data) / 2),
 		]
 		
+		ui.setupWindow()
 		self.window = ui.createPlotWindow(strings.thresholdAdjusterWindowTitle)
 		self.windowScaling = ui.getWindowScaling()
-		
+	
 		self.figure, self.axes, self.dataPlot, self.dotScatter, self.blobScatter = ui.createPlots(
-																					self.data, 
-																					userSettings)
+			self.image.data, userSettings)
 
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		
 		self.displayCorrectMarkerSize(self.index)
-		
+	
 		self.canvas = FigureCanvasTkAgg(self.figure, master=self.window)
 		self.canvas.draw()
 		
+		if not drawUi: # For unit testing
+			return
+		
 		self.buttonBar = tk.Frame(self.window)
 		
 		self.viewItem = tk.Frame(self.window)
 		self.viewButtons = tk.Frame(self.window)
 		self.leftViewButtons = tk.Frame(self.window)
 		self.rightViewButtons = tk.Frame(self.window)
 		self.fourViewButtons = tk.Frame(self.window)
@@ -71,18 +72,18 @@
 		self.blobsButtons = tk.Frame(self.window)
 		
 		self.thresholdEditItem = tk.Frame(self.window)
 		
 		self.viewLabel = tk.Label(self.window, text="View:")
 		self.viewTopLeftButton = tk.Button(self.window, text="⌜", command=self.showTopLeftRegion)
 		self.viewBottomLeftButton = tk.Button(self.window, text="⌞", 
-												command=self.showBottomLeftRegion)
+			command=self.showBottomLeftRegion)
 		self.viewTopRightButton = tk.Button(self.window, text="⌝", command=self.showTopRightRegion)
 		self.viewBottomRightButton = tk.Button(self.window, text="⌟", 
-												command=self.showBottomRightRegion)
+			command=self.showBottomRightRegion)
 		self.viewFullButton = tk.Button(self.window, text="Full", command=self.showWholeImage)
 		
 		self.contrastLabel = tk.Label(self.window, text="Contrast:")
 		self.contrastUpButton = tk.Button(self.window, text="ʌ", command=self.upperContrastDown)
 		self.contrastDownButton = tk.Button(self.window, text="v", command=self.upperContrastUp)
 		
 		self.dotsLabel = tk.Label(self.window, text="Dots:")
@@ -94,33 +95,33 @@
 		self.blobsDownButton = tk.Button(self.window, text="v", command=self.upperDotThresholdScaleUp)
 		
 		self.thresholdsLabel = tk.Label(self.window, text="Thresholds:")
 		
 		self.editButton = tk.Button(self.window, text="Edit", command=self.edit)
 		
 		self.resetButton = tk.Button(self.window, text="Reset", 
-										command=self.resetThreshScalesToDefaultValues)
+			command=self.resetThreshScalesToDefaultValues)
 		
 		self.doneButton = tk.Button(self.window, text="Done", command=self.finish, fg="blue", 
-									font=tk.font.Font(weight="bold"))
+			font=tk.font.Font(weight="bold"))
 		
 		self.buttonBar.pack(side=tk.LEFT, expand=False)
 		self.canvas.get_tk_widget().pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
 		
 		self.viewItem.pack(in_=self.buttonBar, side=tk.TOP, pady=(0, 5))
 		self.contrastItem.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.dotsItem.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.blobsItem.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.thresholdEditItem.pack(in_=self.buttonBar, side=tk.TOP, pady=(5, 0))
 		self.spacer = tk.Label(self.window, text="---------", fg="lightgray")
 		self.spacer.pack(in_=self.buttonBar, side=tk.TOP)
 		if self.skipButtonExists:
 			self.window.bind("<Escape>", self.skipWithEscapeKey)
 			self.skipButton = tk.Button(self.window, text="Skip", command=self.skip, 
-										fg="darkgoldenrod")
+				fg="darkgoldenrod")
 			self.skipButton.pack(in_=self.buttonBar, side=tk.TOP)
 		self.doneButton.pack(in_=self.buttonBar, side=tk.TOP)
 		
 		self.viewTopLeftButton.pack(in_=self.leftViewButtons, side=tk.TOP)
 		self.viewBottomLeftButton.pack(in_=self.leftViewButtons, side=tk.TOP)
 		self.viewTopRightButton.pack(in_=self.rightViewButtons, side=tk.TOP)
 		self.viewBottomRightButton.pack(in_=self.rightViewButtons, side=tk.TOP)
@@ -164,16 +165,24 @@
 		self.entryThreshold2 = tk.Entry(self.window, width=5)
 		self.entryThreshold2.insert(0, userSettings.upperDotThresh)
 		
 		self.entryThresholdLabel3 = tk.Label(self.window, text="Blob lower:")
 		self.entryThreshold3 = tk.Entry(self.window, width=5)
 		self.entryThreshold3.insert(0, userSettings.lowerBlobThresh)
 		
+		self.entryDotSizeLabel = tk.Label(self.window, text="Dot size:")
+		self.entryDotSize = tk.Entry(self.window, width=5)
+		self.entryDotSize.insert(0, userSettings.dotSize)
+		
+		self.entryBlobSizeLabel = tk.Label(self.window, text="Blob size:")
+		self.entryBlobSize = tk.Entry(self.window, width=5)
+		self.entryBlobSize.insert(0, userSettings.blobSize)
+		
 		self.editDoneButton = tk.Button(self.window, text="Done", command=self.editFinish, 
-										fg="blue", font=tk.font.Font(weight="bold"))
+			fg="blue", font=tk.font.Font(weight="bold"))
 		
 		self.window.protocol("WM_DELETE_WINDOW", quit)
 		self.window.bind("<q>", self.quitWithQKey)
 		self.window.bind("<Return>", self.finishWithReturnKey)
 		self.window.bind("<space>", self.cycleViews)
 		self.window.bind("<Up>", self.lowerDotThresholdScaleDownWithUpKey)
 		self.window.bind("<Down>", self.lowerDotThresholdScaleUpWithDownKey)
@@ -212,14 +221,19 @@
 		self.editSpacer.pack(in_=self.buttonBar, side=tk.TOP)
 		self.entryThresholdLabel1.pack(in_=self.buttonBar, side=tk.TOP, pady=(0, 5))
 		self.entryThreshold1.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.entryThresholdLabel2.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.entryThreshold2.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.entryThresholdLabel3.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.entryThreshold3.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
+		
+		self.entryDotSizeLabel.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
+		self.entryDotSize.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
+		self.entryBlobSizeLabel.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
+		self.entryBlobSize.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.editDoneButton.pack(in_=self.buttonBar, side=tk.TOP, pady=(5, 0))
 		
 		self.window.update()
 	
 	def editFinish(self):
 		self.window.unbind("<Return>")
 		self.window.bind("<Up>", self.lowerDotThresholdScaleDownWithUpKey)
@@ -231,14 +245,19 @@
 		self.editSpacer.pack_forget()
 		self.entryThresholdLabel1.pack_forget()
 		self.entryThreshold1.pack_forget()
 		self.entryThresholdLabel2.pack_forget()
 		self.entryThreshold2.pack_forget()
 		self.entryThresholdLabel3.pack_forget()
 		self.entryThreshold3.pack_forget()
+		
+		self.entryDotSizeLabel.pack_forget()
+		self.entryDotSize.pack_forget()
+		self.entryBlobSizeLabel.pack_forget()
+		self.entryBlobSize.pack_forget()
 		self.editDoneButton.pack_forget()
 		
 		self.dotsItem.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.blobsItem.pack(in_=self.buttonBar, side=tk.TOP, pady=5)
 		self.thresholdEditItem.pack(in_=self.buttonBar, side=tk.TOP, pady=(5, 0))
 		self.spacer.pack(in_=self.buttonBar, side=tk.TOP)
 		if self.skipButtonExists:
@@ -252,20 +271,33 @@
 			newThresholds = (numberIn1, numberIn2, numberIn3)
 		
 		except:
 			self.setThresholdEntries(self.image.thresholds)
 			print(strings.invalidThresholdEdit)
 			return
 		
+		try:
+			self.dotSize = int(round(float(self.entryDotSize.get()), 0))
+			self.blobSize = int(round(float(self.entryBlobSize.get()), 0))
+			self.image.dotSize = self.dotSize
+			self.image.blobSize = self.blobSize
+			self.userSettings.dotSize = self.dotSize
+			self.userSettings.blobSize = self.blobSize
+		
+		except:
+			self.setDotAndBlobSizeEntries(self.dotSize, self.blobSize)
+			print(strings.invalidDotAndBlobSizeEdit)
+			return
+		
 		self.image.setThresholds(newThresholds)
 		self.setThresholdEntries(self.image.thresholds)
 		
 		self.image.dotCoords, self.image.blobCoords = self.image.getCoords()
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def editFinishWithReturnKey(self, event):
 		self.editFinish()
 	
 	def finish(self):
 		self.window.destroy()
@@ -274,39 +306,45 @@
 	def finishWithReturnKey(self, event):
 		self.finish()
 	
 	def lowerDotThresholdScaleDown(self):
 		self.image.decreaseLowerDotThreshScale()
 		self.setThresholdEntries(self.image.thresholds)
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def lowerDotThresholdScaleDownWithUpKey(self, event):
 		self.lowerDotThresholdScaleDown()
 
 	def lowerDotThresholdScaleUp(self):
 		self.image.increaseLowerDotThreshScale()
 		self.setThresholdEntries(self.image.thresholds)
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def lowerDotThresholdScaleUpWithDownKey(self, event):
 		self.lowerDotThresholdScaleUp()
 	
 	def setThresholdEntries(self, thresholds):
 		thresh1, thresh2, thresh3 = thresholds
 		self.entryThreshold1.delete(0, tk.END)
 		self.entryThreshold2.delete(0, tk.END)
 		self.entryThreshold3.delete(0, tk.END)
 		self.entryThreshold1.insert(0, thresh1)
 		self.entryThreshold2.insert(0, thresh2)
 		self.entryThreshold3.insert(0, thresh3)
 	
+	def setDotAndBlobSizeEntries(self, dotSize, blobSize):
+		self.entryDotSize.delete(0, tk.END)
+		self.entryBlobSize.delete(0, tk.END)
+		self.entryDotSize.insert(0, dotSize)
+		self.entryBlobSize.insert(0, blobSize)
+	
 	def showCorrectImage(self, index):
 		self.displayCorrectMarkerSize(index)
 		self.axes.set_xbound(self.xBounds[index])
 		self.axes.set_ybound(self.yBounds[index])
 		self.canvas.draw()
 
 	def showWholeImage(self):
@@ -341,41 +379,41 @@
 
 	def resetThreshScalesToDefaultValues(self):
 		self.image.setThresholds(self.defaultThresholds)
 		self.setThresholdEntries(self.defaultThresholds)
 		
 		self.image.dotCoords, self.image.blobCoords = self.image.getCoords()
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def upperContrastDown(self):
 		self.userSettings.decreaseUpperContrast()
 		self.dataPlot.set_clim(self.userSettings.lowerContrast, 
-								self.userSettings.upperContrast * np.std(self.data))
+			self.userSettings.upperContrast * np.std(self.image.data))
 		self.canvas.draw()
 	
 	def upperContrastUp(self):
 		self.userSettings.increaseUpperContrast()
 		self.dataPlot.set_clim(self.userSettings.lowerContrast, 
-								self.userSettings.upperContrast * np.std(self.data))
+			self.userSettings.upperContrast * np.std(self.image.data))
 		self.canvas.draw()
 	
 	def upperDotThresholdScaleDown(self):
 		self.image.decreaseUpperDotThreshScale()
 		self.setThresholdEntries(self.image.thresholds)
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def upperDotThresholdScaleDownWithRightKey(self, event):
 		self.upperDotThresholdScaleDown()
 
 	def upperDotThresholdScaleUp(self):
 		self.image.increaseUpperDotThreshScale()
 		self.setThresholdEntries(self.image.thresholds)
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
-							self.blobScatter)
+			self.blobScatter)
 		self.canvas.draw()
 	
 	def upperDotThresholdScaleUpWithLeftKey(self, event):
 		self.upperDotThresholdScaleUp()
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.0/dotscanner/ui/UserSettings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import dotscanner.files as files
 import dotscanner.strings as strings
+from dotscanner.strings import ProgramType
 import dotscanner.ui.window as ui
 from dotscanner.ui.DefaultUserSettingsEditor import DefaultUserSettingsEditor
 import settings.config as cfg
 import os
 import tkinter as tk
 from tkinter import filedialog
 
 class UserSettings:
 	def __init__(self):
 		self.window = ui.createConfigurationsWindow()
 
 		self.filepath = cfg.FILEPATH		
 		self.startImage = ""
-		self.program = cfg.PROGRAM
+		self.program = self.getProgramType(cfg.PROGRAM)
 		self.blobSize = round(cfg.BLOB_SIZE, 0)
 		self.dotSize = round(cfg.DOT_SIZE, 0)
 		self.lowerDotThresh = round(cfg.LOWER_DOT_THRESH_SCALE, 1)
 		self.upperDotThresh = round(cfg.UPPER_DOT_THRESH_SCALE, 1)
 		self.lowerBlobThresh = round(cfg.LOWER_BLOB_THRESH_SCALE, 1)
+		self.thresholds = (self.lowerDotThresh, self.upperDotThresh, self.lowerBlobThresh)
 		self.lowerContrast = round(cfg.LOWER_CONTRAST, 1)
 		self.upperContrast = round(cfg.UPPER_CONTRAST, 1)
 		self.saveFigures = cfg.SAVE_FIGURES
 		self.removeEdgeFrames = cfg.REMOVE_EDGE_FRAMES
 		self.skipsAllowed = round(cfg.SKIPS_ALLOWED, 0)
+		self.reanalysis = False
+		self.polygon = None
+		self.densityData = {}
 		
 		self.filepathFrame = tk.Frame(self.window)
 		
 		self.labelFilepath = tk.Label(self.window, text="Filepath:")
 		self.labelSelectedPath = tk.Label(self.window, text="Select a file or folder for analysis", 
-											fg="red", bg="white")
+			fg="red", bg="white")
 		self.showFilepath()
 		
 		self.labelFilepath.pack(in_=self.filepathFrame, side=tk.LEFT)
 		self.labelSelectedPath.pack(in_=self.filepathFrame, side=tk.LEFT)
 		
 		self.navigation = tk.Frame(self.window)
 		
@@ -42,22 +47,22 @@
 		self.buttonSelectFile = tk.Button(self.window, text="File", command=self.browseFiles)
 
 		self.buttonSelectFolder = tk.Button(self.window, text="Folder", command=self.browseFolders)
 		
 		self.labelProgram = tk.Label(self.window, text="Program:")
 
 		self.menuProgramSelectVar = tk.StringVar(self.window)
-		self.menuProgramSelectVar.set(self.program.capitalize()) # default value
-		self.menuProgramSelect = tk.OptionMenu(self.window, self.menuProgramSelectVar, "Density", 
-												"Lifetime", command=self.toggleExtraOptions)
+		self.menuProgramSelectVar.set(self.program) # default value
+		self.menuProgramSelect = tk.OptionMenu(self.window, self.menuProgramSelectVar, 
+			ProgramType.DENSITY, ProgramType.LIFETIME, command=self.toggleExtraOptions)
 		
 		self.checkboxSaveFigsVar = tk.BooleanVar()
-		self.checkboxSaveFigs = tk.Checkbutton(self.window, text='Save figures', 
-												variable=self.checkboxSaveFigsVar, onvalue=True, 
-												offvalue=False, command=self.setSaveFigs)
+		self.checkboxSaveFigs = tk.Checkbutton(self.window, text="Save figures", 
+			variable=self.checkboxSaveFigsVar, onvalue=True, offvalue=False, 
+			command=self.setSaveFigs)
 		self.checkboxSaveFigsVar.set(self.saveFigures)
 		
 		self.labelBrowse.pack(in_=self.navigation, side=tk.LEFT)
 		self.buttonSelectFile.pack(in_=self.navigation, side=tk.LEFT)
 		self.buttonSelectFolder.pack(in_=self.navigation, side=tk.LEFT)
 		self.labelProgram.pack(in_=self.navigation, side=tk.LEFT)
 		self.menuProgramSelect.pack(in_=self.navigation, side=tk.LEFT)
@@ -93,41 +98,43 @@
 		self.entryThreshold2.pack(in_=self.entries, side=tk.LEFT)
 		self.entryThreshold3.pack(in_=self.entries, side=tk.LEFT)
 		
 		self.lifetimeOptions = tk.Frame(self.window)
 
 		self.labelStartImage = tk.Label(self.window, text="Start image:")
 		self.buttonSelectStartingImage = tk.Button(self.window, text="Browse...", 
-													command=self.browseStartingImage)
+			command=self.browseStartingImage)
 
 		self.labelSkipsAllowed = tk.Label(self.window, text="Skips allowed:")
 		self.entrySkipsAllowed = tk.Entry(self.window, width=5)
 		self.entrySkipsAllowed.insert(0, self.skipsAllowed)
 
 		self.checkboxRemoveEdgeVar = tk.BooleanVar()
 		self.checkboxRemoveEdge = tk.Checkbutton(self.window, text='Remove edge frames', 
-													variable=self.checkboxRemoveEdgeVar, 
-													onvalue=True, offvalue=False, 
-													command=self.setRemoveEdge)
+			variable=self.checkboxRemoveEdgeVar, onvalue=True, offvalue=False, 
+			command=self.setRemoveEdge)
 		self.checkboxRemoveEdgeVar.set(self.removeEdgeFrames)
 		
 		self.labelStartImage.pack(in_=self.lifetimeOptions, side=tk.LEFT)
 		self.buttonSelectStartingImage.pack(in_=self.lifetimeOptions, side=tk.LEFT)
 		self.labelSkipsAllowed.pack(in_=self.lifetimeOptions, side=tk.LEFT)
 		self.entrySkipsAllowed.pack(in_=self.lifetimeOptions, side=tk.LEFT)
 		self.checkboxRemoveEdge.pack(in_=self.lifetimeOptions, side=tk.LEFT)
 		
 		self.bottomButtons = tk.Frame(self.window)
 		
 		self.buttonEditDefaults = tk.Button(self.window, text="Edit defaults...", 
-											command=self.editDefaults)
+			command=self.editDefaults)
+		self.buttonUsePreviousAnalysis = tk.Button(self.window, text="Use previous analysis...", 
+			command=self.usePreviousAnalysis)
 		self.buttonNext = tk.Button(self.window, text="Next", command=self.done, fg="blue", 
-									font=tk.font.Font(weight="bold"))
+			font=tk.font.Font(weight="bold"))
 		
 		self.buttonEditDefaults.pack(in_=self.bottomButtons, side=tk.LEFT)
+		self.buttonUsePreviousAnalysis.pack(in_=self.bottomButtons, side=tk.LEFT)
 		self.buttonNext.pack(in_=self.bottomButtons, side=tk.LEFT)
 		
 		self.labelWarning = tk.Label(self.window, text="", fg="red")
 				
 		self.filepathFrame.pack()
 		self.navigation.pack()
 		self.entries.pack()
@@ -141,33 +148,33 @@
 		self.window.bind("<q>", self.quitWithQKey)
 		self.window.bind("<Return>", self.doneWithReturnKey)
 		
 		self.window.mainloop()
 
 	def browseFiles(self):
 		chosenFile = filedialog.askopenfilename(initialdir=self.filepath, 
-												title="Select a file to analyze")
+			title="Select a file to analyze")
 		if chosenFile not in ["", " ", "/"]:
 			self.filepath = chosenFile
 			self.showFilepath()
 		self.window.focus_force()
 		self.checkForWarning()
 
 	def browseFolders(self):
 		chosenFolder = filedialog.askdirectory(initialdir=self.filepath, 
-												title="Select a folder with images to analyze")
+			title="Select a folder with images to analyze")
 		if chosenFolder not in ["", " ", "/"]:
 			self.filepath = chosenFolder
 			self.showFilepath()
 		self.window.focus_force()
 		self.checkForWarning()
 
 	def browseStartingImage(self):
 		chosenFilepath = filedialog.askopenfilename(initialdir=self.filepath, 
-									title="Select the starting image for the lifetime measurement")
+			title="Select the starting image for the lifetime measurement")
 		chosenImage = os.path.basename(chosenFilepath)
 		if chosenImage != "":
 			if os.path.isfile(self.filepath):
 				self.buttonSelectStartingImage.config(text="Browse...", fg="black")
 				self.startImage = ""
 				self.labelWarning.configure(text = strings.lifetimeSingleFileWarning)
 			elif os.path.dirname(chosenFilepath) != self.filepath:
@@ -187,14 +194,20 @@
 					self.buttonSelectStartingImage.config(text="Browse...", fg="black")
 					self.startImage = ""
 					self.labelWarning.configure(text = strings.fileNumberingWarning)
 		
 		self.window.update()
 		self.window.focus_force()
 	
+	def checkForWarning(self):
+		if os.path.isfile(self.filepath) and self.program == ProgramType.LIFETIME:
+			self.labelWarning.configure(text = strings.lifetimeSingleFileWarning)
+		else:
+			self.labelWarning.configure(text = "")
+	
 	def decreaseUpperContrast(self):
 		value = self.upperContrast - cfg.CONTRAST_DELTA
 		value = round(value, 1)
 		if value <= self.lowerContrast:
 			print(strings.maxContrastWarning)
 			return
 		self.upperContrast = value
@@ -217,14 +230,22 @@
 	
 	def doneWithReturnKey(self, event):        
 		self.done()
 	
 	def editDefaults(self):
 		DefaultUserSettingsEditor(self)
 	
+	def getProgramType(self, programString):
+		if programString.lower() == "density":
+			return ProgramType.DENSITY
+		elif programString.lower() == "lifetime":
+			return ProgramType.LIFETIME
+		else:
+			raise Exception(strings.programNameException)
+	
 	def increaseUpperContrast(self):
 		value = self.upperContrast + cfg.CONTRAST_DELTA
 		value = round(value, 1)
 		self.upperContrast = value
 	
 	def quitWithQKey(self, event):
 		quit()
@@ -242,36 +263,133 @@
 		else:
 			self.saveFigures = False
 		self.checkForWarning()
 	
 	def showFilepath(self):
 		if self.filepath in ["", " ", "/"]:
 			self.labelSelectedPath.configure(text="Select a file or folder for analysis", fg="red", 
-												bg="white")
+				bg="white")
 		else:
 			displayedFilepath = self.filepath
 			if len(displayedFilepath) > 50:
 				displayedFilepath = "..." + displayedFilepath[-50:]
 			self.labelSelectedPath.configure(text=displayedFilepath, bg="white", fg="black")
 
 	def toggleExtraOptions(self, click):
-		if click == "Lifetime":
-			self.program = "lifetime"
+		if click == ProgramType.LIFETIME:
+			self.program = ProgramType.LIFETIME
 			self.bottomButtons.pack_forget()
 			self.labelWarning.pack_forget()
 			self.lifetimeOptions.pack()
 			self.bottomButtons.pack()
 			self.labelWarning.pack()
 		else:
-			self.program = "density"
+			self.program = ProgramType.DENSITY
 			self.lifetimeOptions.pack_forget()
 			self.bottomButtons.pack_forget()
 			self.labelWarning.pack_forget()
 			self.bottomButtons.pack()
 			self.labelWarning.pack()
 		self.checkForWarning()
-
-	def checkForWarning(self):
-		if os.path.isfile(self.filepath) and self.program == "lifetime":
-			self.labelWarning.configure(text = strings.lifetimeSingleFileWarning)
-		else:
-			self.labelWarning.configure(text = "")
+	
+	def usePreviousAnalysis(self):
+		chosenFile = filedialog.askopenfilename(initialdir=self.filepath, 
+			title="Select a .txt file generated by a previous analysis")
+		if chosenFile not in ["", " ", "/"]:
+			self.reanalysis = True
+			self.parseAnalysisFile(chosenFile)
+	
+	def parseAnalysisFile(self, chosenFile):
+		with open(chosenFile, "r") as file:
+			for line in file:
+				if not line.startswith("#"):
+					break
+				
+				lineArray = line.split()
+				if len(lineArray) < 2:
+					continue
+				
+				if lineArray[1] == "Generated":
+					programString = lineArray[5]
+					if programString == "density":
+						self.program = ProgramType.DENSITY
+						self.parseDensityFile(chosenFile)
+					else:
+						self.program = ProgramType.LIFETIME
+						self.parseLifetimeFile(chosenFile)
+	
+	def parseDensityFile(self, chosenFile):
+		self.filepath = os.path.dirname(chosenFile)
+		with open(chosenFile, "r") as file:
+			for line in file:
+				if line.startswith("#"):
+					continue
+				
+				splitLine = line.split()
+				if splitLine[1] == "skipped":
+					continue
+				
+				filename = splitLine[0]
+				lowerDotThreshScale = round(float(splitLine[5]), 1)
+				upperDotThreshScale = round(float(splitLine[6]), 1)
+				lowerBlobThreshScale = round(float(splitLine[7]), 1)
+				blobSize = int(splitLine[8])
+				dotSize = int(splitLine[9])
+				lowerContrast = round(float(splitLine[10]), 1)
+				upperContrast = round(float(splitLine[11]), 1)
+				polygonString = line.split("(")[1:]
+				polygonPairsStringArray = [item.split(")")[0] for item in polygonString]
+				polygon = []
+				for pair in polygonPairsStringArray:
+					x, y = pair.split(",")
+					polygon.append([int(y), int(x)]) # More convenient shape for densities
+				polygon.append([polygon[0][0], polygon[0][1]])
+				
+				self.densityData[filename] = [lowerDotThreshScale, upperDotThreshScale, 
+				lowerBlobThreshScale, blobSize, dotSize, lowerContrast, upperContrast, polygon]
+						
+		self.window.destroy()
+		self.window.quit()
+	
+	def parseLifetimeFile(self, chosenFile):
+		self.filepath = os.path.dirname(chosenFile)
+		self.polygon = [[], []]
+		with open(chosenFile, "r") as file:
+			for line in file:
+				if not line.startswith("#"): # Only read the header
+					break
+				
+				lineArray = line.split()
+				if len(lineArray) < 3:
+					continue
+				
+				if lineArray[1] == "Polygon":
+					polygonData = line.split(":")[1].split(")")
+					for item in polygonData:
+						polygonDataArray = item.split("(")
+						if len(polygonDataArray) > 1:
+							x, y = polygonDataArray[1].split(",")
+							self.polygon[0].append(int(x)) # More convenient shape for lifetimes
+							self.polygon[1].append(int(y))
+				
+				elif lineArray[1] == "Threshold":
+					parsedThresholds = [float(value) for value in line.split(":")[1].split(",")]
+					self.lowerDotThresh = round(parsedThresholds[0], 1)
+					self.upperDotThresh = round(parsedThresholds[1], 1)
+					self.lowerBlobThresh = round(parsedThresholds[2], 1)
+					self.thresholds = (self.lowerDotThresh, self.upperDotThresh, self.lowerBlobThresh)
+				
+				elif lineArray[1] == "Contrast":
+					parsedContrasts = [float(value) for value in line.split(":")[1].split(",")]
+					self.lowerContrast = round(parsedContrasts[0], 1)
+					self.upperContrast = round(parsedContrasts[1], 1)
+				
+				elif lineArray[1] == "Dot" and lineArray[2] == "size:":
+					valueArray = [item.split(":")[1] for item in line.split("|")]
+					self.dotSize = int(valueArray[0])
+					self.blobSize = int(valueArray[1])
+					self.removeEdgeFrames = bool(valueArray[2])
+					self.saveFigures = bool(valueArray[3])
+					self.skipsAllowed = int(valueArray[4])
+				
+		self.window.destroy()
+		self.window.quit()
```

### Comparing `dotscanner-1.2.9/dotscanner/ui/window.py` & `dotscanner-1.3.0/dotscanner/ui/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import dotscanner.strings as strings
 import settings.config as cfg
 import matplotlib
+
 matplotlib.use("TkAgg")
+
 import matplotlib.pyplot as pl
 import numpy as np
 import os
 import tkinter as tk
 
 def createPlots(data, userSettings):
 	windowScaling = getWindowScaling()
 	figure, axes = pl.subplots()
 	dataPlot = axes.imshow(data, origin="lower", cmap="gray", vmin=userSettings.lowerContrast, 
-							vmax=userSettings.upperContrast * np.std(data))
+		vmax=userSettings.upperContrast * np.std(data))
 	dotScatter = axes.scatter([None], [None], s=5 * userSettings.dotSize * windowScaling, 
-								facecolors="none", edgecolors=cfg.DOT_COLOR, 
-								linewidths=cfg.DOT_THICKNESS)
+		facecolors="none", edgecolors=cfg.DOT_COLOR, linewidths=cfg.DOT_THICKNESS)
 	blobScatter = axes.scatter([None], [None], s=2 * userSettings.blobSize * windowScaling, 
-								facecolors="none", edgecolor=cfg.BLOB_COLOR, 
-								linewidths=cfg.BLOB_THICKNESS)
+		facecolors="none", edgecolor=cfg.BLOB_COLOR, linewidths=cfg.BLOB_THICKNESS)
 	return figure, axes, dataPlot, dotScatter, blobScatter
 
 def createConfigurationsWindow():
 	window = tk.Tk()
 	window.title(strings.configurationsWindowTitle)
 	width, _ = getWindowDimensions()
 	if width > 650:
@@ -65,16 +65,16 @@
 	
 	return width, height
 
 def getWindowScaling():
 	_, height = getWindowDimensions()
 	return height / 550
 
-def printProgressBar (iteration, total, prefix = "", suffix = "", decimals = 1, 
-						barLength = 50, fill = "█", printEnd = "\r"):
+def printProgressBar (iteration, total, prefix = "", suffix = "", decimals = 1, barLength = 50, 
+	fill = "█", printEnd = "\r"):
 	percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
 	filledLength = int(barLength * iteration // total)
 	bar = fill * filledLength + "-" * (barLength - filledLength)
 	print(f"\r{prefix} |{bar}| {percent}% {suffix}", end = printEnd)
 	
 	if iteration == total: 
 		print()
```

### Comparing `dotscanner-1.2.9/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.0/dotscanner.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,193 +1,199 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.2.9
+Version: 1.3.0
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
-Description: # Dot Scanner
-        > Software designed for analysis of microscope imaging data
-        
-        [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
-        
-        Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
-        
-        ## Getting Started
-        
-        ### Dependencies
-        
-        [Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
-        
-        ### Installation
-        
-        To install Dot Scanner, open a terminal window and run the following command:
-        
-        ```
-        pip install dotscanner
-        ```
-        
-        *(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
-        
-        ### Running the Software
-        
-        To launch the main graphical user interface (GUI), run the following command:
-        
-        ```
-        dotscanner
-        ```
-        
-        Some demo images are included in the `images/demo/` folder, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
-        
-        ## The Configurations Window
-        The first window displayed in the GUI is the Configurations Window:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
-        
-        If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the `images/demo/` folder can be downloaded to try this out for oneself):
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
-        
-        If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
-        
-        The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
-        
-        If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
-        
-        If **Lifetime** is selected, some additional options will appear:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
-        
-        ### Descriptions of Configuration Options
-        
-        #### Save figures
-        Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
-        
-        #### Blob size
-        This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
-        
-        #### Dot size
-        Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
-        
-        #### Thresholds
-        There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
-        1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
-        2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
-        3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
-        
-        ### Descriptions of Configuration Options for the Lifetime Program
-        
-        #### Start image
-        This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
-        
-        #### Skips allowed
-        This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
-              
-        #### Remove edge frames
-        This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
-        
-        #### Edit defaults
-        This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
-        
-        Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
-        
-        ## The Threshold Adjustment Window
-        This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
-        
-        From top to bottom, these button groups perform the following actions:
-        
-        #### View
-        These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
-        
-        #### Contrast
-        These buttons adjust the contrast of the image.
-        
-        #### Dots
-        These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
-        
-        #### Blobs
-        These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
-        
-        #### Edit
-        This button changes the left button bar view to display some manual threshold adjustment options:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
-        
-        *(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
-        
-        #### Reset
-        This button resets the adjusted thresholds back to the default values.
-        
-        #### Skip
-        This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
-        
-        ## The Region Selector Window
-        Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
-        ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
-        
-        This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
-        
-        Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
-        
-        ## Authors
-        
-        Holly Allen (holly.allen@colorado.edu)
-        
-        Brian Davis
-        
-        ## Release History
-        
-        * 1.2.9
-             * Bug fixes
-        * 1.2.0
-             * Added options for editing the configuration file
-             * Added startup processes to check the configuration file for errors
-        * 1.1.0
-             * Migrated the remaining portions of the app from a terminal interface to a GUI
-        * 1.0.0
-             * Initial Release
-        
-        ## License
-        
-        This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
-        
-        ## Development
-        
-        To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
-        
-        ```
-        python -m dotscanner
-        ```
-        
-        *(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
-        
-        ### Testing
-        
-        Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
-        
-        ```
-        python -m unittest
-        ```
-        
-        *(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
-        
-        ### Bug Reports and Feature Requests
-        
-        To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
-        
-        ## Citations
-        
-        When using this program on data used in published works, please cite:
-        
-        Allen, H., Davis, B., Patel, J., & Gu, Y. 2022 (in prep.)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dot Scanner
+> Software designed for analysis of microscope imaging data
+
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
+
+Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
+
+## Getting Started
+
+### Dependencies
+
+[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
+
+### Installation
+
+To install Dot Scanner, open a terminal window and run the following command:
+
+```
+pip install dotscanner
+```
+
+*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+
+### Running the Software
+
+To launch the main graphical user interface (GUI), run the following command:
+
+```
+dotscanner
+```
+
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+
+## The Configurations Window
+The first window displayed in the GUI is the Configurations Window:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
+
+If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
+![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
+
+If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
+
+The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
+
+If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
+
+If **Lifetime** is selected, some additional options will appear:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
+
+### Descriptions of Configuration Options
+
+#### Save figures
+Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
+
+#### Blob size
+This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
+
+#### Dot size
+Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
+
+#### Thresholds
+There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
+1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
+2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
+3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
+
+#### Edit defaults
+This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
+
+#### Use previous analysis
+This opens a new window that allows the user to browse for a previous analysis file to use to repeat analysis.
+
+Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
+
+### Descriptions of Configuration Options for the Lifetime Program
+
+#### Start image
+This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
+
+#### Skips allowed
+This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
+      
+#### Remove edge frames
+This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
+
+## The Threshold Adjustment Window
+This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
+
+From top to bottom, these button groups perform the following actions:
+
+#### View
+These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
+
+#### Contrast
+These buttons adjust the contrast of the image.
+
+#### Dots
+These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
+
+#### Blobs
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
+
+#### Edit
+This button changes the left button bar view to display some manual threshold and size adjustment options:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
+
+*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+
+#### Reset
+This button resets the adjusted thresholds back to the default values.
+
+#### Skip
+This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
+
+## The Region Selector Window
+Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
+![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
+
+This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
+
+Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
+
+*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+
+## Authors
+
+Holly Allen (holly.allen@colorado.edu)
+
+Brian Davis
+
+## Release History
+
+* 1.3.0
+     * Added option to re-analyze data without redrawing regions
+     * Added particle displacement tracking during lifetime measurement
+     * Added histogram output for lifetimes measurements
+* 1.2.0
+     * Added options for editing the configuration file
+     * Added startup processes to check the configuration file for errors
+* 1.1.0
+     * Migrated the remaining portions of the app from a terminal interface to a GUI
+* 1.0.0
+     * Initial Release
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
+
+## Development
+
+To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
+
+```
+python -m dotscanner
+```
+
+*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+
+### Testing
+
+Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
+
+```
+python -m unittest
+```
+
+*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+
+### Bug Reports and Feature Requests
+
+To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
+
+## Citations
+
+When using this program on data used in published works, please cite:
+
+Allen, H., Davis, B., Patel, J., & Gu, Y. 2023 (in prep.)
```

### Comparing `dotscanner-1.2.9/settings/config.py` & `dotscanner-1.3.0/settings/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 FILEPATH = ""
 # Path to the file or directory of files that should be used. The default value is an empty string: ""
 
 PROGRAM = "density"
 # Whether a "density" program or "lifetime" program should be run
 
 SCALE = None
-# Scale of the image (in nanometers per pixel). If unknown, leave as None.
+# Linear scale of the image (width of a single pixel in nanometers per pixel). Default value is None. If None is entered, the final density output will be in dots per pixel^2. If a numerical value is entered, the final density output will be in dots per micron^2.
 
 ############################################
 ############ THRESHOLD SETTINGS ############
 ############################################
 
 LOWER_DOT_THRESH_SCALE = 1.5
-# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
+# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5,which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
 
 UPPER_DOT_THRESH_SCALE = 5.0
 # Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 
 LOWER_BLOB_THRESH_SCALE = 2.0
 # Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
@@ -118,8 +118,14 @@
 DENSITY_OUTPUT_FILENAME = "densities.txt"
 # The filename to be saved in the directory containing the images used for density measurement. This file will contain the measurements for each of those image files.
 
 LIFETIME_OUTPUT_FILENAME = "lifetimes.txt"
 # The filename to be saved in the directory containing the images used for lifetime measurement.
 
 FIGURE_DIRECTORY_NAME = "figures/"
-# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.
+# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.
+
+FIGURE_FILETYPES = ["pdf"]
+# The filetypes for the output figures. Multiple types can also be selected, e.g., ["png", "pdf", "tif"]. Only use the supported filetypes ("eps", "tif", "ps", "tiff", "rgba", "svg", "png", "jpg", "raw", "pdf", "svgz", "pgf", and "jpeg").
+
+FIGURE_RESOLUTION = 300
+# Resolution (DPI) of the output figures. This is for images only; PDF outputs are unaffected by this value.
```

### Comparing `dotscanner-1.2.9/settings/configmanagement.py` & `dotscanner-1.3.0/settings/configmanagement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dotscanner.ui.DialogWindow import DialogWindow
+import matplotlib.colors as colors
 import traceback
 
 def runChecks():
 	try:
 		scanConfigFileForErrors()
 	except Exception as exception:
 		print("\n", traceback.format_exc())
 		showStartupErrorDialog()
 		quit()
 
 def scanConfigFileForErrors():
 	import settings.config as cfg
-	import matplotlib.colors as colors
 	
 	matplotlibColors = set(colors.BASE_COLORS.keys())
 	for color in colors.TABLEAU_COLORS.keys():
 		matplotlibColors.add(color)
 	for color in colors.CSS4_COLORS.keys():
 		matplotlibColors.add(color)
 	
@@ -59,14 +59,21 @@
 	assert type(cfg.WINDOW_X) in [int, float]
 	assert type(cfg.WINDOW_Y) in [int, float]
 	
 	assert type(cfg.SAVE_FIGURES) == bool
 	assert type(cfg.DENSITY_OUTPUT_FILENAME) == str
 	assert type(cfg.LIFETIME_OUTPUT_FILENAME) == str
 	assert type(cfg.FIGURE_DIRECTORY_NAME) == str
+	assert type(cfg.FIGURE_FILETYPES) == list
+	assert type(cfg.FIGURE_FILETYPES[0]) == str
+	
+	supportedPlotOutputTypes = {"eps", "tif", "ps", "tiff", "rgba", "svg", "png", "jpg", "raw", 
+	"pdf", "svgz", "pgf", "jpeg"}
+	for fileExtension in cfg.FIGURE_FILETYPES:
+		assert fileExtension in supportedPlotOutputTypes
 
 def showEditConfigFileDialog():
 	DialogWindow(
 		title="Edit config file?",
 		message="\
 Are you sure you want to edit this file? \n\
 Dot scanner will close during editing. \n\
@@ -142,22 +149,22 @@
 FILEPATH = ""\n\
 # Path to the file or directory of files that should be used. The default value is an empty string: ""\n\
 \n\
 PROGRAM = "density"\n\
 # Whether a "density" program or "lifetime" program should be run\n\
 \n\
 SCALE = None\n\
-# Scale of the image (in nanometers per pixel). If unknown, leave as None.\n\
+# Linear scale of the image (width of a single pixel in nanometers per pixel). Default value is None. If None is entered, the final density output will be in dots per pixel^2. If a numerical value is entered, the final density output will be in dots per micron^2.\n\
 \n\
 ############################################\n\
 ############ THRESHOLD SETTINGS ############\n\
 ############################################\n\
 \n\
 LOWER_DOT_THRESH_SCALE = 1.5\n\
-# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.\n\
+# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5,which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.\n\
 \n\
 UPPER_DOT_THRESH_SCALE = 5.0\n\
 # Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.\n\
 \n\
 LOWER_BLOB_THRESH_SCALE = 2.0\n\
 # Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE. Lower this value to increase the number of blobs detected, or raise it to reduce the number.\n\
 \n\
@@ -257,11 +264,17 @@
 DENSITY_OUTPUT_FILENAME = "densities.txt"\n\
 # The filename to be saved in the directory containing the images used for density measurement. This file will contain the measurements for each of those image files.\n\
 \n\
 LIFETIME_OUTPUT_FILENAME = "lifetimes.txt"\n\
 # The filename to be saved in the directory containing the images used for lifetime measurement.\n\
 \n\
 FIGURE_DIRECTORY_NAME = "figures/"\n\
-# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.\
+# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.\n\
+\n\
+FIGURE_FILETYPES = ["pdf"]\n\
+# The filetypes for the output figures. Multiple types can also be selected, e.g., ["png", "pdf", "tif"]. Only use the supported filetypes ("eps", "tif", "ps", "tiff", "rgba", "svg", "png", "jpg", "raw", "pdf", "svgz", "pgf", and "jpeg").\n\
+\n\
+FIGURE_RESOLUTION = 300\n\
+# Resolution (DPI) of the output figures. This is for images only; PDF outputs are unaffected by this value.\
 ')
 	
 	quit()
```

### Comparing `dotscanner-1.2.9/setup.py` & `dotscanner-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setup(
-    name="dotscanner",
-    version="1.2.9",
-    description="A program designed for analysis of microscope imaging data",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/bdavis222/dotscanner",
-    author="Holly Allen and Brian Davis",
-    author_email="holly.allen@colorado.edu",
-    classifiers=[
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows"
-    ],
-    packages=find_packages(),
-    py_modules=["dotscanner", "dotscanner.ui", "settings", "tests"],
-    python_requires=">=3.7, <4",
-    install_requires=["matplotlib", "numpy"],
-    project_urls={
-        "Bug Reports": "https://github.com/bdavis222/dotscanner/issues",
-        "Funding": "https://www.paypal.com/donate/?business=UA5NL9MJSFMVY",
-        "Source": "https://github.com/bdavis222/dotscanner",
-    },
-    entry_points={
-        "console_scripts": [
-            "dotscanner = dotscanner.__main__:main"
-        ]
-    }
-)
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / 'README.md').read_text(encoding='utf-8')
+
+setup(
+    name='dotscanner',
+    version='1.3.0', # Required 
+    description='A program designed for analysis of microscope imaging data',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/bdavis222/dotscanner',
+    author='Holly Allen and Brian Davis',
+    author_email='holly.allen@colorado.edu',
+    classifiers=[
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Operating System :: Unix',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Microsoft :: Windows'
+    ],
+    packages=find_packages(),
+    py_modules=['dotscanner', 'dotscanner.ui', 'settings', 'tests', 'tests.ui'],
+    python_requires='>=3.7, <4',
+    install_requires=['matplotlib', 'numpy'],
+    project_urls={
+        'Bug Reports': 'https://github.com/bdavis222/dotscanner/issues',
+        'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
+        'Source': 'https://github.com/bdavis222/dotscanner',
+    },
+    entry_points={
+        'console_scripts': [
+            'dotscanner = dotscanner.__main__:main'
+        ]
+    }
+)
```

### Comparing `dotscanner-1.2.9/tests/test_MicroscopeImage.py` & `dotscanner-1.3.0/tests/ui/test_MicroscopeImage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 from dotscanner.ui.MicroscopeImage import MicroscopeImage
-from tests.FakeUserSettings import FakeUserSettings
+from tests.ui.FakeUserSettings import FakeUserSettings
 import mock
 import numpy as np
 import unittest
 
 class TestMicroscopeImage(unittest.TestCase):
 	@mock.patch("dotscanner.dataprocessing.getData")
-	def getMicroscopeImage(self, mock_getData):
+	def getMicroscopeImageAndUserSettings(self, mock_getData):
 		mock_getData.return_value = np.array([
 			[0, 0, 0, 0, 0, 0, 0, 0, 0],
 			[0, 5, 8, 0, 0, 1, 0, 0, 0],
 			[0, 0, 0, 0, 0, 0, 0, 0, 0],
 			[0, 10, 0, 0, 0, 0, 0, 0, 0],
 			[0, 0, 0, 7, 0, 0, 0, 0, 1],
 			[0, 0, 0, 0, 0, 0, 0, 0, 0]
 		])
-		fakeUserSettings = FakeUserSettings(
+		userSettings = FakeUserSettings(
 							dotSize=2,
 							blobSize=5,
 							saveFigures=False,
 							startImage="fakeImage01.png",
 							skipsAllowed=3,
 							removeEdgeFrames=True,
 							thresholds=(1.5, 5.0, 2.0))
-		return MicroscopeImage("test/directory/", "filename.png", fakeUserSettings)
+		return MicroscopeImage("test/directory/", "filename.png", userSettings), userSettings
 	
 	def test_properLoading_whenClassInitializes(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, userSettings = self.getMicroscopeImageAndUserSettings()
 		
-		self.assertEqual(microscopeImage.dotSize, 2)
-		self.assertEqual(microscopeImage.blobSize, 5)
-		self.assertEqual(microscopeImage.saveFigures, False)
-		self.assertEqual(microscopeImage.startImage, "fakeImage01.png")
-		self.assertEqual(microscopeImage.skipsAllowed, 3)
-		self.assertEqual(microscopeImage.removeEdgeFrames, True)
+		self.assertEqual(userSettings.dotSize, 2)
+		self.assertEqual(userSettings.blobSize, 5)
+		self.assertEqual(userSettings.saveFigures, False)
+		self.assertEqual(userSettings.startImage, "fakeImage01.png")
+		self.assertEqual(userSettings.skipsAllowed, 3)
+		self.assertEqual(userSettings.removeEdgeFrames, True)
 		self.assertEqual(microscopeImage.thresholds, (1.5, 5.0, 2.0))
 		self.assertIn(3, microscopeImage.dotCoords)
 		self.assertIn(1, microscopeImage.dotCoords[3])
 		self.assertEqual(microscopeImage.blobCoords, {})
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
 	@mock.patch('settings.config.LOWER_DOT_THRESH_SCALE', 1.5)
 	def test_decreaseLowerDotThreshScale(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.decreaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.4)
 		
 		microscopeImage.decreaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.3)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
 	@mock.patch('settings.config.LOWER_DOT_THRESH_SCALE', 1.5)
 	def test_increaseLowerDotThreshScale(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.increaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.6)
 		
 		microscopeImage.increaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.7)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
 	@mock.patch('settings.config.UPPER_DOT_THRESH_SCALE', 5.0)
 	def test_decreaseUpperDotThreshScale(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.decreaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 4.9)
 		
 		microscopeImage.decreaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 4.8)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
 	@mock.patch('settings.config.UPPER_DOT_THRESH_SCALE', 5.0)
 	def test_increaseUpperDotThreshScale(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.increaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 5.1)
 		
 		microscopeImage.increaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 5.2)
 	
 	def test_setThresholds(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.setThresholds((1.26, 5.2, 3))
 		
 		self.assertEqual(microscopeImage.thresholds, (1.3, 5.2, 3.0))
 	
 	def test_updateThresholds(self):
-		microscopeImage = self.getMicroscopeImage()
+		microscopeImage, _ = self.getMicroscopeImageAndUserSettings()
 		
 		microscopeImage.lowerDotThreshScale = 1.2
 		microscopeImage.lowerBlobThreshScale = 2.2
 		microscopeImage.updateThresholds()
 		
 		self.assertEqual(microscopeImage.thresholds, (1.2, 5.0, 2.2))
```

### Comparing `dotscanner-1.2.9/tests/test_lifetime.py` & `dotscanner-1.3.0/tests/test_lifetime.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dotscanner.lifetime as lifetime
-from tests.FakeUserSettings import FakeUserSettings
+from tests.ui.FakeUserSettings import FakeUserSettings
 import mock
 import unittest
 
 class TestLifetime(unittest.TestCase):
 	def test_addToPlotCoords(self):
 		coordsToPlot = {}
 		
@@ -23,15 +23,14 @@
 		self.assertIn((13, 8), coordsToPlot[7])
 	
 	def test_coordExistsInPrevFrame(self):
 		result = lifetime.coordExistsInPrevFrame(
 			y=8,
 			x=13,
 			imageNumber=5,
-			edgeFrameNumbers=[0, 1, 9, 10],
 			imageNumberToCoordMap={
 				0: {},
 				1: {},
 				2: {},
 				3: {4 : {6, 15}, 7 : {14}},
 				4: {},
 				5: {8 : {13}},
@@ -46,15 +45,14 @@
 		
 		self.assertTrue(result)
 		
 		result2 = lifetime.coordExistsInPrevFrame(
 			y=8,
 			x=13,
 			imageNumber=5,
-			edgeFrameNumbers=[0, 1, 9, 10],
 			imageNumberToCoordMap={
 				0: {},
 				1: {},
 				2: {},
 				3: {4 : {6, 15}, 1 : {14}},
 				4: {},
 				5: {8 : {13}},
@@ -115,16 +113,16 @@
 		self.assertIn(2, edgeFrameNumbers)
 		self.assertIn(5, edgeFrameNumbers)
 		self.assertIn(6, edgeFrameNumbers)
 		self.assertIn(7, edgeFrameNumbers)
 		self.assertNotIn(3, edgeFrameNumbers)
 		self.assertNotIn(4, edgeFrameNumbers)
 	
-	def test_getCoordLifetime(self):
-		result = lifetime.getCoordLifetime(
+	def test_getCoordLifetimeAndDisplacement(self):
+		time, displacement = lifetime.getCoordLifetimeAndDisplacement(
 			y=8,
 			x=13,
 			imageNumber=5,
 			edgeFrameNumbers=[0, 1, 9, 10],
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
@@ -138,18 +136,44 @@
 				9: {},
 				10: {}},
 			dotSize=2,
 			skipsAllowed=2,
 			removeEdgeFrames=True
 		)
 		
-		self.assertEqual(result, 3)
+		self.assertEqual(time, 3)
+		self.assertEqual(displacement, 1) # Displacement is actually squared
+		
+		time2, displacement2 = lifetime.getCoordLifetimeAndDisplacement(
+			y=8,
+			x=13,
+			imageNumber=5,
+			edgeFrameNumbers=[0, 1, 9, 10],
+			imageNumberToCoordMap={
+				0: {}, 
+				1: {}, 
+				2: {}, 
+				3: {}, 
+				4: {}, 
+				5: {8 : {13}},
+				6: {10 : {14}},
+				7: {12 : {7, 16}},
+				8: {}, 
+				9: {},
+				10: {}},
+			dotSize=2,
+			skipsAllowed=2,
+			removeEdgeFrames=True
+		)
+		
+		self.assertEqual(time2, 3)
+		self.assertEqual(displacement2, 25) # Displacement is actually squared
 	
 	def test_getCoordLifetime_returnsNone_whenRunningToEdgeFrameWithEdgeFramesRemoved(self):
-		result = lifetime.getCoordLifetime(
+		time, displacement = lifetime.getCoordLifetimeAndDisplacement(
 			y=8,
 			x=13,
 			imageNumber=5,
 			edgeFrameNumbers=[0, 1, 6, 7],
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
@@ -160,29 +184,32 @@
 				6: {9 : {14}},
 				7: {9 : {7, 13}}},
 			dotSize=2,
 			skipsAllowed=2,
 			removeEdgeFrames=True
 		)
 		
-		self.assertEqual(result, None)
+		self.assertEqual(time, None)
+		self.assertEqual(displacement, None)
 	
-	def test_updateLifetimeResults_doesNotUpdateContainers_whenImageNumberLessThanOrEqualToSkipsAllowedAndEdgeFramesRemoved(self):
+	def test_updateLifetimes_notUpdateContainers_whenImNumLessThanSkipsAndEdgeFramesRemoved(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=1,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {}, 
 				4: {}, 
 				5: {8 : {13}},
@@ -204,23 +231,25 @@
 		self.assertEqual(len(startImages), 0)
 		self.assertEqual(coordsToPlot, {})
 		
 	def test_updateLifetimeResults_doesNotUpdateContainers_whenCoordExistsInPrevFrame(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=1,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {4 : {6, 15}, 7 : {14}}, 
 				4: {}, 
 				5: {8 : {13}},
@@ -242,23 +271,25 @@
 		self.assertEqual(len(startImages), 0)
 		self.assertEqual(coordsToPlot, {})
 	
 	def test_updateLifetimeResults_doesNotUpdateContainers_whenCoordLifetimeIsNone(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=5,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {}, 
 				4: {}, 
 				5: {8 : {13}}},
@@ -276,23 +307,25 @@
 		self.assertEqual({}, coordsToPlot)
 	
 	@mock.patch("settings.config.LIFETIME_MIN_FOR_PLOT", 1)
 	def test_updateLifetimeResults_updatesAllContainersButCoordsToPlot_whenNotSavingFigures(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=5,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {}, 
 				4: {}, 
 				5: {8 : {13}},
@@ -318,23 +351,25 @@
 		self.assertEqual(coordsToPlot, {})
 	
 	@mock.patch("settings.config.LIFETIME_MIN_FOR_PLOT", 1)
 	def test_updateLifetimeResults_updatesAllContainers_whenSavingFigures(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=5,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {}, 
 				4: {}, 
 				5: {8 : {13}},
@@ -361,23 +396,25 @@
 		self.assertIn((13, 8), coordsToPlot[5])
 		
 	@mock.patch("settings.config.LIFETIME_MIN_FOR_PLOT", 4)
 	def test_updateLifetimeResults_updatesAllContainersButCoordsToPlot_whenLifetimeMinForPlotIsLarge(self):
 		lifetimes = []
 		resultCoords = []
 		startImages = []
+		displacements = []
 		coordsToPlot = {}
 		
 		lifetime.updateLifetimeResults(
 			imageNumber=5,
 			y=8,
 			x=13,
 			lifetimes=lifetimes,
 			resultCoords=resultCoords,
 			startImages=startImages,
+			displacements=displacements,
 			imageNumberToCoordMap={
 				0: {}, 
 				1: {}, 
 				2: {}, 
 				3: {}, 
 				4: {}, 
 				5: {8 : {13}},
```

