# Comparing `tmp/pandas_stubs-2.0.1.230501.tar.gz` & `tmp/pandas_stubs-2.0.2.230605.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_stubs-2.0.1.230501.tar", max compression
+gzip compressed data, was "pandas_stubs-2.0.2.230605.tar", max compression
```

## Comparing `pandas_stubs-2.0.1.230501.tar` & `pandas_stubs-2.0.2.230605.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.0.1.230501/LICENSE
--rw-r--r--   0        0        0     3717 2023-04-05 02:20:38.238520 pandas_stubs-2.0.1.230501/pandas-stubs/__init__.pyi
--rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.0.1.230501/pandas-stubs/_config/__init__.pyi
--rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-2.0.1.230501/pandas-stubs/_config/config.pyi
--rw-r--r--   0        0        0      251 2022-08-08 01:00:32.265011 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/__init__.pyi
--rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/indexing.pyi
--rw-r--r--   0        0        0     8318 2023-04-30 02:38:30.381115 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/interval.pyi
--rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/json.pyi
--rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/lib.pyi
--rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/missing.pyi
--rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/ops_dispatch.pyi
--rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/properties.pyi
--rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/sparse.pyi
--rw-r--r--   0        0        0      573 2022-12-28 15:28:49.657656 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/__init__.pyi
--rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/base.pyi
--rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/conversion.pyi
--rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/dtypes.pyi
--rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/nattype.pyi
--rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/np_datetime.pyi
--rw-r--r--   0        0        0     8230 2023-02-23 17:31:11.763588 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/offsets.pyi
--rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/parsing.pyi
--rw-r--r--   0        0        0     6525 2023-02-23 17:31:11.764590 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/period.pyi
--rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/strptime.pyi
--rw-r--r--   0        0        0    14082 2023-04-05 02:20:38.239523 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timedeltas.pyi
--rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timestamps.pyi
--rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/tzconversion.pyi
--rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/vectorized.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.0.1.230501/pandas-stubs/_libs/window/__init__.pyi
--rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-2.0.1.230501/pandas-stubs/_testing/__init__.pyi
--rw-r--r--   0        0        0    15505 2023-04-25 19:40:11.552225 pandas_stubs-2.0.1.230501/pandas-stubs/_typing.pyi
--rw-r--r--   0        0        0      124 2023-05-01 21:56:21.743993 pandas_stubs-2.0.1.230501/pandas-stubs/_version.pyi
--rw-r--r--   0        0        0       94 2022-08-08 01:00:32.471998 pandas_stubs-2.0.1.230501/pandas-stubs/api/__init__.pyi
--rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.0.1.230501/pandas-stubs/api/extensions/__init__.pyi
--rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.0.1.230501/pandas-stubs/api/indexers/__init__.pyi
--rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.0.1.230501/pandas-stubs/api/interchange/__init__.pyi
--rw-r--r--   0        0        0     1959 2022-12-28 15:28:49.665655 pandas_stubs-2.0.1.230501/pandas-stubs/api/types/__init__.pyi
--rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.0.1.230501/pandas-stubs/arrays/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.0.1.230501/pandas-stubs/core/__init__.pyi
--rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-2.0.1.230501/pandas-stubs/core/accessor.pyi
--rw-r--r--   0        0        0     2309 2023-05-01 21:55:22.558166 pandas_stubs-2.0.1.230501/pandas-stubs/core/algorithms.pyi
--rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.0.1.230501/pandas-stubs/core/api.pyi
--rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-2.0.1.230501/pandas-stubs/core/arraylike.pyi
--rw-r--r--   0        0        0      726 2022-08-10 19:03:04.648579 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/__init__.pyi
--rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/arrow/dtype.pyi
--rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/base.pyi
--rw-r--r--   0        0        0      954 2023-02-27 22:18:36.854305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/boolean.pyi
--rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/categorical.pyi
--rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimelike.pyi
--rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimes.pyi
--rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/floating.pyi
--rw-r--r--   0        0        0     1010 2023-02-27 03:32:24.827813 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/integer.pyi
--rw-r--r--   0        0        0     2689 2023-05-01 21:55:22.558166 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/interval.pyi
--rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/masked.pyi
--rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numeric.pyi
--rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numpy_.pyi
--rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/period.pyi
--rw-r--r--   0        0        0      210 2022-12-28 15:28:49.674654 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/__init__.pyi
--rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/accessor.pyi
--rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/array.pyi
--rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/dtype.pyi
--rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/string_.pyi
--rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/timedeltas.pyi
--rw-r--r--   0        0        0     2681 2023-04-01 02:35:39.717031 pandas_stubs-2.0.1.230501/pandas-stubs/core/base.pyi
--rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.0.1.230501/pandas-stubs/core/common.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/__init__.pyi
--rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/align.pyi
--rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/api.pyi
--rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/common.pyi
--rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/engines.pyi
--rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/eval.pyi
--rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expr.pyi
--rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expressions.pyi
--rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/ops.pyi
--rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/parsing.pyi
--rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/pytables.pyi
--rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/scope.pyi
--rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-2.0.1.230501/pandas-stubs/core/config_init.pyi
--rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.0.1.230501/pandas-stubs/core/construction.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/__init__.pyi
--rw-r--r--   0        0        0     1625 2022-12-28 15:28:49.680655 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/api.pyi
--rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/base.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/cast.pyi
--rw-r--r--   0        0        0     2377 2023-02-23 17:31:11.770587 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/common.pyi
--rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/concat.pyi
--rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/dtypes.pyi
--rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/generic.pyi
--rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/inference.pyi
--rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/missing.pyi
--rw-r--r--   0        0        0    65002 2023-05-01 14:59:34.187821 pandas_stubs-2.0.1.230501/pandas-stubs/core/frame.pyi
--rw-r--r--   0        0        0    15017 2023-04-25 19:40:11.553225 pandas_stubs-2.0.1.230501/pandas-stubs/core/generic.pyi
--rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/__init__.pyi
--rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/base.pyi
--rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/categorical.pyi
--rw-r--r--   0        0        0    12835 2023-03-04 20:30:27.574572 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/generic.pyi
--rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/groupby.pyi
--rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/grouper.pyi
--rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/ops.pyi
--rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexers.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/__init__.pyi
--rw-r--r--   0        0        0    12913 2023-04-05 02:20:38.241521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/accessors.pyi
--rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/api.pyi
--rw-r--r--   0        0        0    10393 2023-04-12 19:14:53.209396 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/base.pyi
--rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/category.pyi
--rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimelike.pyi
--rw-r--r--   0        0        0     4393 2023-04-05 02:20:38.243522 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimes.pyi
--rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/extension.pyi
--rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/frozen.pyi
--rw-r--r--   0        0        0    13292 2023-05-01 21:55:22.559166 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/interval.pyi
--rw-r--r--   0        0        0     5428 2023-04-01 02:35:39.720026 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/multi.pyi
--rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/period.pyi
--rw-r--r--   0        0        0     2853 2023-04-05 02:20:38.244521 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/range.pyi
--rw-r--r--   0        0        0     2713 2023-02-23 17:31:11.783587 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/timedeltas.pyi
--rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.0.1.230501/pandas-stubs/core/indexing.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/__init__.pyi
--rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/dataframe_protocol.pyi
--rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/from_dataframe.pyi
--rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.0.1.230501/pandas-stubs/core/missing.pyi
--rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/__init__.pyi
--rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/array_ops.pyi
--rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/common.pyi
--rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/dispatch.pyi
--rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/docstrings.pyi
--rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/invalid.pyi
--rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/mask_ops.pyi
--rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-2.0.1.230501/pandas-stubs/core/resample.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/__init__.pyi
--rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/api.pyi
--rw-r--r--   0        0        0     2872 2023-04-12 19:14:53.210397 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/concat.pyi
--rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/encoding.pyi
--rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/melt.pyi
--rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/merge.pyi
--rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/pivot.pyi
--rw-r--r--   0        0        0     7900 2023-04-05 02:20:38.246521 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/tile.pyi
--rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/util.pyi
--rw-r--r--   0        0        0    63031 2023-05-01 21:55:22.560166 pandas_stubs-2.0.1.230501/pandas-stubs/core/series.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.0.1.230501/pandas-stubs/core/sparse/__init__.pyi
--rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.0.1.230501/pandas-stubs/core/strings.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/__init__.pyi
--rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/datetimes.pyi
--rw-r--r--   0        0        0     1140 2023-04-25 19:40:11.555225 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/numeric.pyi
--rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/timedeltas.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.0.1.230501/pandas-stubs/core/util/__init__.pyi
--rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.0.1.230501/pandas-stubs/core/util/hashing.pyi
--rw-r--r--   0        0        0      274 2022-08-08 01:00:33.545825 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/__init__.pyi
--rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/ewm.pyi
--rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/expanding.pyi
--rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-2.0.1.230501/pandas-stubs/core/window/rolling.pyi
--rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.0.1.230501/pandas-stubs/errors/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.0.1.230501/pandas-stubs/io/__init__.pyi
--rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.0.1.230501/pandas-stubs/io/api.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboard/__init__.pyi
--rw-r--r--   0        0        0     7153 2023-04-25 19:40:11.555225 pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboards.pyi
--rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.0.1.230501/pandas-stubs/io/common.pyi
--rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/__init__.pyi
--rw-r--r--   0        0        0     7816 2023-04-25 19:40:11.556233 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_base.pyi
--rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_util.pyi
--rw-r--r--   0        0        0      446 2023-04-25 19:40:11.557224 pandas_stubs-2.0.1.230501/pandas-stubs/io/feather_format.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/__init__.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/css.pyi
--rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/format.pyi
--rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style.pyi
--rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style_render.pyi
--rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.0.1.230501/pandas-stubs/io/gbq.pyi
--rw-r--r--   0        0        0     1493 2023-04-25 19:40:11.557224 pandas_stubs-2.0.1.230501/pandas-stubs/io/html.pyi
--rw-r--r--   0        0        0      170 2022-08-29 12:14:24.789359 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/__init__.pyi
--rw-r--r--   0        0        0     4377 2023-04-25 19:40:11.558224 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_json.pyi
--rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_normalize.pyi
--rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_table_schema.pyi
--rw-r--r--   0        0        0      393 2023-04-25 19:40:11.558224 pandas_stubs-2.0.1.230501/pandas-stubs/io/orc.pyi
--rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.0.1.230501/pandas-stubs/io/parquet.pyi
--rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/__init__.pyi
--rw-r--r--   0        0        0    16138 2023-04-25 19:40:11.559237 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/readers.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers.pyi
--rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.0.1.230501/pandas-stubs/io/pickle.pyi
--rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-2.0.1.230501/pandas-stubs/io/pytables.pyi
--rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/__init__.pyi
--rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sas7bdat.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sas_xport.pyi
--rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sasreader.pyi
--rw-r--r--   0        0        0      361 2023-04-25 19:40:11.560224 pandas_stubs-2.0.1.230501/pandas-stubs/io/spss.pyi
--rw-r--r--   0        0        0     5312 2023-04-25 19:40:11.560224 pandas_stubs-2.0.1.230501/pandas-stubs/io/sql.pyi
--rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.0.1.230501/pandas-stubs/io/stata.pyi
--rw-r--r--   0        0        0     1126 2023-04-25 19:40:11.561224 pandas_stubs-2.0.1.230501/pandas-stubs/io/xml.pyi
--rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/__init__.pyi
--rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_core.pyi
--rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_misc.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.0.1.230501/pandas-stubs/py.typed
--rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.0.1.230501/pandas-stubs/testing.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.614504 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/__init__.pyi
--rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/api.pyi
--rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/frequencies.pyi
--rw-r--r--   0        0        0     4142 2023-05-01 21:55:22.561166 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/holiday.pyi
--rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.0.1.230501/pandas-stubs/tseries/offsets.pyi
--rw-r--r--   0        0        0      255 2022-12-28 15:28:49.723655 pandas_stubs-2.0.1.230501/pandas-stubs/util/__init__.pyi
--rw-r--r--   0        0        0     1230 2023-02-04 17:09:12.332423 pandas_stubs-2.0.1.230501/pandas-stubs/util/_decorators.pyi
--rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.0.1.230501/pandas-stubs/util/_doctools.pyi
--rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.0.1.230501/pandas-stubs/util/_exceptions.pyi
--rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.0.1.230501/pandas-stubs/util/_print_versions.pyi
--rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.0.1.230501/pandas-stubs/util/_tester.pyi
--rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.0.1.230501/pandas-stubs/util/_validators.pyi
--rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.0.1.230501/pandas-stubs/util/version/__init__.pyi
--rw-r--r--   0        0        0     6935 2023-05-01 21:55:48.619914 pandas_stubs-2.0.1.230501/pyproject.toml
--rw-r--r--   0        0        0     8415 2023-04-12 21:57:46.990004 pandas_stubs-2.0.1.230501/README.md
--rw-r--r--   0        0        0    10415 1970-01-01 00:00:00.000000 pandas_stubs-2.0.1.230501/setup.py
--rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 pandas_stubs-2.0.1.230501/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.0.2.230605/LICENSE
+-rw-r--r--   0        0        0     3805 2023-05-22 14:12:55.264847 pandas_stubs-2.0.2.230605/pandas-stubs/__init__.pyi
+-rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.0.2.230605/pandas-stubs/_config/__init__.pyi
+-rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-2.0.2.230605/pandas-stubs/_config/config.pyi
+-rw-r--r--   0        0        0      285 2023-05-22 14:12:55.265853 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/__init__.pyi
+-rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/indexing.pyi
+-rw-r--r--   0        0        0     8341 2023-06-05 12:34:31.503869 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/interval.pyi
+-rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/json.pyi
+-rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/lib.pyi
+-rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/missing.pyi
+-rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/ops_dispatch.pyi
+-rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/properties.pyi
+-rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/sparse.pyi
+-rw-r--r--   0        0        0      666 2023-05-22 14:12:55.265853 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/__init__.pyi
+-rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/base.pyi
+-rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/conversion.pyi
+-rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/dtypes.pyi
+-rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/nattype.pyi
+-rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/np_datetime.pyi
+-rw-r--r--   0        0        0     8311 2023-05-22 14:12:55.266819 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/offsets.pyi
+-rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/parsing.pyi
+-rw-r--r--   0        0        0     6542 2023-05-22 14:12:55.267817 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/period.pyi
+-rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/strptime.pyi
+-rw-r--r--   0        0        0    14082 2023-04-05 02:20:38.239523 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/timedeltas.pyi
+-rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/timestamps.pyi
+-rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/tzconversion.pyi
+-rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/vectorized.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.0.2.230605/pandas-stubs/_libs/window/__init__.pyi
+-rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-2.0.2.230605/pandas-stubs/_testing/__init__.pyi
+-rw-r--r--   0        0        0    16274 2023-06-05 12:34:31.504832 pandas_stubs-2.0.2.230605/pandas-stubs/_typing.pyi
+-rw-r--r--   0        0        0      124 2023-06-05 12:37:30.685555 pandas_stubs-2.0.2.230605/pandas-stubs/_version.pyi
+-rw-r--r--   0        0        0      141 2023-06-05 12:34:31.504832 pandas_stubs-2.0.2.230605/pandas-stubs/api/__init__.pyi
+-rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.0.2.230605/pandas-stubs/api/extensions/__init__.pyi
+-rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.0.2.230605/pandas-stubs/api/indexers/__init__.pyi
+-rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.0.2.230605/pandas-stubs/api/interchange/__init__.pyi
+-rw-r--r--   0        0        0     2020 2023-06-05 12:34:31.505846 pandas_stubs-2.0.2.230605/pandas-stubs/api/types/__init__.pyi
+-rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.0.2.230605/pandas-stubs/arrays/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.0.2.230605/pandas-stubs/core/__init__.pyi
+-rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-2.0.2.230605/pandas-stubs/core/accessor.pyi
+-rw-r--r--   0        0        0     2309 2023-05-01 21:55:22.558166 pandas_stubs-2.0.2.230605/pandas-stubs/core/algorithms.pyi
+-rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.0.2.230605/pandas-stubs/core/api.pyi
+-rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-2.0.2.230605/pandas-stubs/core/arraylike.pyi
+-rw-r--r--   0        0        0      924 2023-05-22 14:12:55.269816 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/__init__.pyi
+-rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/arrow/dtype.pyi
+-rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/base.pyi
+-rw-r--r--   0        0        0      970 2023-05-22 14:12:55.269816 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/boolean.pyi
+-rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/categorical.pyi
+-rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/datetimelike.pyi
+-rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/datetimes.pyi
+-rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/floating.pyi
+-rw-r--r--   0        0        0     1028 2023-05-22 14:12:55.270817 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/integer.pyi
+-rw-r--r--   0        0        0     2689 2023-05-01 21:55:22.558166 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/interval.pyi
+-rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/masked.pyi
+-rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/numeric.pyi
+-rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/numpy_.pyi
+-rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/period.pyi
+-rw-r--r--   0        0        0      285 2023-05-22 14:12:55.271819 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/__init__.pyi
+-rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/accessor.pyi
+-rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/array.pyi
+-rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/dtype.pyi
+-rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/string_.pyi
+-rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/timedeltas.pyi
+-rw-r--r--   0        0        0     2681 2023-04-01 02:35:39.717031 pandas_stubs-2.0.2.230605/pandas-stubs/core/base.pyi
+-rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.0.2.230605/pandas-stubs/core/common.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/__init__.pyi
+-rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/align.pyi
+-rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/api.pyi
+-rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/common.pyi
+-rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/engines.pyi
+-rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/eval.pyi
+-rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/expr.pyi
+-rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/expressions.pyi
+-rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/ops.pyi
+-rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/parsing.pyi
+-rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/pytables.pyi
+-rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/scope.pyi
+-rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-2.0.2.230605/pandas-stubs/core/config_init.pyi
+-rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.0.2.230605/pandas-stubs/core/construction.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/__init__.pyi
+-rw-r--r--   0        0        0     1686 2023-06-05 12:34:31.505846 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/api.pyi
+-rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/base.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/cast.pyi
+-rw-r--r--   0        0        0     2450 2023-06-05 12:34:31.506833 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/common.pyi
+-rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/concat.pyi
+-rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/dtypes.pyi
+-rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/generic.pyi
+-rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/inference.pyi
+-rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/missing.pyi
+-rw-r--r--   0        0        0    69055 2023-06-05 12:34:31.507869 pandas_stubs-2.0.2.230605/pandas-stubs/core/frame.pyi
+-rw-r--r--   0        0        0    15017 2023-04-25 19:40:11.553225 pandas_stubs-2.0.2.230605/pandas-stubs/core/generic.pyi
+-rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/base.pyi
+-rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/categorical.pyi
+-rw-r--r--   0        0        0    12079 2023-05-22 14:12:55.273815 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/generic.pyi
+-rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/groupby.pyi
+-rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/grouper.pyi
+-rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/ops.pyi
+-rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexers.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/__init__.pyi
+-rw-r--r--   0        0        0    12913 2023-04-05 02:20:38.241521 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/accessors.pyi
+-rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/api.pyi
+-rw-r--r--   0        0        0    10458 2023-06-05 12:34:31.507869 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/base.pyi
+-rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/category.pyi
+-rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/datetimelike.pyi
+-rw-r--r--   0        0        0     4393 2023-05-25 18:30:24.475398 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/datetimes.pyi
+-rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/extension.pyi
+-rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/frozen.pyi
+-rw-r--r--   0        0        0    13472 2023-05-06 15:31:59.882980 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/interval.pyi
+-rw-r--r--   0        0        0     5428 2023-04-01 02:35:39.720026 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/multi.pyi
+-rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/period.pyi
+-rw-r--r--   0        0        0     2853 2023-04-05 02:20:38.244521 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/range.pyi
+-rw-r--r--   0        0        0     2740 2023-05-25 18:30:24.476413 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/timedeltas.pyi
+-rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.0.2.230605/pandas-stubs/core/indexing.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.0.2.230605/pandas-stubs/core/interchange/__init__.pyi
+-rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.0.2.230605/pandas-stubs/core/interchange/dataframe_protocol.pyi
+-rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.0.2.230605/pandas-stubs/core/interchange/from_dataframe.pyi
+-rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.0.2.230605/pandas-stubs/core/missing.pyi
+-rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/__init__.pyi
+-rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/array_ops.pyi
+-rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/common.pyi
+-rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/dispatch.pyi
+-rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/docstrings.pyi
+-rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/invalid.pyi
+-rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/mask_ops.pyi
+-rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-2.0.2.230605/pandas-stubs/core/resample.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/__init__.pyi
+-rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/api.pyi
+-rw-r--r--   0        0        0     2872 2023-04-12 19:14:53.210397 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/concat.pyi
+-rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/encoding.pyi
+-rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/melt.pyi
+-rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/merge.pyi
+-rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/pivot.pyi
+-rw-r--r--   0        0        0     7900 2023-04-05 02:20:38.246521 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/tile.pyi
+-rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/util.pyi
+-rw-r--r--   0        0        0    65542 2023-06-05 12:34:31.508833 pandas_stubs-2.0.2.230605/pandas-stubs/core/series.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.0.2.230605/pandas-stubs/core/sparse/__init__.pyi
+-rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.0.2.230605/pandas-stubs/core/strings.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/__init__.pyi
+-rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/datetimes.pyi
+-rw-r--r--   0        0        0     1140 2023-04-25 19:40:11.555225 pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/numeric.pyi
+-rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/timedeltas.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.0.2.230605/pandas-stubs/core/util/__init__.pyi
+-rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.0.2.230605/pandas-stubs/core/util/hashing.pyi
+-rw-r--r--   0        0        0      338 2023-05-22 14:12:55.274817 pandas_stubs-2.0.2.230605/pandas-stubs/core/window/__init__.pyi
+-rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-2.0.2.230605/pandas-stubs/core/window/ewm.pyi
+-rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-2.0.2.230605/pandas-stubs/core/window/expanding.pyi
+-rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-2.0.2.230605/pandas-stubs/core/window/rolling.pyi
+-rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.0.2.230605/pandas-stubs/errors/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.0.2.230605/pandas-stubs/io/__init__.pyi
+-rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.0.2.230605/pandas-stubs/io/api.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.0.2.230605/pandas-stubs/io/clipboard/__init__.pyi
+-rw-r--r--   0        0        0     7153 2023-04-25 19:40:11.555225 pandas_stubs-2.0.2.230605/pandas-stubs/io/clipboards.pyi
+-rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.0.2.230605/pandas-stubs/io/common.pyi
+-rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.0.2.230605/pandas-stubs/io/excel/__init__.pyi
+-rw-r--r--   0        0        0     7850 2023-05-22 14:12:55.275814 pandas_stubs-2.0.2.230605/pandas-stubs/io/excel/_base.pyi
+-rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.0.2.230605/pandas-stubs/io/excel/_util.pyi
+-rw-r--r--   0        0        0      446 2023-04-25 19:40:11.557224 pandas_stubs-2.0.2.230605/pandas-stubs/io/feather_format.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/css.pyi
+-rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/format.pyi
+-rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/style.pyi
+-rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/style_render.pyi
+-rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.0.2.230605/pandas-stubs/io/gbq.pyi
+-rw-r--r--   0        0        0     1493 2023-04-25 19:40:11.557224 pandas_stubs-2.0.2.230605/pandas-stubs/io/html.pyi
+-rw-r--r--   0        0        0      140 2023-05-22 14:12:55.276816 pandas_stubs-2.0.2.230605/pandas-stubs/io/json/__init__.pyi
+-rw-r--r--   0        0        0     4426 2023-05-25 18:30:30.309588 pandas_stubs-2.0.2.230605/pandas-stubs/io/json/_json.pyi
+-rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.0.2.230605/pandas-stubs/io/json/_normalize.pyi
+-rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.0.2.230605/pandas-stubs/io/json/_table_schema.pyi
+-rw-r--r--   0        0        0      393 2023-04-25 19:40:11.558224 pandas_stubs-2.0.2.230605/pandas-stubs/io/orc.pyi
+-rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.0.2.230605/pandas-stubs/io/parquet.pyi
+-rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.0.2.230605/pandas-stubs/io/parsers/__init__.pyi
+-rw-r--r--   0        0        0    16285 2023-05-22 14:12:55.276816 pandas_stubs-2.0.2.230605/pandas-stubs/io/parsers/readers.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.0.2.230605/pandas-stubs/io/parsers.pyi
+-rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.0.2.230605/pandas-stubs/io/pickle.pyi
+-rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-2.0.2.230605/pandas-stubs/io/pytables.pyi
+-rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.0.2.230605/pandas-stubs/io/sas/__init__.pyi
+-rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.0.2.230605/pandas-stubs/io/sas/sas7bdat.pyi
+-rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.0.2.230605/pandas-stubs/io/sas/sas_xport.pyi
+-rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.0.2.230605/pandas-stubs/io/sas/sasreader.pyi
+-rw-r--r--   0        0        0      361 2023-04-25 19:40:11.560224 pandas_stubs-2.0.2.230605/pandas-stubs/io/spss.pyi
+-rw-r--r--   0        0        0     5414 2023-05-22 14:12:46.119590 pandas_stubs-2.0.2.230605/pandas-stubs/io/sql.pyi
+-rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.0.2.230605/pandas-stubs/io/stata.pyi
+-rw-r--r--   0        0        0     1126 2023-04-25 19:40:11.561224 pandas_stubs-2.0.2.230605/pandas-stubs/io/xml.pyi
+-rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.0.2.230605/pandas-stubs/plotting/__init__.pyi
+-rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-2.0.2.230605/pandas-stubs/plotting/_core.pyi
+-rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.0.2.230605/pandas-stubs/plotting/_misc.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.0.2.230605/pandas-stubs/py.typed
+-rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.0.2.230605/pandas-stubs/testing.pyi
+-rw-r--r--   0        0        0       91 2023-05-22 14:12:55.278815 pandas_stubs-2.0.2.230605/pandas-stubs/tseries/__init__.pyi
+-rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.0.2.230605/pandas-stubs/tseries/api.pyi
+-rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.0.2.230605/pandas-stubs/tseries/frequencies.pyi
+-rw-r--r--   0        0        0     4142 2023-05-01 21:55:22.561166 pandas_stubs-2.0.2.230605/pandas-stubs/tseries/holiday.pyi
+-rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.0.2.230605/pandas-stubs/tseries/offsets.pyi
+-rw-r--r--   0        0        0      121 2023-05-22 14:12:55.278815 pandas_stubs-2.0.2.230605/pandas-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0      720 2023-05-22 14:12:55.279814 pandas_stubs-2.0.2.230605/pandas-stubs/util/_decorators.pyi
+-rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.0.2.230605/pandas-stubs/util/_doctools.pyi
+-rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.0.2.230605/pandas-stubs/util/_exceptions.pyi
+-rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.0.2.230605/pandas-stubs/util/_print_versions.pyi
+-rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.0.2.230605/pandas-stubs/util/_tester.pyi
+-rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.0.2.230605/pandas-stubs/util/_validators.pyi
+-rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.0.2.230605/pandas-stubs/util/version/__init__.pyi
+-rw-r--r--   0        0        0     6929 2023-06-05 12:37:10.685992 pandas_stubs-2.0.2.230605/pyproject.toml
+-rw-r--r--   0        0        0     8414 2023-05-22 14:12:55.263817 pandas_stubs-2.0.2.230605/README.md
+-rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 pandas_stubs-2.0.2.230605/setup.py
+-rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 pandas_stubs-2.0.2.230605/PKG-INFO
```

### Comparing `pandas_stubs-2.0.1.230501/LICENSE` & `pandas_stubs-2.0.2.230605/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-from . import (
+from pandas import (
     api as api,
     arrays as arrays,
     errors as errors,
     io as io,
     plotting as plotting,
     testing as testing,
     tseries as tseries,
     util as util,
 )
-from ._config import (
-    describe_option as describe_option,
-    get_option as get_option,
-    option_context as option_context,
-    options as options,
-    reset_option as reset_option,
-    set_option as set_option,
-)
-from .core.api import (
+from pandas.core.api import (
     NA as NA,
     ArrowDtype as ArrowDtype,
     BooleanDtype as BooleanDtype,
     Categorical as Categorical,
     CategoricalDtype as CategoricalDtype,
     CategoricalIndex as CategoricalIndex,
     DataFrame as DataFrame,
@@ -69,17 +61,17 @@
     timedelta_range as timedelta_range,
     to_datetime as to_datetime,
     to_numeric as to_numeric,
     to_timedelta as to_timedelta,
     unique as unique,
     value_counts as value_counts,
 )
-from .core.arrays.sparse import SparseDtype as SparseDtype
-from .core.computation.api import eval as eval
-from .core.reshape.api import (
+from pandas.core.arrays.sparse import SparseDtype as SparseDtype
+from pandas.core.computation.api import eval as eval
+from pandas.core.reshape.api import (
     concat as concat,
     crosstab as crosstab,
     cut as cut,
     from_dummies as from_dummies,
     get_dummies as get_dummies,
     lreshape as lreshape,
     melt as melt,
@@ -87,15 +79,28 @@
     merge_asof as merge_asof,
     merge_ordered as merge_ordered,
     pivot as pivot,
     pivot_table as pivot_table,
     qcut as qcut,
     wide_to_long as wide_to_long,
 )
-from .io.api import (
+
+from pandas._config import (
+    describe_option as describe_option,
+    get_option as get_option,
+    option_context as option_context,
+    options as options,
+    reset_option as reset_option,
+    set_option as set_option,
+)
+
+from pandas.util._print_versions import show_versions as show_versions
+from pandas.util._tester import test as test
+
+from pandas.io.api import (
     ExcelFile as ExcelFile,
     ExcelWriter as ExcelWriter,
     HDFStore as HDFStore,
     read_clipboard as read_clipboard,
     read_csv as read_csv,
     read_excel as read_excel,
     read_feather as read_feather,
@@ -113,14 +118,12 @@
     read_sql_query as read_sql_query,
     read_sql_table as read_sql_table,
     read_stata as read_stata,
     read_table as read_table,
     read_xml as read_xml,
     to_pickle as to_pickle,
 )
-from .io.json import json_normalize as json_normalize
-from .tseries import offsets as offsets
-from .tseries.api import infer_freq as infer_freq
-from .util._print_versions import show_versions as show_versions
-from .util._tester import test as test
+from pandas.io.json._normalize import json_normalize as json_normalize
+from pandas.tseries import offsets as offsets
+from pandas.tseries.api import infer_freq as infer_freq
 
 __version__: str
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_config/config.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_config/config.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/interval.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/interval.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     IntervalT,
     np_ndarray_bool,
     npt,
 )
 
 VALID_CLOSED: frozenset[str]
 
-_OrderableScalarT = TypeVar("_OrderableScalarT", int, float)
-_OrderableTimesT = TypeVar("_OrderableTimesT", Timestamp, Timedelta)
-_OrderableT = TypeVar("_OrderableT", int, float, Timestamp, Timedelta)
+_OrderableScalarT = TypeVar("_OrderableScalarT", bound=int | float)
+_OrderableTimesT = TypeVar("_OrderableTimesT", bound=Timestamp | Timedelta)
+_OrderableT = TypeVar("_OrderableT", bound=int | float | Timestamp | Timedelta)
 
 class _LengthDescriptor:
     @overload
     def __get__(
         self, instance: Interval[_OrderableScalarT], owner: Any
     ) -> _OrderableScalarT: ...
     @overload
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/lib.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/lib.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/missing.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/dtypes.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/nattype.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/nattype.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/offsets.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/offsets.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,19 @@
     overload,
 )
 
 import numpy as np
 from pandas.core.indexes.datetimes import DatetimeIndex
 from typing_extensions import Self
 
+from pandas._libs.tslibs.timedeltas import Timedelta
 from pandas._typing import npt
 
 from pandas.tseries.holiday import AbstractHolidayCalendar
 
-from .timedeltas import Timedelta
-
 _DatetimeT = TypeVar("_DatetimeT", bound=date)
 _TimedeltaT = TypeVar("_TimedeltaT", bound=timedelta)
 
 prefix_mapping: dict[str, type]
 
 class ApplyTypeError(TypeError): ...
 
@@ -175,15 +174,19 @@
 class SemiMonthBegin(SemiMonthOffset): ...
 
 class Week(SingleConstructorOffset):
     def __init__(
         self, n: int = ..., normalize: bool = ..., weekday: int | None = ...
     ) -> None: ...
 
-class WeekOfMonth(WeekOfMonthMixin): ...
+class WeekOfMonth(WeekOfMonthMixin):
+    def __init__(
+        self, n: int = ..., normalize: bool = ..., week: int = ..., weekday: int = ...
+    ) -> None: ...
+
 class LastWeekOfMonth(WeekOfMonthMixin): ...
 
 class FY5253Mixin(SingleConstructorOffset):
     def __init__(
         self,
         n: int = ...,
         normalize: bool = ...,
@@ -261,13 +264,10 @@
 CBMonthEnd = CustomBusinessMonthEnd
 CBMonthBegin = CustomBusinessMonthBegin
 CDay = CustomBusinessDay
 
 def roll_qtrday(
     other: datetime, n: int, month: int, day_opt: str, modby: int
 ) -> int: ...
-
-INVALID_FREQ_ERR_MSG: Literal["Invalid frequency: {0}"]
-
 def shift_months(
     dtindex: npt.NDArray[np.int64], months: int, day_opt: str | None = ...
 ) -> npt.NDArray[np.int64]: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/period.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/period.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,17 @@
     OffsetSeries,
     PeriodSeries,
     TimedeltaSeries,
 )
 from typing_extensions import TypeAlias
 
 from pandas._libs.tslibs import NaTType
+from pandas._libs.tslibs.timestamps import Timestamp
 from pandas._typing import npt
 
-from .timestamps import Timestamp
-
 class IncompatibleFrequency(ValueError): ...
 
 from pandas._libs.tslibs.offsets import BaseOffset
 
 _PeriodAddSub: TypeAlias = (
     Timedelta | datetime.timedelta | np.timedelta64 | np.int64 | int | BaseOffset
 )
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timedeltas.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/timestamps.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/timestamps.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_libs/tslibs/vectorized.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_libs/tslibs/vectorized.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_testing/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/_typing.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/_typing.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     ms: DatetimeDictArg
     us: DatetimeDictArg
     ns: DatetimeDictArg
 
 # dtypes
 NpDtype: TypeAlias = str | np.dtype[np.generic] | type[str | complex | bool | object]
 Dtype: TypeAlias = ExtensionDtype | NpDtype
-DtypeArg: TypeAlias = Dtype | dict[Any, Dtype]
+DtypeArg: TypeAlias = Dtype | Mapping[Any, Dtype]
 DtypeBackend: TypeAlias = Literal["pyarrow", "numpy_nullable"]
 BooleanDtypeArg: TypeAlias = (
     # Builtin bool type and its string alias
     type[bool]  # noqa: Y030
     | Literal["bool"]
     # Pandas nullable boolean type and its string alias
     | pd.BooleanDtype
@@ -306,33 +306,34 @@
     | Series
     | Index
     | np.ndarray
     | Callable[[HashableT], bool]
     | None
 )
 # Scratch types for generics
+
 S1 = TypeVar(
     "S1",
-    str,
-    bytes,
-    datetime.date,
-    datetime.time,
-    bool,
-    int,
-    float,
-    complex,
-    Dtype,
-    Timestamp,
-    Timedelta,
-    Period,
-    Interval[int],
-    Interval[float],
-    Interval[Timestamp],
-    Interval[Timedelta],
-    CategoricalDtype,
+    bound=str
+    | bytes
+    | datetime.date
+    | datetime.time
+    | bool
+    | int
+    | float
+    | complex
+    | Dtype
+    | Timestamp
+    | Timedelta
+    | Period
+    | Interval[int]
+    | Interval[float]
+    | Interval[Timestamp]
+    | Interval[Timedelta]
+    | CategoricalDtype,
 )
 T1 = TypeVar(
     "T1", str, int, np.int64, np.uint64, np.float64, float, np.dtype[np.generic]
 )
 T2 = TypeVar("T2", str, int)
 
 IndexingInt: TypeAlias = (
@@ -355,21 +356,15 @@
 # Series is passed into a function, a Series is always returned and if a DataFrame is
 # passed in, a DataFrame is always returned.
 NDFrameT = TypeVar("NDFrameT", bound=NDFrame)
 
 IndexT = TypeVar("IndexT", bound=Index)
 
 # Interval closed type
-IntervalT = TypeVar(
-    "IntervalT",
-    Interval[int],
-    Interval[float],
-    Interval[Timestamp],
-    Interval[Timedelta],
-)
+IntervalT = TypeVar("IntervalT", bound=Interval)
 IntervalClosedType: TypeAlias = Literal["left", "right", "both", "neither"]
 
 TakeIndexer: TypeAlias = Sequence[int] | Sequence[np.integer] | npt.NDArray[np.integer]
 
 IgnoreRaiseCoerce: TypeAlias = Literal["ignore", "raise", "coerce"]
 
 # Shared by functions such as drop and astype
@@ -400,31 +395,71 @@
 
 # Any plain Python or numpy function
 Function: TypeAlias = np.ufunc | Callable[..., Any]
 # Use a distinct HashableT in shared types to avoid conflicts with
 # shared HashableT and HashableT#. This one can be used if the identical
 # type is need in a function that uses GroupByObjectNonScalar
 _HashableTa = TypeVar("_HashableTa", bound=Hashable)
+ByT = TypeVar(
+    "ByT",
+    bound=str
+    | bytes
+    | datetime.date
+    | datetime.datetime
+    | datetime.timedelta
+    | np.datetime64
+    | np.timedelta64
+    | bool
+    | int
+    | float
+    | complex
+    | Timestamp
+    | Timedelta
+    | Scalar
+    | Period
+    | Interval[int]
+    | Interval[float]
+    | Interval[Timestamp]
+    | Interval[Timedelta]
+    | tuple,
+)
+# Use a distinct SeriesByT when using groupby with Series of known dtype.
+# Essentially, an intersection between Series S1 TypeVar, and ByT TypeVar
+SeriesByT = TypeVar(
+    "SeriesByT",
+    bound=str
+    | bytes
+    | datetime.date
+    | bool
+    | int
+    | float
+    | complex
+    | Timestamp
+    | Timedelta
+    | Period
+    | Interval[int]
+    | Interval[float]
+    | Interval[Timestamp]
+    | Interval[Timedelta],
+)
 GroupByObjectNonScalar: TypeAlias = (
     tuple
     | list[_HashableTa]
     | Function
     | list[Function]
-    | Series
     | list[Series]
     | np.ndarray
     | list[np.ndarray]
     | Mapping[Label, Any]
     | list[Mapping[Label, Any]]
-    | Index
     | list[Index]
     | Grouper
     | list[Grouper]
 )
-GroupByObject: TypeAlias = Scalar | GroupByObjectNonScalar
+GroupByObject: TypeAlias = Scalar | Index | GroupByObjectNonScalar | Series
 
 StataDateFormat: TypeAlias = Literal[
     "tc",
     "%tc",
     "td",
     "%td",
     "tw",
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/api/extensions/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/api/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/api/types/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/api/types/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pandas._libs.lib import infer_dtype as infer_dtype
 
 from pandas.core.dtypes.api import (
+    is_any_real_numeric_dtype as is_any_real_numeric_dtype,
     is_array_like as is_array_like,
     is_bool as is_bool,
     is_bool_dtype as is_bool_dtype,
     is_categorical_dtype as is_categorical_dtype,
     is_complex as is_complex,
     is_complex_dtype as is_complex_dtype,
     is_datetime64_any_dtype as is_datetime64_any_dtype,
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/algorithms.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/algorithms.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/api.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arraylike.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arraylike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/base.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/boolean.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/boolean.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import ClassVar
 
 import numpy as np
+from pandas.core.arrays.masked import BaseMaskedArray as BaseMaskedArray
 
 from pandas._libs.missing import NAType
 from pandas._typing import type_t
 
 from pandas.core.dtypes.base import ExtensionDtype as ExtensionDtype
 
-from .masked import BaseMaskedArray as BaseMaskedArray
-
 class BooleanDtype(ExtensionDtype):
     na_value: ClassVar[NAType]
     @classmethod
     def construct_array_type(cls) -> type_t[BooleanArray]: ...
 
 def coerce_to_array(values, mask=..., copy: bool = ...): ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/categorical.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/categorical.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimelike.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/datetimes.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/integer.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/integer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from pandas.core.arrays.masked import BaseMaskedArray
+
 from pandas._libs.missing import NAType
 
 from pandas.core.dtypes.base import ExtensionDtype as ExtensionDtype
 
-from .masked import BaseMaskedArray
-
 class _IntegerDtype(ExtensionDtype):
     base: None
     @property
     def na_value(self) -> NAType: ...
     @property
     def itemsize(self) -> int: ...
     @classmethod
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/interval.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/masked.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/masked.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/numpy_.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/numpy_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/period.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/accessor.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/accessor.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/sparse/array.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/sparse/array.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/string_.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/string_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/arrays/timedeltas.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/arrays/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/base.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/common.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/eval.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/eval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/expr.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/expr.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/ops.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/pytables.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/computation/scope.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/computation/scope.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/config_init.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/config_init.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/construction.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/construction.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/api.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/api.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pandas.core.dtypes.common import (
+    is_any_real_numeric_dtype as is_any_real_numeric_dtype,
     is_array_like as is_array_like,
     is_bool as is_bool,
     is_bool_dtype as is_bool_dtype,
     is_categorical_dtype as is_categorical_dtype,
     is_complex as is_complex,
     is_complex_dtype as is_complex_dtype,
     is_datetime64_any_dtype as is_datetime64_any_dtype,
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/base.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/common.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/common.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,8 +49,9 @@
 def is_datetime64_ns_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_timedelta64_ns_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_numeric_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_float_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_bool_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_extension_array_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def is_complex_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
+def is_any_real_numeric_dtype(arr_or_dtype: _ArrayOrDtype) -> bool: ...
 def pandas_dtype(dtype: object) -> DtypeObj: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/dtypes.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/inference.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/inference.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/dtypes/missing.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/dtypes/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/frame.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/frame.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections.abc import (
     Callable,
+    Generator,
     Hashable,
     Iterable,
     Iterator,
     Mapping,
     Sequence,
 )
 import datetime
@@ -16,26 +17,30 @@
     TypeVar,
     overload,
 )
 
 from matplotlib.axes import Axes as PlotAxes
 import numpy as np
 from pandas import (
+    Period,
     Timedelta,
     Timestamp,
 )
 from pandas.core.arraylike import OpsMixin
 from pandas.core.generic import NDFrame
-from pandas.core.groupby.generic import (
-    _DataFrameGroupByNonScalar,
-    _DataFrameGroupByScalar,
-)
+from pandas.core.groupby.generic import DataFrameGroupBy
 from pandas.core.groupby.grouper import Grouper
 from pandas.core.indexers import BaseIndexer
 from pandas.core.indexes.base import Index
+from pandas.core.indexes.category import CategoricalIndex
+from pandas.core.indexes.datetimes import DatetimeIndex
+from pandas.core.indexes.interval import IntervalIndex
+from pandas.core.indexes.multi import MultiIndex
+from pandas.core.indexes.period import PeriodIndex
+from pandas.core.indexes.timedeltas import TimedeltaIndex
 from pandas.core.indexing import (
     _iLocIndexer,
     _IndexSliceTuple,
     _LocIndexer,
 )
 from pandas.core.interchange.dataframe_protocol import DataFrame as DataFrameXchg
 from pandas.core.resample import Resampler
@@ -44,14 +49,15 @@
     Expanding,
     ExponentialMovingWindow,
 )
 from pandas.core.window.rolling import (
     Rolling,
     Window,
 )
+from typing_extensions import Self
 import xarray as xr
 
 from pandas._libs.missing import NAType
 from pandas._libs.tslibs import BaseOffset
 from pandas._typing import (
     S1,
     AggFuncTypeBase,
@@ -66,26 +72,26 @@
     AxisIndex,
     CalculationMethod,
     ColspaceArgType,
     CompressionOptions,
     Dtype,
     FilePath,
     FillnaOptions,
-    FloatFormatType,
     FormattersType,
     GroupByObjectNonScalar,
     HashableT,
     HashableT1,
     HashableT2,
     HashableT3,
     IgnoreRaise,
     IndexingInt,
     IndexLabel,
     IndexType,
     IntervalClosedType,
+    IntervalT,
     JoinHow,
     JsonFrameOrient,
     Label,
     Level,
     ListLike,
     ListLikeExceptSeriesAndStr,
     ListLikeU,
@@ -97,14 +103,15 @@
     QuantileInterpolation,
     RandomState,
     ReadBuffer,
     Renamer,
     ReplaceMethod,
     Scalar,
     ScalarT,
+    SeriesByT,
     SortKind,
     StataDateFormat,
     StorageOptions,
     StrLike,
     Suffixes,
     T as TType,
     TimestampConvention,
@@ -145,15 +152,15 @@
         self,
         idx: int
         | IndexType
         | tuple[int, int]
         | tuple[IndexType, int]
         | tuple[IndexType, IndexType]
         | tuple[int, IndexType],
-        value: S1 | Series | DataFrame | np.ndarray | None,
+        value: Scalar | Series | DataFrame | np.ndarray | None,
     ) -> None: ...
 
 class _LocIndexerFrame(_LocIndexer):
     @overload
     def __getitem__(
         self,
         idx: IndexType
@@ -194,21 +201,21 @@
     ) -> Series: ...
     @overload
     def __getitem__(self, idx: tuple[Scalar, slice]) -> Series | DataFrame: ...
     @overload
     def __setitem__(
         self,
         idx: MaskType | StrLike | _IndexSliceTuple | list[ScalarT],
-        value: S1 | ArrayLike | Series | DataFrame | None,
+        value: Scalar | ArrayLike | Series | DataFrame | list | None,
     ) -> None: ...
     @overload
     def __setitem__(
         self,
         idx: tuple[_IndexSliceTuple, HashableT],
-        value: S1 | ArrayLike | Series[S1] | list | None,
+        value: Scalar | ArrayLike | Series | list | None,
     ) -> None: ...
 
 class DataFrame(NDFrame, OpsMixin):
     __hash__: ClassVar[None]  # type: ignore[assignment]
 
     @overload
     def __new__(
@@ -218,24 +225,24 @@
         | dict[Any, Any]
         | Iterable[ListLikeU | tuple[Hashable, ListLikeU] | dict[Any, Any]]
         | None = ...,
         index: Axes | None = ...,
         columns: Axes | None = ...,
         dtype=...,
         copy: _bool = ...,
-    ) -> DataFrame: ...
+    ) -> Self: ...
     @overload
     def __new__(
         cls,
         data: Scalar,
         index: Axes,
         columns: Axes,
         dtype=...,
         copy: _bool = ...,
-    ) -> DataFrame: ...
+    ) -> Self: ...
     def __dataframe__(
         self, nan_as_null: bool = ..., allow_copy: bool = ...
     ) -> DataFrameXchg: ...
     @property
     def axes(self) -> list[Index]: ...
     @property
     def shape(self) -> tuple[int, int]: ...
@@ -541,22 +548,23 @@
     ) -> None: ...
     def memory_usage(self, index: _bool = ..., deep: _bool = ...) -> Series: ...
     def transpose(self, *args, copy: _bool = ...) -> DataFrame: ...
     @property
     def T(self) -> DataFrame: ...
     def __getattr__(self, name: str) -> Series: ...
     @overload
-    def __getitem__(
+    def __getitem__(  # type: ignore[misc]
         self,
         key: Series[_bool]
         | DataFrame
         | Index
         | np_ndarray_str
         | np_ndarray_bool
-        | list[_ScalarOrTupleT],
+        | list[_ScalarOrTupleT]
+        | Generator[_ScalarOrTupleT, None, None],
     ) -> DataFrame: ...
     @overload
     def __getitem__(self, key: slice) -> DataFrame: ...
     @overload
     def __getitem__(self, key: Scalar | Hashable) -> Series: ...
     def isetitem(
         self, loc: int | Sequence[int], value: Scalar | ArrayLike | list[Any]
@@ -1007,28 +1015,106 @@
         level: Level | None = ...,
         as_index: _bool = ...,
         sort: _bool = ...,
         group_keys: _bool = ...,
         squeeze: _bool = ...,
         observed: _bool = ...,
         dropna: _bool = ...,
-    ) -> _DataFrameGroupByScalar: ...
+    ) -> DataFrameGroupBy[Scalar]: ...
+    @overload
+    def groupby(
+        self,
+        by: DatetimeIndex,
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[Timestamp]: ...
+    @overload
+    def groupby(
+        self,
+        by: TimedeltaIndex,
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[Timedelta]: ...
     @overload
     def groupby(
         self,
-        by: GroupByObjectNonScalar | None = ...,
+        by: PeriodIndex,
         axis: Axis = ...,
         level: Level | None = ...,
         as_index: _bool = ...,
         sort: _bool = ...,
         group_keys: _bool = ...,
         squeeze: _bool = ...,
         observed: _bool = ...,
         dropna: _bool = ...,
-    ) -> _DataFrameGroupByNonScalar: ...
+    ) -> DataFrameGroupBy[Period]: ...
+    @overload
+    def groupby(
+        self,
+        by: IntervalIndex[IntervalT],
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[IntervalT]: ...
+    @overload
+    def groupby(
+        self,
+        by: MultiIndex | GroupByObjectNonScalar | None = ...,
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[tuple]: ...
+    @overload
+    def groupby(
+        self,
+        by: Series[SeriesByT],
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[SeriesByT]: ...
+    @overload
+    def groupby(
+        self,
+        by: CategoricalIndex | Index | Series,
+        axis: Axis = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> DataFrameGroupBy[Any]: ...
     def pivot(
         self,
         *,
         index: IndexLabel = ...,
         columns: IndexLabel = ...,
         values: IndexLabel = ...,
     ) -> DataFrame: ...
@@ -1634,15 +1720,15 @@
         method: _str = ...,
         *,
         axis: Axis = ...,
         limit: int | None = ...,
         limit_direction: Literal["forward", "backward", "both"] = ...,
         limit_area: Literal["inside", "outside"] | None = ...,
         downcast: Literal["infer"] | None = ...,
-        inplace: Literal[False],
+        inplace: Literal[False] = ...,
         **kwargs,
     ) -> DataFrame: ...
     @overload
     def interpolate(
         self,
         method: _str = ...,
         *,
@@ -1881,29 +1967,29 @@
         axis: Axis = ...,
         level: Level | None = ...,
         fill_value: float | None = ...,
     ) -> DataFrame: ...
     @overload
     def rolling(
         self,
-        window: int | str | BaseOffset | BaseIndexer,
+        window: int | str | _dt.timedelta | BaseOffset | BaseIndexer,
         min_periods: int | None = ...,
         center: _bool = ...,
         on: Hashable | None = ...,
         axis: Axis = ...,
         closed: IntervalClosedType | None = ...,
         step: int | None = ...,
         method: CalculationMethod = ...,
         *,
         win_type: _str,
     ) -> Window[DataFrame]: ...
     @overload
     def rolling(
         self,
-        window: int | str | BaseOffset | BaseIndexer,
+        window: int | str | _dt.timedelta | BaseOffset | BaseIndexer,
         min_periods: int | None = ...,
         center: _bool = ...,
         on: Hashable | None = ...,
         axis: Axis = ...,
         closed: IntervalClosedType | None = ...,
         step: int | None = ...,
         method: CalculationMethod = ...,
@@ -2008,53 +2094,91 @@
     def to_clipboard(
         self, excel: _bool = ..., sep: _str | None = ..., **kwargs
     ) -> None: ...
     @overload
     def to_json(
         self,
         path_or_buf: FilePath | WriteBuffer[str],
-        orient: JsonFrameOrient | None = ...,
+        *,
+        orient: Literal["records"],
         date_format: Literal["epoch", "iso"] | None = ...,
         double_precision: int = ...,
         force_ascii: _bool = ...,
         date_unit: Literal["s", "ms", "us", "ns"] = ...,
         default_handler: Callable[[Any], _str | float | _bool | list | dict]
         | None = ...,
-        lines: _bool = ...,
+        lines: Literal[True],
         compression: CompressionOptions = ...,
         index: _bool = ...,
         indent: int | None = ...,
+        mode: Literal["a"],
     ) -> None: ...
     @overload
     def to_json(
         self,
         path_or_buf: None = ...,
+        *,
+        orient: Literal["records"],
+        date_format: Literal["epoch", "iso"] | None = ...,
+        double_precision: int = ...,
+        force_ascii: _bool = ...,
+        date_unit: Literal["s", "ms", "us", "ns"] = ...,
+        default_handler: Callable[[Any], _str | float | _bool | list | dict]
+        | None = ...,
+        lines: Literal[True],
+        compression: CompressionOptions = ...,
+        index: _bool = ...,
+        indent: int | None = ...,
+        mode: Literal["a"],
+    ) -> _str: ...
+    @overload
+    def to_json(
+        self,
+        path_or_buf: None = ...,
         orient: JsonFrameOrient | None = ...,
         date_format: Literal["epoch", "iso"] | None = ...,
         double_precision: int = ...,
         force_ascii: _bool = ...,
         date_unit: Literal["s", "ms", "us", "ns"] = ...,
         default_handler: Callable[[Any], _str | float | _bool | list | dict]
         | None = ...,
         lines: _bool = ...,
         compression: CompressionOptions = ...,
         index: _bool = ...,
         indent: int | None = ...,
+        mode: Literal["w"] = ...,
     ) -> _str: ...
     @overload
+    def to_json(
+        self,
+        path_or_buf: FilePath | WriteBuffer[str],
+        orient: JsonFrameOrient | None = ...,
+        date_format: Literal["epoch", "iso"] | None = ...,
+        double_precision: int = ...,
+        force_ascii: _bool = ...,
+        date_unit: Literal["s", "ms", "us", "ns"] = ...,
+        default_handler: Callable[[Any], _str | float | _bool | list | dict]
+        | None = ...,
+        lines: _bool = ...,
+        compression: CompressionOptions = ...,
+        index: _bool = ...,
+        indent: int | None = ...,
+        mode: Literal["w"] = ...,
+    ) -> None: ...
+    @overload
     def to_string(
         self,
         buf: FilePath | WriteBuffer[str],
         columns: list[HashableT1] | Index | Series | None = ...,
         col_space: int | list[int] | dict[HashableT2, int] | None = ...,
         header: _bool | list[_str] | tuple[str, ...] = ...,
         index: _bool = ...,
         na_rep: _str = ...,
         formatters: FormattersType | None = ...,
-        float_format: FloatFormatType | None = ...,
+        float_format: Callable[[float], str] | None = ...,
         sparsify: _bool | None = ...,
         index_names: _bool = ...,
         justify: _str | None = ...,
         max_rows: int | None = ...,
         max_cols: int | None = ...,
         show_dimensions: _bool = ...,
         decimal: _str = ...,
@@ -2069,15 +2193,15 @@
         buf: None = ...,
         columns: list[HashableT] | Index | Series | None = ...,
         col_space: int | list[int] | dict[Hashable, int] | None = ...,
         header: _bool | Sequence[_str] = ...,
         index: _bool = ...,
         na_rep: _str = ...,
         formatters: FormattersType | None = ...,
-        float_format: FloatFormatType | None = ...,
+        float_format: Callable[[float], str] | None = ...,
         sparsify: _bool | None = ...,
         index_names: _bool = ...,
         justify: _str | None = ...,
         max_rows: int | None = ...,
         max_cols: int | None = ...,
         show_dimensions: _bool = ...,
         decimal: _str = ...,
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/generic.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/generic.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/generic.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/generic.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from typing_extensions import TypeAlias
 
 from pandas._typing import (
     S1,
     AggFuncTypeBase,
     AggFuncTypeFrame,
     Axis,
+    ByT,
     Level,
     ListLike,
     RandomState,
     Scalar,
 )
 
 AggScalar: TypeAlias = str | Callable[..., Any]
@@ -41,21 +42,15 @@
 
 class NamedAgg(NamedTuple):
     column: str = ...
     aggfunc: AggScalar = ...
 
 def generate_property(name: str, klass: type[NDFrame]): ...
 
-class _SeriesGroupByScalar(SeriesGroupBy[S1]):
-    def __iter__(self) -> Iterator[tuple[Scalar, Series]]: ...
-
-class _SeriesGroupByNonScalar(SeriesGroupBy[S1]):
-    def __iter__(self) -> Iterator[tuple[tuple, Series]]: ...
-
-class SeriesGroupBy(GroupBy, Generic[S1]):
+class SeriesGroupBy(GroupBy, Generic[S1, ByT]):
     def any(self, skipna: bool = ...) -> Series[bool]: ...
     def all(self, skipna: bool = ...) -> Series[bool]: ...
     def apply(self, func, *args, **kwargs) -> Series: ...
     @overload
     def aggregate(self, func: list[AggFuncTypeBase], *args, **kwargs) -> DataFrame: ...
     @overload
     def aggregate(self, func: AggFuncTypeBase, *args, **kwargs) -> Series: ...
@@ -141,22 +136,18 @@
         bins: int | Sequence = ...,
         backend: str | None = ...,
         legend: bool = ...,
         **kwargs,
     ) -> AxesSubplot: ...
     def idxmax(self, axis: Axis = ..., skipna: bool = ...) -> Series: ...
     def idxmin(self, axis: Axis = ..., skipna: bool = ...) -> Series: ...
+    def __iter__(self) -> Iterator[tuple[ByT, Series[S1]]]: ...
+    def diff(self, periods: int = ..., axis: Axis = ...) -> Series: ...
 
-class _DataFrameGroupByScalar(DataFrameGroupBy):
-    def __iter__(self) -> Iterator[tuple[Scalar, DataFrame]]: ...
-
-class _DataFrameGroupByNonScalar(DataFrameGroupBy):
-    def __iter__(self) -> Iterator[tuple[tuple, DataFrame]]: ...
-
-class DataFrameGroupBy(GroupBy):
+class DataFrameGroupBy(GroupBy, Generic[ByT]):
     def any(self, skipna: bool = ...) -> DataFrame: ...
     def all(self, skipna: bool = ...) -> DataFrame: ...
     # error: Overload 3 for "apply" will never be used because its parameters overlap overload 1
     @overload
     def apply(  # type: ignore[misc]
         self, func: Callable[[DataFrame], Scalar | list | dict], *args, **kwargs
     ) -> Series: ...
@@ -172,17 +163,17 @@
     agg = aggregate
     def transform(self, func: Callable | str, *args, **kwargs) -> DataFrame: ...
     def filter(
         self, func: Callable, dropna: bool = ..., *args, **kwargs
     ) -> DataFrame: ...
     def nunique(self, dropna: bool = ...) -> DataFrame: ...
     @overload
-    def __getitem__(self, item: str) -> SeriesGroupBy: ...
+    def __getitem__(self, item: str) -> SeriesGroupBy[Any, ByT]: ...
     @overload
-    def __getitem__(self, item: list[str]) -> DataFrameGroupBy: ...
+    def __getitem__(self, item: list[str]) -> DataFrameGroupBy[ByT]: ...
     def count(self) -> DataFrame: ...
     def boxplot(
         self,
         grouped: DataFrame,
         subplots: bool = ...,
         column: str | Sequence | None = ...,
         fontsize: float | str = ...,
@@ -216,46 +207,23 @@
     def cummin(
         self, axis: Axis = ..., numeric_only: bool = ..., **kwargs
     ) -> DataFrame: ...
     def cumprod(self, axis: Axis = ..., **kwargs) -> DataFrame: ...
     def cumsum(self, axis: Axis = ..., **kwargs) -> DataFrame: ...
     def describe(self, **kwargs) -> DataFrame: ...
     def ffill(self, limit: int | None = ...) -> DataFrame: ...
-    @overload
     def fillna(
         self,
         value,
         method: str | None = ...,
         axis: Axis = ...,
+        inplace: Literal[False] = ...,
         limit: int | None = ...,
         downcast: dict | None = ...,
-        *,
-        inplace: Literal[True],
-    ) -> None: ...
-    @overload
-    def fillna(
-        self,
-        value,
-        method: str | None = ...,
-        axis: Axis = ...,
-        limit: int | None = ...,
-        downcast: dict | None = ...,
-        *,
-        inplace: Literal[False],
     ) -> DataFrame: ...
-    @overload
-    def fillna(
-        self,
-        value,
-        method: str | None = ...,
-        axis: Axis = ...,
-        inplace: bool = ...,
-        limit: int | None = ...,
-        downcast: dict | None = ...,
-    ) -> DataFrame | None: ...
     def first(self, **kwargs) -> DataFrame: ...
     def head(self, n: int = ...) -> DataFrame: ...
     def hist(
         self,
         data: DataFrame,
         column: str | Sequence | None = ...,
         by=...,
@@ -359,8 +327,9 @@
         self,
         subset: ListLike | None,
         normalize: Literal[True],
         sort: bool = ...,
         ascending: bool = ...,
         dropna: bool = ...,
     ) -> Series[float]: ...
-    def __getattr__(self, name: str) -> SeriesGroupBy: ...
+    def __getattr__(self, name: str) -> SeriesGroupBy[Any, ByT]: ...
+    def __iter__(self) -> Iterator[tuple[ByT, DataFrame]]: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/groupby.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/groupby.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/grouper.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/grouper.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/groupby/ops.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/groupby/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexers.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexers.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/accessors.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/accessors.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/api.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/base.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,38 +66,38 @@
     ) -> Self: ...
     @overload
     def __getitem__(self, idx: int) -> S1: ...
 
 class Index(IndexOpsMixin, PandasObject):
     __hash__: ClassVar[None]  # type: ignore[assignment]
     @overload
-    def __new__(
+    def __new__(  # type: ignore[misc]
         cls,
         data: Iterable,
         dtype: Literal["int"] | type_t[int] | type_t[np.integer],
         copy: bool = ...,
         name=...,
         tupleize_cols: bool = ...,
         **kwargs,
     ) -> _IntIndexType: ...
     @overload
-    def __new__(
+    def __new__(  # type: ignore[misc]
         cls,
         data: Iterable,
         dtype: Literal["float"]
         | type_t[float]
         | type_t[np.float32]
         | type_t[np.float64],
         copy: bool = ...,
         name=...,
         tupleize_cols: bool = ...,
         **kwargs,
     ) -> _FloatIndexType: ...
     @overload
-    def __new__(
+    def __new__(  # type: ignore[misc]
         cls,
         data: Iterable,
         dtype: Literal["complex"] | type_t[complex],
         copy: bool = ...,
         name=...,
         tupleize_cols: bool = ...,
         **kwargs,
@@ -107,15 +107,15 @@
         cls,
         data: Iterable = ...,
         dtype=...,
         copy: bool = ...,
         name=...,
         tupleize_cols: bool = ...,
         **kwargs,
-    ) -> Index: ...
+    ) -> Self: ...
     @property
     def str(self) -> StringMethods[Index, MultiIndex]: ...
     @property
     def asi8(self) -> np_ndarray_int64: ...
     def is_(self, other) -> bool: ...
     def __len__(self) -> int: ...
     def __array__(self, dtype=...) -> np.ndarray: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/category.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/category.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimelike.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/datetimes.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/interval.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/interval.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -367,60 +367,60 @@
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[float]]: ...
 @overload
 def interval_range(
     start: _TimestampLike,
     end: _TimestampLike = ...,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timestamp]]: ...
 @overload
 def interval_range(
     *,
     start: None = ...,
     end: _TimestampLike,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timestamp]]: ...
 @overload
 def interval_range(
     start: _TimestampLike,
     *,
     end: None = ...,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timestamp]]: ...
 @overload
 def interval_range(
     start: _TimedeltaLike,
     end: _TimedeltaLike = ...,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timedelta]]: ...
 @overload
 def interval_range(
     *,
     start: None = ...,
     end: _TimedeltaLike,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timedelta]]: ...
 @overload
 def interval_range(
     start: _TimedeltaLike,
     *,
     end: None = ...,
     periods: int | None = ...,
-    freq: str | BaseOffset | None = ...,
+    freq: str | BaseOffset | pd.Timedelta | dt.timedelta | None = ...,
     name: Hashable = ...,
     closed: IntervalClosedType = ...,
 ) -> IntervalIndex[Interval[pd.Timedelta]]: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/multi.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/multi.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/period.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/range.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/range.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexes/timedeltas.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexes/timedeltas.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -68,11 +68,11 @@
     def insert(self, loc, item): ...
     def to_series(self, index=..., name=...) -> TimedeltaSeries: ...
 
 def timedelta_range(
     start: TimedeltaConvertibleTypes = ...,
     end: TimedeltaConvertibleTypes = ...,
     periods: int | None = ...,
-    freq: str | DateOffset | None = ...,
+    freq: str | DateOffset | Timedelta | dt.timedelta | None = ...,
     name: Hashable | None = ...,
     closed: Literal["left", "right"] | None = ...,
 ) -> TimedeltaIndex: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/indexing.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/indexing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/interchange/dataframe_protocol.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/interchange/dataframe_protocol.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/array_ops.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/array_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/ops/mask_ops.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/ops/mask_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/resample.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/resample.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/api.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/concat.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/concat.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/encoding.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/encoding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/melt.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/melt.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/merge.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/merge.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/pivot.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/pivot.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/reshape/tile.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/reshape/tile.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/series.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/series.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,67 +16,72 @@
     Any,
     ClassVar,
     Generic,
     Literal,
     overload,
 )
 
-from core.api import (
-    Int8Dtype as Int8Dtype,
-    Int16Dtype as Int16Dtype,
-    Int32Dtype as Int32Dtype,
-    Int64Dtype as Int64Dtype,
-)
 from matplotlib.axes import (
     Axes as PlotAxes,
     SubplotBase,
 )
 import numpy as np
 from pandas import (
     Period,
+    PeriodDtype,
     Timedelta,
     Timestamp,
 )
+from pandas.core.api import (
+    Int8Dtype as Int8Dtype,
+    Int16Dtype as Int16Dtype,
+    Int32Dtype as Int32Dtype,
+    Int64Dtype as Int64Dtype,
+)
 from pandas.core.arrays.base import ExtensionArray
 from pandas.core.arrays.categorical import CategoricalAccessor
 from pandas.core.arrays.interval import IntervalArray
-from pandas.core.groupby.generic import (
-    _SeriesGroupByNonScalar,
-    _SeriesGroupByScalar,
-)
+from pandas.core.base import IndexOpsMixin
+from pandas.core.frame import DataFrame
+from pandas.core.generic import NDFrame
+from pandas.core.groupby.generic import SeriesGroupBy
 from pandas.core.indexers import BaseIndexer
 from pandas.core.indexes.accessors import (
     CombinedDatetimelikeProperties,
     PeriodProperties,
     TimedeltaProperties,
     TimestampProperties,
 )
 from pandas.core.indexes.base import Index
+from pandas.core.indexes.category import CategoricalIndex
 from pandas.core.indexes.datetimes import DatetimeIndex
 from pandas.core.indexes.interval import IntervalIndex
+from pandas.core.indexes.multi import MultiIndex
 from pandas.core.indexes.period import PeriodIndex
 from pandas.core.indexes.timedeltas import TimedeltaIndex
 from pandas.core.indexing import (
     _AtIndexer,
     _iAtIndexer,
+    _iLocIndexer,
     _IndexSliceTuple,
+    _LocIndexer,
 )
 from pandas.core.resample import Resampler
 from pandas.core.strings import StringMethods
 from pandas.core.window import (
     Expanding,
     ExponentialMovingWindow,
-    Rolling,
 )
 from pandas.core.window.rolling import (
     Rolling,
     Window,
 )
 from typing_extensions import (
     Never,
+    Self,
     TypeAlias,
 )
 import xarray as xr
 
 from pandas._libs.interval import (
     Interval,
     _OrderableT,
@@ -96,39 +101,42 @@
     AxisIndex,
     BooleanDtypeArg,
     BytesDtypeArg,
     CalculationMethod,
     CategoryDtypeArg,
     ComplexDtypeArg,
     CompressionOptions,
+    Dtype,
     DtypeBackend,
     DtypeObj,
     FilePath,
     FillnaOptions,
     FloatDtypeArg,
     GroupByObjectNonScalar,
     HashableT1,
     HashableT2,
     HashableT3,
     IgnoreRaise,
     IndexingInt,
     IntDtypeArg,
     IntervalClosedType,
+    IntervalT,
     JoinHow,
     JsonSeriesOrient,
     Level,
     ListLike,
     ListLikeU,
     MaskType,
     NaPosition,
     QuantileInterpolation,
     RandomState,
     Renamer,
     ReplaceMethod,
     Scalar,
+    SeriesByT,
     SortKind,
     StrDtypeArg,
     TimedeltaDtypeArg,
     TimestampConvention,
     TimestampDtypeArg,
     WriteBuffer,
     np_ndarray_anyint,
@@ -137,23 +145,14 @@
     num,
 )
 
 from pandas.core.dtypes.base import ExtensionDtype
 
 from pandas.plotting import PlotAccessor
 
-from .base import IndexOpsMixin
-from .frame import DataFrame
-from .generic import NDFrame
-from .indexes.multi import MultiIndex
-from .indexing import (
-    _iLocIndexer,
-    _LocIndexer,
-)
-
 _bool = bool
 _str = str
 
 class _iLocIndexerSeries(_iLocIndexer, Generic[S1]):
     # get item
     @overload
     def __getitem__(self, idx: IndexingInt) -> S1: ...
@@ -175,15 +174,21 @@
         self,
         idx: Scalar | tuple[Scalar, ...],
         # tuple case is for getting a specific element when using a MultiIndex
     ) -> S1: ...
     @overload
     def __getitem__(
         self,
-        idx: MaskType | Index | Sequence[float] | list[str] | slice | _IndexSliceTuple,
+        idx: MaskType
+        | Index
+        | Sequence[float]
+        | list[str]
+        | slice
+        | _IndexSliceTuple
+        | Callable,
         # _IndexSliceTuple is when having a tuple that includes a slice.  Could just
         # be s.loc[1, :], or s.loc[pd.IndexSlice[1, :]]
     ) -> Series[S1]: ...
     @overload
     def __setitem__(
         self,
         idx: Index | MaskType,
@@ -202,124 +207,89 @@
         value: S1 | ArrayLike | Series[S1] | None,
     ) -> None: ...
 
 class Series(IndexOpsMixin, NDFrame, Generic[S1]):
     _ListLike: TypeAlias = ArrayLike | dict[_str, np.ndarray] | list | tuple | Index
     __hash__: ClassVar[None]
 
