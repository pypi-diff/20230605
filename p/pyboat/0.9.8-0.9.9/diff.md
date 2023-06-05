# Comparing `tmp/pyboat-0.9.8.tar.gz` & `tmp/pyboat-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboat-0.9.8.tar", last modified: Fri Apr  1 10:32:25 2022, max compression
+gzip compressed data, was "pyboat-0.9.9.tar", last modified: Fri Jul 29 09:37:17 2022, max compression
```

## Comparing `pyboat-0.9.8.tar` & `pyboat-0.9.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       88 2022-02-15 10:46:13.345650 pyboat-0.9.8/.gitignore
--rw-r--r--   0        0        0     3155 2022-04-01 10:24:29.712997 pyboat-0.9.8/CHANGELOG.md
--rw-r--r--   0        0        0    35067 2022-02-15 10:46:13.345650 pyboat-0.9.8/LICENSE
--rw-r--r--   0        0        0      257 2022-02-15 10:46:13.345650 pyboat-0.9.8/MANIFEST.in
--rw-r--r--   0        0        0     8880 2022-02-15 10:46:13.345650 pyboat-0.9.8/README.md
--rw-r--r--   0        0        0   174413 2022-02-15 10:46:13.345650 pyboat-0.9.8/doc/DataViewer.png
--rw-r--r--   0        0        0      509 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/description.md
--rw-r--r--   0        0        0     1097 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/gui_from_source.md
--rw-r--r--   0        0        0    12639 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/logo_circ128x128.png
--rw-r--r--   0        0        0    89484 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/navigator_install.png
--rw-r--r--   0        0        0    63139 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/navigator_install2.png
--rw-r--r--   0        0        0    36441 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/navigator_update.png
--rw-r--r--   0        0        0    79519 2022-02-15 10:46:13.357645 pyboat-0.9.8/doc/readout.png
--rw-r--r--   0        0        0   152106 2022-02-15 10:46:13.361643 pyboat-0.9.8/doc/spectrum.png
--rw-r--r--   0        0        0     2267 2022-02-15 10:46:13.361643 pyboat-0.9.8/empirical_backgrounds_demo.py
--rw-r--r--   0        0        0     2210 2022-02-15 10:46:13.361643 pyboat-0.9.8/ensemble_demo.py
--rw-r--r--   0        0        0   488314 2022-02-15 10:46:13.361643 pyboat-0.9.8/example_data/AR1_0.7_ensemble.csv
--rw-r--r--   0        0        0     3705 2022-02-15 10:46:13.361643 pyboat-0.9.8/example_data/FIJI_measurement.txt
--rw-r--r--   0        0        0    14940 2022-02-15 10:46:13.361643 pyboat-0.9.8/example_data/synth_signals.csv
--rw-r--r--   0        0        0    16917 2022-02-15 10:46:13.361643 pyboat-0.9.8/example_data/synth_signals.xlsx
--rw-r--r--   0        0        0    32422 2022-02-15 10:46:13.361643 pyboat-0.9.8/pyboat/LICENSE
--rw-r--r--   0        0        0     2027 2022-04-01 10:22:23.593546 pyboat-0.9.8/pyboat/__init__.py
--rw-r--r--   0        0        0       58 2022-02-23 14:51:58.133916 pyboat-0.9.8/pyboat/__main__.py
--rw-r--r--   0        0        0    25728 2022-04-01 10:18:44.924666 pyboat-0.9.8/pyboat/api.py
--rw-r--r--   0        0        0    24191 2022-04-01 10:28:29.133379 pyboat-0.9.8/pyboat/core.py
--rw-r--r--   0        0        0     4289 2022-02-23 14:51:58.177914 pyboat-0.9.8/pyboat/ensemble_measures.py
--rw-r--r--   0        0        0     8845 2022-02-15 10:46:13.361643 pyboat-0.9.8/pyboat/logo_circ128x128.png
--rw-r--r--   0        0        0    19922 2022-02-23 14:57:33.092633 pyboat-0.9.8/pyboat/plotting.py
--rw-r--r--   0        0        0     3281 2022-02-23 14:51:58.189914 pyboat-0.9.8/pyboat/ssg.py
--rw-r--r--   0        0        0    28733 2022-02-23 14:51:12.215170 pyboat-0.9.8/pyboat/ui/analysis.py
--rw-r--r--   0        0        0    23978 2022-02-23 14:50:50.571818 pyboat-0.9.8/pyboat/ui/batch_process.py
--rw-r--r--   0        0        0    38417 2022-04-01 09:52:07.730049 pyboat-0.9.8/pyboat/ui/data_viewer.py
--rw-r--r--   0        0        0    22710 2022-02-24 16:36:24.228268 pyboat-0.9.8/pyboat/ui/start_menu.py
--rw-r--r--   0        0        0    39451 2022-02-23 14:50:50.767812 pyboat-0.9.8/pyboat/ui/synth_gen.py
--rw-r--r--   0        0        0     7465 2022-02-23 14:50:50.399824 pyboat-0.9.8/pyboat/ui/util.py
--rw-r--r--   0        0        0      613 2022-02-23 11:24:53.615711 pyboat-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2761 2022-04-01 10:10:43.664906 pyboat-0.9.8/scripting_demo.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 pyboat-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0       88 2022-02-15 10:46:13.345650 pyboat-0.9.9/.gitignore
+-rw-r--r--   0        0        0     3155 2022-04-01 10:24:29.712997 pyboat-0.9.9/CHANGELOG.md
+-rw-r--r--   0        0        0    35067 2022-02-15 10:46:13.345650 pyboat-0.9.9/LICENSE
+-rw-r--r--   0        0        0      257 2022-02-15 10:46:13.345650 pyboat-0.9.9/MANIFEST.in
+-rw-r--r--   0        0        0     8880 2022-02-15 10:46:13.345650 pyboat-0.9.9/README.md
+-rw-r--r--   0        0        0   174413 2022-02-15 10:46:13.345650 pyboat-0.9.9/doc/DataViewer.png
+-rw-r--r--   0        0        0      509 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/description.md
+-rw-r--r--   0        0        0     1097 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/gui_from_source.md
+-rw-r--r--   0        0        0    12639 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/logo_circ128x128.png
+-rw-r--r--   0        0        0    89484 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/navigator_install.png
+-rw-r--r--   0        0        0    63139 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/navigator_install2.png
+-rw-r--r--   0        0        0    36441 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/navigator_update.png
+-rw-r--r--   0        0        0    79519 2022-02-15 10:46:13.357645 pyboat-0.9.9/doc/readout.png
+-rw-r--r--   0        0        0   152106 2022-02-15 10:46:13.361643 pyboat-0.9.9/doc/spectrum.png
+-rw-r--r--   0        0        0     2267 2022-02-15 10:46:13.361643 pyboat-0.9.9/empirical_backgrounds_demo.py
+-rw-r--r--   0        0        0     2210 2022-02-15 10:46:13.361643 pyboat-0.9.9/ensemble_demo.py
+-rw-r--r--   0        0        0   488314 2022-02-15 10:46:13.361643 pyboat-0.9.9/example_data/AR1_0.7_ensemble.csv
+-rw-r--r--   0        0        0     3705 2022-02-15 10:46:13.361643 pyboat-0.9.9/example_data/FIJI_measurement.txt
+-rw-r--r--   0        0        0    14940 2022-02-15 10:46:13.361643 pyboat-0.9.9/example_data/synth_signals.csv
+-rw-r--r--   0        0        0    16917 2022-02-15 10:46:13.361643 pyboat-0.9.9/example_data/synth_signals.xlsx
+-rw-r--r--   0        0        0    32422 2022-02-15 10:46:13.361643 pyboat-0.9.9/pyboat/LICENSE
+-rw-r--r--   0        0        0     2027 2022-07-29 09:36:27.203912 pyboat-0.9.9/pyboat/__init__.py
+-rw-r--r--   0        0        0       58 2022-02-23 14:51:58.133916 pyboat-0.9.9/pyboat/__main__.py
+-rw-r--r--   0        0        0    25728 2022-04-01 10:18:44.924666 pyboat-0.9.9/pyboat/api.py
+-rw-r--r--   0        0        0    24191 2022-04-01 10:28:29.133379 pyboat-0.9.9/pyboat/core.py
+-rw-r--r--   0        0        0     4289 2022-02-23 14:51:58.177914 pyboat-0.9.9/pyboat/ensemble_measures.py
+-rw-r--r--   0        0        0     8845 2022-02-15 10:46:13.361643 pyboat-0.9.9/pyboat/logo_circ128x128.png
+-rw-r--r--   0        0        0    19961 2022-07-29 09:32:58.116409 pyboat-0.9.9/pyboat/plotting.py
+-rw-r--r--   0        0        0     3281 2022-02-23 14:51:58.189914 pyboat-0.9.9/pyboat/ssg.py
+-rw-r--r--   0        0        0    28733 2022-02-23 14:51:12.215170 pyboat-0.9.9/pyboat/ui/analysis.py
+-rw-r--r--   0        0        0    23978 2022-02-23 14:50:50.571818 pyboat-0.9.9/pyboat/ui/batch_process.py
+-rw-r--r--   0        0        0    38410 2022-07-29 09:29:45.313179 pyboat-0.9.9/pyboat/ui/data_viewer.py
+-rw-r--r--   0        0        0    22710 2022-02-24 16:36:24.228268 pyboat-0.9.9/pyboat/ui/start_menu.py
+-rw-r--r--   0        0        0    39616 2022-07-29 09:28:40.396091 pyboat-0.9.9/pyboat/ui/synth_gen.py
+-rw-r--r--   0        0        0     7465 2022-02-23 14:50:50.399824 pyboat-0.9.9/pyboat/ui/util.py
+-rw-r--r--   0        0        0      613 2022-02-23 11:24:53.615711 pyboat-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2761 2022-04-01 10:10:43.664906 pyboat-0.9.9/scripting_demo.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 pyboat-0.9.9/PKG-INFO
```

### Comparing `pyboat-0.9.8/CHANGELOG.md` & `pyboat-0.9.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/LICENSE` & `pyboat-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/README.md` & `pyboat-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/DataViewer.png` & `pyboat-0.9.9/doc/DataViewer.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/gui_from_source.md` & `pyboat-0.9.9/doc/gui_from_source.md`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/logo_circ128x128.png` & `pyboat-0.9.9/doc/logo_circ128x128.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/navigator_install.png` & `pyboat-0.9.9/doc/navigator_install.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/navigator_install2.png` & `pyboat-0.9.9/doc/navigator_install2.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/navigator_update.png` & `pyboat-0.9.9/doc/navigator_update.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/readout.png` & `pyboat-0.9.9/doc/readout.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/doc/spectrum.png` & `pyboat-0.9.9/doc/spectrum.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/empirical_backgrounds_demo.py` & `pyboat-0.9.9/empirical_backgrounds_demo.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/ensemble_demo.py` & `pyboat-0.9.9/ensemble_demo.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/example_data/AR1_0.7_ensemble.csv` & `pyboat-0.9.9/example_data/AR1_0.7_ensemble.csv`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/example_data/FIJI_measurement.txt` & `pyboat-0.9.9/example_data/FIJI_measurement.txt`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/example_data/synth_signals.csv` & `pyboat-0.9.9/example_data/synth_signals.csv`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/example_data/synth_signals.xlsx` & `pyboat-0.9.9/example_data/synth_signals.xlsx`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/LICENSE` & `pyboat-0.9.9/pyboat/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/__init__.py` & `pyboat-0.9.9/pyboat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ pyBOAT - A Biological Oscillations Analysis Toolkit """
 
 import sys
 import os
 import argparse
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 # the object oriented API
 from .api import WAnalyzer
 
 # the core functions
 from .core import sinc_smooth
 from .core import sliding_window_amplitude
```

