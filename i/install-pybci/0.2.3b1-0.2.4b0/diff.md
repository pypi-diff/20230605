# Comparing `tmp/install-pybci-0.2.3b1.tar.gz` & `tmp/install-pybci-0.2.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.3b1.tar", last modified: Sun Jun  4 12:56:08 2023, max compression
+gzip compressed data, was "install-pybci-0.2.4b0.tar", last modified: Mon Jun  5 17:51:32 2023, max compression
```

## Comparing `install-pybci-0.2.3b1.tar` & `install-pybci-0.2.4b0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/setup.py
```

### Comparing `install-pybci-0.2.3b1/LICENSE` & `install-pybci-0.2.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/PKG-INFO` & `install-pybci-0.2.4b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.3b1
+Version: 0.2.4b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -73,15 +73,17 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
+- Update ReadTheDocs!
+- Finish arduino hand grasp demo and video.
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
-- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
-- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
+- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.3b1/README.md` & `install-pybci-0.2.4b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
+- Update ReadTheDocs!
+- Finish arduino hand grasp demo and video.
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
-- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
-- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
+- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.3b1/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.4b0/install_pybci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.3b1
+Version: 0.2.4b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -73,15 +73,17 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
+- Update ReadTheDocs!
+- Finish arduino hand grasp demo and video.
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
-- run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo]
-- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
+- ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
+- ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.3b1/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.4b0/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.4b0/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ..Utils.Classifier import Classifier 
 from ..Utils.Logger import Logger
 import queue,threading, time
+import numpy as np
 
 class ClassifierThread(threading.Thread):
-    features = []
-    targets = []
+    features = np.array([])#[]
+    targets = np.array([])
     mode = "train"
     guess = " "
     epochCounts = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
                  classifierGuessMarkerQueue, classifierGuessMarkerEvent, queryFeaturesQueue, queryFeaturesEvent,
                  logger = Logger(Logger.INFO), numStreamDevices = 1,
                  minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
@@ -23,46 +24,57 @@
         self.classifierInfoQueue = classifierInfoQueue
         self.classifierGuessMarkerQueue = classifierGuessMarkerQueue
         self.classifierGuessMarkerEvent = classifierGuessMarkerEvent
         self.queryFeaturesQueue = queryFeaturesQueue
         self.queryFeaturesEvent = queryFeaturesEvent
         self.numStreamDevices = numStreamDevices
         self.logger = logger
+        #self.features = np.array([])#[]
+        #self.targets = np.array([])
 
     def run(self):
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
                 try:
                     featuresSingle, devCount, target, self.epochCounts = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
+                    
                     if self.numStreamDevices > 1: # Collects multiple data strems feature sets and synchronise here
                         tempdatatrain[devCount] = featuresSingle
                         if len(tempdatatrain) == self.numStreamDevices:
                             flattened_list = [item for sublist in tempdatatrain.values() for item in sublist]
                             tempdatatrain = {}
-                            self.targets.append(target)
-                            self.features.append(flattened_list)
+                            self.targets = np.append(self.targets, [target], axis = 0)
+                            #print(self.features.shape)
+                            self.features = np.append(self.features, [flattened_list], axis = 0)
                         # need to check if all device data is captured, then flatten and append
                             if len(self.epochCounts) > 1: # check if there is more then one test condition
                                 minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                                 if minNumKeyEpochs < self.minRequiredEpochs:
                                     pass
                                 else: 
                                     start = time.time()
                                     self.classifier.TrainModel(self.features, self.targets)
                                     if (self.logger.level == Logger.TIMING):
                                         end = time.time()
                                         self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
                             if self.classifierGuessMarkerEvent.is_set():
                                 self.classifierGuessMarkerQueue.put(self.guess)
                     else: # Only one device to collect from
-                        self.targets.append(target)
-                        self.features.append(featuresSingle)
+                        #self.targets.append(target)
+                        if self.features.shape[0] == 0:
+                            #print("reshaping")
+                            self.features = self.features.reshape((0,) + featuresSingle.shape)
+                        #self.features.append(featuresSingle)
+                        #print("target shape", self.targets.shape)
+                        self.targets = np.append(self.targets, [target], axis = 0)
+                        #print("feature shape ",self.features.shape)
+                        self.features = np.append(self.features, [featuresSingle], axis = 0)
                         if len(self.epochCounts) > 1: # check if there is more then one test condition
                             minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                             if minNumKeyEpochs < self.minRequiredEpochs:
                                 pass
                             else: 
                                 start = time.time()
                                 self.classifier.TrainModel(self.features, self.targets)