+    # TODO: can __new__ be converted to __init__? Pandas implements __init__
     @overload
     def __new__(
         cls,
         data: DatetimeIndex | Sequence[Timestamp | np.datetime64 | datetime],
         index: Axes | None = ...,
-        dtype=...,
+        dtype: TimestampDtypeArg = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
     ) -> TimestampSeries: ...
     @overload
     def __new__(
         cls,
         data: _ListLike,
-        dtype: Literal["datetime64[ns]"],
         index: Axes | None = ...,
+        *,
+        dtype: TimestampDtypeArg,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
     ) -> TimestampSeries: ...
     @overload
     def __new__(
         cls,
         data: PeriodIndex,
         index: Axes | None = ...,
-        dtype=...,
+        dtype: PeriodDtype = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
     ) -> PeriodSeries: ...
     @overload
     def __new__(
         cls,
         data: TimedeltaIndex | Sequence[Timedelta | np.timedelta64 | timedelta],
         index: Axes | None = ...,
-        dtype=...,
+        dtype: TimedeltaDtypeArg = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
     ) -> TimedeltaSeries: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[int]] | Interval[int] | Sequence[Interval[int]],
+        data: IntervalIndex[Interval[_OrderableT]]
+        | Interval[_OrderableT]
+        | Sequence[Interval[_OrderableT]],
         index: Axes | None = ...,
