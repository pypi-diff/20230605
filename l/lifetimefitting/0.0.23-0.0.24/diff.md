# Comparing `tmp/lifetimefitting-0.0.23.tar.gz` & `tmp/lifetimefitting-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.23.tar", last modified: Wed May 31 05:25:42 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.24.tar", last modified: Mon Jun  5 06:06:22 2023, max compression
```

## Comparing `lifetimefitting-0.0.23.tar` & `lifetimefitting-0.0.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/app/lifetimefitting/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/app/lifetimefitting/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:25:42.771295 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 05:25:42.000000 lifetimefitting-0.0.23/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:25:42.775295 lifetimefitting-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 05:25:31.000000 lifetimefitting-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.076037 lifetimefitting-0.0.24/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.076037 lifetimefitting-0.0.24/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/app/lifetimefitting/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/app/lifetimefitting/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 06:06:22.000000 lifetimefitting-0.0.24/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:06:22.080037 lifetimefitting-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-05 06:06:09.000000 lifetimefitting-0.0.24/setup.py
```

### Comparing `lifetimefitting-0.0.23/LICENSE.md` & `lifetimefitting-0.0.24/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.23/PKG-INFO` & `lifetimefitting-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.23
+Version: 0.0.24
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.23/README.md` & `lifetimefitting-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.23/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.24/app/lifetimefitting/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 from phdimporter import TRF
 from .funcs.gui import Ui_Form
 from .funcs.fittingFuncs import loadAndCull, fitFL
 import sys
 
-def plotFL():
+def plotFL() -> None:
     global csv
     plt.close('all')
     for i in ui.axList:
         i.remove()
     ui.axList = []
     ui.ax1.relim()
     ui.ax1.autoscale_view()
@@ -23,27 +23,27 @@
     ui.ax4.relim()
     ui.ax4.autoscale_view()
     _, irf, loaded1 = loadAndCull(ui.irf_file, ui)
     x, y, loaded2 = loadAndCull(ui.trf_file, ui)
     if loaded1 and loaded2:
         csv = fitFL(ui, x_in=x, y_in=y, irf_in=irf)
 
-def trf_browse():
+def trf_browse() -> None:
     ui.trf_file.setText(file_dialog.getOpenFileName(directory="/Users/adrea/gdrive/Monash/PhD/Fluorophore/data/tr/AAQ", filter="PicoHarp binary of text file (*.phd *.txt)")[0])
 
-def irf_browse():
+def irf_browse() -> None:
     ui.irf_file.setText(file_dialog.getOpenFileName(directory="/Users/adrea/gdrive/Monash/PhD/Fluorophore/data/tr/AAQ", filter="PicoHarp binary of text file (*.phd *.txt)")[0])
 
-def update_max_x():
+def update_max_x() -> None:
     ui.max_x_out.setValue(ui.max_x.value())
 
-def update_max_x_from_out():
+def update_max_x_from_out() -> None:
     ui.max_x.setValue(ui.max_x_out.value())
 
-def setupPlot():
+def setupPlot() -> None:
     ui.verticalLayout_plot = QtWidgets.QVBoxLayout(ui.frame)
     ui.verticalLayout_plot.setObjectName("verticalLayout_plot")
     ui.figure, (ui.ax1, ui.ax3, ui.ax2, ui.ax4) = plt.subplots(4, 1, figsize=(8, 10), sharex=True, height_ratios=[3, 3, 1, 1])
     ui.canvas = FigureCanvas(ui.figure)
     ui.toolbar = NavigationToolbar(ui.canvas)
     ui.verticalLayout_plot.addWidget(ui.canvas)
     ui.verticalLayout_plot.addWidget(ui.toolbar)
@@ -64,15 +64,15 @@
     ui.ax2.axhline(0, c='k', lw=0.5)
     # linear residuals
     ui.ax4.set_xlabel('Time (ns)')
     ui.ax4.set_ylabel('Residuals\n(lin)')
     ui.ax4.axvline(0, c='k', lw=0.5)
     ui.ax4.axhline(0, c='k', lw=0.5)
 