@@ -86,14 +98,15 @@
                             start = time.time()
                             self.guess = self.classifier.TestModel(flattened_list)
                             if (self.logger.level == Logger.TIMING):
                                 end = time.time()
                                 self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     else:
                         start = time.time()
+                        #print(featuresSingle)
                         self.guess = self.classifier.TestModel(featuresSingle)
                         if (self.logger.level == Logger.TIMING):
                             end = time.time()
                             self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
```

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-0.2.4b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/Utils/Classifier.py` & `install-pybci-0.2.4b0/pybci/Utils/Classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,51 +17,61 @@
     def __init__(self, clf = None, model = None, torchModel = None):
         super().__init__()
         if clf != None:
             self.clf = clf
         elif model != None:
             self.model = model
         elif torchModel != None:
-            self.torchModel = model
+            self.torchModel = torchModel
         self.CheckClassifierLibrary()
 
     def CheckClassifierLibrary(self):
         if self.model != None: # maybe requires actual check for tensorflow model
             self.classifierLibrary = "tensor"
         elif self.torchModel != None: # maybe requires actual check for sklearn clf
             self.classifierLibrary = "pyTorch"
         elif self.clf != None: # maybe requires actual check for sklearn clf
             self.classifierLibrary = "sklearn"
 
-
     def TrainModel(self, features, targets):
         x_train, x_test, y_train, y_test = train_test_split(features, targets, shuffle = True, test_size=0.2)
-        self.scaler = StandardScaler() # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
-        self.scaler.fit(x_train)  # Compute the mean and standard deviation based on the training data
-        x_train = self.scaler.transform(x_train)  # Scale the training data
-        x_test = self.scaler.transform(x_test)  # Scale the test data
+        #print(features.shape)
+        #print(x_train.shape)
+        if len(features.shape)==3:
+            self.scaler = [StandardScaler() for scaler in range(features.shape[1])] # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
+            for e in range(features.shape[1]): # this would normalise the channel, maybe better to normalise across other dimension
+                x_train[:,e,:] = self.scaler[e].fit_transform(x_train[:,e,:]) # Compute the mean and standard deviation based on the training data
+                x_test[:,e,:] = self.scaler[e].transform(x_test[:,e,:])  # Scale the test data
+        elif len(features.shape)== 2:    
+            self.scaler = StandardScaler() # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
+            x_train = self.scaler.fit_transform(x_train)  # Compute the mean and standard deviation based on the training data
+            x_test = self.scaler.transform(x_test)  # Scale the test data
         if all(item == y_train[0] for item in y_train):
             pass
         else:
             #print(x_train, y_train)
-            if self.classifierLibrary == "pytorch":
+            if self.classifierLibrary == "pyTorch":
                 self.accuracy, self.pymodel  = self.torchModel(x_train, x_test, y_train, y_test)
             elif self.classifierLibrary == "sklearn":
                 self.clf.fit(x_train, y_train)
                 y_predictions = self.clf.predict(x_test)
                 self.accuracy = sklearn.metrics.accuracy_score(y_test, y_predictions)
             elif self.classifierLibrary == "tensor":
                 self.model.fit(np.array(x_train), np.array(y_train)) # epochs and batch_size should be customisable
                 self.loss, self.accuracy = self.model.evaluate(np.array(x_test), np.array(y_test))
             else:
                 # no classifier library selected, print debug?
                 pass
 
     def TestModel(self, x):
-        x = self.scaler.transform([x])[0]  # Scale the test data
+        if len(x.shape)==2:
+            for e in range(x.shape[0]):
+                x[e,:] = self.scaler[e].transform([x[e,:]])[0]
+        elif len(x.shape)== 1:       
+            x = self.scaler.transform([x])[0]  # Scale the test data
         if self.classifierLibrary == "sklearn":
             x = np.expand_dims(x, axis=0)
             return self.clf.predict(x)
         elif self.classifierLibrary == "tensor":
             x = np.expand_dims(x, axis=0)
             predictions = self.model.predict(x)
             if len (predictions[0]) == 1: # assume binary classification
```

### Comparing `install-pybci-0.2.3b1/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.4b0/pybci/Utils/FeatureExtractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,17 @@
             self.featureChoices.svd_entropy,
             self.featureChoices.samp_entropy,
             self.featureChoices.rms,
             self.featureChoices.meanPSD,
             self.featureChoices.medianPSD,
             self.featureChoices.variance,
             self.featureChoices.meanAbs,
