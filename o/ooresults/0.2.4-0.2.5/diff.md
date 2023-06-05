# Comparing `tmp/ooresults-0.2.4.tar.gz` & `tmp/ooresults-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooresults-0.2.4.tar", last modified: Sun May  7 16:09:25 2023, max compression
+gzip compressed data, was "ooresults-0.2.5.tar", last modified: Mon Jun  5 16:45:52 2023, max compression
```

## Comparing `ooresults-0.2.4.tar` & `ooresults-0.2.5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/
--rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.4/LICENSE
--rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.4/MANIFEST.in
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-05-07 16:09:25.155203 ooresults-0.2.4/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.4/README.rst
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.127203 ooresults-0.2.4/ooresults/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/_server.py
--rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/configuration.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.131203 ooresults-0.2.4/ooresults/handler/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/build_results.py
--rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/demo_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/events.py
--rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/handler/handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    31158 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/handler/model.py
--rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/results.py
--rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/handler/series.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.131203 ooresults-0.2.4/ooresults/pdf/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.135203 ooresults-0.2.4/ooresults/pdf/fonts/
--rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Bold.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Italic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Regular.ttf
--rw-r--r--   0 rainer    (1000) users      (100)     2806 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/pdf.py
--rw-r--r--   0 rainer    (1000) users      (100)    11206 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/pdf/result.py
--rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/pdf/series.py
--rw-r--r--   0 rainer    (1000) users      (100)    10007 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/pdf/splittimes.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.123203 ooresults-0.2.4/ooresults/plugins/imports/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/plugins/imports/entries/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/imports/entries/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/plugins/imports/entries/text.py
--rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/iof_result_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/plugins/oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/reader.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/class_params.py
--rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/repo.py
--rw-r--r--   0 rainer    (1000) users      (100)    16754 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/repo/result_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/series_type.py
--rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/repo/sqlite_repo.py
--rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/start_type.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/repo/update/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/update_008.py
--rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/repo/update/update_tables.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.139203 ooresults-0.2.4/ooresults/schema/
--rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/schema/IOF.xsd
--rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/schema/cardreader_log.json
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/server.py
--rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/set_legacy_mode.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.143203 ooresults-0.2.4/ooresults/static/
--rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/style-tab.css
--rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/style.css
--rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/static/w3.js
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/templates/
--rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/add_class.html
--rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_club.html
--rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_competitor.html
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_course.html
--rw-r--r--   0 rainer    (1000) users      (100)     6405 2023-05-07 16:05:24.000000 ooresults-0.2.4/ooresults/templates/add_entry.html
--rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_entry_competitors.html
--rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/add_entry_result.html
--rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/add_event.html
--rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/base.html
--rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/classes_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/classes_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/clubs_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/clubs_table.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/competitors_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/competitors_table.html
--rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/courses_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/courses_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.4/ooresults/templates/demo_reader.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/entries_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/entries_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/events_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/events_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/main.html
--rw-r--r--   0 rainer    (1000) users      (100)     5924 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/results_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/results_table.html
--rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/root.html
--rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/select_event.html
--rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/series_settings.html
--rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/series_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/series_table.html
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/templates/si/
--rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/si/si1_data.html
--rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si1_error.html
--rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si1_page.html
--rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/templates/si/si2_data.html
--rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/si/si2_page.html
--rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/templates/unauthorized.html
--rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/user.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.147203 ooresults-0.2.4/ooresults/utils/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/utils/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.4/ooresults/utils/globals.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/ooresults/websocket_server/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/si.py
--rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/websocket_handler.py
--rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.4/ooresults/websocket_server/websocket_server.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.127203 ooresults-0.2.4/ooresults.egg-info/
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) users      (100)        1 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) users      (100)      102 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) users      (100)      152 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) users      (100)       10 2023-05-07 16:09:25.000000 ooresults-0.2.4/ooresults.egg-info/top_level.txt
--rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-05-07 16:05:24.000000 ooresults-0.2.4/pyproject.toml
--rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-05-07 16:09:25.155203 ooresults-0.2.4/setup.cfg
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/tests/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/competitor.py
--rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/entry.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.151203 ooresults-0.2.4/tests/model/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/model/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_build_series_result.py
--rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_event_class_results.py
--rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/model/test_parse_cardreader_log.py
--rw-r--r--   0 rainer    (1000) users      (100)    34026 2023-05-07 16:05:24.000000 ooresults-0.2.4/tests/model/test_store_cardreader_result.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/tests/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_export_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_import_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/plugins/test_plugin_iof_result_list.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-05-07 16:09:25.155203 ooresults-0.2.4/tests/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/repo/test_entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_events.py
--rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/repo/test_settings.py
--rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_compute_result_net.py
--rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_compute_result_score.py
--rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_compute_result_standard.py
--rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_configuration.py
--rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_ranking.py
--rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.4/tests/test_series.py
--rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.4/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/
+-rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.5/LICENSE
+-rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.5/MANIFEST.in
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-06-05 16:45:52.971423 ooresults-0.2.5/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.5/README.rst
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/_server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/configuration.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.943423 ooresults-0.2.5/ooresults/handler/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/build_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/demo_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    31158 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/handler/model.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/series.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.943423 ooresults-0.2.5/ooresults/pdf/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.947423 ooresults-0.2.5/ooresults/pdf/fonts/
+-rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)     3687 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/pdf.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11389 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/series.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10868 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/splittimes.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults/plugins/imports/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/plugins/imports/entries/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/imports/entries/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/imports/entries/text.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_result_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/reader.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/class_params.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16754 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/repo/result_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/series_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/repo/sqlite_repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/start_type.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/repo/update/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/update_008.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/update_tables.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.955423 ooresults-0.2.5/ooresults/schema/
+-rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/schema/IOF.xsd
+-rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/schema/cardreader_log.json
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/set_legacy_mode.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.955423 ooresults-0.2.5/ooresults/static/
+-rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/style-tab.css
+-rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/style.css
+-rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/w3.js
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/add_class.html
+-rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_club.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_competitor.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_course.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6405 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/templates/add_entry.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_entry_competitors.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/add_entry_result.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/base.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/classes_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/classes_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/clubs_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/clubs_table.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/competitors_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/competitors_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/courses_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/courses_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.5/ooresults/templates/demo_reader.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/entries_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/entries_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/events_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/events_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/main.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5925 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/templates/results_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/results_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/root.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/select_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/series_settings.html
+-rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/series_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/series_table.html
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/templates/si/
+-rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/si/si1_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si1_error.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si1_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/si/si2_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si2_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/unauthorized.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/utils/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/utils/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/utils/globals.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/websocket_server/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/si.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/websocket_handler.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/websocket_server.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults.egg-info/
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) users      (100)        1 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      102 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      152 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) users      (100)       10 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/top_level.txt
+-rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-06-05 16:41:57.000000 ooresults-0.2.5/pyproject.toml
+-rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-06-05 16:45:52.971423 ooresults-0.2.5/setup.cfg
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.967423 ooresults-0.2.5/tests/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/competitor.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/entry.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.967423 ooresults-0.2.5/tests/model/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/model/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_build_series_result.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_event_class_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_parse_cardreader_log.py
+-rw-r--r--   0 rainer    (1000) users      (100)    34026 2023-05-07 16:05:24.000000 ooresults-0.2.5/tests/model/test_store_cardreader_result.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/tests/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_export_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_import_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_result_list.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/tests/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_settings.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_compute_result_net.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_compute_result_score.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_compute_result_standard.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_configuration.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_ranking.py
+-rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_series.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_user.py
```

### Comparing `ooresults-0.2.4/LICENSE` & `ooresults-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/PKG-INFO` & `ooresults-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.4
+Version: 0.2.5
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.4/README.rst` & `ooresults-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/__init__.py` & `ooresults-0.2.5/ooresults/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/_reader.py` & `ooresults-0.2.5/ooresults/_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/_server.py` & `ooresults-0.2.5/ooresults/_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/configuration.py` & `ooresults-0.2.5/ooresults/configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/__init__.py` & `ooresults-0.2.5/ooresults/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/build_results.py` & `ooresults-0.2.5/ooresults/handler/build_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/classes.py` & `ooresults-0.2.5/ooresults/handler/classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/clubs.py` & `ooresults-0.2.5/ooresults/handler/clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/competitors.py` & `ooresults-0.2.5/ooresults/handler/competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/courses.py` & `ooresults-0.2.5/ooresults/handler/courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/demo_reader.py` & `ooresults-0.2.5/ooresults/handler/demo_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/entries.py` & `ooresults-0.2.5/ooresults/handler/entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/events.py` & `ooresults-0.2.5/ooresults/handler/events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/handicap.py` & `ooresults-0.2.5/ooresults/handler/handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/model.py` & `ooresults-0.2.5/ooresults/handler/model.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/results.py` & `ooresults-0.2.5/ooresults/handler/results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/handler/series.py` & `ooresults-0.2.5/ooresults/handler/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Bold.ttf` & `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-BoldItalic.ttf` & `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Italic.ttf` & `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/fonts/Carlito-Regular.ttf` & `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/pdf.py` & `ooresults-0.2.5/ooresults/websocket_server/websocket_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,72 +13,53 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-import pathlib
-from datetime import datetime
-
-from fpdf import FPDF
-
-from ooresults.repo.result_type import ResultStatus
-
-
-class PDF(FPDF):
-    MAP_STATUS = {
-        ResultStatus.INACTIVE: "",
-        ResultStatus.FINISHED: "Finished",
-        ResultStatus.OK: "OK",
-        ResultStatus.MISSING_PUNCH: "MP",
-        ResultStatus.DID_NOT_START: "DNS",
-        ResultStatus.DID_NOT_FINISH: "DNF",
-        ResultStatus.OVER_TIME: "OTL",
-        ResultStatus.DISQUALIFIED: "DSQ",
-    }
-
-    def __init__(self, name: str, landscape: bool = False):
-        orientation = "landscape" if landscape else "portrait"
-        super().__init__(font_cache_dir=None, orientation=orientation)
-        self.name = name
-        self.creation_time = datetime.now()
-
-        self.fonts_dir = pathlib.Path(__file__).parent / "fonts"
-        self.add_font(
-            family="Carlito",
-            fname=str(self.fonts_dir / "Carlito-Regular.ttf"),
-            uni=True,
-        )
-        self.add_font(
-            family="Carlito",
-            style="B",
-            fname=str(self.fonts_dir / "Carlito-Bold.ttf"),
-            uni=True,
-        )
-        self.add_font(
-            family="Carlito",
-            style="I",
-            fname=str(self.fonts_dir / "Carlito-Italic.ttf"),
-            uni=True,
-        )
-        self.add_font(
-            family="Carlito",
-            style="BI",
-            fname=str(self.fonts_dir / "Carlito-BoldItalic.ttf"),
-            uni=True,
-        )
-
-    def header(self):
-        self.set_font(family="Carlito", size=12)
-        self.cell(w=0, h=10, txt=self.name, border=1, align="C")
-        self.ln(20)
-
-    def footer(self):
-        # Position cursor at 1.5 cm from bottom:
-        self.set_y(-15)
-        self.set_font(family="Carlito", size=12)
-        # Printing page number
-        self.cell(
-            w=0, h=10, txt=self.creation_time.strftime("%Y-%m-%d %H:%M:%S"), align="L"
+import asyncio
+import threading
+import ssl
+
+import websockets
+
+from ooresults.websocket_server.websocket_handler import WebSocketHandler
+
+
+class WebSocketServer(threading.Thread):
+    def __init__(
+        self,
+        handler: WebSocketHandler,
+        host: str = "0.0.0.0",
+        port: int = 8081,
+        ssl_cert=None,
+        ssl_key=None,
+    ):
+        super().__init__()
+        self.daemon = True
+        self.handler = handler
+        self.host = host
+        self.port = port
+        self.ssl_cert = ssl_cert
+        self.ssl_key = ssl_key
+        self.loop = None
+
+    def run(self):
+        if self.ssl_cert is None:
+            ssl_context = None
+        else:
+            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+            ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
+
+        self.loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop=self.loop)
+        start_server = websockets.serve(
+            self.handler.handler, self.host, self.port, loop=self.loop, ssl=ssl_context
         )