-        dtype=...,
+        dtype: Literal["Interval"] = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
-    ) -> IntervalSeries[int]: ...
+    ) -> IntervalSeries[_OrderableT]: ...
     @overload
     def __new__(
         cls,
-        data: IntervalIndex[Interval[float]]
-        | Interval[float]
-        | Sequence[Interval[float]],
-        index: Axes | None = ...,
-        dtype=...,
-        name: Hashable | None = ...,
-        copy: bool = ...,
-        fastpath: bool = ...,
-    ) -> IntervalSeries[float]: ...
-    @overload
-    def __new__(
-        cls,
-        data: IntervalIndex[Interval[Timestamp]]
-        | Interval[Timestamp]
-        | Sequence[Interval[Timestamp]],
-        index: Axes | None = ...,
-        dtype=...,
-        name: Hashable | None = ...,
-        copy: bool = ...,
-        fastpath: bool = ...,
-    ) -> IntervalSeries[Timestamp]: ...
-    @overload
-    def __new__(
-        cls,
-        data: IntervalIndex[Interval[Timedelta]]
-        | Interval[Timedelta]
-        | Sequence[Interval[Timedelta]],
+        data: object | _ListLike | Series[S1] | dict[int, S1] | dict[_str, S1] | None,
+        dtype: type[S1],
         index: Axes | None = ...,
-        dtype=...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
-    ) -> IntervalSeries[Timedelta]: ...
+    ) -> Self: ...
     @overload
     def __new__(
         cls,
-        data: object | _ListLike | Series[S1] | dict[int, S1] | dict[_str, S1] | None,
-        dtype: type[S1],
+        data: Series[S1] | dict[int, S1] | dict[_str, S1] = ...,
         index: Axes | None = ...,
+        dtype: Dtype = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
-    ) -> Series[S1]: ...
+    ) -> Self: ...
     @overload
     def __new__(
         cls,
-        data: object
-        | _ListLike
-        | Series[S1]
-        | dict[int, S1]
-        | dict[_str, S1]
-        | None = ...,
+        data: object | _ListLike | None = ...,
         index: Axes | None = ...,
-        dtype=...,
+        dtype: Dtype = ...,
         name: Hashable | None = ...,
         copy: bool = ...,
-        fastpath: bool = ...,
     ) -> Series: ...
     @property
     def hasnans(self) -> bool: ...
     def div(
         self,
         other: num | _ListLike | Series[S1],
         level: Level | None = ...,
@@ -442,46 +412,72 @@
         allow_duplicates: bool = ...,
     ) -> None: ...
     @overload
     def to_string(
         self,
         buf: FilePath | WriteBuffer[str],
         na_rep: _str = ...,
-        formatters=...,
-        float_format=...,
-        sparsify: _bool | None = ...,
-        index_names: _bool = ...,
-        justify: _str | None = ...,
+        float_format: Callable[[float], str] = ...,
+        header: _bool = ...,
+        index: _bool = ...,
+        length: _bool = ...,
+        dtype: _bool = ...,
+        name: _bool = ...,
         max_rows: int | None = ...,
         min_rows: int | None = ...,
-        max_cols: int | None = ...,
-        show_dimensions: _bool = ...,
-        decimal: _str = ...,
-        line_width: int | None = ...,
-        max_colwidth: int | None = ...,
-        encoding: _str | None = ...,
     ) -> None: ...
     @overload
     def to_string(
         self,
         buf: None = ...,
         na_rep: _str = ...,
-        formatters=...,
-        float_format=...,
-        sparsify: _bool | None = ...,
-        index_names: _bool = ...,
-        justify: _str | None = ...,
+        float_format: Callable[[float], str] = ...,
+        header: _bool = ...,
+        index: _bool = ...,
+        length: _bool = ...,
+        dtype: _bool = ...,
+        name: _bool = ...,
         max_rows: int | None = ...,
         min_rows: int | None = ...,
-        max_cols: int | None = ...,
-        show_dimensions: _bool = ...,
-        decimal: _str = ...,
-        line_width: int | None = ...,
-        max_colwidth: int | None = ...,
-        encoding: _str | None = ...,
+    ) -> _str: ...
+    @overload
+    def to_json(
+        self,
+        path_or_buf: FilePath | WriteBuffer[str],
+        *,
+        orient: Literal["records"],
+        date_format: Literal["epoch", "iso"] | None = ...,
+        double_precision: int = ...,
+        force_ascii: _bool = ...,
+        date_unit: Literal["s", "ms", "us", "ns"] = ...,
+        default_handler: Callable[[Any], _str | float | _bool | list | dict]
+        | None = ...,
+        lines: Literal[True],
+        compression: CompressionOptions = ...,
+        index: _bool = ...,
+        indent: int | None = ...,
+        mode: Literal["a"],
+    ) -> None: ...
+    @overload
+    def to_json(
+        self,
+        path_or_buf: None = ...,
+        *,
+        orient: Literal["records"],
+        date_format: Literal["epoch", "iso"] | None = ...,
+        double_precision: int = ...,
+        force_ascii: _bool = ...,
+        date_unit: Literal["s", "ms", "us", "ns"] = ...,
+        default_handler: Callable[[Any], _str | float | _bool | list | dict]
+        | None = ...,
+        lines: Literal[True],
+        compression: CompressionOptions = ...,
+        index: _bool = ...,
+        indent: int | None = ...,
+        mode: Literal["a"],
     ) -> _str: ...
     @overload
     def to_json(
         self,
         path_or_buf: FilePath | WriteBuffer[str],
         orient: JsonSeriesOrient | None = ...,
         date_format: Literal["epoch", "iso"] | None = ...,
@@ -490,14 +486,15 @@
         date_unit: Literal["s", "ms", "us", "ns"] = ...,
         default_handler: Callable[[Any], _str | float | _bool | list | dict]
         | None = ...,
         lines: _bool = ...,
         compression: CompressionOptions = ...,
         index: _bool = ...,
         indent: int | None = ...,
+        mode: Literal["w"] = ...,
     ) -> None: ...
     @overload
     def to_json(
         self,
         path_or_buf: None = ...,
         orient: JsonSeriesOrient | None = ...,
         date_format: Literal["epoch", "iso"] | None = ...,
@@ -506,14 +503,15 @@
         date_unit: Literal["s", "ms", "us", "ns"] = ...,
         default_handler: Callable[[Any], _str | float | _bool | list | dict]
         | None = ...,
         lines: _bool = ...,
         compression: CompressionOptions = ...,
         index: _bool = ...,
         indent: int | None = ...,
+        mode: Literal["w"] = ...,
     ) -> _str: ...
     def to_xarray(self) -> xr.DataArray: ...
     def items(self) -> Iterable[tuple[Hashable, S1]]: ...
     def keys(self) -> list: ...
     @overload
     def to_dict(self) -> dict[Any, S1]: ...
     @overload
