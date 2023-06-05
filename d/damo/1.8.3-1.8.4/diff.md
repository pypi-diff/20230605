# Comparing `tmp/damo-1.8.3.tar.gz` & `tmp/damo-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.3.tar", last modified: Mon May 29 19:25:42 2023, max compression
+gzip compressed data, was "damo-1.8.4.tar", last modified: Mon Jun  5 19:42:27 2023, max compression
```

## Comparing `damo-1.8.3.tar` & `damo-1.8.4.tar`

### file list

```diff
@@ -1,54 +1,52 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8106 2023-05-29 19:25:42.989174 damo-1.8.3/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7585 2023-05-29 19:25:38.000000 damo-1.8.3/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-29 19:25:38.000000 damo-1.8.3/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-29 19:25:42.989174 damo-1.8.3/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-29 19:25:38.000000 damo-1.8.3/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.977174 damo-1.8.3/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7186 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      825 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34482 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17105 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    21100 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19142 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3753 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13289 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5278 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1312 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2947 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1584 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1522 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-29 19:25:38.000000 damo-1.8.3/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-29 19:25:42.989174 damo-1.8.3/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8106 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1237 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-29 19:25:42.000000 damo-1.8.3/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.117919 damo-1.8.4/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-05 19:42:27.117919 damo-1.8.4/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7641 2023-06-05 19:42:23.000000 damo-1.8.4/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-06-05 19:42:23.000000 damo-1.8.4/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-06-05 19:42:27.117919 damo-1.8.4/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-06-05 19:42:23.000000 damo-1.8.4/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.101920 damo-1.8.4/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.113920 damo-1.8.4/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7358 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34675 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11111 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17097 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    22589 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19134 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3723 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13295 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5615 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1173 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3195 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1582 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1490 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-06-05 19:42:23.000000 damo-1.8.4/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-06-05 19:42:27.117919 damo-1.8.4/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8162 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1174 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-06-05 19:42:27.000000 damo-1.8.4/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.3/PKG-INFO` & `damo-1.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: damo
-Version: 1.8.3
-Summary: DAMON user-space tool
-Home-page: https://github.com/awslabs/damo
-Author: SeongJae Park
-Author-email: sj@kernel.org
-Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
-Project-URL: DAMON, https://damonitor.github.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -42,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +72,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -153,61 +138,62 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 
-Deprecated Features
-===================
+Deprecated, or Will be Deprecated Features
+==========================================
 
-Below are features that deprecated, or will be deprecated.  If you depend on
-any of those, please report your usecase to the community via github issue,
-sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+Below are features that recently deprecated, or will be deprecated.  If you
+depend on any of those, please report your usecase to the community via github
+issue, sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
 
---rbuf option of `damo record`
-------------------------------
 
-Deprecated.
+DAMON record binary format
+--------------------------
 
-Early versions of DAMON supported in-kernel direct monitoring results record
-file generation.  To control the overhead of it, DAMO allowed user to specify
-the size of buffer for the work.  The feature has not merged into the mainline,
-and discarded.  Hence the option was available for only few kernels that ported
-the feature.  For most of kernels, tracepoint based record file generation is
-being used, and the overhead of the approach is subtle.  Hence, the option has
-deprecated.
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
 
 
 DAMOS singline format
 ---------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
 specification to the new json format.
 
 
-`Python2 support
-----------------
-
-Deprecated.  Use Python3.
-
-For some old distros, DAMO initially supported Python2.  Because Python2 is
-really old now, the support has deprecated.  Please use Python3 or newer.
-
-
-DAMON record binary format
---------------------------
+--rbuf option of `damo record`
+------------------------------
 
-Will be deprecated by 2023 Q3.
+Deprecated.
 
-At the beginning, DAMO used its special binary format, namely `record`.  It is
-designed for lightweight saving of the monitoring results.  It is difficult to
-read, and not that efficient compared to fancy compression techniques.  `json`
-based monitoring results can be easier to read, and more efficient when
-compression technique is used.  Hence, the format will be deprecated.  You may
-use `damo convert_record_format` to convert your old record binary format
-monitoring results files to the new format.
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
```

### Comparing `damo-1.8.3/README.md` & `damo-1.8.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 1.8.4
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -27,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -72,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -138,61 +153,62 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 
-Deprecated Features
-===================
+Deprecated, or Will be Deprecated Features
+==========================================
 
-Below are features that deprecated, or will be deprecated.  If you depend on
-any of those, please report your usecase to the community via github issue,
-sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+Below are features that recently deprecated, or will be deprecated.  If you
+depend on any of those, please report your usecase to the community via github
+issue, sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
 
---rbuf option of `damo record`
-------------------------------
 
-Deprecated.
+DAMON record binary format
+--------------------------
 
-Early versions of DAMON supported in-kernel direct monitoring results record
-file generation.  To control the overhead of it, DAMO allowed user to specify
-the size of buffer for the work.  The feature has not merged into the mainline,
-and discarded.  Hence the option was available for only few kernels that ported
-the feature.  For most of kernels, tracepoint based record file generation is
-being used, and the overhead of the approach is subtle.  Hence, the option has
-deprecated.
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
 
 
 DAMOS singline format
 ---------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
 specification to the new json format.
 
 
-`Python2 support
-----------------
-
-Deprecated.  Use Python3.
-
-For some old distros, DAMO initially supported Python2.  Because Python2 is
-really old now, the support has deprecated.  Please use Python3 or newer.
-
-
-DAMON record binary format
---------------------------
+--rbuf option of `damo record`
+------------------------------
 
-Will be deprecated by 2023 Q3.
+Deprecated.
 
-At the beginning, DAMO used its special binary format, namely `record`.  It is
-designed for lightweight saving of the monitoring results.  It is difficult to
-read, and not that efficient compared to fancy compression techniques.  `json`
-based monitoring results can be easier to read, and more efficient when
-compression technique is used.  Hence, the format will be deprecated.  You may
-use `damo convert_record_format` to convert your old record binary format
-monitoring results files to the new format.
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
```

### Comparing `damo-1.8.3/setup.py` & `damo-1.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_deprecated.py` & `damo-1.8.4/src/damo/_damo_deprecated.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,62 @@
 # SPDX-License-Identifier: GPL-2.0
 
