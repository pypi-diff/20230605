# Comparing `tmp/vectorbt-0.25.3.tar.gz` & `tmp/vectorbt-0.25.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorbt-0.25.3.tar", last modified: Wed May 24 02:46:53 2023, max compression
+gzip compressed data, was "vectorbt-0.25.4.tar", last modified: Mon Jun  5 13:45:57 2023, max compression
```

## Comparing `vectorbt-0.25.3.tar` & `vectorbt-0.25.4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.308476 vectorbt-0.25.3/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.25.3/LICENSE.md
--rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.25.3/MANIFEST.in
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-05-24 02:46:53.308097 vectorbt-0.25.3/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8799 2023-01-15 23:29:02.000000 vectorbt-0.25.3/README.md
--rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2023-05-24 02:46:53.308545 vectorbt-0.25.3/setup.cfg
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2496 2023-05-24 01:57:30.000000 vectorbt-0.25.3/setup.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.252550 vectorbt-0.25.3/tests/
--rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.25.3/tests/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   133754 2023-04-26 17:23:51.000000 vectorbt-0.25.3/tests/test_base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    41687 2023-04-26 17:34:55.000000 vectorbt-0.25.3/tests/test_data.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    71129 2023-04-26 17:32:19.000000 vectorbt-0.25.3/tests/test_generic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   113482 2023-04-26 17:28:11.000000 vectorbt-0.25.3/tests/test_indicators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.25.3/tests/test_labels.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   340117 2023-05-05 05:23:25.000000 vectorbt-0.25.3/tests/test_portfolio.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   144385 2023-04-26 17:36:53.000000 vectorbt-0.25.3/tests/test_records.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.25.3/tests/test_returns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.25.3/tests/test_settings.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   116464 2023-04-26 17:22:30.000000 vectorbt-0.25.3/tests/test_signals.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.25.3/tests/test_utils.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.25.3/tests/utils.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.255303 vectorbt-0.25.3/vectorbt/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.25.3/vectorbt/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.25.3/vectorbt/_settings.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.25.3/vectorbt/_typing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2023-05-24 01:51:25.000000 vectorbt-0.25.3/vectorbt/_version.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.269518 vectorbt-0.25.3/vectorbt/base/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/base/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.25.3/vectorbt/base/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.25.3/vectorbt/base/array_wrapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/base/column_grouper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/base/combine_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/base/index_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.25.3/vectorbt/base/indexing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2023-05-05 05:01:15.000000 vectorbt-0.25.3/vectorbt/base/reshape_fns.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.271901 vectorbt-0.25.3/vectorbt/data/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.25.3/vectorbt/data/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30646 2023-05-24 01:51:18.000000 vectorbt-0.25.3/vectorbt/data/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.25.3/vectorbt/data/custom.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.25.3/vectorbt/data/updater.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.278178 vectorbt-0.25.3/vectorbt/generic/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/generic/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100299 2023-04-26 17:29:09.000000 vectorbt-0.25.3/vectorbt/generic/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/generic/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/generic/drawdowns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/generic/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    58884 2022-02-04 19:09:27.000000 vectorbt-0.25.3/vectorbt/generic/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.25.3/vectorbt/generic/plots_builder.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.25.3/vectorbt/generic/plotting.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/generic/ranges.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.25.3/vectorbt/generic/splitters.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.25.3/vectorbt/generic/stats_builder.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.281310 vectorbt-0.25.3/vectorbt/indicators/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.25.3/vectorbt/indicators/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/indicators/basic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/indicators/configs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.25.3/vectorbt/indicators/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/indicators/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.283013 vectorbt-0.25.3/vectorbt/labels/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.25.3/vectorbt/labels/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/labels/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/labels/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/labels/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.283824 vectorbt-0.25.3/vectorbt/messaging/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.25.3/vectorbt/messaging/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/messaging/telegram.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/ohlcv_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.289002 vectorbt-0.25.3/vectorbt/portfolio/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/portfolio/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   238538 2023-04-26 17:22:09.000000 vectorbt-0.25.3/vectorbt/portfolio/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/portfolio/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/portfolio/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.25.3/vectorbt/portfolio/logs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.25.3/vectorbt/portfolio/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/portfolio/orders.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/portfolio/trades.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/px_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.292162 vectorbt-0.25.3/vectorbt/records/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/records/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.25.3/vectorbt/records/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/records/col_mapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/records/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42640 2023-04-26 17:29:08.000000 vectorbt-0.25.3/vectorbt/records/mapped_array.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17680 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/records/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.295255 vectorbt-0.25.3/vectorbt/returns/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.25.3/vectorbt/returns/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.25.3/vectorbt/returns/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/returns/metrics.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.25.3/vectorbt/returns/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.25.3/vectorbt/returns/qs_adapter.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/root_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.298214 vectorbt-0.25.3/vectorbt/signals/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.25.3/vectorbt/signals/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/signals/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/signals/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.25.3/vectorbt/signals/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.25.3/vectorbt/signals/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/signals/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.299388 vectorbt-0.25.3/vectorbt/templates/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/templates/dark.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/templates/light.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/templates/seaborn.json
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.307670 vectorbt-0.25.3/vectorbt/utils/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/utils/array_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.25.3/vectorbt/utils/attr_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/checks.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/colors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.25.3/vectorbt/utils/config.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.25.3/vectorbt/utils/datetime_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.25.3/vectorbt/utils/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.25.3/vectorbt/utils/docs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.25.3/vectorbt/utils/enum_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.25.3/vectorbt/utils/figure.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3037 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/image_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6085 2023-04-26 17:28:11.000000 vectorbt-0.25.3/vectorbt/utils/mapping.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/math_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/module_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.25.3/vectorbt/utils/params.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/random_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.25.3/vectorbt/utils/requests_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.25.3/vectorbt/utils/schedule_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.25.3/vectorbt/utils/tags.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.25.3/vectorbt/utils/template.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-05-24 02:46:53.256688 vectorbt-0.25.3/vectorbt.egg-info/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-05-24 02:46:53.000000 vectorbt-0.25.3/vectorbt.egg-info/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2023-05-24 02:46:53.000000 vectorbt-0.25.3/vectorbt.egg-info/SOURCES.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2023-05-24 02:46:53.000000 vectorbt-0.25.3/vectorbt.egg-info/dependency_links.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)      476 2023-05-24 02:46:53.000000 vectorbt-0.25.3/vectorbt.egg-info/requires.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2023-05-24 02:46:53.000000 vectorbt-0.25.3/vectorbt.egg-info/top_level.txt
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.959469 vectorbt-0.25.4/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.25.4/LICENSE.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.25.4/MANIFEST.in
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-06-05 13:45:57.959063 vectorbt-0.25.4/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8799 2023-01-15 23:29:02.000000 vectorbt-0.25.4/README.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2023-06-05 13:45:57.959534 vectorbt-0.25.4/setup.cfg
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2496 2023-05-24 01:57:30.000000 vectorbt-0.25.4/setup.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.909280 vectorbt-0.25.4/tests/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.25.4/tests/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   133754 2023-04-26 17:23:51.000000 vectorbt-0.25.4/tests/test_base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    41687 2023-04-26 17:34:55.000000 vectorbt-0.25.4/tests/test_data.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    71129 2023-04-26 17:32:19.000000 vectorbt-0.25.4/tests/test_generic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   113482 2023-04-26 17:28:11.000000 vectorbt-0.25.4/tests/test_indicators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.25.4/tests/test_labels.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   340117 2023-05-05 05:23:25.000000 vectorbt-0.25.4/tests/test_portfolio.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   144385 2023-04-26 17:36:53.000000 vectorbt-0.25.4/tests/test_records.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.25.4/tests/test_returns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.25.4/tests/test_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   116464 2023-04-26 17:22:30.000000 vectorbt-0.25.4/tests/test_signals.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.25.4/tests/test_utils.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.25.4/tests/utils.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.911874 vectorbt-0.25.4/vectorbt/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.25.4/vectorbt/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.25.4/vectorbt/_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.25.4/vectorbt/_typing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2023-06-05 13:44:17.000000 vectorbt-0.25.4/vectorbt/_version.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.916407 vectorbt-0.25.4/vectorbt/base/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/base/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.25.4/vectorbt/base/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.25.4/vectorbt/base/array_wrapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/base/column_grouper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/base/combine_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/base/index_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.25.4/vectorbt/base/indexing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2023-05-05 05:01:15.000000 vectorbt-0.25.4/vectorbt/base/reshape_fns.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.918816 vectorbt-0.25.4/vectorbt/data/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.25.4/vectorbt/data/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30646 2023-05-24 01:51:18.000000 vectorbt-0.25.4/vectorbt/data/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.25.4/vectorbt/data/custom.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.25.4/vectorbt/data/updater.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.926595 vectorbt-0.25.4/vectorbt/generic/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/generic/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100299 2023-04-26 17:29:09.000000 vectorbt-0.25.4/vectorbt/generic/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/generic/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/generic/drawdowns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/generic/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    58884 2022-02-04 19:09:27.000000 vectorbt-0.25.4/vectorbt/generic/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.25.4/vectorbt/generic/plots_builder.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.25.4/vectorbt/generic/plotting.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/generic/ranges.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.25.4/vectorbt/generic/splitters.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.25.4/vectorbt/generic/stats_builder.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.930072 vectorbt-0.25.4/vectorbt/indicators/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.25.4/vectorbt/indicators/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/indicators/basic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/indicators/configs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.25.4/vectorbt/indicators/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/indicators/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.931593 vectorbt-0.25.4/vectorbt/labels/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.25.4/vectorbt/labels/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/labels/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/labels/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/labels/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.932367 vectorbt-0.25.4/vectorbt/messaging/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.25.4/vectorbt/messaging/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/messaging/telegram.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/ohlcv_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.939690 vectorbt-0.25.4/vectorbt/portfolio/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/portfolio/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   238538 2023-04-26 17:22:09.000000 vectorbt-0.25.4/vectorbt/portfolio/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/portfolio/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/portfolio/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.25.4/vectorbt/portfolio/logs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.25.4/vectorbt/portfolio/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/portfolio/orders.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/portfolio/trades.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/px_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.942939 vectorbt-0.25.4/vectorbt/records/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/records/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.25.4/vectorbt/records/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/records/col_mapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/records/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42640 2023-04-26 17:29:08.000000 vectorbt-0.25.4/vectorbt/records/mapped_array.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17680 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/records/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.945313 vectorbt-0.25.4/vectorbt/returns/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.25.4/vectorbt/returns/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.25.4/vectorbt/returns/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/returns/metrics.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.25.4/vectorbt/returns/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.25.4/vectorbt/returns/qs_adapter.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/root_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.948659 vectorbt-0.25.4/vectorbt/signals/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.25.4/vectorbt/signals/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/signals/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/signals/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.25.4/vectorbt/signals/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.25.4/vectorbt/signals/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/signals/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.950115 vectorbt-0.25.4/vectorbt/templates/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/templates/dark.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/templates/light.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/templates/seaborn.json
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.958567 vectorbt-0.25.4/vectorbt/utils/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/utils/array_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.25.4/vectorbt/utils/attr_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/checks.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/colors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.25.4/vectorbt/utils/config.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.25.4/vectorbt/utils/datetime_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.25.4/vectorbt/utils/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.25.4/vectorbt/utils/docs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.25.4/vectorbt/utils/enum_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.25.4/vectorbt/utils/figure.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3178 2023-06-05 13:00:32.000000 vectorbt-0.25.4/vectorbt/utils/image_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6085 2023-04-26 17:28:11.000000 vectorbt-0.25.4/vectorbt/utils/mapping.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/math_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/module_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.25.4/vectorbt/utils/params.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/random_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.25.4/vectorbt/utils/requests_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.25.4/vectorbt/utils/schedule_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.25.4/vectorbt/utils/tags.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.25.4/vectorbt/utils/template.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2023-06-05 13:45:57.913179 vectorbt-0.25.4/vectorbt.egg-info/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9941 2023-06-05 13:45:57.000000 vectorbt-0.25.4/vectorbt.egg-info/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2023-06-05 13:45:57.000000 vectorbt-0.25.4/vectorbt.egg-info/SOURCES.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2023-06-05 13:45:57.000000 vectorbt-0.25.4/vectorbt.egg-info/dependency_links.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      476 2023-06-05 13:45:57.000000 vectorbt-0.25.4/vectorbt.egg-info/requires.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2023-06-05 13:45:57.000000 vectorbt-0.25.4/vectorbt.egg-info/top_level.txt
```

### Comparing `vectorbt-0.25.3/LICENSE.md` & `vectorbt-0.25.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/PKG-INFO` & `vectorbt-0.25.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorbt
-Version: 0.25.3
+Version: 0.25.4
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/polakowo/vectorbt
 Author: Oleg Polakow
 Author-email: olegpolakow@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vectorbt-0.25.3/README.md` & `vectorbt-0.25.4/README.md`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/setup.py` & `vectorbt-0.25.4/setup.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_base.py` & `vectorbt-0.25.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_data.py` & `vectorbt-0.25.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_generic.py` & `vectorbt-0.25.4/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_indicators.py` & `vectorbt-0.25.4/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_labels.py` & `vectorbt-0.25.4/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_portfolio.py` & `vectorbt-0.25.4/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_records.py` & `vectorbt-0.25.4/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_returns.py` & `vectorbt-0.25.4/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_signals.py` & `vectorbt-0.25.4/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/test_utils.py` & `vectorbt-0.25.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/tests/utils.py` & `vectorbt-0.25.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/__init__.py` & `vectorbt-0.25.4/vectorbt/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/_settings.py` & `vectorbt-0.25.4/vectorbt/_settings.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/_typing.py` & `vectorbt-0.25.4/vectorbt/_typing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/accessors.py` & `vectorbt-0.25.4/vectorbt/base/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/array_wrapper.py` & `vectorbt-0.25.4/vectorbt/base/array_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/column_grouper.py` & `vectorbt-0.25.4/vectorbt/base/column_grouper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/combine_fns.py` & `vectorbt-0.25.4/vectorbt/base/combine_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/index_fns.py` & `vectorbt-0.25.4/vectorbt/base/index_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/indexing.py` & `vectorbt-0.25.4/vectorbt/base/indexing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/base/reshape_fns.py` & `vectorbt-0.25.4/vectorbt/base/reshape_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/data/__init__.py` & `vectorbt-0.25.4/vectorbt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/data/base.py` & `vectorbt-0.25.4/vectorbt/data/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/data/custom.py` & `vectorbt-0.25.4/vectorbt/data/custom.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/data/updater.py` & `vectorbt-0.25.4/vectorbt/data/updater.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/__init__.py` & `vectorbt-0.25.4/vectorbt/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/accessors.py` & `vectorbt-0.25.4/vectorbt/generic/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/decorators.py` & `vectorbt-0.25.4/vectorbt/generic/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/drawdowns.py` & `vectorbt-0.25.4/vectorbt/generic/drawdowns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/enums.py` & `vectorbt-0.25.4/vectorbt/generic/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/nb.py` & `vectorbt-0.25.4/vectorbt/generic/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/plots_builder.py` & `vectorbt-0.25.4/vectorbt/generic/plots_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/plotting.py` & `vectorbt-0.25.4/vectorbt/generic/plotting.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/ranges.py` & `vectorbt-0.25.4/vectorbt/generic/ranges.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/splitters.py` & `vectorbt-0.25.4/vectorbt/generic/splitters.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/generic/stats_builder.py` & `vectorbt-0.25.4/vectorbt/generic/stats_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/indicators/__init__.py` & `vectorbt-0.25.4/vectorbt/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/indicators/basic.py` & `vectorbt-0.25.4/vectorbt/indicators/basic.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/indicators/configs.py` & `vectorbt-0.25.4/vectorbt/indicators/configs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/indicators/factory.py` & `vectorbt-0.25.4/vectorbt/indicators/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/indicators/nb.py` & `vectorbt-0.25.4/vectorbt/indicators/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/labels/__init__.py` & `vectorbt-0.25.4/vectorbt/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/labels/enums.py` & `vectorbt-0.25.4/vectorbt/labels/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/labels/generators.py` & `vectorbt-0.25.4/vectorbt/labels/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/labels/nb.py` & `vectorbt-0.25.4/vectorbt/labels/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/messaging/telegram.py` & `vectorbt-0.25.4/vectorbt/messaging/telegram.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/ohlcv_accessors.py` & `vectorbt-0.25.4/vectorbt/ohlcv_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/__init__.py` & `vectorbt-0.25.4/vectorbt/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/base.py` & `vectorbt-0.25.4/vectorbt/portfolio/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/decorators.py` & `vectorbt-0.25.4/vectorbt/portfolio/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/enums.py` & `vectorbt-0.25.4/vectorbt/portfolio/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/logs.py` & `vectorbt-0.25.4/vectorbt/portfolio/logs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/nb.py` & `vectorbt-0.25.4/vectorbt/portfolio/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/orders.py` & `vectorbt-0.25.4/vectorbt/portfolio/orders.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/portfolio/trades.py` & `vectorbt-0.25.4/vectorbt/portfolio/trades.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/px_accessors.py` & `vectorbt-0.25.4/vectorbt/px_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/__init__.py` & `vectorbt-0.25.4/vectorbt/records/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/base.py` & `vectorbt-0.25.4/vectorbt/records/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/col_mapper.py` & `vectorbt-0.25.4/vectorbt/records/col_mapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/decorators.py` & `vectorbt-0.25.4/vectorbt/records/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/mapped_array.py` & `vectorbt-0.25.4/vectorbt/records/mapped_array.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/records/nb.py` & `vectorbt-0.25.4/vectorbt/records/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/returns/accessors.py` & `vectorbt-0.25.4/vectorbt/returns/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/returns/metrics.py` & `vectorbt-0.25.4/vectorbt/returns/metrics.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/returns/nb.py` & `vectorbt-0.25.4/vectorbt/returns/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/returns/qs_adapter.py` & `vectorbt-0.25.4/vectorbt/returns/qs_adapter.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/root_accessors.py` & `vectorbt-0.25.4/vectorbt/root_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/__init__.py` & `vectorbt-0.25.4/vectorbt/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/accessors.py` & `vectorbt-0.25.4/vectorbt/signals/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/enums.py` & `vectorbt-0.25.4/vectorbt/signals/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/factory.py` & `vectorbt-0.25.4/vectorbt/signals/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/generators.py` & `vectorbt-0.25.4/vectorbt/signals/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/signals/nb.py` & `vectorbt-0.25.4/vectorbt/signals/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/templates/dark.json` & `vectorbt-0.25.4/vectorbt/templates/dark.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/templates/light.json` & `vectorbt-0.25.4/vectorbt/templates/light.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/templates/seaborn.json` & `vectorbt-0.25.4/vectorbt/templates/seaborn.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/__init__.py` & `vectorbt-0.25.4/vectorbt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/array_.py` & `vectorbt-0.25.4/vectorbt/utils/array_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/attr_.py` & `vectorbt-0.25.4/vectorbt/utils/attr_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/checks.py` & `vectorbt-0.25.4/vectorbt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/colors.py` & `vectorbt-0.25.4/vectorbt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/config.py` & `vectorbt-0.25.4/vectorbt/utils/config.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/datetime_.py` & `vectorbt-0.25.4/vectorbt/utils/datetime_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/decorators.py` & `vectorbt-0.25.4/vectorbt/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/docs.py` & `vectorbt-0.25.4/vectorbt/utils/docs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/enum_.py` & `vectorbt-0.25.4/vectorbt/utils/enum_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/figure.py` & `vectorbt-0.25.4/vectorbt/utils/figure.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/image_.py` & `vectorbt-0.25.4/vectorbt/utils/image_.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,30 +52,34 @@
 
             Should take subset of `index`, `*args`, and `**kwargs`, and return either a Plotly figure,
             image that can be read by `imageio.imread`, or a NumPy array.
         *args: Positional arguments passed to `plot_func`.
         delta (int): Window size of each iteration.
         step (int): Step of each iteration.
         fps (int): Frames per second.
+
+            Will be translated to `duration` by `1000 / fps`.
         writer_kwargs (dict): Keyword arguments passed to `imageio.get_writer`.
         show_progress (bool): Whether to show the progress bar.
         tqdm_kwargs (dict): Keyword arguments passed to `tqdm`.
         to_image_kwargs (dict): Keyword arguments passed to `plotly.graph_objects.Figure.to_image`.
         **kwargs: Keyword arguments passed to `plot_func`.
     """
     if writer_kwargs is None:
         writer_kwargs = {}
+    if "duration" not in writer_kwargs:
+        writer_kwargs["duration"] = 1000 / fps
     if tqdm_kwargs is None:
         tqdm_kwargs = {}
     if to_image_kwargs is None:
         to_image_kwargs = {}
     if delta is None:
         delta = len(index) // 2
 
-    with imageio.get_writer(fname, fps=fps, **writer_kwargs) as writer:
+    with imageio.get_writer(fname, **writer_kwargs) as writer:
         for i in tqdm(range(0, len(index) - delta, step), disable=not show_progress, **tqdm_kwargs):
             fig = plot_func(index[i:i + delta], *args, **kwargs)
             if isinstance(fig, (go.Figure, go.FigureWidget)):
                 fig = fig.to_image(format="png", **to_image_kwargs)
             if not isinstance(fig, np.ndarray):
                 fig = imageio.imread(fig)
             writer.append_data(fig)
```

### Comparing `vectorbt-0.25.3/vectorbt/utils/mapping.py` & `vectorbt-0.25.4/vectorbt/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/math_.py` & `vectorbt-0.25.4/vectorbt/utils/math_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/module_.py` & `vectorbt-0.25.4/vectorbt/utils/module_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/params.py` & `vectorbt-0.25.4/vectorbt/utils/params.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/requests_.py` & `vectorbt-0.25.4/vectorbt/utils/requests_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/schedule_.py` & `vectorbt-0.25.4/vectorbt/utils/schedule_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/tags.py` & `vectorbt-0.25.4/vectorbt/utils/tags.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt/utils/template.py` & `vectorbt-0.25.4/vectorbt/utils/template.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.25.3/vectorbt.egg-info/PKG-INFO` & `vectorbt-0.25.4/vectorbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorbt
-Version: 0.25.3
+Version: 0.25.4
 Summary: Python library for backtesting and analyzing trading strategies at scale
 Home-page: https://github.com/polakowo/vectorbt
 Author: Oleg Polakow
 Author-email: olegpolakow@gmail.com
 License: Apache 2.0 with Commons Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vectorbt-0.25.3/vectorbt.egg-info/SOURCES.txt` & `vectorbt-0.25.4/vectorbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