-        self.cell(w=0, h=10, txt=f"Page {self.page_no()}/{{nb}}", align="R")
+        self.loop.run_until_complete(start_server)
+        if ssl_context is None:
+            print(f"ws://{self.host}:{str(self.port)}")
+        else:
+            print(f"wss://{self.host}:{str(self.port)}")
+        self.loop.run_forever()
+        print("thread finished")
```

### Comparing `ooresults-0.2.4/ooresults/pdf/result.py` & `ooresults-0.2.5/ooresults/pdf/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,20 @@
 
         # print possible voided legs
         if ranked_results and ranked_results[0]["result"] is not None:
             voided_legs = ranked_results[0]["result"].voided_legs()
             if voided_legs:
                 pdf.cell(txt=f'(Voided legs: {", ".join(voided_legs)})')
 
+        # course data
+        course_data = pdf.course_data(class_)
+        if course_data:
+            pdf.set_x(x=max(pdf.get_x() + 15, 100))
+            pdf.cell(txt=course_data)
+
         pdf.ln()
         pdf.ln()
         pdf.set_font(family="Carlito", style="I", size=10)
         cell(w=W_RANK, h=None, txt="Pl", align="R")
         cell(w=W_SPACE, h=None, txt="")
         cell(w=W_NAME, h=None, txt="Name", align="L")
         cell(w=W_SPACE, h=None, txt="")