-"""
-Change human readable data access monitoring-based operation schemes input for
-'damo' to a '_damon.Damos' object.  Currently,
+'''
+Keep code for deprecated features, which still need to help old users migrate,
+e.g., 'translate_damos' and 'convert_record_format'.
+'''
+
+import json
+import os
+import subprocess
+import sys
+
+import _damon
+
+import _damo_deprecation_notice
+import _damo_fmt_str
+
+'''
+Python2 support
+'''
+
+if sys.version.startswith('2.'):
+    _damo_deprecation_notice.deprecated(feature='Python2 support of damo',
+            deadline='2023-Q2')
+
+# For supporting python 2.6
+try:
+    subprocess.DEVNULL = subprocess.DEVNULL
+except AttributeError:
+    subprocess.DEVNULL = open(os.devnull, 'wb')
+
+try:
+    subprocess.check_output = subprocess.check_output
+except AttributeError:
+    def check_output(*popenargs, **kwargs):
+        process = subprocess.Popen(stdout=subprocess.PIPE, *popenargs, **kwargs)
+        output, err = process.communicate()
+        rc = process.poll()
+        if rc:
+            raise subprocess.CalledProcessError(rc, popenargs[0])
+        return output
+
+    subprocess.check_output = check_output
 
-- simple human-readable single line per scheme text (will be deprecated) and
-- json string format
+'''
+DAMOS single-line scheme specification input.
 
-are supported.  Below are the example of the input.
+Change human readable data access monitoring-based operation schemes input for
+'damo' to a '_damon.Damos' object.
+This format has inspired by DAMON debugfs 'schemes' file input/output.  It was
+enough to be used for the initial version, but later extending it made it to
+receive more than 15 fields, and became hard to understand and maintain.
+Hence, replaced by more intuitive command line options and json format.
 
-Below are examples of simple human-readable single line per scheme text.
+Below are examples of the single-line scheme input.
 
     # format is:
     # <min/max size> <min/max frequency (0-100)> <min/max age> <action>
     #
     # B/K/M/G/T for Bytes/KiB/MiB/GiB/TiB
     # us/ms/s/m/h/d for micro-seconds/milli-seconds/seconds/minutes/hours/days
     # 'min/max' for possible min/max value.
@@ -34,54 +77,15 @@
     # >=100ms, let the region to use huge pages (call madvise() with
     # MADV_HUGEPAGE).
     2M      max     90      100     100ms   max hugepage
 
     # If a regions of a size >=2MiB keeps small access frequency for >=100ms,
     # avoid the region using huge pages (call madvise() with MADV_NOHUGEPAGE).
     2M      max     0       25      100ms   max nohugepage
-
-Below is an exaple of the json string format.
-
-    [
-       {
-            "comment": "just for monitoring",
-            "name": "0",
-            "action": "stat",
-            "access_pattern": {
-                "sz_bytes": {"min": "0 B", "max": "max"},
-                "nr_accesses": {"min": "0 %", "max": "100 %"},
-                "age": {"min": "0 ns", "max": "max"}
-            },
-            "quotas": {
-                "time_ms": 0,
-                "sz_bytes": 0,
-                "reset_interval_ms": 0,
-                "weight_sz_permil": 0,
-                "weight_nr_accesses_permil": 0,
-                "weight_age_permil": 0
-            },
-            "watermarks": {
-                "metric": "none",
-                "interval_us": 0,
-                "high_permil": 0,
-                "mid_permil": 0,
-                "low_permil": 0
-            },
-            "filters": []
-        }
-    ]
-"""
-
-import json
-import os
-
-import _damon
-
-import _damo_deprecation_notice
-import _damo_fmt_str
+'''
 
 def fields_to_v0_scheme(fields):
     scheme = _damon.Damos()
     scheme.access_pattern = _damon.DamosAccessPattern(
             sz_bytes = [_damo_fmt_str.text_to_bytes(fields[0]),
                 _damo_fmt_str.text_to_bytes(fields[1])],
             nr_accesses = [_damo_fmt_str.text_to_percent(fields[2]),
```

### Comparing `damo-1.8.3/src/damo/_damo_deprecation_notice.py` & `damo-1.8.4/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_dist.py` & `damo-1.8.4/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_fmt_str.py` & `damo-1.8.4/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_fs.py` & `damo-1.8.4/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_paddr_layout.py` & `damo-1.8.4/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damo_subcmds.py` & `damo-1.8.4/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damon.py` & `damo-1.8.4/src/damo/_damon.py`

 * *Files 1% similar despite different names*

```diff
@@ -883,45 +883,14 @@
 def damon_interface():
     if _damon_fs == _damon_sysfs:
         return 'sysfs'
     elif _damon_fs == _damon_dbgfs:
         return 'debugfs'
     raise Exception('_damo_fs is neither _damon_sysfs nor _damon_dbgfs')
 
-# DAMON status reading
-
-def is_kdamond_running(kdamond_idx):
-    return _damon_fs.is_kdamond_running(kdamond_idx)
-
-def current_kdamonds():
-    return _damon_fs.current_kdamonds()
-
-def nr_current_kdamonds():
-    return _damon_fs.nr_current_kdamonds()
-
-def running_kdamond_idxs():
-    return [idx for idx in range(nr_current_kdamonds())
-            if is_kdamond_running(idx)]
-
-def any_kdamond_running():
-    for idx in range(nr_current_kdamonds()):
-        if is_kdamond_running(idx):
-            return True
-    return False
-
-def wait_current_kdamonds_turned_on():
-    for idx in range(nr_current_kdamonds()):
-        while not is_kdamond_running(idx):
-            time.sleep(1)
-
-def wait_current_kdamonds_turned_off():
-    for idx in range(nr_current_kdamonds()):
-        while is_kdamond_running(idx):
-            time.sleep(1)
-
 # DAMON control
 
 def stage_kdamonds(kdamonds):
     return _damon_fs.stage_kdamonds(kdamonds)
 
 def commit_staged(kdamond_idxs):
     if _damon_fs == _damon_dbgfs:
@@ -943,27 +912,68 @@
     return _damon_fs.update_schemes_stats(kdamond_idxs)
 
 def update_schemes_tried_regions(kdamond_idxs=None):
     if kdamond_idxs == None:
         kdamond_idxs = running_kdamond_idxs()
     return _damon_fs.update_schemes_tried_regions(kdamond_idxs)
 
-def update_schemes_status():
+def update_schemes_status(stats=True, tried_regions=True):
+    '''Returns error string or None'''
     idxs = running_kdamond_idxs()
     if len(idxs) == 0:
         return None
-    err = update_schemes_stats(idxs)
-    if err != None:
-        return err
-    return update_schemes_tried_regions(idxs)
+    if stats:
+        err = update_schemes_stats(idxs)
+        if err != None:
+            return err
+    if tried_regions:
+        return update_schemes_tried_regions(idxs)
+    return None
 
 def turn_damon_on(kdamonds_idxs):
     err = _damon_fs.turn_damon_on(kdamonds_idxs)
     if err:
         return err
-    wait_current_kdamonds_turned_on()
+    wait_kdamonds_turned_on()
 
 def turn_damon_off(kdamonds_idxs):
     err = _damon_fs.turn_damon_off(kdamonds_idxs)
     if err:
         return err
-    wait_current_kdamonds_turned_off()
+    wait_kdamonds_turned_off()
+
+# DAMON status reading
+
+def is_kdamond_running(kdamond_idx):
+    return _damon_fs.is_kdamond_running(kdamond_idx)
+
+def current_kdamonds():
+    return _damon_fs.current_kdamonds()
+
+def update_read_kdamonds():
+    err = update_schemes_status()
+    if err:
+        return None, err
+    return current_kdamonds(), None
+
+def nr_kdamonds():
+    return _damon_fs.nr_kdamonds()
+
+def running_kdamond_idxs():
+    return [idx for idx in range(nr_kdamonds())
+            if is_kdamond_running(idx)]
+
+def any_kdamond_running():
+    for idx in range(nr_kdamonds()):
+        if is_kdamond_running(idx):
+            return True
+    return False
+
+def wait_kdamonds_turned_on():
+    for idx in range(nr_kdamonds()):
+        while not is_kdamond_running(idx):
+            time.sleep(1)
+
+def wait_kdamonds_turned_off():
+    for idx in range(nr_kdamonds()):
+        while is_kdamond_running(idx):
+            time.sleep(1)
```

### Comparing `damo-1.8.3/src/damo/_damon_args.py` & `damo-1.8.4/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/_damon_dbgfs.py` & `damo-1.8.4/src/damo/_damon_dbgfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     pid = files_content['kdamond_pid'].strip()
     return [_damon.Kdamond(state, pid, [ctx])]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(debugfs_damon))
 
-def nr_current_kdamonds():
+def nr_kdamonds():
     # TODO: Support manually created kdamonds
     return 1
 
 # features
 
 feature_supports = None
```

### Comparing `damo-1.8.3/src/damo/_damon_result.py` & `damo-1.8.4/src/damo/_damon_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,74 +12,164 @@
 import _damo_deprecation_notice
 import _damo_fmt_str
 import _damon
 
 PERF = 'perf'
 PERF_EVENT = 'damon:damon_aggregated'
 
-class DAMONSnapshot:
+class DamonSnapshot:
+    '''
+    Contains a snapshot of data access monitoring results
+    '''
     start_time = None
     end_time = None
     regions = None
 
     def __init__(self, start_time, end_time):
         self.start_time = start_time
         self.end_time = end_time
         self.regions = []
 
     @classmethod
     def from_kvpairs(cls, kv):
-        snapshot = DAMONSnapshot(_damo_fmt_str.text_to_ns(kv['start_time']),
+        snapshot = DamonSnapshot(_damo_fmt_str.text_to_ns(kv['start_time']),
                 _damo_fmt_str.text_to_ns(kv['end_time']))
         snapshot.regions = [_damon.DamonRegion.from_kvpairs(r)
                 for r in kv['regions']]
         return snapshot
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('start_time', _damo_fmt_str.format_time_ns_exact(
                 self.start_time, raw)),
             ('end_time', _damo_fmt_str.format_time_ns_exact(
                 self.end_time, raw)),
             ('regions', [r.to_kvpairs() for r in self.regions])])
 
-class DAMONRecord:
+class DamonRecord:
+    '''
+    Contains data access monitoring results for single target
+    '''
+    intervals = None
     target_id = None
     snapshots = None
 
-    def __init__(self, target_id):
+    def __init__(self, intervals, target_id):
+        self.intervals = intervals
         self.target_id = target_id
         self.snapshots = []
 
     @classmethod
     def from_kvpairs(cls, kv):
-        record = DAMONRecord(kv['target_id'])
-        record.snapshots = [DAMONSnapshot.from_kvpairs(s)
+        intervals = None
+        if 'intervals' in kv:
+            intervals = _damon.DamonIntervals.from_kvpairs(kv['intervals'])
+
+        record = DamonRecord(intervals, kv['target_id'])
+        record.snapshots = [DamonSnapshot.from_kvpairs(s)
                 for s in kv['snapshots']]
+
         return record
 
     def to_kvpairs(self, raw=False):
-        return collections.OrderedDict([
-            ('target_id', self.target_id),
-            ('snapshots', [s.to_kvpairs(raw) for s in self.snapshots])])
+        ordered_dict = collections.OrderedDict()
+        if self.intervals != None:
+            ordered_dict['intervals'] = self.intervals.to_kvpairs(raw)
+        ordered_dict['target_id'] = self.target_id
+        ordered_dict['snapshots'] = [s.to_kvpairs(raw) for s in self.snapshots]
+        return ordered_dict
 
-class DAMONResult:
+class DamonResult:
+    '''
+    Contains data access monitoring results.
+    '''
     records = None
 
     def __init__(self):
         self.records = []
 
-    def record_of(self, target_id):
+    def record_of(self, target_id, intervals):
         for record in self.records:
             if record.target_id == target_id:
                 return record
-        record = DAMONRecord(target_id)
+        record = DamonRecord(intervals, target_id)
         self.records.append(record)
         return record
 
+# for monitoring results manipulation
+
+def regions_intersect(r1, r2):
+    return not (r1.end <= r2.start or r2.end <= r1.start)
+
+def add_region(regions, region, nr_acc_to_add):
+    for r in regions:
+        if regions_intersect(r, region):
+            if not r in nr_acc_to_add:
+                nr_acc_to_add[r] = 0
+            nr_acc_to_add[r] = max(nr_acc_to_add[r],
+                    region.nr_accesses.samples)
+
+            new_regions = []
+            if region.start < r.start:
+                new_regions.append(_damon.DamonRegion(
+                    region.start, r.start,
+                    region.nr_accesses.samples, _damon.unit_samepls,
+                    region.age.aggr_intervals, _damon.unit_aggr_intervals))
+            if r.end < region.end:
+                new_regions.append(_damon.DamonRegion(
+                        r.end, region.end,
+                        region.nr_accesses.samples, _damon.unit_samples,
+                        region.age.aggr_intervals,
+                        _damon.unit_aggr_intervals))
+
+            for new_r in new_regions:
+                add_region(regions, new_r, nr_acc_to_add)
+            return
+    regions.append(region)
+
+def aggregate_snapshots(snapshots):
+    new_regions = []
+    for snapshot in snapshots:
+        # Suppose the first snapshot has a region 1-10:5, and the second
+        # snapshot has two regions, 1-5:2, 5-10: 4.  Aggregated snapshot should
+        # be 1-10:9.  That is, we should add maximum nr_accesses of
+        # intersecting regions.  nr_acc_to_add contains the information.
+        nr_acc_to_add = {}
+        for region in snapshot.regions:
+            add_region(new_regions, region, nr_acc_to_add)
+        for region in nr_acc_to_add:
+            region.nr_accesses.samples += nr_acc_to_add[region]
+            region.nr_accesses.val = region.nr_accesses.samples
+            region.nr_accesses.unit = _damon.unit_samples
+
+    new_snapshot = DamonSnapshot(snapshots[0].start_time,
+            snapshots[-1].end_time)
+    new_snapshot.regions = new_regions
+    return new_snapshot
+
+def adjusted_snapshots(snapshots, aggregate_interval_us):
+    adjusted = []
+    to_aggregate = []
+    for snapshot in snapshots:
+        to_aggregate.append(snapshot)
+        interval_ns = to_aggregate[-1].end_time - to_aggregate[0].start_time
+        if interval_ns >= aggregate_interval_us * 1000:
+            adjusted.append(aggregate_snapshots(to_aggregate))
+            to_aggregate = []
+    return adjusted
+
+def adjust_result(result, aggregate_interval, nr_snapshots_to_skip):
+    for record in result.records:
+        if record.intervals != None:
+            record.intervals.aggr = aggregate_interval
+        record.snapshots = adjusted_snapshots(
+                record.snapshots[nr_snapshots_to_skip:], aggregate_interval)
+
+# For reading monitoring results from a file
+
 def read_record_format_version(f):
     # read record format version
     mark = f.read(16)
     if mark == b'damon_recfmt_ver':
         return struct.unpack('i', f.read(4))[0]
     else:
         f.seek(0)
@@ -91,15 +181,15 @@
         return None
     sec = struct.unpack('l', timebin[0:8])[0]
     nsec = struct.unpack('l', timebin[8:16])[0]
     end_time = sec * 1000000000 + nsec
     return end_time
 
 def read_snapshot_from_record_file(f, start_time, end_time):
-    snapshot = DAMONSnapshot(start_time, end_time)
+    snapshot = DamonSnapshot(start_time, end_time)
     nr_regions = struct.unpack('I', f.read(4))[0]
     for r in range(nr_regions):
         start_addr = struct.unpack('L', f.read(8))[0]
         end_addr = struct.unpack('L', f.read(8))[0]
         nr_accesses = struct.unpack('I', f.read(4))[0]
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
@@ -126,31 +216,38 @@
         nr_snapshots = len(snapshots) - 1
         snapshot_time = float(end_time - start_time) / nr_snapshots
         snapshots[0].start_time = snapshots[0].end_time - snapshot_time
 
         if is_fake_snapshot(snapshots[-1]):
             del record.snapshots[-1]
 
-def record_to_damon_result(file_path):
+def warn_record_type_deprecation():
+    _damo_deprecation_notice.will_be_deprecated(
+            feature='\'record\' file type support',
+            deadline='2023-Q3',
+            additional_notice='use json_compressed type instead.')
+
+def parse_binary_format_record(file_path, monitoring_intervals):
+    warn_record_type_deprecation()
     with open(file_path, 'rb') as f:
         fmt_version = read_record_format_version(f)
-        result = DAMONResult()
+        result = DamonResult()
         while True:
             end_time = read_end_time_from_record_file(f)
             if end_time == None:
                 break
 
             nr_tasks = struct.unpack('I', f.read(4))[0]
             for t in range(nr_tasks):
                 if fmt_version == 1:
                     target_id = struct.unpack('i', f.read(4))[0]
                 else:
                     target_id = struct.unpack('L', f.read(8))[0]
 
-                record = result.record_of(target_id)
+                record = result.record_of(target_id, monitoring_intervals)
                 if len(record.snapshots) == 0:
                     start_time = None
                 else:
                     start_time = record.snapshots[-1].end_time
                     if end_time < start_time:
                         return None, 'snapshot is not sorted by time'
                 try:
@@ -193,33 +290,33 @@
             age = None
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
                 age, _damon.unit_aggr_intervals)
 
         return region, end_time, target_id, nr_regions
 
-def perf_script_to_damon_result(script_output):
-    result = DAMONResult()
+def parse_perf_script(script_output, monitoring_intervals):
+    result = DamonResult()
     snapshot = None
 
     for line in script_output.split('\n'):
         region, end_time, target_id, nr_regions = parse_perf_script_line(line)
         if region == None:
             continue
 
-        record = result.record_of(target_id)
+        record = result.record_of(target_id, monitoring_intervals)
         if len(record.snapshots) == 0:
             start_time = None
         else:
             start_time = record.snapshots[-1].end_time
             if start_time > end_time:
                 return None, 'trace is not time-sorted'
 
         if snapshot == None:
-            snapshot = DAMONSnapshot(start_time, end_time)
+            snapshot = DamonSnapshot(start_time, end_time)
             record.snapshots.append(snapshot)
         snapshot = record.snapshots[-1]
         snapshot.regions.append(region)
 
         if len(snapshot.regions) == nr_regions:
             snapshot = None
 
@@ -240,64 +337,87 @@
                     stderr=subprocess.PIPE)
         except:
             err = 'perf record not working with "%s"' % PERF
     except:
         err = 'perf not found at "%s"' % PERF
     return err
 
-def warn_record_type_deprecation():
-    _damo_deprecation_notice.will_be_deprecated(
-            feature='\'record\' file type support',
-            deadline='2023-Q3',
-            additional_notice='use json_compressed type instead.')
-
 def parse_damon_record_json_compressed(result_file):
     with open(result_file, 'rb') as f:
         compressed = f.read()
     decompressed = zlib.decompress(compressed).decode()
     kvpairs = json.loads(decompressed)
-    result = DAMONResult()
-    result.records = [DAMONRecord.from_kvpairs(kvp) for kvp in kvpairs]
+    result = DamonResult()
+    result.records = [DamonRecord.from_kvpairs(kvp) for kvp in kvpairs]
     return result
 
-def parse_damon_result(result_file):
-    script_output = None
+def parse_damon_result(result_file, monitoring_intervals=None):
+    '''
+    Return monitoring results and error string
+    '''
+
     file_type = subprocess.check_output(
             ['file', '-b', result_file]).decode().strip()
     if file_type == 'zlib compressed data':
         try:
             return parse_damon_record_json_compressed(result_file), None
         except Exception as e:
             return None, 'failed parsing json compressed file (%s)' % e
-    elif file_type == 'ASCII text':
+
+    perf_script_output = None
+    if file_type == 'ASCII text':
         with open(result_file, 'r') as f:
-            script_output = f.read()
+            perf_script_output = f.read()
     else:
+        # might be perf data
         try:
             with open(os.devnull, 'w') as fnull:
-                script_output = subprocess.check_output(
+                perf_script_output = subprocess.check_output(
                         [PERF, 'script', '-i', result_file],
                         stderr=fnull).decode()
         except:
+            # Should be record format file
             pass
-    if script_output != None:
-        result, err = perf_script_to_damon_result(script_output)
-    else:
-        warn_record_type_deprecation()
-        result, err = record_to_damon_result(result_file)
+    if perf_script_output != None:
+        return parse_perf_script(perf_script_output, monitoring_intervals)
 
-    return result, err
+    return parse_binary_format_record(result_file, monitoring_intervals)
+
+# for writing monitoring results to a file
 
 def write_damon_record_json_compressed(result, file_path):
     json_str = json.dumps([r.to_kvpairs(r) for r in result.records], indent=4)
     compressed = zlib.compress(json_str.encode())
     with open(file_path, 'wb') as f:
         f.write(compressed)
 
+def add_fake_snapshot_if_needed(result):
+    '''
+    perf and record file format stores only snapshot end time.  For a record
+    having only single snapshot, hence, the reader of the files cannot knwo the
+    start time of the snapshot.  Add a fake snapshot for the case.
+    '''
+
+    for record in result.records:
+        snapshots = record.snapshots
+        if len(snapshots) != 1:
+            continue
+        snapshot = snapshots[0]
+        snap_duration = snapshot.end_time - snapshot.start_time
+        fake_snapshot = DamonSnapshot(snapshot.end_time,
+                snapshot.end_time + snap_duration)
+        # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
+        fake_snapshot.regions = [_damon.DamonRegion(0, 0,
+            -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
+        snapshots.append(fake_snapshot)
+
 def write_damon_record(result, file_path, format_version):
+    warn_record_type_deprecation()
+    add_fake_snapshot_if_needed(result)
+
     with open(file_path, 'wb') as f:
         f.write(b'damon_recfmt_ver')
         f.write(struct.pack('i', format_version))
 
         for record in result.records:
             snapshots = record.snapshots
             for snapshot in snapshots:
@@ -322,14 +442,15 @@
     Example of the normal perf script output:
 
     kdamond.0  4452 [000] 82877.315633: damon:damon_aggregated: \
             target_id=18446623435582458880 nr_regions=17 \
             140731667070976-140731668037632: 0 3
     '''
 
