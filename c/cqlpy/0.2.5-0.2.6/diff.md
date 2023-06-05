# Comparing `tmp/cqlpy-0.2.5.tar.gz` & `tmp/cqlpy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.5.tar", max compression
+gzip compressed data, was "cqlpy-0.2.6.tar", max compression
```

## Comparing `cqlpy-0.2.5.tar` & `cqlpy-0.2.6.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:07:49.980195 cqlpy-0.2.5/LICENSE
--rw-r--r--   0        0        0        8 2023-05-24 13:07:49.980195 cqlpy-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     5073 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0      748 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/cql_value_set_provider.py
--rw-r--r--   0        0        0   342427 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/map.py
--rw-r--r--   0        0        0    16313 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/model.py
--rw-r--r--   0        0        0      689 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     2319 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     1696 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0       92 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      691 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1052 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1165 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      157 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1181 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      404 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      509 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0     9733 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/scripts/fhir_map_generator.py
--rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2459 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      416 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0     1053 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     2003 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/value_set.py
--rw-r--r--   0        0        0      170 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      451 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/context.py
--rw-r--r--   0        0        0     4227 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/operators.py
--rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/__init__.py
--rw-r--r--   0        0        0      216 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/logger.py
--rw-r--r--   0        0        0       15 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/requirements.txt
--rw-r--r--   0        0        0     4871 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/rosetta_valueset_provider.py
--rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/py.typed
--rw-r--r--   0        0        0     1089 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/types.py
--rw-r--r--   0        0        0      670 2023-05-24 13:08:09.424436 cqlpy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-05 20:37:29.512299 cqlpy-0.2.6/LICENSE
+-rw-r--r--   0        0        0        8 2023-06-05 20:37:29.512299 cqlpy-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5339 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0     1801 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/cql_value_set_provider.py
+-rw-r--r--   0        0        0   342427 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/map.py
+-rw-r--r--   0        0        0    16754 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/model.py
+-rw-r--r--   0        0        0      689 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     3016 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     1696 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0      143 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      691 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1052 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1165 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      157 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1181 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      404 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0     9733 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/scripts/fhir_map_generator.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2459 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-06-05 20:37:29.512299 cqlpy-0.2.6/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      416 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0     1053 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2003 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/value_set.py
+-rw-r--r--   0        0        0      735 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/types/value_set_scope.py
+-rw-r--r--   0        0        0      372 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      451 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/context.py
+-rw-r--r--   0        0        0     4227 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/logger.py
+-rw-r--r--   0        0        0       15 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/requirements.txt
+-rw-r--r--   0        0        0     4949 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/providers/rosetta_valueset_provider.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/py.typed
+-rw-r--r--   0        0        0     1089 2023-06-05 20:37:29.516299 cqlpy-0.2.6/cqlpy/types.py
+-rw-r--r--   0        0        0      670 2023-06-05 20:37:53.996531 cqlpy-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.6/PKG-INFO
```

### Comparing `cqlpy-0.2.5/LICENSE` & `cqlpy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/context.py` & `cqlpy-0.2.6/cqlpy/_internal/context/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from cqlpy._internal.context.cql_value_set_provider import CqlValueSetProvider
 
 from cqlpy._internal.context.fhir.r4.model import FhirR4DataModel
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.value_set import ValueSet
+from cqlpy._internal.types.value_set_scope import ValueSetScope
 from cqlpy._internal.valueset_provider import ValueSetProvider
 
 
 class Context:
     """
     A context is a required parameter on every CQL expression that is converted to python as a function.
     The expected signature of every function that implements a CQL Expression is:
@@ -69,30 +70,40 @@
 
         self.parameter_provider = ParameterProvider(parameters)
         self.model = FhirR4DataModel(parsed_bundle, self.parameter_provider)
         self.cql_valueset_provider = CqlValueSetProvider(
             valueset_provider=valueset_provider
         )
 
-    def __getitem__(self, requested_concept: Union[Parameter, ValueSet, str, tuple]):
+    def __getitem__(
+        self,
+        requested_concept: Union[
+            Parameter,
+            ValueSet,
+            ValueSetScope,
+            str,
+            tuple[str, Union[ValueSet, list[Code], Code], str],
+        ],
+    ):
         if isinstance(requested_concept, Parameter):
             # In this case, the return type will be the Cql Type specified by the parameter,
             # i.e. Interval<DateTime>, CqlString, etc.
             return self.parameter_provider[requested_concept]
 
-        elif isinstance(requested_concept, ValueSet):
+        if isinstance(requested_concept, ValueSet) or isinstance(
+            requested_concept, ValueSetScope
+        ):
             # In this case, the return type will be ValueSet (which includes all codes specified by the value set).
             return self.cql_valueset_provider[requested_concept]
 
-        elif isinstance(requested_concept, Code):
+        if isinstance(requested_concept, Code):
             # In this case, there is nothing to lookup... the Code is fully populated.
             return requested_concept
 
-        else:
-            return self.model[requested_concept]
+        return self.model[requested_concept]
 
     def set_context(self, context: str) -> None:
         # At this time, only Patient context is supported and the context is stored without additional action.
         # The current implementation can be extended to support additional contexts by using this stored context in
         # retrieve operations (implemented in __getitem__) to filter the resources returned from the model.
         self.context = context
```

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/map.py` & `cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/map.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/model.py` & `cqlpy-0.2.6/cqlpy/_internal/context/fhir/r4/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 import json
 from typing import Iterator, Optional, Protocol, Sequence, Union
 
 from cqlpy._internal.context.parameter_provider import ParameterProvider
-from cqlpy._internal.context.resource_query import ResourceQuery
+from cqlpy._internal.context.resource_query import ResourceQuery, ResourceQueryFilter
 from cqlpy._internal.context.type_factory import TypeFactory
 from cqlpy._internal.operators.comparison.in_list import in_list
 from cqlpy._internal.operators.list.exists import exists
 from cqlpy._internal.operators.list.intersect import intersect
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.any import CqlAny
@@ -172,24 +172,33 @@
     "Encounter~Procedure": {
         "period": "period:performedDateTime",
         "status": "literal:finished",
     },
 }
 
 
-def _get_filter_codes(
-    filter_: Optional[Union[ValueSet, list[Code], Code]]
-) -> list[Code]:
+def _get_filter_codes(filter_: Optional[ResourceQueryFilter]) -> list[Code]:
     if filter_ is None:
         return []
     if isinstance(filter_, ValueSet):
         return filter_.codes
+    if isinstance(filter_, Code):
+        return [filter_]
     if isinstance(filter_, list):
-        return filter_
-    return [filter_]
+        codes: list[Code] = []
+        for item in filter_:
+            if isinstance(item, ValueSet):
+                codes.extend(item.codes)
+            elif isinstance(item, Code):
+                codes.append(item)
+            else:
+                raise ValueError(f"Unsupported filter item type: {type(item)}")
+        return codes
+
+    raise NotImplementedError
 
 
 class FhirR4DataModel:
     def __init__(self, bundle: dict, parameter_provider: ParameterProvider) -> None:
         self.__parameter_provider = parameter_provider
         self.resource_id_index = {}
         self.resource_type_index: dict[str, list[str]] = {}
@@ -263,22 +272,23 @@
         filter_resource_properties = self.__get_filter_resource_properties(
             resource_type=resource_query.resource_type,
             filter_codes=filter_codes,
             property_name=resource_query.property_name,
         )
 
         if resource_query.property_filter is None:
-            yield from (
-                Resource(self.resource_id_index[id], resource_query.resource_type, self)
-                for id in self.resource_type_index[resource_query.resource_type]
-                if resource_query.resource_type in self.resource_type_index
-            )
+            if resource_query.resource_type in self.resource_type_index:
+                yield from (
+                    Resource(
+                        self.resource_id_index[id], resource_query.resource_type, self
+                    )
+                    for id in self.resource_type_index[resource_query.resource_type]
+                )
             return
 
-        print(filter_resource_properties)
         for filter_resource_type, filter_property_name in filter_resource_properties:
             if filter_resource_type not in self.resource_type_index:
                 continue
 
             for id in self.resource_type_index[filter_resource_type]:
                 resource = Resource(
                     self.resource_id_index[id],
@@ -340,15 +350,17 @@
                 yield related_encounter_resouce
 
             else:
                 yield self.__generate_resource_proxy(resource, resource_type)
 
     def __getitem__(
         self,
-        resource_query: Union[str, tuple[str, Union[ValueSet, list[Code], Code], str]],
+        resource_query: Union[
+            str, tuple[str, Union[ValueSet, list[Code], Code, list[ValueSet]], str]
+        ],
     ) -> Sequence[FhirBase]:
         duration_start_time = datetime.now()
 
         query = ResourceQuery.from_query(resource_query)
 
         if query in self.retrieve_cache:
             print(
```

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.2.6/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.2.6/cqlpy/_internal/context/resource_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Optional, Union
 
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.value_set import ValueSet
 
+ResourceQueryFilter = Union[ValueSet, list[Code], Code, list[ValueSet]]
+
 
 @dataclass(frozen=True, eq=True)
 class ResourceQuery:
     resource_type: str = field()
-    property_filter: Optional[Union[ValueSet, list[Code], Code]] = field(default=None)
+    property_filter: Optional[ResourceQueryFilter] = field(default=None)
     property_name: Optional[str] = field(default=None)
 
     @classmethod
-    def from_query(
-        cls, query: Union[str, tuple[str, Union[ValueSet, list[Code], Code], str]]
-    ):
+    def from_query(cls, query: Union[str, tuple[str, ResourceQueryFilter, str]]):
         if isinstance(query, tuple):
             resource_type = query[0]
             property_filter = query[1] if len(query) > 1 else None
             property_name = query[2] if len(query) > 1 else None
 
         else:
             resource_type = query
@@ -51,12 +51,32 @@
         return f"{self.resource_type} filter on list"
 
     def __hash__(self):
         if self.property_filter is None:
             return hash(self.resource_type)
         if isinstance(self.property_filter, Code):
             return hash((self.resource_type, self.property_filter, self.property_name))
+
         if isinstance(self.property_filter, ValueSet):
             property_filter_hash = hash(tuple(self.property_filter.codes))
-        else:
+        elif isinstance(self.property_filter, list) and isinstance(
+            self.property_filter[0], Code
+        ):
             property_filter_hash = hash(tuple(self.property_filter))
+        elif isinstance(self.property_filter, list) and isinstance(
+            self.property_filter[0], ValueSet
+        ):
+            property_filter_hash = hash(
+                tuple(
+                    [
+                        code
+                        for value_set in self.property_filter
+                        for code in value_set.codes
+                    ]
+                )
+            )
+        else:
+            raise NotImplementedError(
+                f"Unsupported property_filter type: {type(self.property_filter)}"
+            )
+
         return hash((self.resource_type, property_filter_hash, self.property_name))
```

### Comparing `cqlpy-0.2.5/cqlpy/_internal/context/type_factory.py` & `cqlpy-0.2.6/cqlpy/_internal/context/type_factory.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/clinical/any_in_valueset.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/clinical/any_in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/clinical/in_valueset.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/clinical/in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater_or_equal.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/not_equal.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/comparison/not_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/cql_in.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/cql_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/add.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/after.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/after.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/before.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/before.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/calculate_age_at.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/calculate_age_at.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/difference_between.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/duration_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/interval/collapse.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/interval/in_interval.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/interval/in_interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/interval/included_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/interval/overlaps.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/interval/overlaps.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/interval/start.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.2.6/cqlpy/_internal/operators/list/intersect.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/scripts/fhir_map_generator.py` & `cqlpy-0.2.6/cqlpy/_internal/scripts/fhir_map_generator.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/any.py` & `cqlpy-0.2.6/cqlpy/_internal/types/any.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/boolean.py` & `cqlpy-0.2.6/cqlpy/_internal/types/boolean.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/code.py` & `cqlpy-0.2.6/cqlpy/_internal/types/code.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/code_system.py` & `cqlpy-0.2.6/cqlpy/_internal/types/code_system.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/concept.py` & `cqlpy-0.2.6/cqlpy/_internal/types/concept.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/date.py` & `cqlpy-0.2.6/cqlpy/_internal/types/date.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/datetime.py` & `cqlpy-0.2.6/cqlpy/_internal/types/datetime.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/decimal.py` & `cqlpy-0.2.6/cqlpy/_internal/types/decimal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/integer.py` & `cqlpy-0.2.6/cqlpy/_internal/types/integer.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/interval.py` & `cqlpy-0.2.6/cqlpy/_internal/types/interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/list.py` & `cqlpy-0.2.6/cqlpy/_internal/types/list.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/quantity.py` & `cqlpy-0.2.6/cqlpy/_internal/types/quantity.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/string.py` & `cqlpy-0.2.6/cqlpy/_internal/types/string.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/_internal/types/value_set.py` & `cqlpy-0.2.6/cqlpy/_internal/types/value_set.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/operators.py` & `cqlpy-0.2.6/cqlpy/operators.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/cqlpy/providers/rosetta_valueset_provider.py` & `cqlpy-0.2.6/cqlpy/providers/rosetta_valueset_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from datetime import datetime
 import urllib
 import requests
 
 from typing import Optional, Any
 
+from cqlpy._internal.types.value_set import ValueSet
+
 
 FHIR_VERSION = "R4"
 ROSETTA_BASE_URL = (
     f"https://api.rosetta.careevolution.com/terminology/v1/fhir/{FHIR_VERSION}"
 )
 ROSETTA_PAGE_SIZE = 250
 
@@ -94,15 +96,15 @@
         if entry["resource"]["resourceType"] != "ValueSet":
             raise Exception(
                 f"ValueSet search returned unexpected resource {entry['resource']['resourceType']}"
             )
 
         return entry["resource"]
 
-    def get_valuesets_in_scope(self, scope: str):
+    def get_valuesets_in_scope(self, scope: str) -> list[dict[str, Any]]:
         self._logger.info(
             f"RosettaValueSetProvider.get_valuesets_in_scope, fetching valuesets in scope {scope} from {ROSETTA_BASE_URL}"
         )
 
         start_time = datetime.now()
         first_page_result = self._request_paged_valuesets_in_scope(scope=scope)
```

### Comparing `cqlpy-0.2.5/cqlpy/types.py` & `cqlpy-0.2.6/cqlpy/types.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.5/pyproject.toml` & `cqlpy-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^23.3.0"}
```

### Comparing `cqlpy-0.2.5/PKG-INFO` & `cqlpy-0.2.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

