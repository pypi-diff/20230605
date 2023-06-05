# Comparing `tmp/jdNBTExplorer-2.0.tar.gz` & `tmp/jdNBTExplorer-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdNBTExplorer-2.0.tar", last modified: Sat May 27 08:53:19 2023, max compression
+gzip compressed data, was "jdNBTExplorer-2.1.tar", last modified: Mon Jun  5 21:02:15 2023, max compression
```

## Comparing `jdNBTExplorer-2.0.tar` & `jdNBTExplorer-2.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35071 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5178 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3642 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/AboutWindow.py
--rw-r--r--   0 root         (0) root         (0)     4782 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/EditWindow.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Functions.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Languages.py
--rw-r--r--   0 root         (0) root         (0)    17770 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Logo.png
--rw-r--r--   0 root         (0) root         (0)     7815 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/Settings.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/SettingsWindow.py
--rw-r--r--   0 root         (0) root         (0)    14346 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/TreeWidget.py
--rw-r--r--   0 root         (0) root         (0)     2379 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/translations/
--rw-r--r--   0 root         (0) root         (0)    14190 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/translations/jdNBTExplorer_de.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer/ui/
--rw-r--r--   0 root         (0) root         (0)     2020 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/AboutWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2061 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/EditWindow.ui
--rw-r--r--   0 root         (0) root         (0)     5515 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     3188 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/ui/SettingsWindow.ui
--rw-r--r--   0 root         (0) root         (0)        3 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/jdNBTExplorer/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5178 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-27 08:53:19.000000 jdNBTExplorer-2.0/jdNBTExplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2246 2023-05-27 08:52:30.000000 jdNBTExplorer-2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 08:53:19.965159 jdNBTExplorer-2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35071 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4222 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/jdNBTExplorer/
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/AboutWindow.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/EditWindow.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/Functions.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    17770 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/Logo.png
+-rw-r--r--   0 root         (0) root         (0)     7815 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/SettingsWindow.py
+-rw-r--r--   0 root         (0) root         (0)    14346 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/TreeWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/jdNBTExplorer/translations/
+-rw-r--r--   0 root         (0) root         (0)    15016 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/translations/jdNBTExplorer_de.ts
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/translations/jdNBTExplorer_nl.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/jdNBTExplorer/ui/
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/ui/AboutWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/ui/EditWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/ui/SettingsWindow.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/jdNBTExplorer/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 21:02:15.000000 jdNBTExplorer-2.1/jdNBTExplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-06-05 20:57:20.000000 jdNBTExplorer-2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 21:02:15.678318 jdNBTExplorer-2.1/setup.cfg
```

### Comparing `jdNBTExplorer-2.0/BuildBackend.py` & `jdNBTExplorer-2.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/LICENSE` & `jdNBTExplorer-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/PKG-INFO` & `jdNBTExplorer-2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdNBTExplorer
-Version: 2.0
+Version: 2.1
 Summary: A simple program for creating animated Images
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdNBTExplorer
 Project-URL: Issues, https://codeberg.org/JakobDev/jdNBTExplorer/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdNBTExplorer
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -102,7 +102,17 @@
 
 ####  UpdateUnixDataTranslations.py
 This regenerates the translation files in `deploy/translations`. these files contains the translations for the Desktop Entry and the AppStream File.
 It uses gettext, as it is hard to translate this using Qt.
 These files just exists to integrate the translation with Weblate, because Weblate can't translate the Desktop Entry and the AppStream file.
 Make sure you run this when you edited one of these files.
 You need to have gettext installed to use it.