+    add_fake_snapshot_if_needed(result)
     with open(file_path, 'w') as f:
         for record in result.records:
             snapshots = record.snapshots
             for snapshot in snapshots:
                 for region in snapshot.regions:
                     f.write(' '.join(['kdamond.x', 'xxxx', 'xxxx',
                         '%f:' % (snapshot.end_time / 1000000000.0),
@@ -360,137 +481,70 @@
         file_type_perf_script, file_type_record]
 
 def write_damon_result(result, file_path, file_type, file_permission=None):
     '''Returns None if success, an error string otherwise'''
     if not file_type in self_write_supported_file_types:
         return 'write unsupported file type: %s' % file_type
 
-    for record in result.records:
-        snapshots = record.snapshots
-        if len(snapshots) == 1 and file_type in [file_type_record,
-                file_type_perf_script]:
-            # we cannot know start/end time of single snapshot from the file
-            # to allow it with later read, write a fake snapshot
-            snapshot = snapshots[0]
-            snap_duration = snapshot.end_time - snapshot.start_time
-            fake_snapshot = DAMONSnapshot(snapshot.end_time,
-                    snapshot.end_time + snap_duration)
-            # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
-            fake_snapshot.regions = [_damon.DamonRegion(0, 0,
-                -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
-            snapshots.append(fake_snapshot)
-    if file_type == file_type_record:
-        warn_record_type_deprecation()
-        write_damon_record(result, file_path, 2)
+    if file_type == file_type_json_compressed:
+        write_damon_record_json_compressed(result, file_path)
     elif file_type == file_type_perf_script:
         write_damon_perf_script(result, file_path)
-    elif file_type == file_type_json_compressed:
-        write_damon_record_json_compressed(result, file_path)
+    elif file_type == file_type_record:
+        write_damon_record(result, file_path, 2)
+
     if file_permission != None:
         os.chmod(file_path, file_permission)
     return None
 
-def update_result_file(file_path, file_format, file_permission=None):
-    result, err = parse_damon_result(file_path)
+def update_result_file(file_path, file_format, file_permission=None,
+        monitoring_intervals=None):
+    result, err = parse_damon_result(file_path, monitoring_intervals)
     if err:
         return err
     return write_damon_result(result, file_path, file_format, file_permission)
 
-def regions_intersect(r1, r2):
-    return not (r1.end <= r2.start or r2.end <= r1.start)
-
-def add_region(regions, region, nr_acc_to_add):
-    for r in regions:
-        if regions_intersect(r, region):
-            if not r in nr_acc_to_add:
-                nr_acc_to_add[r] = 0
-            nr_acc_to_add[r] = max(nr_acc_to_add[r],
-                    region.nr_accesses.samples)
-
-            new_regions = []
-            if region.start < r.start:
-                new_regions.append(_damon.DamonRegion(
-                    region.start, r.start,
-                    region.nr_accesses.samples, _damon.unit_samepls,
-                    region.age.aggr_intervals, _damon.unit_aggr_intervals))
-            if r.end < region.end:
-                new_regions.append(_damon.DamonRegion(
-                        r.end, region.end,
-                        region.nr_accesses.samples, _damon.unit_samples,
-                        region.age.aggr_intervals,
-                        _damon.unit_aggr_intervals))
-
-            for new_r in new_regions:
-                add_region(regions, new_r, nr_acc_to_add)
-            return
-    regions.append(region)
-
-def aggregate_snapshots(snapshots):
-    new_regions = []
-    for snapshot in snapshots:
-        # Suppose the first snapshot has a region 1-10:5, and the second
-        # snapshot has two regions, 1-5:2, 5-10: 4.  Aggregated snapshot should
-        # be 1-10:9.  That is, we should add maximum nr_accesses of
-        # intersecting regions.  nr_acc_to_add contains the information.
-        nr_acc_to_add = {}
-        for region in snapshot.regions:
-            add_region(new_regions, region, nr_acc_to_add)
-        for region in nr_acc_to_add:
-            region.nr_accesses.samples += nr_acc_to_add[region]
-            region.nr_accesses.val = region.nr_accesses.samples
-            region.nr_accesses.unit = _damon.unit_samples
-
-    new_snapshot = DAMONSnapshot(snapshots[0].start_time,
-            snapshots[-1].end_time)
-    new_snapshot.regions = new_regions
-    return new_snapshot
-
-def adjusted_snapshots(snapshots, aggregate_interval_us):
-    adjusted = []
-    to_aggregate = []
-    for snapshot in snapshots:
-        to_aggregate.append(snapshot)
-        interval_ns = to_aggregate[-1].end_time - to_aggregate[0].start_time
-        if interval_ns >= aggregate_interval_us * 1000:
-            adjusted.append(aggregate_snapshots(to_aggregate))
-            to_aggregate = []
-    return adjusted
-
-def adjust_result(result, aggregate_interval, nr_snapshots_to_skip):
-    for record in result.records:
-        record.snapshots = adjusted_snapshots(
-                record.snapshots[nr_snapshots_to_skip:], aggregate_interval)
+# for recording
 
 record_requests = {}
 '''
 Start recording DAMON's monitoring results using perf.
 
 Returns pipe for the perf.  The pipe should be passed to
 stop_monitoring_record() later.
 '''
-def start_monitoring_record(file_path, file_format, file_permission):
+def start_monitoring_record(file_path, file_format, file_permission,
+        monitoring_intervals):
     pipe = subprocess.Popen(
             [PERF, 'record', '-a', '-e', PERF_EVENT, '-o', file_path])
-    record_requests[pipe] = [file_path, file_format, file_permission]
+    record_requests[pipe] = [file_path, file_format, file_permission,
+            monitoring_intervals]
     return pipe
 
 def stop_monitoring_record(perf_pipe):
-    file_path, file_format, file_permission = record_requests[perf_pipe]
+    file_path, file_format, file_permission = record_requests[perf_pipe][:3]
+    monitoring_intervals = record_requests[perf_pipe][3]
     try:
         perf_pipe.send_signal(signal.SIGINT)
         perf_pipe.wait()
     except:
         # perf might already finished
         pass
-    if file_format != file_type_perf_data:
-        err = update_result_file(file_path, file_format)
-        if err != None:
-            print('converting format from perf_data to %s failed (%s)' %
-                    (file_format, err))
-    os.chmod(file_path, file_permission)
+
+    if file_format == file_type_perf_data:
+        os.chmod(file_path, file_permission)
+        return
+
+    err = update_result_file(file_path, file_format, file_permission,
+            monitoring_intervals)
+    if err != None:
+        print('converting format from perf_data to %s failed (%s)' %
+                (file_format, err))
+
+# for snapshot
 
 def install_scheme(scheme_to_install):
     '''Install given scheme to all contexts if effectively same scheme is not
     installed.
     Returns whether it found a context doesn't having the scheme, and an error
     if something wrong.
     '''
@@ -513,39 +567,40 @@
             return (False,
                     'committing scheme installed kdamonds failed: %s' % err)
     return installed, None
 
 def tried_regions_to_snapshot(tried_regions, intervals):
     snapshot_end_time_ns = time.time() * 1000000000
     snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
-    snapshot = DAMONSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
+    snapshot = DamonSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
         snapshot.regions.append(tried_region)
     return snapshot
 
 def tried_regions_to_snapshots(monitor_scheme):
     snapshots = {} # {kdamond idx: {ctx idx: [Snapshot, intervals]}}
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
         # TODO: Make a cleaner way for passing the index
         for ctx_idx, ctx in enumerate(kdamond.contexts):
             for scheme in ctx.schemes:
-                if scheme.effectively_equal(monitor_scheme, ctx.intervals):
-                    snapshot = tried_regions_to_snapshot(scheme.tried_regions,
-                            ctx.intervals)
-                    if not kdamond_idx in snapshots:
-                        snapshots[kdamond_idx] = {}
-                    snapshots[kdamond_idx][ctx_idx] = [snapshot, ctx.intervals]
-                    break
+                if not scheme.effectively_equal(monitor_scheme, ctx.intervals):
+                    continue
+                snapshot = tried_regions_to_snapshot(scheme.tried_regions,
+                        ctx.intervals)
+                if not kdamond_idx in snapshots:
+                    snapshots[kdamond_idx] = {}
+                snapshots[kdamond_idx][ctx_idx] = [snapshot, ctx.intervals]
+                break
     return snapshots
 
 def get_snapshots(access_pattern):
-    'return DAMONSnapshots and an error'
+    'return DamonSnapshots and an error'
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
     orig_kdamonds = _damon.current_kdamonds()
 
     monitor_scheme = _damon.Damos(access_pattern=access_pattern)
```

### Comparing `damo-1.8.3/src/damo/_damon_sysfs.py` & `damo-1.8.4/src/damo/_damon_sysfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
             for content in numbered_dirs_content(
                 files_contents, 'nr_kdamonds')]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(kdamonds_dir))
 
-def nr_current_kdamonds():
+def nr_kdamonds():
     nr_kdamonds, err = _damo_fs.read_file(nr_kdamonds_file)
     if err != None:
         raise Exception('nr_kdamonds_file read fail (%s)' % err)
     return int(nr_kdamonds)
 
 def commit_staged(kdamond_idxs):
     for kdamond_idx in kdamond_idxs:
```

### Comparing `damo-1.8.3/src/damo/damo.py` & `damo-1.8.4/src/damo/damo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 import argparse
 
 import os
 os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 import sys
 
-import _damo_python2_support
-
 import damo_adjust
 import damo_convert_record_format
 import damo_features
 import damo_fmt_json
 import damo_lru_sort
 import damo_monitor
 import damo_reclaim
```

### Comparing `damo-1.8.3/src/damo/damo_adjust.py` & `damo-1.8.4/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_convert_record_format.py` & `damo-1.8.4/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_features.py` & `damo-1.8.4/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_fmt_json.py` & `damo-1.8.4/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_heats.py` & `damo-1.8.4/src/damo/damo_heats.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     # Compensate the values so that those fit with the resolution
     tmax = tmin + tunit * tres
     amax = amin + aunit * ares
 
     # __pr_heats(damon_result, tid, tunit, tmin, tmax, aunit, amin, amax)
 
-    snapshots = damon_result.record_of(tid).snapshots
+    snapshots = damon_result.record_of(tid, None).snapshots
     pixels = heat_pixels_from_snapshots(snapshots, [tmin, tmax], [amin, amax],
             [tres, ares])
 
     if args.heatmap == 'stdout':
         heatmap_plot_ascii(pixels, [tmin, tmax], [amin, amax], [tres, ares],
                 args.stdout_heatmap_color)
         return
```

### Comparing `damo-1.8.3/src/damo/damo_lru_sort.py` & `damo-1.8.4/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_monitor.py` & `damo-1.8.4/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_nr_regions.py` & `damo-1.8.4/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_reclaim.py` & `damo-1.8.4/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_record.py` & `damo-1.8.4/src/damo/damo_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             choices=_damon_result.file_types,
             default=_damon_result.file_type_json_compressed,
             help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--perf_path', type=str, default='perf',
             help='path of perf tool ')
-    parser.add_argument('--include_childs', action='store_true',
+    parser.add_argument('--include_child_tasks', action='store_true',
             help='record accesses of child processes')
     return parser
 
 def main(args=None):
     global data_for_cleanup
 
     if not args:
@@ -150,22 +150,29 @@
     if not is_ongoing:
         err, kdamonds = _damon_args.turn_damon_on(args)
         if err:
             print('could not turn DAMON on (%s)' % err)
             cleanup_exit(-2)
         data_for_cleanup.kdamonds_idxs = ['%d' % idx
                 for idx, k in enumerate(kdamonds)]
+        # TODO: Support multiple kdamonds, multiple contexts
+        monitoring_intervals = kdamonds[0].contexts[0].intervals
+    else:
+        # TODO: Support multiple kdamonds, multiple contexts
+        monitoring_intervals = data_for_cleanup.orig_kdamonds[
+                0].contexts[0].intervals
 
     data_for_cleanup.perf_pipe = _damon_result.start_monitoring_record(
-            args.out, args.output_type, args.output_permission)
+            args.out, args.output_type, args.output_permission,
+            monitoring_intervals)
     print('Press Ctrl+C to stop')
 
     if _damon_args.self_started_target(args):
-        while poll_target_pids(kdamonds, args.include_childs):
+        while poll_target_pids(kdamonds, args.include_child_tasks):
             time.sleep(1)
 
-    _damon.wait_current_kdamonds_turned_off()
+    _damon.wait_kdamonds_turned_off()
 
     cleanup_exit(0)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.3/src/damo/damo_report_raw.py` & `damo-1.8.4/src/damo/damo_report_raw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
+import json
 import os
 import sys
 
 import _damon_result
 import _damo_fmt_str
 
 def set_argparser(parser):
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
     parser.add_argument('--duration', type=float, metavar='<seconds>', nargs=2,
             help='start and end time offset for record to parse')
     parser.add_argument('--raw_number', action='store_true',
             help='use machine-friendly raw numbers')
+    parser.add_argument('--json', action='store_true',
+            help='print in json format')
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
@@ -33,14 +36,19 @@
                 (file_path, err))
         exit(1)
 
     if not result:
         print('no monitoring result in the file')
         exit(1)
 