```

### Comparing `ooresults-0.2.4/ooresults/pdf/series.py` & `ooresults-0.2.5/ooresults/pdf/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/pdf/splittimes.py` & `ooresults-0.2.5/ooresults/pdf/splittimes.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     # Instantiation of inherited class
     pdf = PDF(name=event.name, landscape=landscape)
     pdf.set_margin(margin=10)
     pdf.set_auto_page_break(auto=True, margin=15)
     pdf.add_page()
     nr_splittimes = 20 if landscape else 12
 
-    def cell(w: int, h: Optional[int] = None, txt: str = "", align: str = "L") -> None:
+    def cell(
+        pdf: PDF, w: int, h: Optional[int] = None, txt: str = "", align: str = "L"
+    ) -> None:
         while pdf.get_string_width(txt) > w:
             txt = txt[:-1]
         pdf.cell(w=w, h=h, txt=txt, align=align)
 
     def format_time(time: int, status: ResultStatus) -> str:
         if status == ResultStatus.OK:
             return globals.minutes_seconds(time=time)
@@ -49,20 +51,20 @@
 
     def format_splittime(time: Optional[int]) -> str:
         if time is not None:
             return globals.minutes_seconds(time=time)
         else:
             return "-----"
 
-    def pre(t1: str = "", t2: str = "", t3: str = "") -> None:
+    def pre(pdf: PDF, t1: str = "", t2: str = "", t3: str = "") -> None:
         pdf.set_font(style="B")
