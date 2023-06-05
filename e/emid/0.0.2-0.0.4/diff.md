# Comparing `tmp/emid-0.0.2.tar.gz` & `tmp/emid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emid-0.0.2.tar", last modified: Mon Jun  5 10:00:52 2023, max compression
+gzip compressed data, was "emid-0.0.4.tar", last modified: Mon Jun  5 14:53:46 2023, max compression
```

## Comparing `emid-0.0.2.tar` & `emid-0.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 10:00:52.842939 emid-0.0.2/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 emid-0.0.2/COPYING.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41759 2023-06-05 10:00:52.841938 emid-0.0.2/PKG-INFO
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      322 2023-05-29 21:01:23.000000 emid-0.0.2/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 10:00:52.831938 emid-0.0.2/emid/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        2 2013-06-07 15:51:15.000000 emid-0.0.2/emid/__init__.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    29705 2023-05-30 05:54:03.000000 emid-0.0.2/emid/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       85 2023-06-05 10:00:19.000000 emid-0.0.2/emid/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16514 2023-05-29 21:03:03.000000 emid-0.0.2/emid/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15048 2023-06-01 15:21:06.000000 emid-0.0.2/emid/dialog_edit_phones.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    20099 2023-06-01 15:26:24.000000 emid-0.0.2/emid/dialog_edit_preferences.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10652 2023-06-01 16:56:06.000000 emid-0.0.2/emid/global_parameters.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     8852 2016-10-20 14:28:32.000000 emid-0.0.2/emid/multirate.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      791 2023-06-05 07:36:18.000000 emid-0.0.2/emid/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)  4027669 2023-06-05 07:36:19.000000 emid-0.0.2/emid/qrc_resources.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 emid-0.0.2/emid/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1554 2023-05-29 21:04:16.000000 emid-0.0.2/emid/utils_redirect_stream_to_file.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 emid-0.0.2/emid/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 emid-0.0.2/emid/wavpy_sndf.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 10:00:52.833938 emid-0.0.2/emid.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41759 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1171 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       40 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        5 2023-06-05 10:00:52.000000 emid-0.0.2/emid.egg-info/top_level.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 10:00:52.837938 emid-0.0.2/icons/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 emid-0.0.2/icons/audio-headphones.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 emid-0.0.2/icons/help-about.svgz
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 emid-0.0.2/icons/help-contents.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 emid-0.0.2/icons/help-contextual.svgz
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1220 2022-09-28 06:09:21.000000 emid-0.0.2/icons/oem-face-angry.svg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1516 2022-09-28 06:12:15.000000 emid-0.0.2/icons/oem-face-anguished.svg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      875 2022-09-28 06:11:07.000000 emid-0.0.2/icons/oem-face-frowning.svg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      816 2022-09-28 06:09:45.000000 emid-0.0.2/icons/oem-face-neutral.svg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      791 2022-09-28 06:10:15.000000 emid-0.0.2/icons/oem-face-smiling.svg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1218 2022-09-28 06:11:56.000000 emid-0.0.2/icons/oem-face-worried.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 emid-0.0.2/icons/preferences-other.svgz
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 10:00:52.841938 emid-0.0.2/prep-release/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      341 2023-05-29 20:58:30.000000 emid-0.0.2/prep-release/emid.pro
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_el.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_en_GB.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_en_US.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_es.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16660 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_fr.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.2/prep-release/emid_it.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-05 10:00:19.000000 emid-0.0.2/prep-release/minor_minor_number.txt
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      145 2023-05-29 20:58:52.000000 emid-0.0.2/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      410 2023-05-30 15:52:18.000000 emid-0.0.2/prep-release/mkupdate_pyqt6.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2537 2023-06-05 08:19:48.000000 emid-0.0.2/prep-release/release.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      904 2023-05-29 20:59:48.000000 emid-0.0.2/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      904 2023-05-29 20:59:58.000000 emid-0.0.2/prep-release/switch_pyqt6.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1206 2023-06-05 10:00:19.000000 emid-0.0.2/pyproject.toml
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      998 2023-05-29 20:57:10.000000 emid-0.0.2/resources.qrc
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 10:00:52.842939 emid-0.0.2/setup.cfg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 14:53:46.531411 emid-0.0.4/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 emid-0.0.4/COPYING.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41759 2023-06-05 14:53:46.531411 emid-0.0.4/PKG-INFO
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      322 2023-05-29 21:01:23.000000 emid-0.0.4/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 14:53:45.335380 emid-0.0.4/emid/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        2 2013-06-07 15:51:15.000000 emid-0.0.4/emid/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    32747 2023-06-05 14:52:56.000000 emid-0.0.4/emid/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       85 2023-06-05 14:53:16.000000 emid-0.0.4/emid/_version_info.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16514 2023-05-29 21:03:03.000000 emid-0.0.4/emid/audio_manager.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15048 2023-06-01 15:21:06.000000 emid-0.0.4/emid/dialog_edit_phones.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20099 2023-06-01 15:26:24.000000 emid-0.0.4/emid/dialog_edit_preferences.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10652 2023-06-01 16:56:06.000000 emid-0.0.4/emid/global_parameters.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     8852 2016-10-20 14:28:32.000000 emid-0.0.4/emid/multirate.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      791 2023-06-05 13:56:19.000000 emid-0.0.4/emid/pyqtver.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)  4027669 2023-06-05 07:36:19.000000 emid-0.0.4/emid/qrc_resources.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 emid-0.0.4/emid/sndlib.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1554 2023-05-29 21:04:16.000000 emid-0.0.4/emid/utils_redirect_stream_to_file.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 emid-0.0.4/emid/wavpy.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 emid-0.0.4/emid/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 14:53:45.337380 emid-0.0.4/emid.egg-info/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41759 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1171 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       40 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        5 2023-06-05 14:53:45.000000 emid-0.0.4/emid.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 14:53:45.341380 emid-0.0.4/icons/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 emid-0.0.4/icons/audio-headphones.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 emid-0.0.4/icons/help-about.svgz
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 emid-0.0.4/icons/help-contents.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 emid-0.0.4/icons/help-contextual.svgz
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1220 2022-09-28 06:09:21.000000 emid-0.0.4/icons/oem-face-angry.svg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1516 2022-09-28 06:12:15.000000 emid-0.0.4/icons/oem-face-anguished.svg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      875 2022-09-28 06:11:07.000000 emid-0.0.4/icons/oem-face-frowning.svg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      816 2022-09-28 06:09:45.000000 emid-0.0.4/icons/oem-face-neutral.svg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      791 2022-09-28 06:10:15.000000 emid-0.0.4/icons/oem-face-smiling.svg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1218 2022-09-28 06:11:56.000000 emid-0.0.4/icons/oem-face-worried.svg
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 emid-0.0.4/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 14:53:46.530411 emid-0.0.4/prep-release/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      341 2023-05-29 20:58:30.000000 emid-0.0.4/prep-release/emid.pro
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_el.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_en_GB.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_en_US.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_es.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16660 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_fr.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16516 2023-06-05 07:36:19.000000 emid-0.0.4/prep-release/emid_it.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-05 14:53:16.000000 emid-0.0.4/prep-release/minor_minor_number.txt
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      145 2023-05-29 20:58:52.000000 emid-0.0.4/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      410 2023-05-30 15:52:18.000000 emid-0.0.4/prep-release/mkupdate_pyqt6.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2537 2023-06-05 08:19:48.000000 emid-0.0.4/prep-release/release.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      904 2023-05-29 20:59:48.000000 emid-0.0.4/prep-release/switch_pyqt5.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      904 2023-05-29 20:59:58.000000 emid-0.0.4/prep-release/switch_pyqt6.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1206 2023-06-05 14:53:16.000000 emid-0.0.4/pyproject.toml
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      998 2023-05-29 20:57:10.000000 emid-0.0.4/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 14:53:46.531411 emid-0.0.4/setup.cfg
```

### Comparing `emid-0.0.2/COPYING.txt` & `emid-0.0.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/PKG-INFO` & `emid-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emid
-Version: 0.0.2
+Version: 0.0.4
 Summary: emid is a software for running a voice emotion identification experiment
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `emid-0.0.2/emid/__main__.py` & `emid-0.0.4/emid/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,14 +84,26 @@
         self.fileMenu.addAction(self.editPhonesAction)
         self.editPhonesAction.triggered.connect(self.onEditPhones)
         
         self.editPrefAction = QAction(QIcon.fromTheme("preferences-other", QIcon(":/preferences-other")), self.tr('Preferences'), self)
         self.fileMenu.addAction(self.editPrefAction)
         self.editPrefAction.triggered.connect(self.onEditPref)
 
+        self.onShowManualHtmlAction = QAction(self.tr('Manual (html)'), self)
+        self.fileMenu.addAction(self.onShowManualHtmlAction)
+        self.onShowManualHtmlAction.triggered.connect(self.onShowManualHtml)
+
+        self.onShowManualPdfAction = QAction(self.tr('Manual (pdf)'), self)
+        self.fileMenu.addAction(self.onShowManualPdfAction)
+        self.onShowManualPdfAction.triggered.connect(self.onShowManualPdf)
+
+        self.onAboutAction = QAction(QIcon.fromTheme("help-about", QIcon(":/help-about")), self.tr('About emid'), self)
+        self.fileMenu.addAction(self.onAboutAction)
+        self.onAboutAction.triggered.connect(self.onAbout)
+
         self.iconButtonWidth = 200
         self.iconButtonHeight = 200
         self.happySmiley = QIcon.fromTheme("oem-face-smiling", QIcon(":/oem-face-smiling"))
         self.sadSmiley = QIcon.fromTheme("oem-face-frowning", QIcon(":/oem-face-frowning"))
         self.neutralSmiley = QIcon.fromTheme("oem-face-neutral", QIcon(":/oem-face-neutral"))
         self.scaredSmiley = QIcon.fromTheme("oem-face-anguished", QIcon(":/oem-face-anguished"))
         self.angrySmiley = QIcon.fromTheme("oem-face-angry", QIcon(":/oem-face-angry"))
@@ -330,14 +342,51 @@
             try:
                 currPhoneIdx = self.prm["phones"]["phonesChoices"].index(self.prm["pref"]["sound"]["phones"])
             except:
                 currPhoneIdx = 0
             self.prm["pref"]["sound"]["phones"] = self.prm["phones"]["phonesChoices"][currPhoneIdx]
             self.prm["phones"]["phonesMaxLevel"][self.prm["phones"]["phonesChoices"].index(self.prm["pref"]["sound"]["phones"])]
 
+    def onShowManualPdf(self):
+        fileToOpen = os.path.abspath(os.path.dirname(__file__)) + '/doc/_build/latex/emid.pdf'
+        print(fileToOpen)
+        QDesktopServices.openUrl(QtCore.QUrl.fromLocalFile(fileToOpen))
+        
+    def onShowManualHtml(self):
+        fileToOpen = os.path.abspath(os.path.dirname(__file__)) + '/doc/_build/html/index.html'
+        QDesktopServices.openUrl(QtCore.QUrl.fromLocalFile(fileToOpen))
+
+    def onAbout(self):
+        qt_compiled_ver = QtCore.QT_VERSION_STR
+        qt_runtime_ver = QtCore.qVersion()
+        qt_pybackend_ver = QtCore.PYQT_VERSION_STR
+        qt_pybackend = "PyQt"
+
+
+        QMessageBox.about(self, self.tr("About emid"),
+                              self.tr("""<b>emid - Python app for sound localization experiments</b> <br>
+                              - version: {0}; <br>
+                              - build date: {1} <br>
+                              <p> Copyright &copy; 2022-2023 Samuele Carcagno. <a href="mailto:sam.carcagno@gmail.com">sam.carcagno@gmail.com</a> 
+                              All rights reserved. <p>
+                              This program is free software: you can redistribute it and/or modify
+                              it under the terms of the GNU General Public License as published by
+                              the Free Software Foundation, either version 3 of the License, or
+                              (at your option) any later version.
+                              <p>
+                              This program is distributed in the hope that it will be useful,
+                              but WITHOUT ANY WARRANTY; without even the implied warranty of
+                              MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                              GNU General Public License for more details.
+                              <p>
+                              You should have received a copy of the GNU General Public License
+                              along with this program.  If not, see <a href="http://www.gnu.org/licenses/">http://www.gnu.org/licenses/</a>
+                              <p>Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}""").format(emid_version, emid_builddate, platform.python_version(), qt_pybackend, qt_pybackend_ver, qt_compiled_ver, qt_runtime_ver, platform.system()))
+
+
 
 
 class responseLight(QWidget):
     def __init__(self, parent):
         super(responseLight, self).__init__(parent)
         self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding,
                                        QSizePolicy.Policy.Expanding))
```