-            #self.featureChoices.waveformLength,
-            self.featureChoices.zeroCross]
-            #self.featureChoices.slopeSignChange]
+            self.featureChoices.waveformLength,
+            self.featureChoices.zeroCross,
+            self.featureChoices.slopeSignChange]
         )
         self.numFeatures = (len(self.freqbands)*self.featureChoices.psdBand)+selFeats
 
     def ProcessFeatures(self, epoch, sr, target):
         """Allows 2D time series data to be passed with given sample rate to get various time+frequency based features.
         Best for EEG, EMG, EOG, or other consistent data with a consistent sample rate (pupil labs does not)
         Which features are chosen is based on self.featureChoices with initialisation. self.freqbands sets the limits for
@@ -98,24 +98,24 @@
                 features[(ch* self.numFeatures)+l] = np.sqrt(np.mean(np.array(epoch[:,ch])**2))
             if self.featureChoices.variance: # variance
                 l += 1    
                 features[(ch* self.numFeatures)+l] =  np.var(epoch[:,ch])
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
                 features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in epoch[:,ch]])/len(epoch[:,ch])
-            #if self.featureChoices.waveformLength: # waveformLength
-            #    l += 1
-            #    features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
+            if self.featureChoices.waveformLength: # waveformLength
+                l += 1
+                features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c-epoch[inum,ch]) for inum, c in enumerate(epoch[1:,ch])])
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
-                features[(ch* self.numFeatures)+l] = sum([1 if c*epoch[:,ch][inum+1]<0 else 0 for inum, c in enumerate(epoch[:,ch][:-1])])
-            #if self.featureChoices.slopeSignChange: # slopeSignChange
-            #    l += 1    
-            #    ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
-            #    features[(ch self.numFeatures)+l] = ssc
+                features[(ch* self.numFeatures)+l] = sum([1 if c*epoch[inum+1,ch]<0 else 0 for inum, c in enumerate(epoch[:-1,ch])])
+            if self.featureChoices.slopeSignChange: # slopeSignChange
+                l += 1    
+                ssc = sum([1 if (c-epoch[inum+1,ch])*(c-epoch[inum+1,ch])>=0.1 else 0 for inum, c in enumerate(epoch[:-1,ch])])
+                features[(ch* self.numFeatures)+l] = ssc
         features[np.isnan(features)] = 0 # checks for nans
         features[features == np.inf] = 0#np.iinfo(np.int32).max
         #print(features)
         
         return features
     
 class GazeFeatureExtractor():
```

### Comparing `install-pybci-0.2.3b1/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.4b0/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/Utils/Logger.py` & `install-pybci-0.2.4b0/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b1/pybci/pybci.py` & `install-pybci-0.2.4b0/pybci/pybci.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,16 @@
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
                                                  self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.queryFeaturesQueue, self.queryFeaturesEvent,
                                                  logger = self.logger, numStreamDevices = len(self.dataThreads), minRequiredEpochs = self.minimumEpochsRequired,
                                                 clf = self.clf, model = self.model, torchModel = self.torchModel)
         self.classifierThread.start()
+        self.logger.log(Logger.INFO," Threads initialised.")
+
 
     def StopThreads(self):
         """
         Stops all PyBCI threads.
         """
         self.closeEvent.set()
         self.markerThread.join()
@@ -299,15 +301,15 @@
             self.logger.log(Logger.INFO," Invalid or no sklearn classifier passed to clf. Checking tensorflow model... ")
             if isinstance(model, tf.keras.Model):
                 self.model = model
             else:
                 self.model = None
                 self.logger.log(Logger.INFO," Invalid or no tensorflow model passed to model.  Checking pytorch torchModel...")
                 if callable(torchModel): # isinstance(torchModel, torch.nn.Module):
-                    self.torchModel = model
+                    self.torchModel = torchModel
                 else:
                     self.torchModel = None
                     self.logger.log(Logger.INFO," Invalid or no PyTorch model passed to model. Defaulting to SVM by SkLearn")
     
 
     # Could move all configures to a configuration class, might make options into more descriptive classes?
     def ConfigureEpochWindowSettings(self, globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}):
```

### Comparing `install-pybci-0.2.3b1/setup.py` & `install-pybci-0.2.4b0/setup.py`

 * *Files identical despite different names*

