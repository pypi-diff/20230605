# Comparing `tmp/ultrasync-0.9.7.tar.gz` & `tmp/ultrasync-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultrasync-0.9.7.tar", last modified: Sat May  6 17:20:32 2023, max compression
+gzip compressed data, was "ultrasync-0.9.8.tar", last modified: Mon Jun  5 02:45:19 2023, max compression
```

## Comparing `ultrasync-0.9.7.tar` & `ultrasync-0.9.8.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.856993 ultrasync-0.9.7/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1090 2020-11-22 16:33:46.000000 ultrasync-0.9.7/LICENSE
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      191 2020-11-22 16:33:46.000000 ultrasync-0.9.7/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-05-06 17:20:32.856993 ultrasync-0.9.7/PKG-INFO
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6235 2021-09-20 21:40:13.000000 ultrasync-0.9.7/README.md
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       43 2020-11-22 16:33:46.000000 ultrasync-0.9.7/dev-requirements.txt
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       15 2020-11-22 16:33:46.000000 ultrasync-0.9.7/requirements.txt
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      335 2023-05-06 17:20:32.857993 ultrasync-0.9.7/setup.cfg
--rwxr-xr-x   0 l2g       (1000) l2g       (1000)     3031 2023-05-06 17:19:41.000000 ultrasync-0.9.7/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.830993 ultrasync-0.9.7/tests/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     5121 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/test_cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7424 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_106.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6360 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_comnav_0_108-zone-check.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6635 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_108.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4922 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_108_burglar_alarm_on.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     3873 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/test_config.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     4828 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/test_xgen8_bypass.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7289 2021-09-20 21:40:13.000000 ultrasync-0.9.7/tests/test_xgen8_nxg8zbo.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7984 2021-09-19 13:53:23.000000 ultrasync-0.9.7/tests/test_xgen_general.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     4590 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_zerowire_armed.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6543 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_zerowire_general.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/comnav/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.833993 ultrasync-0.9.7/tests/var/comnav/0.106/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1892 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    36123 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    21526 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1832 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.bank0.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       81 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.bank4.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.837993 ultrasync-0.9.7/tests/var/comnav/0.108/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1971 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    23023 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2793 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       98 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.839993 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1983 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    23026 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      447 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2791 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.841993 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2044 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      458 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2327 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       91 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/xgen/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.845993 ultrasync-0.9.7/tests/var/xgen/general/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1862 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    13088 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/seq.w.update.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18618 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      188 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2071 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zstate.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/xgen8/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.847993 ultrasync-0.9.7/tests/var/xgen8/bypass/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2217 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      326 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zonefunction.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2054 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.849993 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/seq.w.update.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      563 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2088 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zstate.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.824993 ultrasync-0.9.7/tests/var/zerowire/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.851993 ultrasync-0.9.7/tests/var/zerowire/armed/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      165 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2582 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.852993 ultrasync-0.9.7/tests/var/zerowire/general/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      160 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/zerowire/general/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/zerowire/general/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2574 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.855993 ultrasync-0.9.7/ultrasync/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1793 2023-05-06 17:19:51.000000 ultrasync-0.9.7/ultrasync/__init__.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     8954 2022-07-01 13:18:56.000000 ultrasync-0.9.7/ultrasync/cli.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     8351 2021-09-20 21:40:13.000000 ultrasync-0.9.7/ultrasync/common.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6747 2021-09-12 19:13:27.000000 ultrasync-0.9.7/ultrasync/config.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2020-12-06 19:13:13.000000 ultrasync-0.9.7/ultrasync/logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    83078 2023-05-06 17:19:29.000000 ultrasync-0.9.7/ultrasync/main.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.856993 ultrasync-0.9.7/ultrasync.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       50 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/top_level.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.755961 ultrasync-0.9.8/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1090 2023-06-05 02:41:15.000000 ultrasync-0.9.8/LICENSE
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      191 2023-06-05 02:41:15.000000 ultrasync-0.9.8/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7188 2023-06-05 02:45:19.755961 ultrasync-0.9.8/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6235 2023-06-05 02:41:15.000000 ultrasync-0.9.8/README.md
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       43 2023-06-05 02:41:15.000000 ultrasync-0.9.8/dev-requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-06-05 02:41:15.000000 ultrasync-0.9.8/requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      335 2023-06-05 02:45:19.755961 ultrasync-0.9.8/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     3031 2023-06-05 02:41:43.000000 ultrasync-0.9.8/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.748961 ultrasync-0.9.8/tests/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5121 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7424 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_106.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6360 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108-zone-check.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6635 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4922 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108_burglar_alarm_on.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3873 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4828 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen8_bypass.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7289 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen8_nxg8zbo.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7984 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen_general.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4590 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_zerowire_armed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6543 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_zerowire_general.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/comnav/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.749961 ultrasync-0.9.8/tests/var/comnav/0.106/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1892 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    36123 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21526 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1832 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.bank0.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       81 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.bank4.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.750961 ultrasync-0.9.8/tests/var/comnav/0.108/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1971 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23023 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2793 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       98 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.751961 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1983 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23026 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2791 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.751961 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2044 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      458 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2327 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       91 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/xgen/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.752961 ultrasync-0.9.8/tests/var/xgen/general/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1862 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13088 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/seq.w.update.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18618 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      188 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2071 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zstate.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/xgen8/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.752961 ultrasync-0.9.8/tests/var/xgen8/bypass/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2217 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      326 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zonefunction.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2054 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.753961 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/seq.w.update.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      563 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2088 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zstate.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/zerowire/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.753961 ultrasync-0.9.8/tests/var/zerowire/armed/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      165 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2582 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.754961 ultrasync-0.9.8/tests/var/zerowire/general/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      160 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2574 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.754961 ultrasync-0.9.8/ultrasync/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1793 2023-06-05 02:41:59.000000 ultrasync-0.9.8/ultrasync/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8954 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8351 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6747 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    82964 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/main.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.755961 ultrasync-0.9.8/ultrasync.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7188 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       49 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/top_level.txt
```

### Comparing `ultrasync-0.9.7/LICENSE` & `ultrasync-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/PKG-INFO` & `ultrasync-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.7
+Version: 0.9.8
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -150,9 +149,7 @@
 | **ULTRASYNC_USER** | Provides the `user` variable to the library
 | **ULTRASYNC_HOST** | Provides the `host` variable to the library
 | **ULTRASYNC_SSL_VERIFY** | Provides the `verify` variable to the library
 
 ## Disclaimer
 
 This software was created by reverse engineering my own personal security system. All of this code was generated through trial and error since there is no documentation that I could find that explains the registers. If you can help out by filling in some of the blanks throughout the code base, I would be greatly appreciative of it! Alternatively [buying me a coffee](https://paypal.me/lead2gold?locale.x=en_US) greatly inspires me to continue improving the application.
-
-
```

### Comparing `ultrasync-0.9.7/README.md` & `ultrasync-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/setup.py` & `ultrasync-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['ultrasync = ultrasync.cli:main']
 
 setup(
     name='ultrasync',
-    version='0.9.7',
+    version='0.9.8',
     description='Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync '
                 'ZeroWire',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/caronc/ultrasync',
     keywords='XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire '
```

### Comparing `ultrasync-0.9.7/tests/test_cli.py` & `ultrasync-0.9.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_comnav_0_106.py` & `ultrasync-0.9.8/tests/test_comnav_0_106.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_comnav_0_108-zone-check.py` & `ultrasync-0.9.8/tests/test_comnav_0_108-zone-check.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_comnav_0_108.py` & `ultrasync-0.9.8/tests/test_comnav_0_108.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_comnav_0_108_burglar_alarm_on.py` & `ultrasync-0.9.8/tests/test_comnav_0_108_burglar_alarm_on.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_config.py` & `ultrasync-0.9.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_xgen8_bypass.py` & `ultrasync-0.9.8/tests/test_xgen8_bypass.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_xgen8_nxg8zbo.py` & `ultrasync-0.9.8/tests/test_xgen8_nxg8zbo.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_xgen_general.py` & `ultrasync-0.9.8/tests/test_xgen_general.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_zerowire_armed.py` & `ultrasync-0.9.8/tests/test_zerowire_armed.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/test_zerowire_general.py` & `ultrasync-0.9.8/tests/test_zerowire_general.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.106/area.htm` & `ultrasync-0.9.8/tests/var/comnav/0.106/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.106/master.js` & `ultrasync-0.9.8/tests/var/comnav/0.106/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.106/status.js` & `ultrasync-0.9.8/tests/var/comnav/0.106/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.106/zones.htm` & `ultrasync-0.9.8/tests/var/comnav/0.106/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108/area.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108/master.js` & `ultrasync-0.9.8/tests/var/comnav/0.108/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108/status.js` & `ultrasync-0.9.8/tests/var/comnav/0.108/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108/zones.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/area.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/master.js` & `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.js` & `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zones.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/area.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zones.htm` & `ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen/general/area.htm` & `ultrasync-0.9.8/tests/var/xgen/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen/general/master.js` & `ultrasync-0.9.8/tests/var/xgen/general/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen/general/status.js` & `ultrasync-0.9.8/tests/var/xgen/general/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen/general/zones.htm` & `ultrasync-0.9.8/tests/var/xgen/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen8/bypass/area.htm` & `ultrasync-0.9.8/tests/var/xgen8/bypass/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen8/bypass/zones.htm` & `ultrasync-0.9.8/tests/var/xgen8/bypass/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/area.htm` & `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/status.json` & `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/status.json`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zones.htm` & `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/zerowire/armed/area.htm` & `ultrasync-0.9.8/tests/var/zerowire/armed/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/zerowire/armed/zones.htm` & `ultrasync-0.9.8/tests/var/zerowire/armed/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/zerowire/general/area.htm` & `ultrasync-0.9.8/tests/var/zerowire/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/tests/var/zerowire/general/zones.htm` & `ultrasync-0.9.8/tests/var/zerowire/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/ultrasync/__init__.py` & `ultrasync-0.9.8/ultrasync/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020 Chris Caron <lead2gold@gmail.com>
+# Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>
 # All rights reserved.
 #
 # This code is licensed under the MIT License.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files(the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -20,15 +20,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 __title__ = 'ultrasync'
-__version__ = '0.9.7'
+__version__ = '0.9.8'
 __author__ = 'Chris Caron'
 __license__ = 'MIT'
 __copywrite__ = 'Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .main import UltraSync
```

### Comparing `ultrasync-0.9.7/ultrasync/cli.py` & `ultrasync-0.9.8/ultrasync/cli.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/ultrasync/common.py` & `ultrasync-0.9.8/ultrasync/common.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/ultrasync/config.py` & `ultrasync-0.9.8/ultrasync/config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/ultrasync/logger.py` & `ultrasync-0.9.8/ultrasync/logger.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.7/ultrasync/main.py` & `ultrasync-0.9.8/ultrasync/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,17 +629,14 @@
  
         else:   # self.vendor is NX595EVendor.{ZEROWIRE, XGEN}
 
             logger.error(
                 'Bypass not implemented for vendor {}'.format(self.vendor))
             return False
 
-        # Send our response
-        response = self.__get(
-            '/user/zonefunction.cgi', payload=payload)
 
         if not response:
             logger.info(
                 'Failed to set bypass={} for zone {}'.format(state, zone))
             has_error = True
 
         logger.info(
```

### Comparing `ultrasync-0.9.7/ultrasync.egg-info/PKG-INFO` & `ultrasync-0.9.8/ultrasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.7
+Version: 0.9.8
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -150,9 +149,7 @@
 | **ULTRASYNC_USER** | Provides the `user` variable to the library
 | **ULTRASYNC_HOST** | Provides the `host` variable to the library
 | **ULTRASYNC_SSL_VERIFY** | Provides the `verify` variable to the library
 
 ## Disclaimer
 
 This software was created by reverse engineering my own personal security system. All of this code was generated through trial and error since there is no documentation that I could find that explains the registers. If you can help out by filling in some of the blanks throughout the code base, I would be greatly appreciative of it! Alternatively [buying me a coffee](https://paypal.me/lead2gold?locale.x=en_US) greatly inspires me to continue improving the application.
-
-
```

### Comparing `ultrasync-0.9.7/ultrasync.egg-info/SOURCES.txt` & `ultrasync-0.9.8/ultrasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

