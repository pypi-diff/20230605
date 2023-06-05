# Comparing `tmp/google-apps-script-type-0.3.1.tar.gz` & `tmp/google-apps-script-type-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-apps-script-type-0.3.1.tar", last modified: Mon Jan 23 15:07:34 2023, max compression
+gzip compressed data, was "google-apps-script-type-0.3.2.tar", last modified: Mon Jun  5 13:59:59 2023, max compression
```

## Comparing `google-apps-script-type-0.3.1.tar` & `google-apps-script-type-0.3.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4626 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3712 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.779018 google-apps-script-type-0.3.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.779018 google-apps-script-type-0.3.1/google/apps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.779018 google-apps-script-type-0.3.1/google/apps/script/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/
--rw-rw-r--   0 root         (0)     1003     1262 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/calendar/
--rw-rw-r--   0 root         (0)     1003      949 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/__init__.py
--rw-rw-r--   0 root         (0)     1003      253 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/calendar/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/calendar/types/
--rw-rw-r--   0 root         (0)     1003      820 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6215 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/calendar/types/calendar_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/docs/
--rw-rw-r--   0 root         (0)     1003      862 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/__init__.py
--rw-rw-r--   0 root         (0)     1003      245 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/docs/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.783018 google-apps-script-type-0.3.1/google/apps/script/type/docs/types/
--rw-rw-r--   0 root         (0)     1003      737 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2185 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/docs/types/docs_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/drive/
--rw-rw-r--   0 root         (0)     1003      868 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/__init__.py
--rw-rw-r--   0 root         (0)     1003      247 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/drive/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/drive/types/
--rw-rw-r--   0 root         (0)     1003      742 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2289 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/drive/types/drive_addon_manifest.py
--rw-rw-r--   0 root         (0)     1003      235 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/gmail/
--rw-rw-r--   0 root         (0)     1003     1017 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/__init__.py
--rw-rw-r--   0 root         (0)     1003      247 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/gmail/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/gmail/types/
--rw-rw-r--   0 root         (0)     1003      891 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8148 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/gmail/types/gmail_addon_manifest.py
--rw-rw-r--   0 root         (0)     1003       84 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/sheets/
--rw-rw-r--   0 root         (0)     1003      874 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/__init__.py
--rw-rw-r--   0 root         (0)     1003      249 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/sheets/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.787019 google-apps-script-type-0.3.1/google/apps/script/type/sheets/types/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2207 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/sheets/types/sheets_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/google/apps/script/type/slides/
--rw-rw-r--   0 root         (0)     1003      874 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/__init__.py
--rw-rw-r--   0 root         (0)     1003      249 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/google/apps/script/type/slides/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/google/apps/script/type/slides/types/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2207 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/slides/types/slides_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/google/apps/script/type/types/
--rw-rw-r--   0 root         (0)     1003     1130 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2381 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/types/addon_widget_set.py
--rw-rw-r--   0 root         (0)     1003     3987 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/types/extension_point.py
--rw-rw-r--   0 root         (0)     1003     6278 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/google/apps/script/type/types/script_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/
--rw-r--r--   0 root         (0)     1003     4626 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3401 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:07:34.000000 google-apps-script-type-0.3.1/google_apps_script_type.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2988 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/tests/unit/gapic/calendar/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/calendar/__init__.py
--rw-rw-r--   0 root         (0)     1003      813 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/calendar/test_calendar.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.791019 google-apps-script-type-0.3.1/tests/unit/gapic/docs/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/docs/__init__.py
--rw-rw-r--   0 root         (0)     1003      797 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/docs/test_docs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/tests/unit/gapic/drive/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/drive/__init__.py
--rw-rw-r--   0 root         (0)     1003      801 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/drive/test_drive.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/tests/unit/gapic/gmail/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/gmail/__init__.py
--rw-rw-r--   0 root         (0)     1003      801 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/gmail/test_gmail.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/tests/unit/gapic/sheets/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/sheets/__init__.py
--rw-rw-r--   0 root         (0)     1003      805 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/sheets/test_sheets.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/tests/unit/gapic/slides/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/slides/__init__.py
--rw-rw-r--   0 root         (0)     1003      805 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/slides/test_slides.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:07:34.795019 google-apps-script-type-0.3.1/tests/unit/gapic/type/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      789 2023-01-23 15:04:10.000000 google-apps-script-type-0.3.1/tests/unit/gapic/type/test_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4609 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3695 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/apps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/apps/script/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/
+-rw-rw-r--   0 root         (0)     1003     1262 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/
+-rw-rw-r--   0 root         (0)     1003      949 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/__init__.py
+-rw-rw-r--   0 root         (0)     1003      253 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/
+-rw-rw-r--   0 root         (0)     1003      820 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6251 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/calendar_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/
+-rw-rw-r--   0 root         (0)     1003      862 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/__init__.py
+-rw-rw-r--   0 root         (0)     1003      245 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/
+-rw-rw-r--   0 root         (0)     1003      737 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2221 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/docs_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/
+-rw-rw-r--   0 root         (0)     1003      868 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/__init__.py
+-rw-rw-r--   0 root         (0)     1003      247 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/
+-rw-rw-r--   0 root         (0)     1003      742 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2325 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/drive_addon_manifest.py
+-rw-rw-r--   0 root         (0)     1003      235 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/
+-rw-rw-r--   0 root         (0)     1003     1017 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/__init__.py
+-rw-rw-r--   0 root         (0)     1003      247 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/
+-rw-rw-r--   0 root         (0)     1003      891 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8184 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/gmail_addon_manifest.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/
+-rw-rw-r--   0 root         (0)     1003      874 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      249 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/
+-rw-rw-r--   0 root         (0)     1003      747 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2243 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/sheets_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/slides/
+-rw-rw-r--   0 root         (0)     1003      874 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/__init__.py
+-rw-rw-r--   0 root         (0)     1003      249 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/slides/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/
+-rw-rw-r--   0 root         (0)     1003      747 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2243 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/slides_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/types/
+-rw-rw-r--   0 root         (0)     1003     1130 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2417 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/addon_widget_set.py
+-rw-rw-r--   0 root         (0)     1003     4023 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/extension_point.py
+-rw-rw-r--   0 root         (0)     1003     6314 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/script_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/
+-rw-r--r--   0 root         (0)     1003     4609 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3401 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/__init__.py
+-rw-rw-r--   0 root         (0)     1003      813 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/test_calendar.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/docs/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/docs/__init__.py
+-rw-rw-r--   0 root         (0)     1003      797 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/docs/test_docs.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/drive/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/drive/__init__.py
+-rw-rw-r--   0 root         (0)     1003      801 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/drive/test_drive.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/__init__.py
+-rw-rw-r--   0 root         (0)     1003      801 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/test_gmail.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      805 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/test_sheets.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/slides/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/slides/__init__.py
+-rw-rw-r--   0 root         (0)     1003      805 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/slides/test_slides.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/type/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      789 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/type/test_type.py
```

### Comparing `google-apps-script-type-0.3.1/LICENSE` & `google-apps-script-type-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/MANIFEST.in` & `google-apps-script-type-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/PKG-INFO` & `google-apps-script-type-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-script-type
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Apps Script Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -35,15 +35,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. _Google Apps Script Type Protos: https://developers.google.com/apps-script/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/type/latest
+.. _Client Library Documentation: https://googleapis.dev/python/type/latest
 .. _Product Documentation:  https://developers.google.com/apps-script/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-apps-script-type-0.3.1/README.rst` & `google-apps-script-type-0.3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. _Google Apps Script Type Protos: https://developers.google.com/apps-script/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/type/latest