+    if args.json:
+        print(json.dumps([r.to_kvpairs(args.raw_number)
+            for r in result.records], indent=4))
+        exit(0)
+
     for record in result.records:
         snapshots = record.snapshots
         if len(snapshots) == 0:
             continue
 
         base_time = snapshots[0].start_time
         print('base_time_absolute: %s\n' %
```

### Comparing `damo-1.8.3/src/damo/damo_schemes.py` & `damo-1.8.4/src/damo/damo_schemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import signal
 
 import _damon
 import _damon_args
 
 def cleanup_exit(exit_code):
     # ignore returning error, as kdamonds may already finished
-    _damon.turn_damon_off(kdamonds_idxs)
+    err = _damon.turn_damon_off(kdamonds_idxs)
     if err:
         print('failed to turn damon off (%s)' % err)
     err = _damon.stage_kdamonds(orig_kdamonds)
     if err:
         print('failed restoring previous kdamonds setup (%s)' % err)
     exit(exit_code)
 
@@ -50,13 +50,13 @@
 
     kdamonds_idxs = ['%d' % idx for idx, k in enumerate(kdamonds)]
 
     print('Press Ctrl+C to stop')
     if _damon_args.self_started_target(args):
         os.waitpid(kdamonds[0].contexts[0].targets[0].pid, 0)
     # damon will turn it off by itself if the target tasks are terminated.
-    _damon.wait_current_kdamonds_turned_off()
+    _damon.wait_kdamonds_turned_off()
 
     cleanup_exit(0)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.3/src/damo/damo_start.py` & `damo-1.8.4/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_stat.py` & `damo-1.8.4/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_stat_kdamonds.py` & `damo-1.8.4/src/damo/damo_stat_kdamonds.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,18 @@
     summary = [k.summary_str() for k in kdamonds]
     if json_format:
         print(json.dumps(summary, indent=4))
         return
     print('\n'.join(summary))
 
 def update_pr_kdamonds(json_format, raw_nr):
-    err = _damon.update_schemes_status()
+    kdamonds, err = _damon.update_read_kdamonds()
     if err:
         print(err)
         return
-    kdamonds = _damon.current_kdamonds()
     if json_format:
         print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
     else:
         for idx, k in enumerate(kdamonds):
             print('kdamond %d' % idx)
             print(_damo_fmt_str.indent_lines( k.to_str(raw_nr), 4))
```

### Comparing `damo-1.8.3/src/damo/damo_stat_regions.py` & `damo-1.8.4/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_stat_schemes.py` & `damo-1.8.4/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_stop.py` & `damo-1.8.4/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_translate_damos.py` & `damo-1.8.4/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_tune.py` & `damo-1.8.4/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_validate.py` & `damo-1.8.4/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo/damo_wss.py` & `damo-1.8.4/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.3/src/damo.egg-info/PKG-INFO` & `damo-1.8.4/src/damo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.3
+Version: 1.8.4
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.3/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.4/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -87,19 +87,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.3/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.4/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
@@ -153,61 +153,62 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 
-Deprecated Features
-===================
+Deprecated, or Will be Deprecated Features
+==========================================
 
-Below are features that deprecated, or will be deprecated.  If you depend on
-any of those, please report your usecase to the community via github issue,
-sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
+Below are features that recently deprecated, or will be deprecated.  If you
+depend on any of those, please report your usecase to the community via github
+issue, sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
 
---rbuf option of `damo record`
-------------------------------
 
-Deprecated.
+DAMON record binary format
+--------------------------
 
-Early versions of DAMON supported in-kernel direct monitoring results record
-file generation.  To control the overhead of it, DAMO allowed user to specify
-the size of buffer for the work.  The feature has not merged into the mainline,
-and discarded.  Hence the option was available for only few kernels that ported
-the feature.  For most of kernels, tracepoint based record file generation is
-being used, and the overhead of the approach is subtle.  Hence, the option has
-deprecated.
+Will be deprecated by 2023 Q3.
+
+At the beginning, DAMO used its special binary format, namely `record`.  It is
+designed for lightweight saving of the monitoring results.  It is difficult to
+read, and not that efficient compared to fancy compression techniques.  `json`
+based monitoring results can be easier to read, and more efficient when
+compression technique is used.  Hence, the format will be deprecated.  You may
+use `damo convert_record_format` to convert your old record binary format
+monitoring results files to the new format.
+
+
+`Python2 support
+----------------
+
+Deprecated.  Use Python3.
+
+For some old distros, DAMO initially supported Python2.  Because Python2 is
+really old now, the support has deprecated.  Please use Python3 or newer.
 
 
 DAMOS singline format
 ---------------------
 
 Deprecated.  Use `--damos_*` command line options or json format input.
 
 One-line scheme specification format like below was initially supported.
 Because it is not flexible for extension of features, it has deprecated now.
 You may use `--damos_*` command line options or json format instead.  You may
 use `damo translate_damos` to convert your old single line DAMOS schemes
 specification to the new json format.
 
 
-`Python2 support
-----------------
-
-Deprecated.  Use Python3.
-
-For some old distros, DAMO initially supported Python2.  Because Python2 is
-really old now, the support has deprecated.  Please use Python3 or newer.
-
-
-DAMON record binary format
---------------------------
+--rbuf option of `damo record`
+------------------------------
 
-Will be deprecated by 2023 Q3.
+Deprecated.
 
-At the beginning, DAMO used its special binary format, namely `record`.  It is
-designed for lightweight saving of the monitoring results.  It is difficult to
-read, and not that efficient compared to fancy compression techniques.  `json`
-based monitoring results can be easier to read, and more efficient when
-compression technique is used.  Hence, the format will be deprecated.  You may
-use `damo convert_record_format` to convert your old record binary format
-monitoring results files to the new format.
+Early versions of DAMON supported in-kernel direct monitoring results record
+file generation.  To control the overhead of it, DAMO allowed user to specify
+the size of buffer for the work.  The feature has not merged into the mainline,
+and discarded.  Hence the option was available for only few kernels that ported
+the feature.  For most of kernels, tracepoint based record file generation is
+being used, and the overhead of the approach is subtle.  Hence, the option has
+deprecated.
```

### Comparing `damo-1.8.3/src/damo.egg-info/SOURCES.txt` & `damo-1.8.4/src/damo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 src/damo/__init__.py
 src/damo/_damo_deprecated.py
 src/damo/_damo_deprecation_notice.py
 src/damo/_damo_dist.py
 src/damo/_damo_fmt_str.py
 src/damo/_damo_fs.py
 src/damo/_damo_paddr_layout.py
-src/damo/_damo_python2_support.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
 src/damo/_damon_dbgfs.py
 src/damo/_damon_result.py
 src/damo/_damon_sysfs.py
 src/damo/damo.py
@@ -23,15 +22,14 @@
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
 src/damo/damo_report.py
-src/damo/damo_report_json.py
 src/damo/damo_report_raw.py
 src/damo/damo_schemes.py
 src/damo/damo_start.py
 src/damo/damo_stat.py
 src/damo/damo_stat_kdamonds.py
 src/damo/damo_stat_regions.py
 src/damo/damo_stat_schemes.py
```