@@ -527,28 +525,106 @@
         level: Level | None = ...,
         as_index: _bool = ...,
         sort: _bool = ...,
         group_keys: _bool = ...,
         squeeze: _bool = ...,
         observed: _bool = ...,
         dropna: _bool = ...,
-    ) -> _SeriesGroupByScalar[S1]: ...
+    ) -> SeriesGroupBy[S1, Scalar]: ...
+    @overload
+    def groupby(
+        self,
+        by: DatetimeIndex,
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, Timestamp]: ...
+    @overload
+    def groupby(
+        self,
+        by: TimedeltaIndex,
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, Timedelta]: ...
+    @overload
+    def groupby(
+        self,
+        by: PeriodIndex,
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, Period]: ...
+    @overload
+    def groupby(
+        self,
+        by: IntervalIndex[IntervalT],
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, IntervalT]: ...
+    @overload
+    def groupby(
+        self,
+        by: MultiIndex | GroupByObjectNonScalar = ...,
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, tuple]: ...
+    @overload
+    def groupby(
+        self,
+        by: Series[SeriesByT],
+        axis: AxisIndex = ...,
+        level: Level | None = ...,
+        as_index: _bool = ...,
+        sort: _bool = ...,
+        group_keys: _bool = ...,
+        squeeze: _bool = ...,
+        observed: _bool = ...,
+        dropna: _bool = ...,
+    ) -> SeriesGroupBy[S1, SeriesByT]: ...
     @overload
     def groupby(
         self,
-        by: GroupByObjectNonScalar = ...,
+        by: CategoricalIndex | Index | Series,
         axis: AxisIndex = ...,
         level: Level | None = ...,
         as_index: _bool = ...,
         sort: _bool = ...,
         group_keys: _bool = ...,
         squeeze: _bool = ...,
         observed: _bool = ...,
         dropna: _bool = ...,
-    ) -> _SeriesGroupByNonScalar[S1]: ...
+    ) -> SeriesGroupBy[S1, Any]: ...
     # need the ignore because None is Hashable
     @overload
     def count(self, level: None = ...) -> int: ...  # type: ignore[misc]
     @overload
     def count(self, level: Hashable) -> Series[S1]: ...
     def mode(self, dropna=...) -> Series[S1]: ...
     def unique(self) -> np.ndarray: ...