-        cell(w=7, h=None, txt=t1, align="R")
-        cell(w=2, h=None, txt="")
-        cell(w=33, h=None, txt=t2, align="L")
-        cell(w=12, h=None, txt=t3, align="R")
+        cell(pdf=pdf, w=7, h=None, txt=t1, align="R")
+        cell(pdf=pdf, w=2, h=None, txt="")
+        cell(pdf=pdf, w=33, h=None, txt=t2, align="L")
+        cell(pdf=pdf, w=12, h=None, txt=t3, align="R")
         pdf.set_font(style="")
 
     def t(a: Optional[datetime], b: Optional[datetime]) -> Optional[int]:
         if a is not None and b is not None:
             diff = b.replace(microsecond=0) - a.replace(microsecond=0)
             return int(diff.total_seconds())
         else:
@@ -86,15 +88,24 @@
 
         # print possible voided legs
         if ranked_results and ranked_results[0]["result"] is not None:
             voided_legs = ranked_results[0]["result"].voided_legs()
             if voided_legs:
                 pdf.cell(txt=f'(Voided legs: {", ".join(voided_legs)})')
 
+        # course data
+        course_data = pdf.course_data(class_)
+        if course_data:
+            pdf.set_x(x=max(pdf.get_x() + 12, 67))
+            pdf.cell(txt=course_data)
+
         pdf.ln()