### Comparing `pyboat-0.9.8/pyboat/api.py` & `pyboat-0.9.9/pyboat/api.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/core.py` & `pyboat-0.9.9/pyboat/core.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/ensemble_measures.py` & `pyboat-0.9.9/pyboat/ensemble_measures.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/logo_circ128x128.png` & `pyboat-0.9.9/pyboat/logo_circ128x128.png`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/plotting.py` & `pyboat-0.9.9/pyboat/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 
 
 def draw_detrended(ax, time_vector, detrended):
 
     m, lw = get_marker_lw(detrended)
 
     ax2 = ax.twinx()
+    ax2.spines["top"].set_visible(False)
+
     ax2.plot(
         time_vector,
         detrended,
         "-",
         marker=m,
         ms=MARKER_SIZE,
         color=DETREND_COLOR,
@@ -693,30 +695,30 @@
     ax1.set_ylabel(f"Period ({time_unit})", fontsize=label_size)
     ax1.tick_params(axis="both", labelsize=tick_label_size)
 
     # phase coherence
     ax2.plot(tvec, phases["R"], c=PHASE_COLOR, lw=3, alpha=0.8)
 
     ax2.set_ylim((0, 1.1))
-    ax2.set_ylabel(f"Phase Coherence", fontsize=label_size)
+    ax2.set_ylabel("Phase Coherence", fontsize=label_size)
     ax2.tick_params(axis="both", labelsize=tick_label_size)
 
     # amplitudes
     ax3.plot(tvec, amplitudes["median"], c=AMPLITUDE_COLOR, lw=2, alpha=0.6)
     ax3.fill_between(
         tvec, amplitudes["Q1"], amplitudes["Q3"], color=AMPLITUDE_COLOR, alpha=0.2
     )
-    ax3.set_ylabel(f"Amplitude (a.u.)", fontsize=label_size)
+    ax3.set_ylabel("Amplitude (a.u.)", fontsize=label_size)
     ax3.tick_params(axis="both", labelsize=tick_label_size)
     ax3.set_xlabel(f"Time ({time_unit})", fontsize=label_size)
 
     # powers
     ax4.plot(tvec, powers["median"], c=POWER_COLOR, lw=2, alpha=0.6)
     ax4.fill_between(tvec, powers["Q1"], powers["Q3"], color=POWER_COLOR, alpha=0.2)
-    ax4.set_ylabel(f"Power (a.u.)", fontsize=label_size)
+    ax4.set_ylabel("Power (a.u.)", fontsize=label_size)
     ax4.tick_params(axis="both", labelsize=tick_label_size)
     ax4.set_xlabel(f"Time ({time_unit})", fontsize=label_size)
 
     fig.subplots_adjust(wspace=0.3, left=0.11, top=0.98, right=0.97, bottom=0.14)
 
     # fig.subplots_adjust(bottom = 0.1, left = 0.2, top = 0.95, hspace = 0.1)
     return axs
```

### Comparing `pyboat-0.9.8/pyboat/ssg.py` & `pyboat-0.9.9/pyboat/ssg.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/ui/analysis.py` & `pyboat-0.9.9/pyboat/ui/analysis.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/ui/batch_process.py` & `pyboat-0.9.9/pyboat/ui/batch_process.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/ui/data_viewer.py` & `pyboat-0.9.9/pyboat/ui/data_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,16 @@
         self.set_initial_T_c()
         self.doPlot()
 
     # probably all the toggle state variables are not needed -> read out checkboxes directly
     def toggle_raw(self, state):
         if state == Qt.Checked:
             self.plot_raw = True
+            # untoggle the detrended cb
+            self.cb_detrend.setChecked(False)
         else:
             self.plot_raw = False
 
         # signal selected?
         if self.signal_id:
             self.doPlot()
 
@@ -439,15 +441,21 @@
             print("new state:", self.cb_trend.isChecked())
 
         # trying to plot the trend
         if state == Qt.Checked:
             T_c = self.get_T_c(self.T_c_edit)
             if not T_c:
                 self.cb_trend.setChecked(False)
-                # self.cb_use_detrended.setChecked(False)
+                self.cb_detrend.setChecked(False)
+                self.cb_use_detrended.setChecked(False)
+                return
+
+            # don't plot raw and detrended together (trend is ok)
+            if self.cb_detrend.isChecked():
+                self.cb_raw.setChecked(False)
 
         # signal selected?
         if self.signal_id:
             self.doPlot()
 
     def toggle_envelope(self, state):
 
@@ -518,15 +526,15 @@
             if self.debug:
                 print("T_c set to:", T_c)
             return T_c
 
         # empty line edit
         except ValueError:
 
-            msgBox = QMessageBox()
+            msgBox = QMessageBox(parent=self)
             msgBox.setWindowTitle("Missing Parameter")
             msgBox.setText("Detrending parameter not set, specify a cut-off period!")
             msgBox.exec()
 
             if self.debug:
                 print("T_c ValueError", tc)
             return None
@@ -537,15 +545,15 @@
         window_size = wsize_edit.text().replace(",", ".")
         try:
             window_size = float(window_size)
 
         # empty line edit
         except ValueError:
 
-            msgBox = QMessageBox()
+            msgBox = QMessageBox(parent=self)
             msgBox.setWindowTitle("Missing Parameter")
             msgBox.setText(
                 "Amplitude envelope parameter not set, specify a sliding window size!"
             )
 
             msgBox.exec()
 
@@ -831,41 +839,30 @@
 
         window_size = self.get_wsize(self.wsize_edit)
         if not window_size:
             return
         if self.debug:
             print("Calculating envelope with window_size = ", window_size)
 
-        # cut of frequency set?!
-        if self.get_T_c(self.T_c_edit):
+        # cut of frequency set and detended plot activated?
+        if self.cb_detrend.isChecked():
 
             trend = self.calc_trend()
             if trend is None:
                 return
 
             signal = self.raw_signal - trend
-            envelope = pyboat.sliding_window_amplitude(signal, window_size, dt=self.dt)
-
-            if self.cb_detrend.isChecked():
-                return envelope
-
-            # fits on the original signal!
-            else:
-                return envelope + trend
-
-        # otherwise add the mean
         else:
-            if self.debug:
-                print("calculating envelope for raw signal", window_size)
+            signal = self.raw_signal
 
-            mean = self.raw_signal.mean()
-            envelope = pyboat.sliding_window_amplitude(
-                self.raw_signal, window_size=window_size, dt=self.dt
-            )
-            return envelope + mean
+        envelope = pyboat.sliding_window_amplitude(signal,
+                                                   window_size,
+                                                   dt=self.dt)
+
+        return envelope
 
     def doPlot(self):
 
         """
         Checks the checkboxes for trend and envelope..
         """
```

### Comparing `pyboat-0.9.8/pyboat/ui/start_menu.py` & `pyboat-0.9.9/pyboat/ui/start_menu.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyboat/ui/synth_gen.py` & `pyboat-0.9.9/pyboat/ui/synth_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,31 +497,41 @@
         self.setCentralWidget(main_widget)
         self.show()
 
     # probably all the toggle state variables are not needed -> read out checkboxes directly
     def toggle_raw(self, state):
         if state == Qt.Checked:
             self.plot_raw = True
+            # untoggle the detrended cb
+            self.cb_detrend.setChecked(False)
         else:
             self.plot_raw = False
 
         if self.raw_signal is not None:
             self.doPlot()
 
     def toggle_trend(self, state):
 
         if self.debug:
-            print("new state:", self.cb_trend.isChecked())
+            print("new state:", self.cb_trend.isChecked(), state, Qt.Checked)
 
         # trying to plot the trend
         if state == Qt.Checked:
             T_c = self.get_T_c(self.T_c_edit)
             if not T_c:
-                self.cb_trend.setChecked(False)
-                # self.cb_use_detrended.setChecked(False)
+                if self.cb_trend.isChecked():
+                    self.cb_trend.setChecked(False)
+                if self.cb_detrend.isChecked():
+                    self.cb_detrend.setChecked(False)
+                self.cb_use_detrended.setChecked(False)
+                return
+
+            # don't plot raw and detrended together (trend is ok)
+            if self.cb_detrend.isChecked():
+                self.cb_raw.setChecked(False)
 
         # signal selected?
         if np.any(self.raw_signal):
             self.doPlot()
 
     def toggle_envelope(self, state):
 
@@ -584,37 +594,40 @@
             T_c = float(tc)
             if self.debug:
                 print("T_c set to:", T_c)
             return T_c
 
         # empty line edit
         except ValueError:
-            self.NoTrend = MessageWindow(
-                "Detrending parameter not set,\n" + "specify a cut-off period!",
-                "No Trend",
+            msgBox = QMessageBox(parent=self)
+            msgBox.setWindowTitle("Missing Parameter")
+            msgBox.setText(
+                "Detrending parameter not set,\n" + "specify a cut-off period!"
             )
+            msgBox.exec()
 
             if self.debug:
                 print("T_c ValueError", tc)
             return None
 
     def get_L(self, L_edit):
 
         # value checking done by validator, accepts also comma '1,1' !
         L = L_edit.text().replace(",", ".")
         try:
             L = int(L)
 
         # empty line edit
         except ValueError:
-            self.NoTrend = MessageWindow(
-                "Envelope parameter not set,\n" + "specify a sliding window size!",
-                "No Envelope",
+            msgBox = QMessageBox(parent=self)
+            msgBox.setWindowTitle("Missing Parameter")
+            msgBox.setText(
+                "Envelope parameter not set,\n" + "specify a sliding window size!"
             )
-
+            msgBox.exec()
             if self.debug:
                 print("L ValueError", L)
             return None
 
         if self.debug:
             print("L set to:", L)
         return L
@@ -823,43 +836,29 @@
             self.OutOfBounds = MessageWindow(
                 f"Maximum sliding window size is {maxL:.2f} {self.time_unit}!",
                 "Value Error",
             )
             L = None
             return
 
-        # cut of frequency set?!
-        if self.get_T_c(self.T_c_edit):
+        # cut of frequency set and detended plot activated?
+        if self.cb_detrend.isChecked():
 
             trend = self.calc_trend()
             if trend is None:
                 return
-
             signal = self.raw_signal - trend
-            envelope = pyboat.sliding_window_amplitude(
-                signal, window_size=L, dt=self.dt
-            )
-
-            if self.cb_detrend.isChecked():
-                return envelope
-
-            # fits on the original signal!
-            else:
-                return envelope + trend
-
-        # otherwise add the mean
         else:
-            if self.debug:
-                print("calculating envelope for raw signal", L)
+            signal = self.raw_signal
 
-            mean = self.raw_signal.mean()
-            envelope = pyboat.sliding_window_amplitude(
-                self.raw_signal, window_size=L, dt=self.dt
-            )
-            return envelope + mean
+        envelope = pyboat.sliding_window_amplitude(
+            signal, window_size=L, dt=self.dt
+        )
+
+        return envelope
 
     def create_signal(self):
 
         """
         Retrieves all paramters from the synthesizer controls
         and calls the ssg. All line edits have validators set,
         however we have to check for intermediate empty inputs..
```

### Comparing `pyboat-0.9.8/pyboat/ui/util.py` & `pyboat-0.9.9/pyboat/ui/util.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/pyproject.toml` & `pyboat-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/scripting_demo.py` & `pyboat-0.9.9/scripting_demo.py`

 * *Files identical despite different names*

### Comparing `pyboat-0.9.8/PKG-INFO` & `pyboat-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboat
-Version: 0.9.8
+Version: 0.9.9
 Summary: pyBOAT - A Biological Oscillations Analysis Toolkit 
 Home-page: https://github.com/tensionhead/pyBOAT
 Author: Gregor Mönke
 Author-email: gregor.moenke@esi-frankfurt.de
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