@@ -771,15 +847,15 @@
         axis: AxisIndex = ...,
         *args,
         **kwargs,
     ) -> DataFrame: ...
     @overload
     def apply(
         self,
-        func: Callable[..., Scalar | Sequence | set | Mapping],
+        func: Callable[..., Scalar | Sequence | set | Mapping | None],
         convertDType: _bool = ...,
         args: tuple = ...,
         **kwds,
     ) -> Series: ...
     @overload
     def apply(
         self,
@@ -1726,29 +1802,29 @@
         level: Level | None = ...,
         fill_value: float | None = ...,
         axis: AxisIndex = ...,
     ) -> Series[S1]: ...
     @overload
     def rolling(
         self,
-        window: int | _str | BaseOffset | BaseIndexer,
+        window: int | _str | timedelta | BaseOffset | BaseIndexer,
         min_periods: int | None = ...,
         center: _bool = ...,
         on: _str | None = ...,
         axis: AxisIndex = ...,
         closed: IntervalClosedType | None = ...,
         step: int | None = ...,
         method: CalculationMethod = ...,
         *,
         win_type: _str,
     ) -> Window[Series]: ...
     @overload
     def rolling(
         self,
-        window: int | _str | BaseOffset | BaseIndexer,
+        window: int | _str | timedelta | BaseOffset | BaseIndexer,
         min_periods: int | None = ...,
         center: _bool = ...,
         on: _str | None = ...,
         axis: AxisIndex = ...,
         closed: IntervalClosedType | None = ...,
         step: int | None = ...,
         method: CalculationMethod = ...,
@@ -1815,15 +1891,15 @@
         level: Level | None = ...,
         fill_value: float | None = ...,
         axis: AxisIndex | None = ...,
     ) -> Series[S1]: ...
     # ignore needed because of mypy, for using `Never` as type-var.
     @overload
     def sum(
-        self: Series[Never],  # type: ignore[type-var]
+        self: Series[Never],
         axis: AxisIndex | None = ...,
         skipna: _bool | None = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         min_count: int = ...,
         **kwargs,
     ) -> Any: ...