-def saveCSV():
+def saveCSV() -> None:
     global csv
     if 'csv' in globals():
         save_csv_dialog = QFileDialog()
         name = save_csv_dialog.getSaveFileName(filter="CSV Sheet (*.csv)")[0]
         if name != '':
             with open(name, 'w+') as f:
                 f.writelines(csv)
```

### Comparing `lifetimefitting-0.0.23/app/lifetimefitting/funcs/expFuncs.py` & `lifetimefitting-0.0.24/app/lifetimefitting/funcs/expFuncs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-import numpy as np 
-def expFunc(t, I0, τ) -> float:
+import numpy as np
+
+def expFunc(t: list[float], I0: int, τ: float) -> float:
     return np.multiply(np.exp(np.negative(np.divide(t, τ))), I0)
 
-def expFuncWC(t, I0, τ, c) -> float:
+def expFuncWC(t: list[float], I0: int, τ: float, c: float) -> float:
     return np.multiply(expFunc(t, I0, τ), c)
 
-def expFuncx2(t, I0, τ_1, c_1, τ_2, c_2):
+def expFuncx2(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float) -> float:
     return np.add(np.multiply(expFunc(t, I0, τ_1), c_1),
                   np.multiply(expFunc(t, I0, τ_2), c_2))
 
-def expFuncx3(t, I0, τ_1, c_1, τ_2, c_2, τ_3, c_3):
+def expFuncx3(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float, τ_3: float, c_3: float) -> float:
     return np.add(np.add(np.multiply(expFunc(t, I0, τ_1), c_1),
                          np.multiply(expFunc(t, I0, τ_2), c_2)),
                   np.multiply(expFunc(t, I0, τ_3), c_3))
 
-def expFuncx4(t, I0, τ_1, c_1, τ_2, c_2, τ_3, c_3, τ_4, c_4):
+def expFuncx4(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float, τ_3: float, c_3: float, τ_4: float, c_4: float) -> float:
     return np.add(np.add(np.add(np.multiply(expFunc(t, I0, τ_1), c_1),
                                 np.multiply(expFunc(t, I0, τ_2), c_2)),
                          np.multiply(expFunc(t, I0, τ_3), c_3)),
                   np.multiply(expFunc(t, I0, τ_4), c_4))
 
-def linFunc(t, I0, τ) -> float:
+def linFunc(t: list[float], I0: int, τ: float) -> float:
     # return np.add(np.negative(np.divide(t, τ)), np.log(I0))
     return np.multiply(np.exp(np.negative(np.divide(t, τ))), I0)
 
-def linFuncWC(t, I0, τ, c) -> float:
+def linFuncWC(t: list[float], I0: int, τ: float, c: float) -> float:
     return np.log(np.multiply(linFunc(t, I0, τ), c))
 
