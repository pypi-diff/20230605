# Comparing `tmp/wpcsys-2.0.3.tar.gz` & `tmp/wpcsys-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.0.3.tar", last modified: Sat Mar 25 09:57:37 2023, max compression
+gzip compressed data, was "wpcsys-2.1.2.tar", last modified: Mon Jun  5 06:51:42 2023, max compression
```

## Comparing `wpcsys-2.0.3.tar` & `wpcsys-2.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 09:57:37.671971 wpcsys-2.0.3/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.0.3/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9996 2023-03-25 09:57:37.668947 wpcsys-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8935 2023-03-24 02:04:02.000000 wpcsys-2.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-25 09:57:37.672957 wpcsys-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:57:37.624080 wpcsys-2.0.3/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.0.3/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.0.3/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  6763520 2023-03-25 09:54:48.000000 wpcsys-2.0.3/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  7304192 2023-03-25 09:56:51.000000 wpcsys-2.0.3/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  7313408 2023-03-25 09:56:13.000000 wpcsys-2.0.3/wpcsys/pywpc.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-03-25 09:57:37.667489 wpcsys-2.0.3/wpcsys.egg-info/
--rw-rw-rw-   0        0        0     9996 2023-03-25 09:57:37.000000 wpcsys-2.0.3/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-25 09:57:37.000000 wpcsys-2.0.3/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 09:57:37.000000 wpcsys-2.0.3/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-03-25 09:57:37.000000 wpcsys-2.0.3/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-25 09:57:37.000000 wpcsys-2.0.3/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.462447 wpcsys-2.1.2/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9924 2023-06-05 06:51:42.455429 wpcsys-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8863 2023-06-05 06:31:04.000000 wpcsys-2.1.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-05 06:51:42.463430 wpcsys-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.403247 wpcsys-2.1.2/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.2/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.2/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  6996992 2023-06-05 06:49:32.000000 wpcsys-2.1.2/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  7545344 2023-06-05 06:50:46.000000 wpcsys-2.1.2/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  7555072 2023-06-05 06:50:13.000000 wpcsys-2.1.2/wpcsys/pywpc.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.452429 wpcsys-2.1.2/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0     9924 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.0.3/LICENSE` & `wpcsys-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.0.3/PKG-INFO` & `wpcsys-2.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.0.3
+Version: 2.1.2
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -87,18 +87,16 @@
 Quick Start
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
-   >>> pywpc.__version__
-   2.0.3
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -117,14 +115,19 @@
 
 .. code-block:: shell
 
    pip install -r requirements.txt
 
 Products
 --------
+
+Controller
+
+- STEM
+
 Ethernet based motion card
 
 - EMotion
 
 Ethernet based DAQ card
 
 - Ethan-A
@@ -154,43 +157,45 @@
 Wifi based DAQ card
 
 - Wifi-DAQ-E3-A
 
 I/O Function Table
 ------------------
 
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Model          |AI |AO |DI        |DO        |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Emotion        |   |   |          |          |    |     |     |     |    |   |0     |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-A        |0  |   |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-D        |   |   |1         |0         |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-L        |   |   |          |0         |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-O        |   | 0 |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-D   |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |1, 2 |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-DSNK|   |   |0, 1      |      2, 3|    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AD  |0  |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-TD  |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |    |1  |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-RD  |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |1   |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-CD  |   |   |0, 1, 2, 3|0, 1, 2, 3|1   |1, 2 |2    |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AOD |0  |0  |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |     |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-E3-A  |1  |   |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| STEM           |1,3,4|1,3,4|0~7 |0~7 |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-L        |     |     |    |0   |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-O        |     | 0   |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
```

### Comparing `wpcsys-2.0.3/README.rst` & `wpcsys-2.1.2/wpcsys.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: wpcsys
+Version: 2.1.2
+Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
+Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
+Author: chunglee_people, Chieh-An Lin
+Author-email: wu@wpc.com.tw
+License: MIT
+Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware :: Hardware Drivers
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Overview
 --------
 
 **WPC Python driver**, also known as `pywpc`, contains APIs for interacting with basically WPC DAQ cards or any other WPC USB, WiFi and Ethernet based devices.
 It supports Python version from 3.8 to 3.10 under Windows 10 operating systems.
 
 Our APIs support synchronous and asynchronous modes for computer processes or threads.
@@ -63,18 +87,16 @@
 Quick Start
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
-   >>> pywpc.__version__
-   2.0.3
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -93,14 +115,19 @@
 
 .. code-block:: shell
 
    pip install -r requirements.txt
 
 Products
 --------
+
+Controller
+
+- STEM
+
 Ethernet based motion card
 
 - EMotion
 
 Ethernet based DAQ card
 
 - Ethan-A
@@ -130,43 +157,45 @@
 Wifi based DAQ card
 
 - Wifi-DAQ-E3-A
 
 I/O Function Table
 ------------------
 
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Model          |AI |AO |DI        |DO        |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Emotion        |   |   |          |          |    |     |     |     |    |   |0     |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-A        |0  |   |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-D        |   |   |1         |0         |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-L        |   |   |          |0         |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Ethan-O        |   | 0 |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-D   |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |1, 2 |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-DSNK|   |   |0, 1      |      2, 3|    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AD  |0  |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-TD  |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |    |1  |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-RD  |   |   |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |2    |1, 2 |1   |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-CD  |   |   |0, 1, 2, 3|0, 1, 2, 3|1   |1, 2 |2    |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| USB-DAQ-F1-AOD |0  |0  |0, 1, 2, 3|0, 1, 2, 3|    |1, 2 |     |1, 2 |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
-| Wifi-DAQ-E3-A  |1  |   |          |          |    |     |     |     |    |   |      |
-+----------------+---+---+----------+----------+----+-----+-----+-----+----+---+------+
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| STEM           |1,3,4|1,3,4|0~7 |0~7 |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-L        |     |     |    |0   |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Ethan-O        |     | 0   |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-D   |     |     |0~3 |0~3 |    |1, 2 |1, 2 |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-DSNK|     |     |0, 1|2, 3|    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-AD  |0    |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-TD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |    |1  |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-RD  |     |     |0~3 |0~3 |    |1, 2 |2    |1, 2 |1   |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
```

### Comparing `wpcsys-2.0.3/setup.py` & `wpcsys-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wpcsys-2.0.3/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.2/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