@@ -1900,24 +1976,24 @@
     ) -> Series[S1]: ...
     def __iter__(self) -> Iterator[S1]: ...
 
 class TimestampSeries(Series[Timestamp]):
     # ignore needed because of mypy
     @property
     def dt(self) -> TimestampProperties: ...  # type: ignore[override]
-    def __add__(self, other: TimedeltaSeries | np.timedelta64) -> TimestampSeries: ...  # type: ignore[override]
-    def __radd__(self, other: TimedeltaSeries | np.timedelta64) -> TimestampSeries: ...  # type: ignore[override]
+    def __add__(self, other: TimedeltaSeries | np.timedelta64 | timedelta) -> TimestampSeries: ...  # type: ignore[override]
+    def __radd__(self, other: TimedeltaSeries | np.timedelta64 | timedelta) -> TimestampSeries: ...  # type: ignore[override]
     @overload  # type: ignore[override]
     def __sub__(
         self, other: Timestamp | datetime | TimestampSeries
     ) -> TimedeltaSeries: ...
     @overload
     def __sub__(
         self,
-        other: Timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64,
+        other: timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64,
     ) -> TimestampSeries: ...
     def __mul__(self, other: float | Series[int] | Series[float] | Sequence[float]) -> TimestampSeries: ...  # type: ignore[override]
     def __truediv__(self, other: float | Series[int] | Series[float] | Sequence[float]) -> TimestampSeries: ...  # type: ignore[override]
     def mean(  # type: ignore[override]
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/strings.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/strings.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/datetimes.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/numeric.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/numeric.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/tools/timedeltas.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/tools/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/ewm.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/window/ewm.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/expanding.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/window/expanding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/core/window/rolling.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/core/window/rolling.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/errors/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/errors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/api.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/clipboards.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/clipboards.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/excel/_base.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/excel/_base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     keep_default_na: bool = ...,
     na_filter: bool = ...,
     verbose: bool = ...,
     parse_dates: bool
     | Sequence[int]
     | Sequence[Sequence[str] | Sequence[int]]
     | dict[str, Sequence[int] | list[str]] = ...,
-    date_parser: Callable | None = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     thousands: str | None = ...,
     decimal: str = ...,
     comment: str | None = ...,
     skipfooter: int = ...,
     storage_options: StorageOptions = ...,
     dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> dict[int | str, DataFrame]: ...
@@ -97,15 +97,15 @@
     keep_default_na: bool = ...,
     na_filter: bool = ...,
     verbose: bool = ...,
     parse_dates: bool
     | Sequence[int]
     | Sequence[Sequence[str] | Sequence[int]]
     | dict[str, Sequence[int] | list[str]] = ...,
-    date_parser: Callable | None = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     thousands: str | None = ...,
     decimal: str = ...,
     comment: str | None = ...,
     skipfooter: int = ...,
     storage_options: StorageOptions = ...,
     dtype_backend: DtypeBackend | NoDefault = ...,
 ) -> DataFrame: ...
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/style.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/formats/style_render.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/formats/style_render.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/gbq.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/gbq.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/html.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/html.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/json/_json.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/json/_json.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import abc
+from collections.abc import Mapping
 from types import TracebackType
 from typing import (
     Generic,
     Literal,
     overload,
 )
 