+
+#### UpdateTranslators.py
+This uses git to get a list of all Translators and writes it to `jdNBTExplorer/data/translators.json`.
+This is used to display the translators in the About Dialog.
+You need git to run this script.
+
+#### WriteChangelogHtml.py
+This read the Changelog from `deploy/page.codeberg.JakobDev.jdNBTExplorer.metainfo.xml`, converts it to HTML and writes it to `jdNBTExplorer/data/changelog.html`.
+This is used to display the Changelog in the About Dialog.
+You need [appstream-python](https://pypi.org/project/appstream-python) to be installed to use this script.
```

### Comparing `jdNBTExplorer-2.0/README.md` & `jdNBTExplorer-2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -68,7 +68,17 @@
 
 ####  UpdateUnixDataTranslations.py
 This regenerates the translation files in `deploy/translations`. these files contains the translations for the Desktop Entry and the AppStream File.
 It uses gettext, as it is hard to translate this using Qt.
 These files just exists to integrate the translation with Weblate, because Weblate can't translate the Desktop Entry and the AppStream file.
 Make sure you run this when you edited one of these files.
 You need to have gettext installed to use it.
+
+#### UpdateTranslators.py
+This uses git to get a list of all Translators and writes it to `jdNBTExplorer/data/translators.json`.
+This is used to display the translators in the About Dialog.
+You need git to run this script.
+
+#### WriteChangelogHtml.py
+This read the Changelog from `deploy/page.codeberg.JakobDev.jdNBTExplorer.metainfo.xml`, converts it to HTML and writes it to `jdNBTExplorer/data/changelog.html`.
+This is used to display the Changelog in the About Dialog.
+You need [appstream-python](https://pypi.org/project/appstream-python) to be installed to use this script.
```

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/EditWindow.py` & `jdNBTExplorer-2.1/jdNBTExplorer/EditWindow.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/Environment.py` & `jdNBTExplorer-2.1/jdNBTExplorer/Environment.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/Functions.py` & `jdNBTExplorer-2.1/jdNBTExplorer/Functions.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/Logo.png` & `jdNBTExplorer-2.1/jdNBTExplorer/Logo.png`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/MainWindow.py` & `jdNBTExplorer-2.1/jdNBTExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/Settings.py` & `jdNBTExplorer-2.1/jdNBTExplorer/Settings.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/SettingsWindow.py` & `jdNBTExplorer-2.1/jdNBTExplorer/SettingsWindow.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/TreeWidget.py` & `jdNBTExplorer-2.1/jdNBTExplorer/TreeWidget.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/__init__.py` & `jdNBTExplorer-2.1/jdNBTExplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/translations/jdNBTExplorer_de.ts` & `jdNBTExplorer-2.1/jdNBTExplorer/translations/jdNBTExplorer_de.ts`

 * *Files 1% similar despite different names*

#### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/translations/jdNBTExplorer_de.ts` & `jdNBTExplorer-2.1/jdNBTExplorer/translations/jdNBTExplorer_de.ts`

```diff
@@ -1,26 +1,42 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1" language="de">
   <context>
     <name>AboutWindow</name>
     <message>
       <location filename="../ui/AboutWindow.ui" line="0"/>
+      <location filename="../ui/AboutWindow.ui" line="0"/>
       <source>About</source>
       <translation>Über</translation>
     </message>
     <message>
       <location filename="../ui/AboutWindow.ui" line="0"/>
       <source>An editor for Minecraft NBT files</source>
       <translation>Ein Editor für Minecraft NBT Dateien</translation>
     </message>
     <message>
       <location filename="../ui/AboutWindow.ui" line="0"/>
-      <source>This program is licensed under GNU GPL 3</source>
-      <translation>Dieses Programm ist unter der GNU GPL 3 lizenziert</translation>
+      <source>This Program is licensed under GPL 3</source>
+      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutWindow.ui" line="0"/>
+      <source>Translators</source>
+      <translation>Übersetzer</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutWindow.ui" line="0"/>
+      <source>The following people translated jdNBTExplorer:</source>
+      <translation>Die folgenden Personen haben jdNBTExplorer übersetzt:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutWindow.ui" line="0"/>
+      <source>Changelog</source>
+      <translation>Änderungsprotokoll</translation>
     </message>
     <message>
       <location filename="../ui/AboutWindow.ui" line="0"/>
       <source>Close</source>
       <translation>Schließen</translation>
     </message>
   </context>
@@ -84,14 +100,19 @@
       <translation>Englisch</translation>
     </message>
     <message>
       <location filename="../Languages.py" line="7"/>
       <source>German</source>
       <translation>Deutsch</translation>
     </message>
+    <message>
+      <location filename="../Languages.py" line="8"/>
+      <source>Dutch</source>
+      <translation>Niederländisch</translation>
+    </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
       <location filename="../MainWindow.py" line="63"/>
       <source>File not found</source>
       <translation>Datei nicht gefunden</translation>
```

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/ui/AboutWindow.ui` & `jdNBTExplorer-2.1/jdNBTExplorer/ui/EditWindow.ui`

 * *Files 22% similar despite different names*

#### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/ui/AboutWindow.ui` & `jdNBTExplorer-2.1/jdNBTExplorer/ui/EditWindow.ui`

```diff
@@ -1,77 +1,77 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>AboutWindow</class>
-  <widget class="QDialog" name="AboutWindow">
+  <class>EditWindow</class>
+  <widget class="QDialog" name="EditWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>400</width>
-        <height>300</height>
+        <width>218</width>
+        <height>127</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>About</string>
+      <string notr="true">EditWindow</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <widget class="QLabel" name="iconLabel">
-          <property name="text">
-            <string notr="true">{{icon}}</string>
+        <layout class="QFormLayout" name="formLayout">
+          <item row="0" column="0">
+            <widget class="QLabel" name="label">
+              <property name="text">
+                <string>Name:</string>
+              </property>
+            </widget>
+          </item>
+          <item row="1" column="0">
+            <widget class="QLabel" name="label_2">
+              <property name="text">
+                <string>Value:</string>
+              </property>
+            </widget>
+          </item>
+          <item row="2" column="0">
+            <widget class="QLabel" name="label_3">
+              <property name="text">
+                <string>Type:</string>
+              </property>
+            </widget>
+          </item>
+          <item row="0" column="1">
+            <widget class="QLineEdit" name="nameEdit"/>
+          </item>
+          <item row="1" column="1">
+            <widget class="QLineEdit" name="valueEdit"/>
+          </item>
+          <item row="2" column="1">
+            <widget class="QComboBox" name="typeComboBox"/>
+          </item>
+        </layout>
+      </item>
+      <item>
+        <spacer name="verticalSpacer">
+          <property name="orientation">
+            <enum>Qt::Vertical</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>40</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
+      <item>
+        <widget class="QDialogButtonBox" name="buttonBox">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="versionLabel">
-          <property name="text">
-            <string notr="true">jdNbtExplorer {{version}}</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_3">
-          <property name="text">
-            <string>An editor for Minecraft NBT files</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_4">
-          <property name="text">
-            <string>This program is licensed under GNU GPL 3</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label">
-          <property name="text">
-            <string notr="true">Copyright © 2021-2023 JakobDev</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QPushButton" name="closeButton">
-          <property name="text">
-            <string>Close</string>
+          <property name="standardButtons">
+            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Ok</set>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
```

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/ui/EditWindow.ui` & `jdNBTExplorer-2.1/jdNBTExplorer/ui/SettingsWindow.ui`

 * *Files 17% similar despite different names*

#### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/ui/EditWindow.ui` & `jdNBTExplorer-2.1/jdNBTExplorer/ui/SettingsWindow.ui`

```diff
@@ -1,78 +1,121 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>EditWindow</class>
-  <widget class="QDialog" name="EditWindow">
+  <class>SettingsWindow</class>
+  <widget class="QDialog" name="SettingsWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>218</width>
-        <height>127</height>
+        <width>400</width>
+        <height>155</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string notr="true">EditWindow</string>
+      <string>Settings</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
         <layout class="QFormLayout" name="formLayout">
           <item row="0" column="0">
-            <widget class="QLabel" name="label">
-              <property name="text">
-                <string>Name:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="0">
             <widget class="QLabel" name="label_2">
               <property name="text">
-                <string>Value:</string>
+                <string>Language:</string>
               </property>
             </widget>
           </item>
-          <item row="2" column="0">
+          <item row="0" column="1">
+            <layout class="QHBoxLayout" name="horizontalLayout">
+              <item>
+                <widget class="QComboBox" name="languageComboBox"/>
+              </item>
+              <item>
+                <widget class="QLabel" name="label">
+                  <property name="text">
+                    <string>(needs Restart)</string>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </item>
+          <item row="1" column="0">
             <widget class="QLabel" name="label_3">
               <property name="text">
-                <string>Type:</string>
+                <string>Length of recent files list:</string>
               </property>
             </widget>
           </item>
-          <item row="0" column="1">
-            <widget class="QLineEdit" name="nameEdit"/>
-          </item>
           <item row="1" column="1">
-            <widget class="QLineEdit" name="valueEdit"/>
-          </item>
-          <item row="2" column="1">
-            <widget class="QComboBox" name="typeComboBox"/>
+            <widget class="QSpinBox" name="recentFilesSpinBox"/>
           </item>
         </layout>
       </item>
       <item>
+        <widget class="QCheckBox" name="checkSaveCheckBox">
+          <property name="text">
+            <string>Ask before closing unsaved Files</string>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QCheckBox" name="showWelcomeMessageCheckBox">
+          <property name="text">
+            <string>Show welcome message on startup</string>
+          </property>
+        </widget>
+      </item>
+      <item>
         <spacer name="verticalSpacer">
           <property name="orientation">
             <enum>Qt::Vertical</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
               <height>40</height>
             </size>
           </property>
         </spacer>
       </item>
       <item>
-        <widget class="QDialogButtonBox" name="buttonBox">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Ok</set>
-          </property>
-        </widget>
+        <layout class="QHBoxLayout" name="horizontalLayout_2">
+          <item>
+            <widget class="QPushButton" name="resetButton">
+              <property name="text">
+                <string>Reset</string>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <spacer name="horizontalSpacer">
+              <property name="orientation">
+                <enum>Qt::Horizontal</enum>
+              </property>
+              <property name="sizeHint" stdset="0">
+                <size>
+                  <width>40</width>
+                  <height>20</height>
+                </size>
+              </property>
+            </spacer>
+          </item>
+          <item>
+            <widget class="QPushButton" name="okButton">
+              <property name="text">
+                <string>OK</string>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <widget class="QPushButton" name="cancelButton">
+              <property name="text">
+                <string>Cancel</string>
+              </property>
+            </widget>
+          </item>
+        </layout>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer/ui/MainWindow.ui` & `jdNBTExplorer-2.1/jdNBTExplorer/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer.egg-info/PKG-INFO` & `jdNBTExplorer-2.1/jdNBTExplorer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdNBTExplorer
-Version: 2.0
+Version: 2.1
 Summary: A simple program for creating animated Images
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdNBTExplorer
 Project-URL: Issues, https://codeberg.org/JakobDev/jdNBTExplorer/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdNBTExplorer
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -102,7 +102,17 @@
 
 ####  UpdateUnixDataTranslations.py
 This regenerates the translation files in `deploy/translations`. these files contains the translations for the Desktop Entry and the AppStream File.
 It uses gettext, as it is hard to translate this using Qt.
 These files just exists to integrate the translation with Weblate, because Weblate can't translate the Desktop Entry and the AppStream file.
 Make sure you run this when you edited one of these files.
 You need to have gettext installed to use it.
+
+#### UpdateTranslators.py
+This uses git to get a list of all Translators and writes it to `jdNBTExplorer/data/translators.json`.
+This is used to display the translators in the About Dialog.
+You need git to run this script.
+
+#### WriteChangelogHtml.py
+This read the Changelog from `deploy/page.codeberg.JakobDev.jdNBTExplorer.metainfo.xml`, converts it to HTML and writes it to `jdNBTExplorer/data/changelog.html`.
+This is used to display the Changelog in the About Dialog.
+You need [appstream-python](https://pypi.org/project/appstream-python) to be installed to use this script.
```

### Comparing `jdNBTExplorer-2.0/jdNBTExplorer.egg-info/SOURCES.txt` & `jdNBTExplorer-2.1/jdNBTExplorer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 jdNBTExplorer.egg-info/PKG-INFO
 jdNBTExplorer.egg-info/SOURCES.txt
 jdNBTExplorer.egg-info/dependency_links.txt
 jdNBTExplorer.egg-info/entry_points.txt
 jdNBTExplorer.egg-info/requires.txt
 jdNBTExplorer.egg-info/top_level.txt
 jdNBTExplorer/translations/jdNBTExplorer_de.ts
+jdNBTExplorer/translations/jdNBTExplorer_nl.ts
 jdNBTExplorer/ui/AboutWindow.ui
 jdNBTExplorer/ui/EditWindow.ui
 jdNBTExplorer/ui/MainWindow.ui
 jdNBTExplorer/ui/SettingsWindow.ui
```

### Comparing `jdNBTExplorer-2.0/pyproject.toml` & `jdNBTExplorer-2.1/pyproject.toml`

 * *Files identical despite different names*