-def linFuncx2(t, I0, τ_1, c_1, τ_2, c_2):
-    return np.log(np.add(np.multiply(linFunc(t, I0, τ_1), c_1), 
+def linFuncx2(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float) -> float:
+    return np.log(np.add(np.multiply(linFunc(t, I0, τ_1), c_1),
                          np.multiply(linFunc(t, I0, τ_2), c_2)))
 
-def linFuncx3(t, I0, τ_1, c_1, τ_2, c_2, τ_3, c_3):
+def linFuncx3(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float, τ_3: float, c_3: float) -> float:
     return np.log(np.add(np.add(np.multiply(linFunc(t, I0, τ_1), c_1),
                                 np.multiply(linFunc(t, I0, τ_2), c_2)),
                          np.multiply(linFunc(t, I0, τ_3), c_3)))
 
-def linFuncx4(t, I0, τ_1, c_1, τ_2, c_2, τ_3, c_3, τ_4, c_4):
-    return np.log(np.add(np.add(np.add(np.multiply(linFunc(t, I0, τ_1), c_1), 
-                                       np.multiply(linFunc(t, I0, τ_2), c_2)), 
-                                np.multiply(linFunc(t, I0, τ_3), c_3)), 
-                         np.multiply(linFunc(t, I0, τ_4), c_4)))
+def linFuncx4(t: list[float], I0: int, τ_1: float, c_1: float, τ_2: float, c_2: float, τ_3: float, c_3: float, τ_4: float, c_4: float) -> float:
+    return np.log(np.add(np.add(np.add(np.multiply(linFunc(t, I0, τ_1), c_1),
+                                       np.multiply(linFunc(t, I0, τ_2), c_2)),
+                                np.multiply(linFunc(t, I0, τ_3), c_3)),
+                         np.multiply(linFunc(t, I0, τ_4), c_4)))
+
+FLFuncList = [expFuncWC, expFuncWC, expFuncx2, expFuncx3, expFuncx4]
+FLLinFuncList = [linFuncWC, linFuncWC, linFuncx2, linFuncx3, linFuncx4]
```

### Comparing `lifetimefitting-0.0.23/app/lifetimefitting/funcs/fittingFuncs.py` & `lifetimefitting-0.0.24/app/lifetimefitting/funcs/fittingFuncs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import struct
 import numpy as np
 from phdimporter import TRF
 from scipy.optimize import curve_fit
-from PyQt6.QtWidgets import QFileDialog, QMessageBox, QLineEdit
+from PyQt6.QtWidgets import QMessageBox, QLineEdit
 from .gui import Ui_Form
-from .expFuncs import linFuncWC, linFuncx2, linFuncx3, linFuncx4
-from .expFuncs import expFunc, expFuncWC, expFuncx2, expFuncx3, expFuncx4
+from .expFuncs import expFunc, expFuncWC
+from .expFuncs import FLFuncList, FLLinFuncList
 
-
-def chiSQ(y_obs, y_pred, popt) -> float:
+def chiSQ(y_obs: list[float], y_pred: list[float], popt: list[float]) -> float:
     dof = len(y_obs) - (len(popt))
     # ensure no divide by 0
     y_pred_max_1 = [i + 1 if i == 0 else i for i in y_pred]
     return np.sum(np.divide(np.square(np.subtract(y_obs, y_pred)), y_pred_max_1)) / len(y_pred)
 
 
-def loadAndCull(fc: QLineEdit, ui: Ui_Form):
+def loadAndCull(fc: QLineEdit, ui: Ui_Form) -> tuple[list[float], list[int], bool]:
     loaded = False
     x = y = []
 
     if fc.text() == '':
         QMessageBox(icon=QMessageBox.Icon.Critical, text='TRF or IRF not loaded!').exec()
     else:
         filename = fc.text().split("/")[-1].split("\\")[-1]
@@ -32,58 +31,51 @@
         except struct.error:
             QMessageBox(icon=QMessageBox.Icon.Critical, text=f'There was a problem reading {filename}').exec()
         except UnboundLocalError:
             QMessageBox(icon=QMessageBox.Icon.Critical, text=f'There was a problem reading {filename}').exec()
 
     return x, y, loaded
 
-def fitLifetime(ui, x, y, maxIter):
-    global FLFuncList
-    global FLLinFuncList
+def fitLifetime(ui: Ui_Form, x: list[float], y: list[float], maxIter: int) -> tuple[list[float], int]:
     expCount = ui.expCount_widg.value()
 
     minbounds = [max(y) - 500]
     maxbounds = [max(y) + 500]
 
     fitFunc = FLFuncList[expCount]
     if ui.logFit_widg.isChecked():
         y = np.log(y)
         fitFunc = FLLinFuncList[expCount]
 
     for i in range(expCount):
-        minbounds += [0,     0]
+        minbounds += [0, 0]
         maxbounds += [99999999, 1]
 
     popt, pcov = curve_fit(fitFunc, x, y,
-                           bounds=(minbounds, maxbounds), 
-                           # maxfev=maxIter,
+                           bounds=(minbounds, maxbounds),
+                           maxfev=maxIter,
                            max_nfev=999999999999,
                            # verbose=2,
                            )
 
     residual = np.sum(np.subtract(y, FLFuncList[expCount](x, *popt)))
 
     return popt, residual
 
-def fitFL(ui, plot=True, x_in=None, y_in=None, irf_in=None) -> None:
+def fitFL(ui: Ui_Form, plot: bool = True, x_in: list[float] = None, y_in: list[int] = None, irf_in: list[int] = None) -> str:
     csv = 'x,y_lin,y_log\n'
     csvTail = '\n'
     outPrint = ''
     maxIter = ui.maxIter_widg.value()
     binSize = ui.binSize_widg.value()
     expCount = ui.expCount_widg.value()
 
-    global FLFuncList
-    global FLLinFuncList
     global t
     global spectrumObject
 
-    FLFuncList = [expFuncWC, expFuncWC, expFuncx2, expFuncx3, expFuncx4]
-    FLLinFuncList = [linFuncWC, linFuncWC, linFuncx2, linFuncx3, linFuncx4]
-
     irf = irf_in
     irf = np.array(irf)
 
     irfMaxBin = irf.tolist().index(max(irf))
     for c, i in enumerate(irf[irfMaxBin:]):
         if i == 0:
             zeroBin = c + irfMaxBin
@@ -96,15 +88,15 @@
             break
     irf = irf[zeroBin:]
 
     x_raw = x_in
     y_raw = y_in
 
     max_y = max(y_raw)
-    irf = list(reversed(irf)) # the kernel is flipped in convolutions
+    irf = list(reversed(irf))  # the kernel is flipped in convolutions
     y_raw = np.append(y_raw, np.zeros((len(y_raw), 1)))
     y_raw = np.convolve(y_raw, irf, 'full')
     x_raw = [i*binSize*1e-3 for i in range(len(y_raw))]
 
     y_raw = np.divide(y_raw, max(y_raw)/max_y)
 
     maxTime = ui.maxTime_widg.value()
```

### Comparing `lifetimefitting-0.0.23/app/lifetimefitting/funcs/gui.py` & `lifetimefitting-0.0.24/app/lifetimefitting/funcs/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
-
+from PyQt6 import QtCore, QtWidgets
 
 class Ui_Form(object):
-    def setupUi(self, Form):
+    def setupUi(self, Form: QtWidgets.QWidget):
         Form.setObjectName("Form")
         Form.setEnabled(True)
         Form.resize(1024, 900)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Maximum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(Form.sizePolicy().hasHeightForWidth())
@@ -192,15 +191,15 @@
         self.frame.setObjectName("frame")
         self.horizontalLayout_4.addWidget(self.frame)
         self.verticalLayout_11.addWidget(self.groupBox)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
-    def retranslateUi(self, Form):
+    def retranslateUi(self, Form: QtWidgets.QWidget):
         _translate = QtCore.QCoreApplication.translate
         Form.setWindowTitle(_translate("Form", "Lifetime Fitting"))
         self.groupBox_4.setTitle(_translate("Form", "Input"))
         self.trf_browse.setText(_translate("Form", "Browse for TRF"))
         self.irf_browse.setText(_translate("Form", "Browse for IRF"))
         self.groupBox.setTitle(_translate("Form", "Fitting"))
         self.label.setText(_translate("Form", "Bin Width (ps)"))
```

### Comparing `lifetimefitting-0.0.23/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.24/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.23
+Version: 0.0.24
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.23/setup.py` & `lifetimefitting-0.0.24/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.23",
+    version = "0.0.24",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