@@ -25,15 +26,15 @@
 
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonSeriesOrient | None = ...,
     typ: Literal["series"],
-    dtype: bool | dict[HashableT, DtypeArg] | None = ...,
+    dtype: bool | Mapping[HashableT, DtypeArg] | None = ...,
     convert_axes: bool | None = ...,
     convert_dates: bool | list[str] = ...,
     keep_default_dates: bool = ...,
     precise_float: bool = ...,
     date_unit: Literal["s", "ms", "us", "ns"] | None = ...,
     encoding: str | None = ...,
     encoding_errors: Literal[
@@ -49,15 +50,15 @@
 ) -> JsonReader[Series]: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonFrameOrient | None = ...,
     typ: Literal["frame"] = ...,
-    dtype: bool | dict[HashableT, DtypeArg] | None = ...,
+    dtype: bool | Mapping[HashableT, DtypeArg] | None = ...,
     convert_axes: bool | None = ...,
     convert_dates: bool | list[str] = ...,
     keep_default_dates: bool = ...,
     precise_float: bool = ...,
     date_unit: Literal["s", "ms", "us", "ns"] | None = ...,
     encoding: str | None = ...,
     encoding_errors: Literal[
@@ -73,15 +74,15 @@
 ) -> JsonReader[DataFrame]: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonSeriesOrient | None = ...,
     typ: Literal["series"],
-    dtype: bool | dict[HashableT, DtypeArg] | None = ...,
+    dtype: bool | Mapping[HashableT, DtypeArg] | None = ...,
     convert_axes: bool | None = ...,
     convert_dates: bool | list[str] = ...,
     keep_default_dates: bool = ...,
     precise_float: bool = ...,
     date_unit: Literal["s", "ms", "us", "ns"] | None = ...,
     encoding: str | None = ...,
     encoding_errors: Literal[
@@ -97,15 +98,15 @@
 ) -> Series: ...
 @overload
 def read_json(
     path_or_buf: FilePath | ReadBuffer[str] | ReadBuffer[bytes],
     *,
     orient: JsonFrameOrient | None = ...,
     typ: Literal["frame"] = ...,
-    dtype: bool | dict[HashableT, DtypeArg] | None = ...,
+    dtype: bool | Mapping[HashableT, DtypeArg] | None = ...,
     convert_axes: bool | None = ...,
     convert_dates: bool | list[str] = ...,
     keep_default_dates: bool = ...,
     precise_float: bool = ...,
     date_unit: Literal["s", "ms", "us", "ns"] | None = ...,
     encoding: str | None = ...,
     encoding_errors: Literal[
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/parsers/readers.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/parsers/readers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import (
     abc,
     defaultdict,
 )
 from collections.abc import (
     Callable,
+    Hashable,
     Mapping,
     Sequence,
 )
 import csv
 from types import TracebackType
 from typing import (
     Any,
@@ -64,16 +65,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
-    date_format: str | Mapping[int | str, str] | None = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[True],
     chunksize: int | None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -125,16 +125,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
-    date_format: str | Mapping[int | str, str] | None = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: bool = ...,
     chunksize: int,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -186,16 +185,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
-    date_format: str | Mapping[int | str, str] | None = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[False] = ...,
     chunksize: None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -247,15 +245,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[True],
     chunksize: int | None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -306,15 +304,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: bool = ...,
     chunksize: int,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -365,15 +363,15 @@
     parse_dates: bool
     | list[int]
     | list[str]
     | Sequence[Sequence[int]]
     | Mapping[str, Sequence[int | str]] = ...,
     infer_datetime_format: bool = ...,
     keep_date_col: bool = ...,
-    date_parser: Callable = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     dayfirst: bool = ...,
     cache_dates: bool = ...,
     iterator: Literal[False] = ...,
     chunksize: None = ...,
     compression: CompressionOptions = ...,
     thousands: str | None = ...,
     decimal: str = ...,
@@ -398,38 +396,41 @@
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
     dtype_backend: DtypeBackend | NoDefault = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     iterator: Literal[True],
     chunksize: int | None = ...,
     **kwds: Any,
 ) -> TextFileReader: ...
 @overload
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
     dtype_backend: DtypeBackend | NoDefault = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     iterator: bool = ...,
     chunksize: int,
     **kwds: Any,
 ) -> TextFileReader: ...
 @overload
 def read_fwf(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     colspecs: Sequence[tuple[int, int]] | Literal["infer"] | None = ...,
     widths: Sequence[int] | None = ...,
     infer_nrows: int = ...,
     dtype_backend: DtypeBackend | NoDefault = ...,
+    date_format: dict[Hashable, str] | str | None = ...,
     iterator: Literal[False] = ...,
     chunksize: None = ...,
     **kwds: Any,
 ) -> DataFrame: ...
 
 class TextFileReader(abc.Iterator):
     engine: CSVEngine
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/pickle.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/pickle.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/pytables.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/sas/sasreader.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/sas/sasreader.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/sql.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/sql.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,33 @@
     Literal,
     overload,
 )
 
 from pandas.core.base import PandasObject
 from pandas.core.frame import DataFrame
 import sqlalchemy.engine
