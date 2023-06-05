# Comparing `tmp/SALTISE_course_flow-0.8.4.tar.gz` & `tmp/SALTISE_course_flow-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SALTISE_course_flow-0.8.4.tar", last modified: Thu Jun  1 03:42:26 2023, max compression
+gzip compressed data, was "SALTISE_course_flow-0.8.5.tar", last modified: Mon Jun  5 03:24:28 2023, max compression
```

## Comparing `SALTISE_course_flow-0.8.4.tar` & `SALTISE_course_flow-0.8.5.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.442291 SALTISE_course_flow-0.8.4/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    11538 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/LICENSE.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      490 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.4/MANIFEST.in
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      808 2023-06-01 03:42:26.442291 SALTISE_course_flow-0.8.4/PKG-INFO
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1577 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/README.md
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.302289 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      808 2023-06-01 03:42:26.000000 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/PKG-INFO
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    19806 2023-06-01 03:42:26.000000 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/SOURCES.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        1 2023-06-01 03:42:26.000000 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/dependency_links.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      210 2023-06-01 03:42:26.000000 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/requires.txt
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       12 2023-06-01 03:42:26.000000 SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/top_level.txt
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.310289 SALTISE_course_flow-0.8.4/course_flow/
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      179 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/__init__.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1439 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/admin.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5545 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/analytics.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      264 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.4/course_flow/apps.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      523 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/asgi.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2121 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/celery.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1004 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/checks.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3758 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/consumers.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1584 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/context_processors.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    25874 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/decorators.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    26283 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/export_functions.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      588 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/forms.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     7897 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/import_functions.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.294289 SALTISE_course_flow-0.8.4/course_flow/locale/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.294289 SALTISE_course_flow-0.8.4/course_flow/locale/fr/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.314289 SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    15049 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    24934 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    24855 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    71639 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/djangojs.po
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      520 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.4/course_flow/lti.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.294289 SALTISE_course_flow-0.8.4/course_flow/management/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.314289 SALTISE_course_flow-0.8.4/course_flow/management/commands/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1996 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/management/commands/clear_orphaned_objects.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1256 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/management/commands/create_base_disciplines.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1083 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/management/commands/create_instances.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    35387 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.4/course_flow/management/commands/create_saltise_strategies.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.338290 SALTISE_course_flow-0.8.4/course_flow/migrations/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    39023 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0001_initial.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      658 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0047_auto_20210315_1952.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      565 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0048_auto_20210315_2023.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1348 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0049_projectfavourite.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      456 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0050_workflow_disciplines.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      459 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0051_outcome_disciplines.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2329 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0052_outcomefavourite_workflowfavourite.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3399 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0053_auto_20210318_2131.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     4650 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0054_auto_20210331_1748.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      309 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0055_delete_outcomeworkflow.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1765 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0056_auto_20210427_2228.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      920 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0057_auto_20210505_1753.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2106 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0058_auto_20210506_2247.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1130 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0059_auto_20210621_2154.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      446 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0060_auto_20210621_2207.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      411 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0061_outcomehorizontallink_degree.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1094 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0062_auto_20210721_1733.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3144 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0063_auto_20210728_2238.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      771 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0064_auto_20210810_2256.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2440 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0065_auto_20210818_2256.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      990 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0066_auto_20210827_2042.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      416 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0067_customterm_translation_plural.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      423 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0068_workflow_code.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1484 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0069_auto_20210909_2140.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2109 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0070_auto_20210920_2129.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      402 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0071_workflow_edit_count.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1169 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0072_auto_20211115_2237.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      395 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0073_nodelink_deleted.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1483 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0074_auto_20211210_1907.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1492 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0075_auto_20211217_2053.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1368 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0076_auto_20211217_2107.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      573 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0077_workflow_condensed.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1522 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0078_auto_20220112_2255.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2360 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0079_auto_20220228_1845.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1141 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0080_auto_20220308_1956.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      362 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0081_auto_20220321_1802.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      811 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0082_auto_20220321_1804.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      375 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0083_auto_20220322_2153.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      393 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0084_week_is_dropped.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      408 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0085_nodelink_text_position.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      403 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0086_workflow_static_view.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      382 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0087_auto_20220704_1828.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1193 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0088_liveproject.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1066 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0089_auto_20220930_1527.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      463 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0090_project_hash.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      520 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0091_auto_20220930_1948.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      467 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0092_auto_20220930_1948.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1655 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0093_liveprojectuser.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3338 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0094_liveassignment_userassignment.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      980 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0095_updatenotification.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      417 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0096_auto_20221118_1539.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      403 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0097_userassignment_completed_on.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1848 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0098_auto_20230118_1413.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      755 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0099_alter_courseflowuser_user.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      497 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0100_courseflowuser_notifications.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      595 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0101_auto_20230118_2202.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1930 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0102_auto_20230205_1612.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      542 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0103_auto_20230205_1626.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      375 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0104_rename_author_temp_workflow_author.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2416 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0105_auto_20230205_1753.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      398 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0106_project_is_strategy.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3153 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0107_alter_objectpermission_content_type.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      698 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0108_alter_objectpermission_content_type.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      474 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0109_objectpermission_last_viewed.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3026 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0110_alter_favourite_content_type.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      684 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0111_alter_favourite_content_type.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      420 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/0112_column_icon.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/migrations/__init__.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    78687 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/models.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     7007 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/redux_actions.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      225 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/routing.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    60845 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/serializers.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7337 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/settings.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.294289 SALTISE_course_flow-0.8.4/course_flow/static/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.294289 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.342290 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    28162 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/base_style.css
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   230832 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/preact_styles.css
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    43175 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/workflow_styles.css
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.350290 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       77 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/CourseFlow Thumbnail.svg:Zone.Identifier
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2597 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/CourseFlow_Thumbnail.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      277 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/add-square-button.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5251 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/classroom-blue.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5264 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/classroom.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3235 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/courseflow-favicon.png
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3577 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/crowd-of-users.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      299 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/file_copy-24px.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1660 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/home-24px.svg
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.410291 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12409 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/activity.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      277 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add-square-button.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5541 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2815 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2969 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new_blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2437 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new_white.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13249 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13242 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person_black.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13472 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person_grey.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13100 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/analyze.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2530 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowdown.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2533 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowright.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2555 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowright_white.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16780 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/artifact.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4393 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/assessment.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3302 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/assignment.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12608 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/attributeindicator.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3898 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/case-studies.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3295 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/check.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7803 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/chem.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    18292 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/class.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3211 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/close.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6354 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/collapse.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3069 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/comment.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2634 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/comment_new.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12590 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/competency.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7014 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/copy.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12580 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/course.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13738 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/create.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4262 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/create_new_child.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3614 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/createchild.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16539 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/curation.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2498 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/dashed.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    18010 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/debate.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13280 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/decision.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3791 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/delrect.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14421 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/design.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12710 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/discuss.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5495 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/distributed-problem-solving.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3429 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/download.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2540 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/droptriangledown.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2538 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/droptriangleup.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3245 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3338 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate_checked.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3374 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate_clipboard.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4474 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2838 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit_pencil.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2998 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit_pencil_blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12603 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/elementofcompetency.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2825 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/enterlinked.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7949 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/exam.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5286 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/exercise.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6364 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/expand.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17081 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/experiment.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12042 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/explore.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12317 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/favourite.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      299 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/file_copy-24px.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3787 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/gallery-walk.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    20789 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/gears.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    11347 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/general.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2559 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/goback.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12598 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/graduateattribute.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16295 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/group.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12317 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/help.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14323 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/home.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1662 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/home_black.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14602 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/homework.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2926 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/import.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5122 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/info.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13165 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instrevaluate.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14274 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instruct.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14274 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instructor.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3231 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/jigsaw.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4211 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav_2.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3361 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav_white.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12602 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/learningobjective.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4888 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/lefticon.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15322 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/lesson.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2326 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/logo-courseflow-beta.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2103 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/logo-courseflow.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2438 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/minus.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13328 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/more_options.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2534 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/movedown.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4478 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/movehandle.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2532 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/moveup.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12320 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/no_favourite.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2805 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/nocheck.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4841 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/nodebar.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4428 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/one-minute-paper.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15910 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/ooci.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    43171 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/open_basic.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14656 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/orchestration.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2796 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/other-strat.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14325 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/other.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5753 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/outcomes_blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2989 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/page_view.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      451 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/pageview-24px.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3369 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peer-assessment.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3697 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peer-instruction.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17082 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peerreview.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/pencil-blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3320 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/pin.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14512 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/play.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2851 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/plus.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2861 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/plusblack.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2868 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/port.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12520 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/practice.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15736 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/present.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17218 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/problem.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17732 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/process.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12582 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/program.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3503 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/published.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3565 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/puzzle.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12723 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/quiz.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15642 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/reading.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/reflective-writing.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13759 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/research.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3315 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/restore.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3350 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/restore_blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3469 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/return_to_project.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2524 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/returnimg.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4876 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/righticon.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/rubbish-bin-delete-button.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2710 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/rubbish.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15199 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/science.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5166 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/settings.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5522 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/show_legend.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3151 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/solid_check.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14348 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/solo.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3170 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/spectrum.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3093 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/strategy.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3483 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/strategy_blue.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    21373 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/students.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8298 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/target.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6843 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/test.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3104 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/text.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6753 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/toolkit.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5038 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/two-stage-exam.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3791 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/unassign.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2750 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/upload.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3370 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/validate.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3807 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/validationerror.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4188 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/view.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4472 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/view_none.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3812 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/warningcheck.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5777 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstyle.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4793 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstyleparts.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3253 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstylesimple.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6263 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/wflink.svg
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13944 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/write.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      313 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/info-24px.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      311 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/info-green.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5387 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/logo-courseflow.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      146 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/logo-courseflow.svg:Zone.Identifier
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1844 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/multiple-users-silhouette-blue.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1845 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/multiple-users-silhouette.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      451 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/pageview-24px.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      460 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/pageview-grey.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/pencil-blue.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      313 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/pencil.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      223 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/reorder-option (1).svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      214 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/reorder-option-blue.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/rubbish-bin-delete-button.svg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5364 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/saltise_logo.svg
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.430291 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    32898 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/AlignmentView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4771 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ColumnView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1977 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ColumnWorkflowView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16256 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ComparisonView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    40345 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/CompetencyMatrixView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    65915 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ComponentJSON.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3806 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ConnectedUsers.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15549 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Constants.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4499 2022-10-14 03:15:36.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ExportMenu.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14862 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/FindState.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7692 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/GridView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2209 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ImportMenu.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    30668 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Library.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    28227 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/LiveAssignmentView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    29021 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/LiveProjectView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    48094 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/MenuComponents.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3692 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeLinkView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    19376 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1827 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeWeekView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    11829 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeEditView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8761 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeHorizontalLink.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12387 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeNode.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3987 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeOutcomeView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2764 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeTopView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    38015 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1648 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeWorkflowView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    37639 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/PostFunctions.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    78337 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Reducers.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15912 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ShareMenu.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2318 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Strategy.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6828 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/StudentManagement.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3998 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/TermView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13109 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WeekView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2884 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WeekWorkflowView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5909 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowLegend.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8215 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowOutcomeView.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    50517 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowView.js
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.430291 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/__tests__/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      570 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/__tests__/scripts.test.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      126 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/__tests__/setup.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    90666 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/course_flow.css
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2063 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-library.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   520312 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-library.min.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1834 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-live.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   590934 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-live.min.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    21880 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-wf-redux.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   894246 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-wf-redux.min.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    30960 2022-11-30 03:31:25.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      311 2022-11-30 03:31:25.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts.min.js
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      162 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/wdyr.js
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3721 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/tasks.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.298289 SALTISE_course_flow-0.8.4/course_flow/templates/
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.438291 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      762 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/activity_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    24131 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/base.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4141 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/comparison.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      756 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/course_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      826 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/courseflowuser_update.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1019 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/explore.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      929 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/favourites.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      976 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/home.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1685 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/import.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      923 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/library.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1040 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_assignment_update.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      660 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_project_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1130 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_project_update.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1336 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/my_live_projects.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1354 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/myprojects.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1353 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/myshared.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1353 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/mytemplates.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      733 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/outcome_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      757 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/program_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      743 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/project_create.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1325 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/project_update.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      932 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/saltise_admin.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2487 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/saltise_analytics.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      174 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/workflow_detail.html
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4367 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/workflow_update.html
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.438291 SALTISE_course_flow-0.8.4/course_flow/templatetags/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/templatetags/__init__.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    10366 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/templatetags/course_flow_templatetags.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1195 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/test_urls.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.438291 SALTISE_course_flow-0.8.4/course_flow/tests/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/__init__.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      892 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.4/course_flow/tests/conftest.py
-drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-01 03:42:26.442291 SALTISE_course_flow-0.8.4/course_flow/tests/models/
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/__init__.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   153772 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_functional.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    24559 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_json.json
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    38369 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_live_views.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   143274 2023-04-11 03:40:11.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_models.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      132 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_nodes.csv
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5632 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_nodes.xls
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      182 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_outcomes.csv
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5632 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/test_outcomes.xls
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1708 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.4/course_flow/tests/models/utils.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3550 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.4/course_flow/tests/test_decorators.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13580 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/urls.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    10623 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/utils.py
--rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   236479 2023-06-01 03:37:12.000000 SALTISE_course_flow-0.8.4/course_flow/views.py
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      727 2023-02-19 04:54:27.000000 SALTISE_course_flow-0.8.4/pyproject.toml
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      180 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/pytest.ini
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1078 2023-06-01 03:42:26.446291 SALTISE_course_flow-0.8.4/setup.cfg
--rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       38 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.4/setup.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.910483 SALTISE_course_flow-0.8.5/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    11538 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/LICENSE.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      490 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.5/MANIFEST.in
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      808 2023-06-05 03:24:28.910483 SALTISE_course_flow-0.8.5/PKG-INFO
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1577 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/README.md
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.786482 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      808 2023-06-05 03:24:28.000000 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/PKG-INFO
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    19806 2023-06-05 03:24:28.000000 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        1 2023-06-05 03:24:28.000000 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      210 2023-06-05 03:24:28.000000 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/requires.txt
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       12 2023-06-05 03:24:28.000000 SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/top_level.txt
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.798482 SALTISE_course_flow-0.8.5/course_flow/
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      179 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/__init__.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1439 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/admin.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5545 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/analytics.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      264 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.5/course_flow/apps.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      523 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/asgi.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2121 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/celery.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1004 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/checks.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3758 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/consumers.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1584 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/context_processors.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    25874 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/decorators.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    26283 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/export_functions.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      588 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/forms.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     7897 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/import_functions.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.782482 SALTISE_course_flow-0.8.5/course_flow/locale/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.782482 SALTISE_course_flow-0.8.5/course_flow/locale/fr/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.798482 SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    15049 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    24934 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    24855 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    71639 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      520 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.5/course_flow/lti.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.782482 SALTISE_course_flow-0.8.5/course_flow/management/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.802482 SALTISE_course_flow-0.8.5/course_flow/management/commands/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1996 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/management/commands/clear_orphaned_objects.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1256 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/management/commands/create_base_disciplines.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1083 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/management/commands/create_instances.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    35387 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.5/course_flow/management/commands/create_saltise_strategies.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.826482 SALTISE_course_flow-0.8.5/course_flow/migrations/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    39023 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0001_initial.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      658 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0047_auto_20210315_1952.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      565 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0048_auto_20210315_2023.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1348 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0049_projectfavourite.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      456 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0050_workflow_disciplines.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      459 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0051_outcome_disciplines.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2329 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0052_outcomefavourite_workflowfavourite.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3399 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0053_auto_20210318_2131.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     4650 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0054_auto_20210331_1748.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      309 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0055_delete_outcomeworkflow.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1765 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0056_auto_20210427_2228.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      920 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0057_auto_20210505_1753.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2106 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0058_auto_20210506_2247.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1130 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0059_auto_20210621_2154.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      446 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0060_auto_20210621_2207.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      411 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0061_outcomehorizontallink_degree.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1094 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0062_auto_20210721_1733.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3144 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0063_auto_20210728_2238.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      771 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0064_auto_20210810_2256.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2440 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0065_auto_20210818_2256.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      990 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0066_auto_20210827_2042.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      416 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0067_customterm_translation_plural.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      423 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0068_workflow_code.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1484 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0069_auto_20210909_2140.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2109 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0070_auto_20210920_2129.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      402 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0071_workflow_edit_count.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1169 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0072_auto_20211115_2237.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      395 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0073_nodelink_deleted.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1483 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0074_auto_20211210_1907.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1492 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0075_auto_20211217_2053.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1368 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0076_auto_20211217_2107.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      573 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0077_workflow_condensed.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1522 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0078_auto_20220112_2255.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2360 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0079_auto_20220228_1845.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1141 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0080_auto_20220308_1956.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      362 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0081_auto_20220321_1802.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      811 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0082_auto_20220321_1804.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      375 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0083_auto_20220322_2153.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      393 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0084_week_is_dropped.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      408 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0085_nodelink_text_position.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      403 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0086_workflow_static_view.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      382 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0087_auto_20220704_1828.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1193 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0088_liveproject.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1066 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0089_auto_20220930_1527.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      463 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0090_project_hash.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      520 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0091_auto_20220930_1948.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      467 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0092_auto_20220930_1948.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1655 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0093_liveprojectuser.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3338 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0094_liveassignment_userassignment.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      980 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0095_updatenotification.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      417 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0096_auto_20221118_1539.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      403 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0097_userassignment_completed_on.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1848 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0098_auto_20230118_1413.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      755 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0099_alter_courseflowuser_user.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      497 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0100_courseflowuser_notifications.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      595 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0101_auto_20230118_2202.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1930 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0102_auto_20230205_1612.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      542 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0103_auto_20230205_1626.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      375 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0104_rename_author_temp_workflow_author.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2416 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0105_auto_20230205_1753.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      398 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0106_project_is_strategy.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3153 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0107_alter_objectpermission_content_type.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      698 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0108_alter_objectpermission_content_type.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      474 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0109_objectpermission_last_viewed.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3026 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0110_alter_favourite_content_type.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      684 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0111_alter_favourite_content_type.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      420 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/0112_column_icon.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/migrations/__init__.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    78687 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/models.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     7007 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/redux_actions.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      225 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/routing.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    60845 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/serializers.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7337 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/settings.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.782482 SALTISE_course_flow-0.8.5/course_flow/static/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.786482 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.826482 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    28162 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/base_style.css
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   230832 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/preact_styles.css
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    43175 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/workflow_styles.css
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.834482 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       77 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/CourseFlow Thumbnail.svg:Zone.Identifier
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     2597 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/CourseFlow_Thumbnail.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      277 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/add-square-button.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5251 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/classroom-blue.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5264 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/classroom.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3235 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/courseflow-favicon.png
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3577 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/crowd-of-users.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      299 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/file_copy-24px.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1660 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/home-24px.svg
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.886483 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12409 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/activity.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      277 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add-square-button.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5541 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2815 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2969 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new_blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2437 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new_white.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13249 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13242 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person_black.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13472 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person_grey.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13100 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/analyze.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2530 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowdown.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2533 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowright.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2555 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowright_white.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16780 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/artifact.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4393 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/assessment.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3302 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/assignment.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12608 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/attributeindicator.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3898 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/case-studies.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3295 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/check.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7803 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/chem.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    18292 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/class.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3211 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/close.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6354 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/collapse.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3069 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/comment.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2634 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/comment_new.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12590 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/competency.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7014 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/copy.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12580 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/course.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13738 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/create.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4262 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/create_new_child.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3614 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/createchild.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16539 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/curation.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2498 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/dashed.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    18010 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/debate.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13280 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/decision.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3791 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/delrect.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14421 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/design.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12710 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/discuss.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5495 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/distributed-problem-solving.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3429 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/download.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2540 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/droptriangledown.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2538 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/droptriangleup.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3245 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3338 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate_checked.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3374 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate_clipboard.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4474 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2838 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit_pencil.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2998 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit_pencil_blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12603 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/elementofcompetency.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2825 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/enterlinked.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7949 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/exam.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5286 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/exercise.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6364 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/expand.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17081 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/experiment.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12042 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/explore.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12317 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/favourite.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      299 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/file_copy-24px.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3787 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/gallery-walk.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    20789 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/gears.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    11347 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/general.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2559 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/goback.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12598 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/graduateattribute.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16295 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/group.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12317 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/help.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14323 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/home.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1662 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/home_black.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14602 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/homework.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2926 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/import.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5122 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/info.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13165 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instrevaluate.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14274 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instruct.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14274 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instructor.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3231 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/jigsaw.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4211 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav_2.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3361 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav_white.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12602 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/learningobjective.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4888 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/lefticon.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15322 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/lesson.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2326 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/logo-courseflow-beta.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2103 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/logo-courseflow.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2438 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/minus.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13328 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/more_options.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2534 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/movedown.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4478 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/movehandle.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2532 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/moveup.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12320 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/no_favourite.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2805 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/nocheck.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4841 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/nodebar.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4428 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/one-minute-paper.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15910 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/ooci.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    43171 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/open_basic.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14656 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/orchestration.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2796 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/other-strat.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14325 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/other.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5753 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/outcomes_blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2989 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/page_view.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      451 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/pageview-24px.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3369 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peer-assessment.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3697 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peer-instruction.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17082 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peerreview.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/pencil-blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3320 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/pin.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14512 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/play.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2851 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/plus.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2861 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/plusblack.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2868 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/port.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12520 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/practice.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15736 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/present.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17218 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/problem.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    17732 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/process.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12582 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/program.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3503 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/published.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3565 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/puzzle.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12723 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/quiz.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15642 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/reading.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/reflective-writing.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13759 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/research.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3315 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/restore.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3350 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/restore_blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3469 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/return_to_project.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2524 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/returnimg.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4876 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/righticon.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/rubbish-bin-delete-button.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2710 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/rubbish.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15199 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/science.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5166 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/settings.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5522 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/show_legend.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3151 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/solid_check.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14348 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/solo.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3170 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/spectrum.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3093 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/strategy.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3483 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/strategy_blue.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    21373 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/students.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8298 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/target.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6843 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/test.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3104 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/text.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6753 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/toolkit.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5038 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/two-stage-exam.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3791 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/unassign.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2750 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/upload.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3370 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/validate.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3807 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/validationerror.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4188 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/view.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4472 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/view_none.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3812 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/warningcheck.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5777 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstyle.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4793 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstyleparts.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3253 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstylesimple.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6263 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/wflink.svg
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13944 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/write.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      313 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/info-24px.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      311 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/info-green.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5387 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/logo-courseflow.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      146 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/logo-courseflow.svg:Zone.Identifier
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1844 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/multiple-users-silhouette-blue.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1845 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/multiple-users-silhouette.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      451 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/pageview-24px.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      460 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/pageview-grey.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      304 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/pencil-blue.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      313 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/pencil.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      223 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/reorder-option (1).svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      214 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/reorder-option-blue.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      241 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/rubbish-bin-delete-button.svg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     5364 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/saltise_logo.svg
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.902483 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    32898 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/AlignmentView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4771 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ColumnView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1977 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ColumnWorkflowView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    16256 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ComparisonView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    40345 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/CompetencyMatrixView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    65915 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ComponentJSON.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3806 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ConnectedUsers.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15549 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Constants.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4499 2022-10-14 03:15:36.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ExportMenu.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    14862 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/FindState.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     7692 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/GridView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2209 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ImportMenu.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    30668 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Library.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    28227 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/LiveAssignmentView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    29021 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/LiveProjectView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    48094 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/MenuComponents.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3692 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeLinkView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    19376 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1827 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeWeekView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    11829 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeEditView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8761 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeHorizontalLink.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    12387 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeNode.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3987 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeOutcomeView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2764 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeTopView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    38015 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1648 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeWorkflowView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    37639 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/PostFunctions.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    78337 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Reducers.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    15912 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ShareMenu.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2318 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Strategy.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     6828 2022-11-30 03:31:24.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/StudentManagement.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     3998 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/TermView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13109 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WeekView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2884 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WeekWorkflowView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5909 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowLegend.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     8215 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowOutcomeView.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    50517 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowView.js
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.902483 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/__tests__/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      570 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/__tests__/scripts.test.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      126 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/__tests__/setup.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)    90666 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/course_flow.css
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2063 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-library.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   520312 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-library.min.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1834 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-live.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   590934 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-live.min.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    21880 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-wf-redux.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   894246 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-wf-redux.min.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    30960 2022-11-30 03:31:25.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      311 2022-11-30 03:31:25.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts.min.js
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      162 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/wdyr.js
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3721 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/tasks.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.786482 SALTISE_course_flow-0.8.5/course_flow/templates/
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.906483 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      762 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/activity_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    24131 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/base.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4141 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/comparison.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      756 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/course_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      826 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/courseflowuser_update.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1019 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/explore.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      929 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/favourites.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      976 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/home.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1685 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/import.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      923 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/library.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1040 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_assignment_update.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      660 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_project_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1130 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_project_update.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1336 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/my_live_projects.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1354 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/myprojects.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1353 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/myshared.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1353 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/mytemplates.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      733 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/outcome_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      757 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/program_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      743 2022-11-06 04:13:26.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/project_create.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     1325 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/project_update.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      932 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/saltise_admin.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     2487 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/saltise_analytics.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      174 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/workflow_detail.html
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     4367 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/workflow_update.html
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.906483 SALTISE_course_flow-0.8.5/course_flow/templatetags/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/templatetags/__init__.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    10366 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/templatetags/course_flow_templatetags.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1195 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/test_urls.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.910483 SALTISE_course_flow-0.8.5/course_flow/tests/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/__init__.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      892 2022-10-14 02:12:19.000000 SALTISE_course_flow-0.8.5/course_flow/tests/conftest.py
+drwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2023-06-05 03:24:28.910483 SALTISE_course_flow-0.8.5/course_flow/tests/models/
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)        0 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/__init__.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   153772 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_functional.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    24559 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_json.json
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    38369 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_live_views.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   143274 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_models.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      132 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_nodes.csv
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5632 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_nodes.xls
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)      182 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_outcomes.csv
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)     5632 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/test_outcomes.xls
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1708 2023-02-19 04:53:18.000000 SALTISE_course_flow-0.8.5/course_flow/tests/models/utils.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     3550 2023-01-13 02:04:14.000000 SALTISE_course_flow-0.8.5/course_flow/tests/test_decorators.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    13580 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/urls.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)    10623 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/utils.py
+-rwxrwxr-x   0 sbhatnagar  (1000) sbhatnagar  (1000)   236479 2023-06-05 03:15:05.000000 SALTISE_course_flow-0.8.5/course_flow/views.py
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      727 2023-02-19 04:54:27.000000 SALTISE_course_flow-0.8.5/pyproject.toml
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)      180 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/pytest.ini
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)     1078 2023-06-05 03:24:28.914483 SALTISE_course_flow-0.8.5/setup.cfg
+-rw-rw-r--   0 sbhatnagar  (1000) sbhatnagar  (1000)       38 2022-07-06 16:14:20.000000 SALTISE_course_flow-0.8.5/setup.py
```

### Comparing `SALTISE_course_flow-0.8.4/LICENSE.txt` & `SALTISE_course_flow-0.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/PKG-INFO` & `SALTISE_course_flow-0.8.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SALTISE_course_flow
-Version: 0.8.4
+Version: 0.8.5
 Summary: CourseFlow
 Home-page: https://www.example.com/
 Author: Arthur Ayestas Hilgert, Jeremie Choquette
 Author-email: aahilgert@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `SALTISE_course_flow-0.8.4/README.md` & `SALTISE_course_flow-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/PKG-INFO` & `SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SALTISE-course-flow
-Version: 0.8.4
+Version: 0.8.5
 Summary: CourseFlow
 Home-page: https://www.example.com/
 Author: Arthur Ayestas Hilgert, Jeremie Choquette
 Author-email: aahilgert@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `SALTISE_course_flow-0.8.4/SALTISE_course_flow.egg-info/SOURCES.txt` & `SALTISE_course_flow-0.8.5/SALTISE_course_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/admin.py` & `SALTISE_course_flow-0.8.5/course_flow/admin.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/analytics.py` & `SALTISE_course_flow-0.8.5/course_flow/analytics.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/asgi.py` & `SALTISE_course_flow-0.8.5/course_flow/asgi.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/celery.py` & `SALTISE_course_flow-0.8.5/course_flow/celery.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/checks.py` & `SALTISE_course_flow-0.8.5/course_flow/checks.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/consumers.py` & `SALTISE_course_flow-0.8.5/course_flow/consumers.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/context_processors.py` & `SALTISE_course_flow-0.8.5/course_flow/context_processors.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/decorators.py` & `SALTISE_course_flow-0.8.5/course_flow/decorators.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/export_functions.py` & `SALTISE_course_flow-0.8.5/course_flow/export_functions.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/forms.py` & `SALTISE_course_flow-0.8.5/course_flow/forms.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/import_functions.py` & `SALTISE_course_flow-0.8.5/course_flow/import_functions.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/django.mo` & `SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/django.po` & `SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/djangojs.mo` & `SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/locale/fr/LC_MESSAGES/djangojs.po` & `SALTISE_course_flow-0.8.5/course_flow/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/lti.py` & `SALTISE_course_flow-0.8.5/course_flow/lti.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/management/commands/clear_orphaned_objects.py` & `SALTISE_course_flow-0.8.5/course_flow/management/commands/clear_orphaned_objects.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/management/commands/create_base_disciplines.py` & `SALTISE_course_flow-0.8.5/course_flow/management/commands/create_base_disciplines.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/management/commands/create_instances.py` & `SALTISE_course_flow-0.8.5/course_flow/management/commands/create_instances.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/management/commands/create_saltise_strategies.py` & `SALTISE_course_flow-0.8.5/course_flow/management/commands/create_saltise_strategies.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0001_initial.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0047_auto_20210315_1952.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0047_auto_20210315_1952.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0048_auto_20210315_2023.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0048_auto_20210315_2023.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0049_projectfavourite.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0049_projectfavourite.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0052_outcomefavourite_workflowfavourite.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0052_outcomefavourite_workflowfavourite.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0053_auto_20210318_2131.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0053_auto_20210318_2131.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0054_auto_20210331_1748.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0054_auto_20210331_1748.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0056_auto_20210427_2228.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0056_auto_20210427_2228.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0057_auto_20210505_1753.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0057_auto_20210505_1753.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0058_auto_20210506_2247.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0058_auto_20210506_2247.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0059_auto_20210621_2154.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0059_auto_20210621_2154.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0062_auto_20210721_1733.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0062_auto_20210721_1733.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0063_auto_20210728_2238.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0063_auto_20210728_2238.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0064_auto_20210810_2256.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0064_auto_20210810_2256.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0065_auto_20210818_2256.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0065_auto_20210818_2256.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0066_auto_20210827_2042.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0066_auto_20210827_2042.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0069_auto_20210909_2140.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0069_auto_20210909_2140.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0070_auto_20210920_2129.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0070_auto_20210920_2129.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0072_auto_20211115_2237.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0072_auto_20211115_2237.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0074_auto_20211210_1907.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0074_auto_20211210_1907.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0075_auto_20211217_2053.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0075_auto_20211217_2053.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0076_auto_20211217_2107.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0076_auto_20211217_2107.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0077_workflow_condensed.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0077_workflow_condensed.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0078_auto_20220112_2255.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0078_auto_20220112_2255.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0079_auto_20220228_1845.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0079_auto_20220228_1845.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0080_auto_20220308_1956.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0080_auto_20220308_1956.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0082_auto_20220321_1804.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0082_auto_20220321_1804.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0088_liveproject.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0088_liveproject.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0089_auto_20220930_1527.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0089_auto_20220930_1527.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0091_auto_20220930_1948.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0091_auto_20220930_1948.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0093_liveprojectuser.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0093_liveprojectuser.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0094_liveassignment_userassignment.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0094_liveassignment_userassignment.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0095_updatenotification.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0095_updatenotification.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0098_auto_20230118_1413.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0098_auto_20230118_1413.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0099_alter_courseflowuser_user.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0099_alter_courseflowuser_user.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0101_auto_20230118_2202.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0101_auto_20230118_2202.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0102_auto_20230205_1612.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0102_auto_20230205_1612.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0103_auto_20230205_1626.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0103_auto_20230205_1626.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0105_auto_20230205_1753.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0105_auto_20230205_1753.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0107_alter_objectpermission_content_type.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0107_alter_objectpermission_content_type.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0108_alter_objectpermission_content_type.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0108_alter_objectpermission_content_type.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0110_alter_favourite_content_type.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0110_alter_favourite_content_type.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/migrations/0111_alter_favourite_content_type.py` & `SALTISE_course_flow-0.8.5/course_flow/migrations/0111_alter_favourite_content_type.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/models.py` & `SALTISE_course_flow-0.8.5/course_flow/models.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/redux_actions.py` & `SALTISE_course_flow-0.8.5/course_flow/redux_actions.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/serializers.py` & `SALTISE_course_flow-0.8.5/course_flow/serializers.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/settings.py` & `SALTISE_course_flow-0.8.5/course_flow/settings.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/base_style.css` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/base_style.css`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/preact_styles.css` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/preact_styles.css`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/css/workflow_styles.css` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/css/workflow_styles.css`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/CourseFlow_Thumbnail.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/CourseFlow_Thumbnail.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/classroom-blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/classroom-blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/classroom.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/classroom.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/courseflow-favicon.png` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/courseflow-favicon.png`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/crowd-of-users.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/crowd-of-users.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/home-24px.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/home-24px.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/activity.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/activity.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new_blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new_blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_new_white.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_new_white.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person_black.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person_black.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/add_person_grey.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/add_person_grey.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/analyze.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/analyze.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowdown.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowdown.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowright.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowright.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/arrowright_white.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/arrowright_white.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/artifact.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/artifact.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/assessment.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/assessment.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/assignment.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/assignment.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/attributeindicator.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/attributeindicator.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/case-studies.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/case-studies.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/check.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/check.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/chem.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/chem.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/class.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/class.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/close.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/close.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/collapse.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/collapse.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/comment.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/comment.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/comment_new.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/comment_new.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/competency.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/competency.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/copy.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/copy.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/course.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/course.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/create.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/create.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/create_new_child.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/create_new_child.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/createchild.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/createchild.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/curation.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/curation.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/dashed.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/dashed.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/debate.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/debate.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/decision.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/decision.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/delrect.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/delrect.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/design.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/design.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/discuss.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/discuss.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/distributed-problem-solving.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/distributed-problem-solving.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/download.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/download.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/droptriangledown.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/droptriangledown.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/droptriangleup.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/droptriangleup.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate_checked.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate_checked.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/duplicate_clipboard.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/duplicate_clipboard.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit_pencil.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit_pencil.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/edit_pencil_blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/edit_pencil_blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/elementofcompetency.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/elementofcompetency.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/enterlinked.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/enterlinked.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/exam.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/exam.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/exercise.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/exercise.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/expand.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/expand.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/experiment.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/experiment.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/explore.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/explore.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/favourite.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/favourite.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/gallery-walk.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/gallery-walk.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/gears.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/gears.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/general.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/general.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/goback.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/goback.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/graduateattribute.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/graduateattribute.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/group.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/group.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/help.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/help.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/home.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/home.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/home_black.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/home_black.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/homework.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/homework.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/import.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/import.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/info.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/info.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instrevaluate.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instrevaluate.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instruct.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instruct.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/instructor.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/instructor.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/jigsaw.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/jigsaw.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav_2.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav_2.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/layoutnav_white.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/layoutnav_white.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/learningobjective.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/learningobjective.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/lefticon.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/lefticon.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/lesson.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/lesson.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/logo-courseflow-beta.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/logo-courseflow-beta.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/logo-courseflow.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/logo-courseflow.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/minus.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/minus.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/more_options.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/more_options.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/movedown.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/movedown.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/movehandle.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/movehandle.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/moveup.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/moveup.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/no_favourite.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/no_favourite.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/nocheck.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/nocheck.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/nodebar.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/nodebar.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/one-minute-paper.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/one-minute-paper.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/ooci.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/ooci.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/open_basic.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/open_basic.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/orchestration.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/orchestration.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/other-strat.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/other-strat.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/other.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/other.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/outcomes_blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/outcomes_blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/page_view.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/page_view.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peer-assessment.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peer-assessment.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peer-instruction.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peer-instruction.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/peerreview.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/peerreview.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/pin.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/pin.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/play.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/play.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/plus.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/plus.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/plusblack.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/plusblack.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/port.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/port.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/practice.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/practice.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/present.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/present.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/problem.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/problem.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/process.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/process.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/program.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/program.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/published.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/published.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/puzzle.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/puzzle.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/quiz.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/quiz.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/reading.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/reading.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/reflective-writing.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/reflective-writing.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/research.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/research.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/restore.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/restore.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/restore_blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/restore_blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/return_to_project.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/return_to_project.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/returnimg.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/returnimg.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/righticon.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/righticon.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/rubbish.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/rubbish.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/science.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/science.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/settings.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/settings.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/show_legend.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/show_legend.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/solid_check.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/solid_check.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/solo.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/solo.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/spectrum.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/spectrum.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/strategy.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/strategy.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/strategy_blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/strategy_blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/students.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/students.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/target.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/target.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/test.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/test.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/text.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/text.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/toolkit.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/toolkit.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/two-stage-exam.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/two-stage-exam.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/unassign.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/unassign.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/upload.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/upload.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/validate.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/validate.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/validationerror.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/validationerror.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/view.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/view.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/view_none.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/view_none.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/warningcheck.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/warningcheck.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstyle.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstyle.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstyleparts.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstyleparts.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/weekstylesimple.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/weekstylesimple.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/wflink.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/wflink.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/images_svg/write.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/images_svg/write.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/logo-courseflow.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/logo-courseflow.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/multiple-users-silhouette-blue.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/multiple-users-silhouette-blue.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/multiple-users-silhouette.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/multiple-users-silhouette.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/img/saltise_logo.svg` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/img/saltise_logo.svg`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/AlignmentView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/AlignmentView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ColumnView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ColumnView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ColumnWorkflowView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ColumnWorkflowView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ComparisonView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ComparisonView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/CompetencyMatrixView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/CompetencyMatrixView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ComponentJSON.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ComponentJSON.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ConnectedUsers.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ConnectedUsers.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Constants.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Constants.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ExportMenu.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ExportMenu.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/FindState.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/FindState.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/GridView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/GridView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ImportMenu.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ImportMenu.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Library.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Library.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/LiveAssignmentView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/LiveAssignmentView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/LiveProjectView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/LiveProjectView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/MenuComponents.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/MenuComponents.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeLinkView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeLinkView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/NodeWeekView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/NodeWeekView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeEditView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeEditView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeHorizontalLink.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeHorizontalLink.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeNode.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeNode.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeOutcomeView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeOutcomeView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeTopView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeTopView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/OutcomeWorkflowView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/OutcomeWorkflowView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/PostFunctions.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/PostFunctions.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Reducers.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Reducers.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/ShareMenu.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/ShareMenu.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/Strategy.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/Strategy.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/StudentManagement.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/StudentManagement.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/TermView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/TermView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WeekView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WeekView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WeekWorkflowView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WeekWorkflowView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowLegend.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowLegend.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowOutcomeView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowOutcomeView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/WorkflowView.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/WorkflowView.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/__tests__/scripts.test.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/__tests__/scripts.test.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/course_flow.css` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/course_flow.css`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-library.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-library.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-library.min.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-library.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-live.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-live.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-live.min.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-live.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-wf-redux.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-wf-redux.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts-wf-redux.min.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts-wf-redux.min.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/static/course_flow/js/scripts.js` & `SALTISE_course_flow-0.8.5/course_flow/static/course_flow/js/scripts.js`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tasks.py` & `SALTISE_course_flow-0.8.5/course_flow/tasks.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/activity_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/activity_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/base.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/base.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/comparison.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/comparison.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/course_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/course_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/courseflowuser_update.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/courseflowuser_update.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/explore.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/explore.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/favourites.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/favourites.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/home.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/home.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/import.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/import.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/library.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/library.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_assignment_update.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_assignment_update.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_project_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_project_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/live_project_update.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/live_project_update.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/my_live_projects.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/my_live_projects.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/myprojects.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/myprojects.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/myshared.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/myshared.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/mytemplates.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/mytemplates.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/outcome_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/outcome_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/program_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/program_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/project_create.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/project_create.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/project_update.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/project_update.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/saltise_admin.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/saltise_admin.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/saltise_analytics.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/saltise_analytics.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templates/course_flow/workflow_update.html` & `SALTISE_course_flow-0.8.5/course_flow/templates/course_flow/workflow_update.html`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/templatetags/course_flow_templatetags.py` & `SALTISE_course_flow-0.8.5/course_flow/templatetags/course_flow_templatetags.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/test_urls.py` & `SALTISE_course_flow-0.8.5/course_flow/test_urls.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/conftest.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_functional.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_functional.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_json.json` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_json.json`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_live_views.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_live_views.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_models.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_nodes.xls` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_nodes.xls`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/test_outcomes.xls` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/test_outcomes.xls`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/models/utils.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/tests/test_decorators.py` & `SALTISE_course_flow-0.8.5/course_flow/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/urls.py` & `SALTISE_course_flow-0.8.5/course_flow/urls.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/utils.py` & `SALTISE_course_flow-0.8.5/course_flow/utils.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/course_flow/views.py` & `SALTISE_course_flow-0.8.5/course_flow/views.py`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/pyproject.toml` & `SALTISE_course_flow-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SALTISE_course_flow-0.8.4/setup.cfg` & `SALTISE_course_flow-0.8.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SALTISE_course_flow
-version = 0.8.4
+version = 0.8.5
 description = CourseFlow
 long_description = file: README.rst
 url = https://www.example.com/
 author = Arthur Ayestas Hilgert, Jeremie Choquette
 author_email = aahilgert@gmail.com
 license_files = LICENSE.txt
 classifiers =
```