+.. _Client Library Documentation: https://googleapis.dev/python/type/latest
 .. _Product Documentation:  https://developers.google.com/apps-script/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/calendar/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/calendar/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/calendar/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/calendar/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/calendar/types/calendar_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/calendar_addon_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/docs/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/docs/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/docs/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/docs/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/docs/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/docs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/docs/types/docs_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/docs/types/docs_addon_manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/drive/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/drive/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/drive/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/drive/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/drive/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/drive/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/drive/types/drive_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/drive/types/drive_addon_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.3.1"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gmail/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gmail/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gmail/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gmail/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/gmail/types/gmail_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/gmail_addon_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/sheets/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/sheets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/sheets/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/sheets/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/sheets/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/sheets/types/sheets_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/sheets_addon_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/slides/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/slides/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/slides/gapic_version.py` & `google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.3.2"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/slides/services/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/slides/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/slides/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/slides/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/slides/types/slides_addon_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/slides/types/slides_addon_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 import google.apps.script.type.types  # type: ignore
 
 __protobuf__ = proto.module(
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/types/__init__.py` & `google-apps-script-type-0.3.2/google/apps/script/type/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/types/addon_widget_set.py` & `google-apps-script-type-0.3.2/google/apps/script/type/types/addon_widget_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.apps.script.type",
     manifest={
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/types/extension_point.py` & `google-apps-script-type-0.3.2/google/apps/script/type/types/extension_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import wrappers_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.apps.script.type",
```

### Comparing `google-apps-script-type-0.3.1/google/apps/script/type/types/script_manifest.py` & `google-apps-script-type-0.3.2/google/apps/script/type/types/script_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import struct_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.apps.script.type.types import addon_widget_set, extension_point
```

### Comparing `google-apps-script-type-0.3.1/google_apps_script_type.egg-info/PKG-INFO` & `google-apps-script-type-0.3.2/google_apps_script_type.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-script-type
-Version: 0.3.1
+Version: 0.3.2
 Summary: Google Apps Script Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -35,15 +35,15 @@
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-apps-script-type.svg
    :target: https://pypi.org/project/google-apps-script-type/
 .. _Google Apps Script Type Protos: https://developers.google.com/apps-script/
-.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/type/latest
+.. _Client Library Documentation: https://googleapis.dev/python/type/latest
 .. _Product Documentation:  https://developers.google.com/apps-script/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
```

### Comparing `google-apps-script-type-0.3.1/google_apps_script_type.egg-info/SOURCES.txt` & `google-apps-script-type-0.3.2/google_apps_script_type.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/setup.py` & `google-apps-script-type-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,15 @@
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
+namespaces = ["google", "google.apps", "google.apps.script"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-apps-script-type-0.3.1/tests/__init__.py` & `google-apps-script-type-0.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/calendar/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/calendar/test_calendar.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/calendar/test_calendar.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/docs/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/docs/test_docs.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/docs/test_docs.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/drive/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/drive/test_drive.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/drive/test_drive.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/gmail/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/gmail/test_gmail.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/gmail/test_gmail.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/sheets/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/sheets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/sheets/test_sheets.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/sheets/test_sheets.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/slides/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/slides/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/slides/test_slides.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/slides/test_slides.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/type/__init__.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.1/tests/unit/gapic/type/test_type.py` & `google-apps-script-type-0.3.2/tests/unit/gapic/type/test_type.py`

 * *Files identical despite different names*