+        # add a separator line (1/2 height of a line)
+        pdf.ln(0.5 * 0.3515 * 8)
+
         # print list of control codes as header
         codes = []
         for i, j in enumerate(
             [
                 t
                 for t in ranked_results[0]["result"].split_times
                 if t.status != "Additional"
@@ -105,16 +116,16 @@
             else:
                 codes.append(f"{str(i+1)}")
         codes.append("F")
         for i, j in enumerate(codes):
             if i % nr_splittimes == 0:
                 if i >= nr_splittimes:
                     pdf.ln()
-                pre()
-            cell(w=10, h=None, txt=j, align="R")
+                pre(pdf=pdf)
+            cell(pdf=pdf, w=10, h=None, txt=j, align="R")
 
         pdf.ln()
         pdf.ln()
 
         ranked = False
         for result in ranked_results:
 
@@ -180,82 +191,87 @@
                         else:
                             yield f"*({i.control_code})", format_splittime(i.time), ""
 
             if result["result"].status not in (
                 ResultStatus.INACTIVE,
                 ResultStatus.DID_NOT_START,
             ):
-                pdf.set_font(family="Carlito", size=8)
-                if result.rank is not None:
-                    ranked = True
-                elif ranked:
-                    ranked = False
-                    pdf.ln()
-
-                sp = 0
-                result_data = Result(result=result["result"])
-
-                def print_line_1(sp: int, line_1: List[str]) -> None:
-                    if sp <= nr_splittimes:
-                        running_time = result["result"].extensions.get(
-                            "running_time", result["result"].time
-                        )
-
-                        pre(
-                            t1=str(get(result, "rank"))
-                            if not get(result, "not_competing")
-                            else "AK",
-                            t2=get(result, "last_name")
-                            + " "
-                            + get(result, "first_name"),
-                            t3=format_time(running_time, result["result"].status),
-                        )
-                    else:
-                        pdf.ln()
-                        pre()
-
-                    for i in line_1:
-                        cell(w=10, h=None, txt=i, align="R")
-
-                def print_line_2(sp: int, line_2: List[str]) -> None:
-                    if sp <= nr_splittimes:
-                        pdf.ln()
-                        # first line: rank, lastname+firstname, time, splittimes
-                        pre(t2=get(result, "club"))
-                    else:
-                        pdf.ln()
-                        pre()
+                with pdf.unbreakable() as doc:
+                    doc.set_font(family="Carlito", size=8)
+                    if result.rank is not None:
+                        ranked = True
+                    elif ranked:
+                        ranked = False
+                        doc.ln()
+
+                    sp = 0
+                    result_data = Result(result=result["result"])
+
+                    def print_line_1(sp: int, line_1: List[str]) -> None:
+                        if sp <= nr_splittimes:
+                            running_time = result["result"].extensions.get(
+                                "running_time", result["result"].time
+                            )
+
+                            pre(
+                                pdf=doc,
+                                t1=str(get(result, "rank"))
+                                if not get(result, "not_competing")
+                                else "AK",
+                                t2=get(result, "last_name")
+                                + " "
+                                + get(result, "first_name"),
+                                t3=format_time(running_time, result["result"].status),
+                            )
+                        else:
+                            doc.ln()
+                            pre(pdf=doc)
 
-                    for i in line_2:
-                        cell(w=10, h=None, txt=i, align="R")
+                        for i in line_1:
+                            cell(pdf=doc, w=10, h=None, txt=i, align="R")
 
-                def print_line_3(sp: int, line_3: List[str]) -> None:
-                    pdf.ln()
-                    pre()
+                    def print_line_2(sp: int, line_2: List[str]) -> None:
+                        if sp <= nr_splittimes:
+                            doc.ln()
+                            # first line: rank, lastname+firstname, time, splittimes
+                            pre(pdf=doc, t2=get(result, "club"))
+                        else:
+                            doc.ln()
+                            pre(pdf=doc)
 
-                    for i in line_3:
-                        cell(w=10, h=None, txt=i, align="R")
+                        for i in line_2:
+                            cell(pdf=doc, w=10, h=None, txt=i, align="R")
 
-                line_1 = []
-                line_2 = []
-                line_3 = []
-                for i, j, k in result_data.next():
-                    line_1.append(i)
-                    line_2.append(j)
-                    line_3.append(k)
-                    sp += 1
-                    if sp % nr_splittimes == 0:
+                    def print_line_3(sp: int, line_3: List[str]) -> None:
+                        doc.ln()
+                        pre(pdf=doc)
+
+                        for i in line_3:
+                            cell(pdf=doc, w=10, h=None, txt=i, align="R")
+
+                    line_1 = []
+                    line_2 = []
+                    line_3 = []
+                    for i, j, k in result_data.next():
+                        line_1.append(i)
+                        line_2.append(j)
+                        line_3.append(k)
+                        sp += 1
+                        if sp % nr_splittimes == 0:
+                            print_line_1(sp=sp, line_1=line_1)
+                            print_line_2(sp=sp, line_2=line_2)
+                            if not standard:
+                                print_line_3(sp=sp, line_3=line_3)
+                            line_1 = []
+                            line_2 = []
+                            line_3 = []
+                    if line_1 != []:
                         print_line_1(sp=sp, line_1=line_1)
                         print_line_2(sp=sp, line_2=line_2)
                         if not standard:
                             print_line_3(sp=sp, line_3=line_3)
-                        line_1 = []
-                        line_2 = []
-                        line_3 = []
-                if line_1 != []:
-                    print_line_1(sp=sp, line_1=line_1)
-                    print_line_2(sp=sp, line_2=line_2)
-                    if not standard:
-                        print_line_3(sp=sp, line_3=line_3)
-                pdf.ln()
+                    doc.ln()
+
+                # add a separator line (1/2 height of a line)
+                pdf.ln(0.5 * 0.3515 * 8)
 
     return bytes(pdf.output())
```

### Comparing `ooresults-0.2.4/ooresults/plugins/__init__.py` & `ooresults-0.2.5/ooresults/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/imports/entries/__init__.py` & `ooresults-0.2.5/ooresults/plugins/imports/entries/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/imports/entries/text.py` & `ooresults-0.2.5/ooresults/plugins/imports/entries/text.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/iof_class_list.py` & `ooresults-0.2.5/ooresults/plugins/iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/iof_competitor_list.py` & `ooresults-0.2.5/ooresults/plugins/iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/iof_course_data.py` & `ooresults-0.2.5/ooresults/plugins/iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/iof_entry_list.py` & `ooresults-0.2.5/ooresults/plugins/iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/iof_result_list.py` & `ooresults-0.2.5/ooresults/plugins/iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/oe12.py` & `ooresults-0.2.5/ooresults/plugins/oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/plugins/oe2003.py` & `ooresults-0.2.5/ooresults/plugins/oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/reader.py` & `ooresults-0.2.5/ooresults/reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/__init__.py` & `ooresults-0.2.5/ooresults/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/class_params.py` & `ooresults-0.2.5/ooresults/repo/class_params.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/repo.py` & `ooresults-0.2.5/ooresults/repo/repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/result_type.py` & `ooresults-0.2.5/ooresults/repo/result_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/series_type.py` & `ooresults-0.2.5/ooresults/repo/series_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/sqlite_repo.py` & `ooresults-0.2.5/ooresults/repo/sqlite_repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/start_type.py` & `ooresults-0.2.5/ooresults/repo/start_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/update/__init__.py` & `ooresults-0.2.5/ooresults/repo/update/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/update/update_008.py` & `ooresults-0.2.5/ooresults/repo/update/update_008.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/repo/update/update_tables.py` & `ooresults-0.2.5/ooresults/repo/update/update_tables.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/schema/IOF.xsd` & `ooresults-0.2.5/ooresults/schema/IOF.xsd`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/schema/cardreader_log.json` & `ooresults-0.2.5/ooresults/schema/cardreader_log.json`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/server.py` & `ooresults-0.2.5/ooresults/server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/set_legacy_mode.py` & `ooresults-0.2.5/ooresults/set_legacy_mode.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/static/style-tab.css` & `ooresults-0.2.5/ooresults/static/style-tab.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/static/style.css` & `ooresults-0.2.5/ooresults/static/style.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/static/w3.js` & `ooresults-0.2.5/ooresults/static/w3.js`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_class.html` & `ooresults-0.2.5/ooresults/templates/add_class.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_club.html` & `ooresults-0.2.5/ooresults/templates/add_club.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_competitor.html` & `ooresults-0.2.5/ooresults/templates/add_competitor.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_course.html` & `ooresults-0.2.5/ooresults/templates/add_course.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_entry.html` & `ooresults-0.2.5/ooresults/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_entry_competitors.html` & `ooresults-0.2.5/ooresults/templates/add_entry_competitors.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_entry_result.html` & `ooresults-0.2.5/ooresults/templates/add_entry_result.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/add_event.html` & `ooresults-0.2.5/ooresults/templates/add_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/classes_tab_content.html` & `ooresults-0.2.5/ooresults/templates/classes_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/classes_table.html` & `ooresults-0.2.5/ooresults/templates/classes_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/clubs_tab_content.html` & `ooresults-0.2.5/ooresults/templates/clubs_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/competitors_tab_content.html` & `ooresults-0.2.5/ooresults/templates/competitors_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/competitors_table.html` & `ooresults-0.2.5/ooresults/templates/competitors_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/courses_tab_content.html` & `ooresults-0.2.5/ooresults/templates/courses_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/courses_table.html` & `ooresults-0.2.5/ooresults/templates/courses_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/demo_reader.html` & `ooresults-0.2.5/ooresults/templates/demo_reader.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/entries_tab_content.html` & `ooresults-0.2.5/ooresults/templates/entries_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/entries_table.html` & `ooresults-0.2.5/ooresults/templates/entries_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/events_tab_content.html` & `ooresults-0.2.5/ooresults/templates/events_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/events_table.html` & `ooresults-0.2.5/ooresults/templates/events_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/main.html` & `ooresults-0.2.5/ooresults/templates/main.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/results_tab_content.html` & `ooresults-0.2.5/ooresults/templates/results_tab_content.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
 <!-- Tab content -->
 <div id="Results" class="tabcontent">
   <div class="actions">
     <!-- Trigger/Open The Modal -->
     <button id="res.myBtnReload" onclick="res_update()">Reload</button>
     <button id="res.myBtnPdfResult" onclick="res_myPdfResult()">Print results ...</button>
-    <button id="res.myBtnPdfSplittimes" onclick="res_myPdfSplittimes()">Print splittimes ...</button>
+    <button id="res.myBtnPdfSplittimes" onclick="res_myPdfSplittimes()">Print split times ...</button>
   </div>
 
   <div id="res.results" class="data">
     $:results
   </div>
 
   <!-- The Modal -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 $def with (results)
- Reload Print results ... Print splittimes ...
+ Reload Print results ... Print split times ...
 $:results
 ×
 ⁰ Include not started competitors
 Create PDF Cancel
 ×
 ⁰ Landscape (page orientation)
 Create PDF Cancel
```

### Comparing `ooresults-0.2.4/ooresults/templates/results_table.html` & `ooresults-0.2.5/ooresults/templates/results_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/root.html` & `ooresults-0.2.5/ooresults/templates/root.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/select_event.html` & `ooresults-0.2.5/ooresults/templates/select_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/series_settings.html` & `ooresults-0.2.5/ooresults/templates/series_settings.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/series_tab_content.html` & `ooresults-0.2.5/ooresults/templates/series_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/series_table.html` & `ooresults-0.2.5/ooresults/templates/series_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/si/si1_data.html` & `ooresults-0.2.5/ooresults/templates/si/si1_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/si/si1_page.html` & `ooresults-0.2.5/ooresults/templates/si/si1_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/si/si2_data.html` & `ooresults-0.2.5/ooresults/templates/si/si2_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/templates/si/si2_page.html` & `ooresults-0.2.5/ooresults/templates/si/si2_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/user.py` & `ooresults-0.2.5/ooresults/user.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/utils/__init__.py` & `ooresults-0.2.5/ooresults/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/utils/globals.py` & `ooresults-0.2.5/ooresults/utils/globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/websocket_server/__init__.py` & `ooresults-0.2.5/ooresults/websocket_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/websocket_server/si.py` & `ooresults-0.2.5/ooresults/websocket_server/si.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults/websocket_server/websocket_handler.py` & `ooresults-0.2.5/ooresults/websocket_server/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/ooresults.egg-info/PKG-INFO` & `ooresults-0.2.5/ooresults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.4
+Version: 0.2.5
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.4/ooresults.egg-info/SOURCES.txt` & `ooresults-0.2.5/ooresults.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/pyproject.toml` & `ooresults-0.2.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooresults"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   {name="Rainer Garus"},
 ]
 description = "A software for the evaluation of the results of orienteering events"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `ooresults-0.2.4/setup.cfg` & `ooresults-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/__init__.py` & `ooresults-0.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/competitor.py` & `ooresults-0.2.5/tests/competitor.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/entry.py` & `ooresults-0.2.5/tests/entry.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/__init__.py` & `ooresults-0.2.5/tests/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/test_build_series_result.py` & `ooresults-0.2.5/tests/model/test_build_series_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/test_courses.py` & `ooresults-0.2.5/tests/model/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/test_event_class_results.py` & `ooresults-0.2.5/tests/model/test_event_class_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/test_parse_cardreader_log.py` & `ooresults-0.2.5/tests/model/test_parse_cardreader_log.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/model/test_store_cardreader_result.py` & `ooresults-0.2.5/tests/model/test_store_cardreader_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_export_competitors_oe2003.py` & `ooresults-0.2.5/tests/plugins/test_export_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_import_competitors_oe2003.py` & `ooresults-0.2.5/tests/plugins/test_import_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_plugin_iof_class_list.py` & `ooresults-0.2.5/tests/plugins/test_plugin_iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_plugin_iof_competitor_list.py` & `ooresults-0.2.5/tests/plugins/test_plugin_iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_plugin_iof_course_data.py` & `ooresults-0.2.5/tests/plugins/test_plugin_iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_plugin_iof_entry_list.py` & `ooresults-0.2.5/tests/plugins/test_plugin_iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/plugins/test_plugin_iof_result_list.py` & `ooresults-0.2.5/tests/plugins/test_plugin_iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/__init__.py` & `ooresults-0.2.5/tests/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_classes.py` & `ooresults-0.2.5/tests/repo/test_classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_clubs.py` & `ooresults-0.2.5/tests/repo/test_clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_competitors.py` & `ooresults-0.2.5/tests/repo/test_competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_courses.py` & `ooresults-0.2.5/tests/repo/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_entries.py` & `ooresults-0.2.5/tests/repo/test_entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_events.py` & `ooresults-0.2.5/tests/repo/test_events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/repo/test_settings.py` & `ooresults-0.2.5/tests/repo/test_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_compute_result_net.py` & `ooresults-0.2.5/tests/test_compute_result_net.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_compute_result_score.py` & `ooresults-0.2.5/tests/test_compute_result_score.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_compute_result_standard.py` & `ooresults-0.2.5/tests/test_compute_result_standard.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_configuration.py` & `ooresults-0.2.5/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_globals.py` & `ooresults-0.2.5/tests/test_globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_handicap.py` & `ooresults-0.2.5/tests/test_handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_ranking.py` & `ooresults-0.2.5/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_series.py` & `ooresults-0.2.5/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.4/tests/test_user.py` & `ooresults-0.2.5/tests/test_user.py`

 * *Files identical despite different names*

