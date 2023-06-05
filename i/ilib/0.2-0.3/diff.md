# Comparing `tmp/ilib-0.2.tar.gz` & `tmp/ilib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilib-0.2.tar", last modified: Wed May 31 16:02:06 2023, max compression
+gzip compressed data, was "ilib-0.3.tar", last modified: Mon Jun  5 03:54:59 2023, max compression
```

## Comparing `ilib-0.2.tar` & `ilib-0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.193215 ilib-0.2/
--rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.2/LICENSE
--rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-31 16:02:06.193326 ilib-0.2/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)     2366 2023-05-31 03:59:09.000000 ilib-0.2/README.md
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.192074 ilib-0.2/ilib/
--rw-r--r--   0 devinthakker   (501) staff       (20)     4476 2023-05-31 04:15:02.000000 ilib-0.2/ilib/ADX.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2296 2023-05-31 03:54:59.000000 ilib-0.2/ilib/ATR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2014 2023-05-30 16:10:37.000000 ilib-0.2/ilib/BOLLINGERBANDS.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2431 2023-05-30 22:30:49.000000 ilib-0.2/ilib/CCI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1810 2023-05-29 23:50:04.000000 ilib-0.2/ilib/EMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-05-31 03:55:36.000000 ilib-0.2/ilib/MACD.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1937 2023-05-31 03:55:51.000000 ilib-0.2/ilib/RSI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1159 2023-05-30 16:16:06.000000 ilib-0.2/ilib/SMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2723 2023-05-31 04:07:30.000000 ilib-0.2/ilib/STOCHOSCILLATOR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2738 2023-05-31 04:10:04.000000 ilib-0.2/ilib/VWAP.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      260 2023-05-31 04:00:43.000000 ilib-0.2/ilib/__init__.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-05-31 16:02:06.193067 ilib-0.2/ilib.egg-info/
--rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)      360 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/SOURCES.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/dependency_links.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       13 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/requires.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-05-31 16:02:06.000000 ilib-0.2/ilib.egg-info/top_level.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-05-31 16:02:06.193841 ilib-0.2/setup.cfg
--rw-r--r--   0 devinthakker   (501) staff       (20)      905 2023-05-31 16:00:21.000000 ilib-0.2/setup.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-05 03:54:59.350358 ilib-0.3/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-05-30 17:52:43.000000 ilib-0.3/LICENSE
+-rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-06-05 03:54:59.350468 ilib-0.3/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2454 2023-05-31 18:07:31.000000 ilib-0.3/README.md
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-05 03:54:59.349080 ilib-0.3/ilib/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     5989 2023-06-05 03:41:39.000000 ilib-0.3/ilib/ADX.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3360 2023-06-04 23:51:32.000000 ilib-0.3/ilib/ATR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3334 2023-06-03 22:50:35.000000 ilib-0.3/ilib/BOLLINGERBANDS.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3461 2023-06-05 03:19:37.000000 ilib-0.3/ilib/CCI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2752 2023-06-05 00:00:34.000000 ilib-0.3/ilib/EMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-05-31 03:55:36.000000 ilib-0.3/ilib/MACD.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3030 2023-06-01 23:03:18.000000 ilib-0.3/ilib/RSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2271 2023-06-01 23:05:22.000000 ilib-0.3/ilib/SMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     4217 2023-06-05 03:52:21.000000 ilib-0.3/ilib/STOCHOSCILLATOR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3630 2023-06-05 03:40:39.000000 ilib-0.3/ilib/STOCHRSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3454 2023-06-05 03:41:04.000000 ilib-0.3/ilib/VWAP.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      260 2023-05-31 04:00:43.000000 ilib-0.3/ilib/__init__.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-05 03:54:59.350195 ilib-0.3/ilib.egg-info/
+-rw-r--r--   0 devinthakker   (501) staff       (20)      598 2023-06-05 03:54:59.000000 ilib-0.3/ilib.egg-info/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)      377 2023-06-05 03:54:59.000000 ilib-0.3/ilib.egg-info/SOURCES.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-06-05 03:54:59.000000 ilib-0.3/ilib.egg-info/dependency_links.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       24 2023-06-05 03:54:59.000000 ilib-0.3/ilib.egg-info/requires.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        5 2023-06-05 03:54:59.000000 ilib-0.3/ilib.egg-info/top_level.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-06-05 03:54:59.350997 ilib-0.3/setup.cfg
+-rw-r--r--   0 devinthakker   (501) staff       (20)      919 2023-06-05 03:54:07.000000 ilib-0.3/setup.py
```

### Comparing `ilib-0.2/LICENSE` & `ilib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ilib-0.2/PKG-INFO` & `ilib-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.2
+Version: 0.3
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.2.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.3.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