### Comparing `emid-0.0.2/emid/audio_manager.py` & `emid-0.0.4/emid/audio_manager.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/dialog_edit_phones.py` & `emid-0.0.4/emid/dialog_edit_phones.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/dialog_edit_preferences.py` & `emid-0.0.4/emid/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/global_parameters.py` & `emid-0.0.4/emid/global_parameters.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/multirate.py` & `emid-0.0.4/emid/multirate.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/pyqtver.py` & `emid-0.0.4/emid/pyqtver.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/qrc_resources.py` & `emid-0.0.4/emid/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/sndlib.py` & `emid-0.0.4/emid/sndlib.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/utils_redirect_stream_to_file.py` & `emid-0.0.4/emid/utils_redirect_stream_to_file.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/wavpy.py` & `emid-0.0.4/emid/wavpy.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid/wavpy_sndf.py` & `emid-0.0.4/emid/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/emid.egg-info/PKG-INFO` & `emid-0.0.4/emid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emid
-Version: 0.0.2
+Version: 0.0.4
 Summary: emid is a software for running a voice emotion identification experiment
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `emid-0.0.2/emid.egg-info/SOURCES.txt` & `emid-0.0.4/emid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/audio-headphones.svgz` & `emid-0.0.4/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/help-about.svgz` & `emid-0.0.4/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/help-contents.svgz` & `emid-0.0.4/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/help-contextual.svgz` & `emid-0.0.4/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-angry.svg` & `emid-0.0.4/icons/oem-face-angry.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-anguished.svg` & `emid-0.0.4/icons/oem-face-anguished.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-frowning.svg` & `emid-0.0.4/icons/oem-face-frowning.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-neutral.svg` & `emid-0.0.4/icons/oem-face-neutral.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-smiling.svg` & `emid-0.0.4/icons/oem-face-smiling.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/oem-face-worried.svg` & `emid-0.0.4/icons/oem-face-worried.svg`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/icons/preferences-other.svgz` & `emid-0.0.4/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_el.ts` & `emid-0.0.4/prep-release/emid_el.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_en_GB.ts` & `emid-0.0.4/prep-release/emid_en_GB.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_en_US.ts` & `emid-0.0.4/prep-release/emid_en_US.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_es.ts` & `emid-0.0.4/prep-release/emid_es.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_fr.ts` & `emid-0.0.4/prep-release/emid_fr.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/emid_it.ts` & `emid-0.0.4/prep-release/emid_it.ts`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/release.py` & `emid-0.0.4/prep-release/release.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/switch_pyqt5.py` & `emid-0.0.4/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/prep-release/switch_pyqt6.py` & `emid-0.0.4/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `emid-0.0.2/pyproject.toml` & `emid-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emid"
-version="0.0.2"
+version="0.0.4"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "emid is a software for running a voice emotion identification experiment"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `emid-0.0.2/resources.qrc` & `emid-0.0.4/resources.qrc`

 * *Files identical despite different names*