+from sqlalchemy.orm import FromStatement
 import sqlalchemy.sql.expression
 from typing_extensions import TypeAlias
 
 from pandas._libs.lib import NoDefault
 from pandas._typing import (
     DtypeArg,
     DtypeBackend,
     npt,
 )
 
 _SQLConnection: TypeAlias = str | sqlalchemy.engine.Connectable | sqlite3.Connection
 
 _SQLStatement: TypeAlias = (
-    str | sqlalchemy.sql.expression.Selectable | sqlalchemy.sql.expression.TextClause
+    str
+    | sqlalchemy.sql.expression.Selectable
+    | sqlalchemy.sql.expression.TextClause
+    | sqlalchemy.sql.Select
+    | FromStatement
 )
 
 @overload
 def read_sql_table(
     table_name: str,
     con: _SQLConnection,
     schema: str | None = ...,
```

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/stata.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/stata.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/io/xml.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/io/xml.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/plotting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_core.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/plotting/_core.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/plotting/_misc.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/plotting/_misc.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/tseries/holiday.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/tseries/holiday.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/tseries/offsets.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/tseries/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/util/_validators.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/util/_validators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pandas-stubs/util/version/__init__.pyi` & `pandas_stubs-2.0.2.230605/pandas-stubs/util/version/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-2.0.1.230501/pyproject.toml` & `pandas_stubs-2.0.2.230605/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-stubs"
-version = "2.0.1.230501"
+version = "2.0.2.230605"
 description = "Type annotations for pandas"
 authors = ["The Pandas Development Team <pandas-dev@python.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pandas.pydata.org"
 repository = "https://github.com/pandas-dev/pandas-stubs"
 classifiers = [
@@ -29,42 +29,42 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pandas-dev/pandas-stubs/issues"
 "Documentation" = "https://pandas.pydata.org/pandas-docs/stable"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 types-pytz = ">= 2022.1.1"
+numpy = ">=1.24.3"
 
 [tool.poetry.dev-dependencies]
-mypy = "1.2.0"
+mypy = "1.3.0"
+pandas = "2.0.2"
 pyarrow = ">=10.0.1"
 pytest = ">=7.1.2"
-pyright = ">= 1.1.305"
+pyright = ">= 1.1.310"
 poethepoet = ">=0.16.5"
 loguru = ">=0.6.0"
-pandas = "2.0.1"
-numpy = ">=1.24.3"
 typing-extensions = ">=4.4.0"
 matplotlib = ">=3.5.1"
 pre-commit = ">=2.19.0"
 black = ">=23.3.0"
 isort = ">=5.12.0"
 openpyxl = ">=3.0.10"
 tables = { version = ">=3.7.0" , python = "<4"}  # 3.8.0 depends on blosc2 which caps python to <4
-lxml = { version = ">=4.7.1,<4.9.0", python = "<3.11" }
+lxml = ">=4.9.1"
 pyreadstat = ">=1.2.0"
 xlrd = ">=2.0.1"
 xlsxwriter = ">=3.0.3"
 pyxlsb = ">=1.0.10"
 odfpy = ">=1.4.1"
 xarray = ">=22.6.0"
 tabulate = ">=0.8.10"
-jinja2 = "^3.1"
+jinja2 = ">=3.1"
 scipy = ">=1.9.1"
-SQLAlchemy = "<=1.4.45"
+SQLAlchemy = ">=2.0.12"
 types-python-dateutil = ">=2.8.19"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks.test_all]
@@ -191,10 +191,11 @@
 reportUnknownParameterType = false
 reportUnknownVariableType = false
 reportUntypedBaseClass = false
 reportUnusedVariable = false
 reportPrivateUsage = false
 # enable optional checks
 reportMissingModuleSource = true
+useLibraryCodeForTypes = false
 
 [tool.codespell]
 ignore-words-list = "indext, mose, sav, ser"
```

### Comparing `pandas_stubs-2.0.1.230501/README.md` & `pandas_stubs-2.0.2.230605/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
 ## Differences between type declarations in pandas and pandas-stubs
 
 The <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API's.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.
 
 The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
 
-If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.
+If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints> for a discussion of typing standards used within the pandas code.
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  
 
 ## Discussion and Development
```

### Comparing `pandas_stubs-2.0.1.230501/setup.py` & `pandas_stubs-2.0.2.230605/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,21 @@
                   'io/sas/*',
                   'plotting/*',
                   'tseries/*',
                   'util/*',
                   'util/version/*']}
 
 install_requires = \
-['types-pytz>=2022.1.1']
+['numpy>=1.24.3', 'types-pytz>=2022.1.1']
 
 setup_kwargs = {
     'name': 'pandas-stubs',
-    'version': '2.0.1.230501',
+    'version': '2.0.2.230605',
     'description': 'Type annotations for pandas',
-    'long_description': '# pandas-stubs: Public type stubs for pandas\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![Conda Latest Release](https://anaconda.org/conda-forge/pandas-stubs/badges/version.svg)](https://anaconda.org/conda-forge/pandas-stubs)\n[![Package Status](https://img.shields.io/pypi/status/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![License](https://img.shields.io/pypi/l/pandas-stubs.svg)](https://github.com/pandas-dev/pandas-stubs/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pandas-stubs?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas-stubs)\n[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas)\n[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n\n## What is it?\n\nThese are public type stubs for [**pandas**](http://pandas.pydata.org/), following the\nconvention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of\npandas.  In general, these stubs are narrower than what is possibly allowed by pandas,\nbut follow a convention of suggesting best recommended practices for using pandas.\n\nThe stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.\n\nThe stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension\n[pylance](https://github.com/microsoft/pylance-release#readme).\n\n## Usage\n\nLet’s take this example piece of code in file `round.py`\n\n```python\nimport pandas as pd\n\ndecimals = pd.DataFrame({\'TSLA\': 2, \'AMZN\': 1})\nprices = pd.DataFrame(data={\'date\': [\'2021-08-13\', \'2021-08-07\', \'2021-08-21\'],\n                            \'TSLA\': [720.13, 716.22, 731.22], \'AMZN\': [3316.50, 3200.50, 3100.23]})\nrounded_prices = prices.round(decimals=decimals)\n```\n\nMypy won\'t see any issues with that, but after installing pandas-stubs and running it again:\n\n```sh\nmypy round.py\n```\n\nwe get the following error message:\n\n```text\nround.py:6: error: Argument "decimals" to "round" of "DataFrame" has incompatible type "DataFrame"; expected "Union[int, Dict[Any, Any], Series[Any]]"  [arg-type]\nFound 1 error in 1 file (checked 1 source file)\n```\n\nAnd, if you use pyright:\n\n```sh\npyright round.py\n```\n\nyou get the following error message:\n\n```text\n round.py:6:40 - error: Argument of type "DataFrame" cannot be assigned to parameter "decimals" of type "int | Dict[Unknown, Unknown] | Series[Unknown]" in function "round"\n  \xa0\xa0Type "DataFrame" cannot be assigned to type "int | Dict[Unknown, Unknown] | Series[Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "int"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Dict[Unknown, Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Series[Unknown]" (reportGeneralTypeIssues)\n```\n\nAnd after confirming with the [docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.round.html)\nwe can fix the code:\n\n```python\ndecimals = pd.Series({\'TSLA\': 2, \'AMZN\': 1})\n```\n\n## Version Numbering Convention\n\nThe version number x.y.z.yymmdd corresponds to a test done with pandas version x.y.z, with the stubs released on the date mm/yy/dd.\nIt is anticipated that the stubs will be released more frequently than pandas as the stubs are expected to evolve due to more\npublic visibility.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: <https://github.com/pandas-dev/pandas-stubs>\n\nBinary installers for the latest released version are available at the [Python\nPackage Index (PyPI)](https://pypi.org/project/pandas-stubs) and on [conda-forge](https://conda-forge.org/).\n\n```sh\n# conda\nconda install pandas-stubs\n```\n\n```sh\n# or PyPI\npip install pandas-stubs\n```\n\n## Dependencies\n\n- [pandas: powerful Python data analysis toolkit](https://pandas.pydata.org/)\n- [typing-extensions >= 4.2.0 - supporting the latest typing extensions](https://github.com/python/typing_extensions#readme)\n\n## Installation from sources\n\n- Make sure you have `python >= 3.8` installed.\n- Install poetry\n\n```sh\n# conda\nconda install poetry\n```\n\n```sh\n# or PyPI\npip install poetry\n```\n\n- Install the project dependencies\n\n```sh\npoetry update -vvv\n```\n\n- Build and install the distribution\n\n```sh\npoetry run poe build_dist\npoetry run poe install_dist\n```\n\n## License\n\n[BSD 3](LICENSE)\n\n## Documentation\n\nDocumentation is a work-in-progress.  \n\n## Background\n\nThese stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).\n\nThese stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).\n\nWe are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.\n\n## Differences between type declarations in pandas and pandas-stubs\n\nThe <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API\'s.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.\n\nThe <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.\n\nIf issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.\n\n## Getting help\n\nAsk questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  \n\n## Discussion and Development\n\nMost development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.\n\n## Contributing to pandas-stubs\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.\n',
+    'long_description': '# pandas-stubs: Public type stubs for pandas\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![Conda Latest Release](https://anaconda.org/conda-forge/pandas-stubs/badges/version.svg)](https://anaconda.org/conda-forge/pandas-stubs)\n[![Package Status](https://img.shields.io/pypi/status/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![License](https://img.shields.io/pypi/l/pandas-stubs.svg)](https://github.com/pandas-dev/pandas-stubs/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pandas-stubs?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas-stubs)\n[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas)\n[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n\n## What is it?\n\nThese are public type stubs for [**pandas**](http://pandas.pydata.org/), following the\nconvention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of\npandas.  In general, these stubs are narrower than what is possibly allowed by pandas,\nbut follow a convention of suggesting best recommended practices for using pandas.\n\nThe stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.\n\nThe stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension\n[pylance](https://github.com/microsoft/pylance-release#readme).\n\n## Usage\n\nLet’s take this example piece of code in file `round.py`\n\n```python\nimport pandas as pd\n\ndecimals = pd.DataFrame({\'TSLA\': 2, \'AMZN\': 1})\nprices = pd.DataFrame(data={\'date\': [\'2021-08-13\', \'2021-08-07\', \'2021-08-21\'],\n                            \'TSLA\': [720.13, 716.22, 731.22], \'AMZN\': [3316.50, 3200.50, 3100.23]})\nrounded_prices = prices.round(decimals=decimals)\n```\n\nMypy won\'t see any issues with that, but after installing pandas-stubs and running it again:\n\n```sh\nmypy round.py\n```\n\nwe get the following error message:\n\n```text\nround.py:6: error: Argument "decimals" to "round" of "DataFrame" has incompatible type "DataFrame"; expected "Union[int, Dict[Any, Any], Series[Any]]"  [arg-type]\nFound 1 error in 1 file (checked 1 source file)\n```\n\nAnd, if you use pyright:\n\n```sh\npyright round.py\n```\n\nyou get the following error message:\n\n```text\n round.py:6:40 - error: Argument of type "DataFrame" cannot be assigned to parameter "decimals" of type "int | Dict[Unknown, Unknown] | Series[Unknown]" in function "round"\n  \xa0\xa0Type "DataFrame" cannot be assigned to type "int | Dict[Unknown, Unknown] | Series[Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "int"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Dict[Unknown, Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Series[Unknown]" (reportGeneralTypeIssues)\n```\n\nAnd after confirming with the [docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.round.html)\nwe can fix the code:\n\n```python\ndecimals = pd.Series({\'TSLA\': 2, \'AMZN\': 1})\n```\n\n## Version Numbering Convention\n\nThe version number x.y.z.yymmdd corresponds to a test done with pandas version x.y.z, with the stubs released on the date mm/yy/dd.\nIt is anticipated that the stubs will be released more frequently than pandas as the stubs are expected to evolve due to more\npublic visibility.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: <https://github.com/pandas-dev/pandas-stubs>\n\nBinary installers for the latest released version are available at the [Python\nPackage Index (PyPI)](https://pypi.org/project/pandas-stubs) and on [conda-forge](https://conda-forge.org/).\n\n```sh\n# conda\nconda install pandas-stubs\n```\n\n```sh\n# or PyPI\npip install pandas-stubs\n```\n\n## Dependencies\n\n- [pandas: powerful Python data analysis toolkit](https://pandas.pydata.org/)\n- [typing-extensions >= 4.2.0 - supporting the latest typing extensions](https://github.com/python/typing_extensions#readme)\n\n## Installation from sources\n\n- Make sure you have `python >= 3.8` installed.\n- Install poetry\n\n```sh\n# conda\nconda install poetry\n```\n\n```sh\n# or PyPI\npip install poetry\n```\n\n- Install the project dependencies\n\n```sh\npoetry update -vvv\n```\n\n- Build and install the distribution\n\n```sh\npoetry run poe build_dist\npoetry run poe install_dist\n```\n\n## License\n\n[BSD 3](LICENSE)\n\n## Documentation\n\nDocumentation is a work-in-progress.  \n\n## Background\n\nThese stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).\n\nThese stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).\n\nWe are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.\n\n## Differences between type declarations in pandas and pandas-stubs\n\nThe <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API\'s.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.\n\nThe <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.\n\nIf issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints> for a discussion of typing standards used within the pandas code.\n\n## Getting help\n\nAsk questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  \n\n## Discussion and Development\n\nMost development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.\n\n## Contributing to pandas-stubs\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.\n',
     'author': 'The Pandas Development Team',
     'author_email': 'pandas-dev@python.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pandas.pydata.org',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pandas_stubs-2.0.1.230501/PKG-INFO` & `pandas_stubs-2.0.2.230605/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-stubs
-Version: 2.0.1.230501
+Version: 2.0.2.230605
 Summary: Type annotations for pandas
 Home-page: https://pandas.pydata.org
 License: BSD-3-Clause
 Author: The Pandas Development Team
 Author-email: pandas-dev@python.org
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
+Requires-Dist: numpy (>=1.24.3)
 Requires-Dist: types-pytz (>=2022.1.1)
 Project-URL: Bug Tracker, https://github.com/pandas-dev/pandas-stubs/issues
 Project-URL: Documentation, https://pandas.pydata.org/pandas-docs/stable
 Project-URL: Repository, https://github.com/pandas-dev/pandas-stubs
 Description-Content-Type: text/markdown
 
 # pandas-stubs: Public type stubs for pandas
@@ -178,15 +179,15 @@
 
 ## Differences between type declarations in pandas and pandas-stubs
 
 The <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API's.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.
 
 The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
 
-If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.
+If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints> for a discussion of typing standards used within the pandas code.
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  
 
 ## Discussion and Development
```