### Comparing `ilib-0.2/README.md` & `ilib-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ILIB - Technical Indicator Library
 
 ![preview](preview.jpg)
 
 ILIB is a library of technical indicators that can be used to build trading strategies. It is written in Python and uses the [Pandas](https://pandas.pydata.org/docs/) and [Numpy](https://numpy.org/doc/stable/) library for data manipulation and [Matplotlib](https://matplotlib.org/) for charting.
 
 [![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/release/python-370/)
-[![PyPI](https://img.shields.io/pypi/v/ilib)](https://pypi.org/project/ilib/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ilib)](https://img.shields.io/github/downloads/devthakker/ilib/total.svg)
-![GitHub](https://img.shields.io/github/license/devthakker/ilib)
+[![PyPI](https://img.shields.io/pypi/v/ilib?color=blue)](https://pypi.org/project/ilib/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ilib?color=blue)](https://img.shields.io/github/downloads/devthakker/ilib/total.svg)
+![GitHub](https://img.shields.io/pypi/l/ilib?color=blue)
 
 ## Features
 
 - Implements various popular technical indicators for financial analysis.
 - Simple and intuitive API for easy integration into your trading systems.
 - Supports Python 3.7 and above.
 - Well-documented codebase and example usage for each indicator.
@@ -30,14 +30,15 @@
 - [x] [Bollinger Bands](https://www.investopedia.com/terms/b/bollingerbands.asp)
 - [x] [Commodity Channel Index](https://www.investopedia.com/terms/c/commoditychannelindex.asp)
 - [x] [Exponential Moving Average](https://www.investopedia.com/terms/e/ema.asp)
 - [x] [Moving Average Convergence Divergence](https://www.investopedia.com/terms/m/macd.asp)
 - [x] [Relative Strength Index](https://www.investopedia.com/terms/r/rsi.asp)
 - [x] [Simple Moving Average](https://www.investopedia.com/terms/s/sma.asp)
 - [x] [Stochastic Oscillator](https://www.investopedia.com/terms/s/stochasticoscillator.asp)
+- [x] [Stochastic RSI](https://www.investopedia.com/terms/s/stochrsi.asp)
 - [x] [Volume Weighted Average Price](https://www.investopedia.com/terms/v/vwap.asp)
 
 ## Usage
 
 ```python
 import ilib as ti
```

### Comparing `ilib-0.2/ilib/CCI.py` & `ilib-0.3/ilib/CCI.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import matplotlib.pyplot as plt
 
 class CCI:
     """
     Calculate the Commodity Channel Index (CCI) of a stock.
     
     Parameters:
     data (list): A list of the stock prices in chronological order, with the most recent price last.
@@ -67,8 +68,39 @@
     def get_cci(self):
         """Return the current CCI value.
 
         Returns:
             float: The current CCI value.
         """
         return self.cci[-1]
+    
+    def plot_show(self):
+        """
+        Plot the CCI values calculated.
+        """
+        fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(12, 6))
+        ax1.set_title('Stock Prices')
+        ax1.plot(self.data, label='High')
+        ax1.legend(loc='upper left')
+        ax2.set_title('CCI - {} period'.format(self.period))
+        ax2.plot(self.cci, label='CCI')
+        plt.tight_layout()
+        plt.show()
+        return
+    
+    def plot_save(self, filename):
+        """
+        Plot the CCI values calculated and save to file.
         
+        Parameters:
+            filename (str): The filename to save the plot to.
+        """
+        fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(12, 6))
+        ax1.set_title('Stock Prices')
+        ax1.plot(self.data, label='High')
+        ax1.legend(loc='upper left')
+        ax2.set_title('CCI - {} period'.format(self.period))
+        ax2.plot(self.cci, label='CCI')
+        plt.tight_layout()
+        plt.savefig(filename)
+        return
+
```

### Comparing `ilib-0.2/ilib/MACD.py` & `ilib-0.3/ilib/MACD.py`

 * *Files identical despite different names*

### Comparing `ilib-0.2/ilib.egg-info/PKG-INFO` & `ilib-0.3/ilib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ilib
-Version: 0.2
+Version: 0.3
 Summary: A package for various technical indicators
 Home-page: https://github.com/devthakker/ilib
-Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.2.tar.gz
+Download-URL: https://github.com/devthakker/ilib/archive/refs/tags/v0.3.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: ilib,technical indicators,finance,trading,stocks,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Developers
```

