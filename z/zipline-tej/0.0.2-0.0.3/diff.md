# Comparing `tmp/zipline-tej-0.0.2.tar.gz` & `tmp/zipline-tej-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline-tej-0.0.2.tar", last modified: Fri Jun  2 09:37:04 2023, max compression
+gzip compressed data, was "zipline-tej-0.0.3.tar", last modified: Mon Jun  5 02:02:54 2023, max compression
```

## Comparing `zipline-tej-0.0.2.tar` & `zipline-tej-0.0.3.tar`

### file list

```diff
@@ -1,147 +1,206 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.672865 zipline-tej-0.0.2/
--rw-rw-rw-   0        0        0    13262 2023-06-02 09:37:04.672865 zipline-tej-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12877 2023-06-02 09:13:48.000000 zipline-tej-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 09:37:04.672865 zipline-tej-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1777 2023-06-02 09:37:01.000000 zipline-tej-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.456732 zipline-tej-0.0.2/zipline-tej/
--rw-rw-rw-   0        0        0     3674 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/__init__.py
--rw-rw-rw-   0        0        0    12296 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/__main__.py
--rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/_version.py
--rw-rw-rw-   0        0        0    89973 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/algorithm.py
--rw-rw-rw-   0        0        0     1678 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/api.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.472355 zipline-tej-0.0.2/zipline-tej/assets/
--rw-rw-rw-   0        0        0     1188 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/__init__.py
--rw-rw-rw-   0        0        0    17577 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/asset_db_migrations.py
--rw-rw-rw-   0        0        0     4943 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/asset_db_schema.py
--rw-rw-rw-   0        0        0    35430 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/asset_writer.py
--rw-rw-rw-   0        0        0    54555 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/assets.py
--rw-rw-rw-   0        0        0     2078 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/exchange_info.py
--rw-rw-rw-   0        0        0      767 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/futures.py
--rw-rw-rw-   0        0        0    11295 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/roll_finder.py
--rw-rw-rw-   0        0        0    10815 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/assets/synthetic.py
--rw-rw-rw-   0        0        0     1799 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/country.py
--rw-rw-rw-   0        0        0     1819 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/currency.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.503603 zipline-tej-0.0.2/zipline-tej/data/
--rw-rw-rw-   0        0        0      209 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/__init__.py
--rw-rw-rw-   0        0        0    26366 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/adjustments.py
--rw-rw-rw-   0        0        0     4181 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/bar_reader.py
--rw-rw-rw-   0        0        0    25147 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/bcolz_daily_bars.py
--rw-rw-rw-   0        0        0     1652 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/benchmarks.py
--rw-rw-rw-   0        0        0    12351 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/continuous_future_reader.py
--rw-rw-rw-   0        0        0    59712 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/data_portal.py
--rw-rw-rw-   0        0        0     4947 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/dispatch_bar_reader.py
--rw-rw-rw-   0        0        0    34276 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/hdf5_daily_bars.py
--rw-rw-rw-   0        0        0    21993 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/history_loader.py
--rw-rw-rw-   0        0        0     5382 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/in_memory_daily_bars.py
--rw-rw-rw-   0        0        0     1272 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/loader.py
--rw-rw-rw-   0        0        0    48513 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/minute_bars.py
--rw-rw-rw-   0        0        0    27729 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/resample.py
--rw-rw-rw-   0        0        0     1817 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/session_bars.py
--rw-rw-rw-   0        0        0     1700 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/data/treasury.py
--rw-rw-rw-   0        0        0      285 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/dispatch.py
--rw-rw-rw-   0        0        0    26888 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.519227 zipline-tej-0.0.2/zipline-tej/examples/
--rw-rw-rw-   0        0        0     2378 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/__init__.py
--rw-rw-rw-   0        0        0     1612 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/buy_and_hold.py
--rw-rw-rw-   0        0        0     2034 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/buyapple.py
--rw-rw-rw-   0        0        0     2439 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/buyapple_ide.py
--rw-rw-rw-   0        0        0     4470 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/dual_ema_talib.py
--rw-rw-rw-   0        0        0     4165 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/dual_moving_average.py
--rw-rw-rw-   0        0        0     3162 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/momentum_pipeline.py
--rw-rw-rw-   0        0        0     4878 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/examples/olmar.py
--rw-rw-rw-   0        0        0     7312 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/extensions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.541362 zipline-tej-0.0.2/zipline-tej/finance/
--rw-rw-rw-   0        0        0      670 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/__init__.py
--rw-rw-rw-   0        0        0     7089 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/asset_restrictions.py
--rw-rw-rw-   0        0        0     2096 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/cancel_policy.py
--rw-rw-rw-   0        0        0    13935 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/commission.py
--rw-rw-rw-   0        0        0     6879 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/constants.py
--rw-rw-rw-   0        0        0    14273 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/controls.py
--rw-rw-rw-   0        0        0     7533 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/execution.py
--rw-rw-rw-   0        0        0    28436 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/ledger.py
--rw-rw-rw-   0        0        0     8621 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/order.py
--rw-rw-rw-   0        0        0     8147 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/position.py
--rw-rw-rw-   0        0        0     1647 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/shared.py
--rw-rw-rw-   0        0        0    22666 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/slippage.py
--rw-rw-rw-   0        0        0     5556 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/trading.py
--rw-rw-rw-   0        0        0     2473 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/finance/transaction.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.541362 zipline-tej-0.0.2/zipline-tej/gens/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/gens/__init__.py
--rw-rw-rw-   0        0        0     1063 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/gens/composites.py
--rw-rw-rw-   0        0        0    12006 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/gens/tradesimulation.py
--rw-rw-rw-   0        0        0     1999 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/gens/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.556988 zipline-tej-0.0.2/zipline-tej/lib/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/lib/__init__.py
--rw-rw-rw-   0        0        0    13462 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/lib/adjusted_array.py
--rw-rw-rw-   0        0        0    28546 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/lib/labelarray.py
--rw-rw-rw-   0        0        0     1813 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/lib/normalize.py
--rw-rw-rw-   0        0        0      389 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/lib/quantiles.py
--rw-rw-rw-   0        0        0     8376 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/master.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.588235 zipline-tej-0.0.2/zipline-tej/pipeline/
--rw-rw-rw-   0        0        0      734 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1707 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/api_utils.py
--rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/common.py
--rw-rw-rw-   0        0        0    14783 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/domain.py
--rw-rw-rw-   0        0        0     1903 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/downsample_helpers.py
--rw-rw-rw-   0        0        0      323 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/dtypes.py
--rw-rw-rw-   0        0        0    36374 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/engine.py
--rw-rw-rw-   0        0        0    10639 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/expression.py
--rw-rw-rw-   0        0        0    17933 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/graph.py
--rw-rw-rw-   0        0        0    24184 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/mixins.py
--rw-rw-rw-   0        0        0    11318 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/pipeline.py
--rw-rw-rw-   0        0        0      197 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/sentinels.py
--rw-rw-rw-   0        0        0    33623 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/term.py
--rw-rw-rw-   0        0        0     6068 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/pipeline/visualize.py
--rw-rw-rw-   0        0        0     8182 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/protocol.py
--rw-rw-rw-   0        0        0    18936 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/test_algorithms.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.588235 zipline-tej-0.0.2/zipline-tej/testing/
--rw-rw-rw-   0        0        0     1404 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/__init__.py
--rw-rw-rw-   0        0        0    55119 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/core.py
--rw-rw-rw-   0        0        0     2683 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/debug.py
--rw-rw-rw-   0        0        0    82068 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/fixtures.py
--rw-rw-rw-   0        0        0     3306 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/pipeline_terms.py
--rw-rw-rw-   0        0        0    17906 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/predicates.py
--rw-rw-rw-   0        0        0     1066 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/testing/slippage.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.657243 zipline-tej-0.0.2/zipline-tej/utils/
--rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/__init__.py
--rw-rw-rw-   0        0        0      787 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/algo_instance.py
--rw-rw-rw-   0        0        0     4268 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/api_support.py
--rw-rw-rw-   0        0        0    10164 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/argcheck.py
--rw-rw-rw-   0        0        0    11721 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/cache.py
--rw-rw-rw-   0        0        0     4063 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/calendar_utils.py
--rw-rw-rw-   0        0        0      191 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/classproperty.py
--rw-rw-rw-   0        0        0     3319 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/cli.py
--rw-rw-rw-   0        0        0      854 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/compat.py
--rw-rw-rw-   0        0        0     2244 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/context_tricks.py
--rw-rw-rw-   0        0        0     7689 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/data.py
--rw-rw-rw-   0        0        0     1774 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/date_utils.py
--rw-rw-rw-   0        0        0     1572 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/deprecate.py
--rw-rw-rw-   0        0        0      248 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/dummy.py
--rw-rw-rw-   0        0        0    25153 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/events.py
--rw-rw-rw-   0        0        0     1226 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/exploding_object.py
--rw-rw-rw-   0        0        0     5023 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/factory.py
--rw-rw-rw-   0        0        0     3902 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/final.py
--rw-rw-rw-   0        0        0     1651 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/formatting.py
--rw-rw-rw-   0        0        0    10662 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/functional.py
--rw-rw-rw-   0        0        0      665 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/idbox.py
--rw-rw-rw-   0        0        0    26914 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/input_validation.py
--rw-rw-rw-   0        0        0     2668 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/math_utils.py
--rw-rw-rw-   0        0        0     7957 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/memoize.py
--rw-rw-rw-   0        0        0    13647 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/numpy_utils.py
--rw-rw-rw-   0        0        0     9268 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/pandas_utils.py
--rw-rw-rw-   0        0        0     5983 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/paths.py
--rw-rw-rw-   0        0        0     7429 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/preprocess.py
--rw-rw-rw-   0        0        0     5025 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/range.py
--rw-rw-rw-   0        0        0    38036 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/run_algo.py
--rw-rw-rw-   0        0        0     5408 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/security_list.py
--rw-rw-rw-   0        0        0     2380 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/sentinel.py
--rw-rw-rw-   0        0        0     3610 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/sharedoc.py
--rw-rw-rw-   0        0        0     1760 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/sqlite_utils.py
--rw-rw-rw-   0        0        0      402 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/utils/string_formatting.py
--rw-rw-rw-   0        0        0      664 2023-06-02 08:45:48.000000 zipline-tej-0.0.2/zipline-tej/zipline_warnings.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:37:04.672865 zipline-tej-0.0.2/zipline_tej.egg-info/
--rw-rw-rw-   0        0        0    13262 2023-06-02 09:37:04.000000 zipline-tej-0.0.2/zipline_tej.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4190 2023-06-02 09:37:04.000000 zipline-tej-0.0.2/zipline_tej.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:37:04.000000 zipline-tej-0.0.2/zipline_tej.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-06-02 09:37:04.000000 zipline-tej-0.0.2/zipline_tej.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 09:37:04.000000 zipline-tej-0.0.2/zipline_tej.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.753879 zipline-tej-0.0.3/
+-rw-rw-rw-   0        0        0    13262 2023-06-05 02:02:54.753879 zipline-tej-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12877 2023-06-02 09:13:48.000000 zipline-tej-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 02:02:54.753879 zipline-tej-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3585 2023-06-05 02:01:55.000000 zipline-tej-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.437410 zipline-tej-0.0.3/zipline-tej/
+-rw-rw-rw-   0        0        0     3674 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/__init__.py
+-rw-rw-rw-   0        0        0    12296 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/__main__.py
+-rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/_version.py
+-rw-rw-rw-   0        0        0    89973 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/algorithm.py
+-rw-rw-rw-   0        0        0     1678 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/api.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.453035 zipline-tej-0.0.3/zipline-tej/assets/
+-rw-rw-rw-   0        0        0     1188 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/__init__.py
+-rw-rw-rw-   0        0        0    17577 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/asset_db_migrations.py
+-rw-rw-rw-   0        0        0     4943 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/asset_db_schema.py
+-rw-rw-rw-   0        0        0    35430 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/asset_writer.py
+-rw-rw-rw-   0        0        0    54555 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/assets.py
+-rw-rw-rw-   0        0        0     2078 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/exchange_info.py
+-rw-rw-rw-   0        0        0      767 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/futures.py
+-rw-rw-rw-   0        0        0    11295 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/roll_finder.py
+-rw-rw-rw-   0        0        0    10815 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/assets/synthetic.py
+-rw-rw-rw-   0        0        0     1799 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/country.py
+-rw-rw-rw-   0        0        0     1819 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/currency.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.484283 zipline-tej-0.0.3/zipline-tej/data/
+-rw-rw-rw-   0        0        0      209 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/__init__.py
+-rw-rw-rw-   0        0        0    26366 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/adjustments.py
+-rw-rw-rw-   0        0        0     4181 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bar_reader.py
+-rw-rw-rw-   0        0        0    25147 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bcolz_daily_bars.py
+-rw-rw-rw-   0        0        0     1652 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/benchmarks.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.484283 zipline-tej-0.0.3/zipline-tej/data/bundles/
+-rw-rw-rw-   0        0        0      627 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bundles/__init__.py
+-rw-rw-rw-   0        0        0    21102 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bundles/core.py
+-rw-rw-rw-   0        0        0     8742 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bundles/csvdir.py
+-rw-rw-rw-   0        0        0     9059 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bundles/quandl.py
+-rw-rw-rw-   0        0        0    12516 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/bundles/tquant.py
+-rw-rw-rw-   0        0        0    12351 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/continuous_future_reader.py
+-rw-rw-rw-   0        0        0    59712 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/data_portal.py
+-rw-rw-rw-   0        0        0     4947 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/dispatch_bar_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.499906 zipline-tej-0.0.3/zipline-tej/data/fx/
+-rw-rw-rw-   0        0        0      366 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/__init__.py
+-rw-rw-rw-   0        0        0     5495 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/base.py
+-rw-rw-rw-   0        0        0      394 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/exploding.py
+-rw-rw-rw-   0        0        0    11540 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/hdf5.py
+-rw-rw-rw-   0        0        0     1843 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/in_memory.py
+-rw-rw-rw-   0        0        0      355 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/fx/utils.py
+-rw-rw-rw-   0        0        0    34276 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/hdf5_daily_bars.py
+-rw-rw-rw-   0        0        0    21993 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/history_loader.py
+-rw-rw-rw-   0        0        0     5382 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/in_memory_daily_bars.py
+-rw-rw-rw-   0        0        0     1272 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/loader.py
+-rw-rw-rw-   0        0        0    48513 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/minute_bars.py
+-rw-rw-rw-   0        0        0    27729 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/resample.py
+-rw-rw-rw-   0        0        0     1817 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/session_bars.py
+-rw-rw-rw-   0        0        0     1700 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/data/treasury.py
+-rw-rw-rw-   0        0        0      285 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/dispatch.py
+-rw-rw-rw-   0        0        0    26888 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.524605 zipline-tej-0.0.3/zipline-tej/examples/
+-rw-rw-rw-   0        0        0     2378 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/buy_and_hold.py
+-rw-rw-rw-   0        0        0     2034 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/buyapple.py
+-rw-rw-rw-   0        0        0     2439 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/buyapple_ide.py
+-rw-rw-rw-   0        0        0     4470 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/dual_ema_talib.py
+-rw-rw-rw-   0        0        0     4165 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/dual_moving_average.py
+-rw-rw-rw-   0        0        0     3162 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/momentum_pipeline.py
+-rw-rw-rw-   0        0        0     4878 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/examples/olmar.py
+-rw-rw-rw-   0        0        0     7312 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/extensions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.537731 zipline-tej-0.0.3/zipline-tej/finance/
+-rw-rw-rw-   0        0        0      670 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/__init__.py
+-rw-rw-rw-   0        0        0     7089 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/asset_restrictions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.553361 zipline-tej-0.0.3/zipline-tej/finance/blotter/
+-rw-rw-rw-   0        0        0      739 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/blotter/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/blotter/blotter.py
+-rw-rw-rw-   0        0        0    17341 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/blotter/simulation_blotter.py
+-rw-rw-rw-   0        0        0     2096 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/cancel_policy.py
+-rw-rw-rw-   0        0        0    13935 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/commission.py
+-rw-rw-rw-   0        0        0     6879 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/constants.py
+-rw-rw-rw-   0        0        0    14273 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/controls.py
+-rw-rw-rw-   0        0        0     7533 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/execution.py
+-rw-rw-rw-   0        0        0    28436 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/ledger.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.553361 zipline-tej-0.0.3/zipline-tej/finance/metrics/
+-rw-rw-rw-   0        0        0     3720 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3095 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/metrics/core.py
+-rw-rw-rw-   0        0        0    29630 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/metrics/metric.py
+-rw-rw-rw-   0        0        0    11837 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/metrics/tracker.py
+-rw-rw-rw-   0        0        0     8621 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/order.py
+-rw-rw-rw-   0        0        0     8147 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/position.py
+-rw-rw-rw-   0        0        0     1647 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/shared.py
+-rw-rw-rw-   0        0        0    22666 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/slippage.py
+-rw-rw-rw-   0        0        0     5556 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/trading.py
+-rw-rw-rw-   0        0        0     2473 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/finance/transaction.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.568985 zipline-tej-0.0.3/zipline-tej/gens/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/gens/__init__.py
+-rw-rw-rw-   0        0        0     1063 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/gens/composites.py
+-rw-rw-rw-   0        0        0    12006 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/gens/tradesimulation.py
+-rw-rw-rw-   0        0        0     1999 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/gens/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.568985 zipline-tej-0.0.3/zipline-tej/lib/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/lib/__init__.py
+-rw-rw-rw-   0        0        0    13462 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/lib/adjusted_array.py
+-rw-rw-rw-   0        0        0    28546 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/lib/labelarray.py
+-rw-rw-rw-   0        0        0     1813 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/lib/normalize.py
+-rw-rw-rw-   0        0        0      389 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/lib/quantiles.py
+-rw-rw-rw-   0        0        0     8376 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/master.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.600233 zipline-tej-0.0.3/zipline-tej/pipeline/
+-rw-rw-rw-   0        0        0      734 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1707 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/api_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.600233 zipline-tej-0.0.3/zipline-tej/pipeline/classifiers/
+-rw-rw-rw-   0        0        0      230 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/classifiers/__init__.py
+-rw-rw-rw-   0        0        0    19647 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/classifiers/classifier.py
+-rw-rw-rw-   0        0        0      518 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/common.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.615857 zipline-tej-0.0.3/zipline-tej/pipeline/data/
+-rw-rw-rw-   0        0        0      382 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/data/__init__.py
+-rw-rw-rw-   0        0        0    33755 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/data/dataset.py
+-rw-rw-rw-   0        0        0      827 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/data/equity_pricing.py
+-rw-rw-rw-   0        0        0    19447 2023-06-02 09:04:44.000000 zipline-tej-0.0.3/zipline-tej/pipeline/data/tejquant.py
+-rw-rw-rw-   0        0        0     1006 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/data/testing.py
+-rw-rw-rw-   0        0        0    14783 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/domain.py
+-rw-rw-rw-   0        0        0     1903 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/downsample_helpers.py
+-rw-rw-rw-   0        0        0      323 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/dtypes.py
+-rw-rw-rw-   0        0        0    36374 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/engine.py
+-rw-rw-rw-   0        0        0    10639 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/expression.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.637990 zipline-tej-0.0.3/zipline-tej/pipeline/factors/
+-rw-rw-rw-   0        0        0     1907 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/__init__.py
+-rw-rw-rw-   0        0        0    16252 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/basic.py
+-rw-rw-rw-   0        0        0     3614 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/events.py
+-rw-rw-rw-   0        0        0    65638 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/factor.py
+-rw-rw-rw-   0        0        0    26905 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/statistical.py
+-rw-rw-rw-   0        0        0    12277 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/factors/technical.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.637990 zipline-tej-0.0.3/zipline-tej/pipeline/filters/
+-rw-rw-rw-   0        0        0      628 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/filters/__init__.py
+-rw-rw-rw-   0        0        0    25761 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/filters/filter.py
+-rw-rw-rw-   0        0        0     1180 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/filters/smoothing.py
+-rw-rw-rw-   0        0        0    17933 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/graph.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.653622 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/
+-rw-rw-rw-   0        0        0      295 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/__init__.py
+-rw-rw-rw-   0        0        0     2245 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/delegate.py
+-rw-rw-rw-   0        0        0     2834 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/iface.py
+-rw-rw-rw-   0        0        0      599 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/no.py
+-rw-rw-rw-   0        0        0    16278 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/progress.py
+-rw-rw-rw-   0        0        0     1901 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/hooks/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.669246 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/
+-rw-rw-rw-   0        0        0      171 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/__init__.py
+-rw-rw-rw-   0        0        0     1599 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/base.py
+-rw-rw-rw-   0        0        0    61161 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/earnings_estimates.py
+-rw-rw-rw-   0        0        0     7578 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/equity_pricing_loader.py
+-rw-rw-rw-   0        0        0     8556 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/events.py
+-rw-rw-rw-   0        0        0     6844 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/frame.py
+-rw-rw-rw-   0        0        0    13063 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/synthetic.py
+-rw-rw-rw-   0        0        0      651 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/testing.py
+-rw-rw-rw-   0        0        0    13306 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/loaders/utils.py
+-rw-rw-rw-   0        0        0    24184 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/mixins.py
+-rw-rw-rw-   0        0        0    11318 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/pipeline.py
+-rw-rw-rw-   0        0        0      197 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/sentinels.py
+-rw-rw-rw-   0        0        0    33623 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/term.py
+-rw-rw-rw-   0        0        0     6068 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/pipeline/visualize.py
+-rw-rw-rw-   0        0        0     8182 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/protocol.py
+-rw-rw-rw-   0        0        0    18936 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/test_algorithms.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.684873 zipline-tej-0.0.3/zipline-tej/testing/
+-rw-rw-rw-   0        0        0     1404 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/__init__.py
+-rw-rw-rw-   0        0        0    55119 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/core.py
+-rw-rw-rw-   0        0        0     2683 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/debug.py
+-rw-rw-rw-   0        0        0    82068 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/fixtures.py
+-rw-rw-rw-   0        0        0     3306 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/pipeline_terms.py
+-rw-rw-rw-   0        0        0    17906 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/predicates.py
+-rw-rw-rw-   0        0        0     1066 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/testing/slippage.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.738248 zipline-tej-0.0.3/zipline-tej/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/algo_instance.py
+-rw-rw-rw-   0        0        0     4268 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/api_support.py
+-rw-rw-rw-   0        0        0    10164 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/argcheck.py
+-rw-rw-rw-   0        0        0    11721 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/cache.py
+-rw-rw-rw-   0        0        0     4063 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/calendar_utils.py
+-rw-rw-rw-   0        0        0      191 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/classproperty.py
+-rw-rw-rw-   0        0        0     3319 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/cli.py
+-rw-rw-rw-   0        0        0      854 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/compat.py
+-rw-rw-rw-   0        0        0     2244 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/context_tricks.py
+-rw-rw-rw-   0        0        0     7689 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/data.py
+-rw-rw-rw-   0        0        0     1774 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/date_utils.py
+-rw-rw-rw-   0        0        0     1572 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/deprecate.py
+-rw-rw-rw-   0        0        0      248 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/dummy.py
+-rw-rw-rw-   0        0        0    25153 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/events.py
+-rw-rw-rw-   0        0        0     1226 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/exploding_object.py
+-rw-rw-rw-   0        0        0     5023 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/factory.py
+-rw-rw-rw-   0        0        0     3902 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/final.py
+-rw-rw-rw-   0        0        0     1651 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/formatting.py
+-rw-rw-rw-   0        0        0    10662 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/functional.py
+-rw-rw-rw-   0        0        0      665 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/idbox.py
+-rw-rw-rw-   0        0        0    26914 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/input_validation.py
+-rw-rw-rw-   0        0        0     2668 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/math_utils.py
+-rw-rw-rw-   0        0        0     7957 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/memoize.py
+-rw-rw-rw-   0        0        0    13647 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/numpy_utils.py
+-rw-rw-rw-   0        0        0     9268 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/pandas_utils.py
+-rw-rw-rw-   0        0        0     5983 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/paths.py
+-rw-rw-rw-   0        0        0     7429 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/preprocess.py
+-rw-rw-rw-   0        0        0     5025 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/range.py
+-rw-rw-rw-   0        0        0    38036 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/run_algo.py
+-rw-rw-rw-   0        0        0     5408 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/security_list.py
+-rw-rw-rw-   0        0        0     2380 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/sentinel.py
+-rw-rw-rw-   0        0        0     3610 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/sharedoc.py
+-rw-rw-rw-   0        0        0     1760 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/sqlite_utils.py
+-rw-rw-rw-   0        0        0      402 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/utils/string_formatting.py
+-rw-rw-rw-   0        0        0      664 2023-06-02 08:45:48.000000 zipline-tej-0.0.3/zipline-tej/zipline_warnings.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:02:54.753879 zipline-tej-0.0.3/zipline_tej.egg-info/
+-rw-rw-rw-   0        0        0    13262 2023-06-05 02:02:54.000000 zipline-tej-0.0.3/zipline_tej.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6085 2023-06-05 02:02:54.000000 zipline-tej-0.0.3/zipline_tej.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 02:02:54.000000 zipline-tej-0.0.3/zipline_tej.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-06-05 02:02:54.000000 zipline-tej-0.0.3/zipline_tej.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-05 02:02:54.000000 zipline-tej-0.0.3/zipline_tej.egg-info/top_level.txt
```

### Comparing `zipline-tej-0.0.2/PKG-INFO` & `zipline-tej-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-tej
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for stock backtesting modified by TEJ.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

### Comparing `zipline-tej-0.0.2/README.md` & `zipline-tej-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/__init__.py` & `zipline-tej-0.0.3/zipline-tej/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/__main__.py` & `zipline-tej-0.0.3/zipline-tej/__main__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/_version.py` & `zipline-tej-0.0.3/zipline-tej/_version.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/algorithm.py` & `zipline-tej-0.0.3/zipline-tej/algorithm.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/api.py` & `zipline-tej-0.0.3/zipline-tej/api.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/__init__.py` & `zipline-tej-0.0.3/zipline-tej/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/asset_db_migrations.py` & `zipline-tej-0.0.3/zipline-tej/assets/asset_db_migrations.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/asset_db_schema.py` & `zipline-tej-0.0.3/zipline-tej/assets/asset_db_schema.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/asset_writer.py` & `zipline-tej-0.0.3/zipline-tej/assets/asset_writer.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/assets.py` & `zipline-tej-0.0.3/zipline-tej/assets/assets.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/exchange_info.py` & `zipline-tej-0.0.3/zipline-tej/assets/exchange_info.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/futures.py` & `zipline-tej-0.0.3/zipline-tej/assets/futures.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/roll_finder.py` & `zipline-tej-0.0.3/zipline-tej/assets/roll_finder.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/assets/synthetic.py` & `zipline-tej-0.0.3/zipline-tej/assets/synthetic.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/country.py` & `zipline-tej-0.0.3/zipline-tej/country.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/currency.py` & `zipline-tej-0.0.3/zipline-tej/currency.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/adjustments.py` & `zipline-tej-0.0.3/zipline-tej/data/adjustments.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/bar_reader.py` & `zipline-tej-0.0.3/zipline-tej/data/bar_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/bcolz_daily_bars.py` & `zipline-tej-0.0.3/zipline-tej/data/bcolz_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/benchmarks.py` & `zipline-tej-0.0.3/zipline-tej/data/benchmarks.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/continuous_future_reader.py` & `zipline-tej-0.0.3/zipline-tej/data/continuous_future_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/data_portal.py` & `zipline-tej-0.0.3/zipline-tej/data/data_portal.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/dispatch_bar_reader.py` & `zipline-tej-0.0.3/zipline-tej/data/dispatch_bar_reader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/hdf5_daily_bars.py` & `zipline-tej-0.0.3/zipline-tej/data/hdf5_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/history_loader.py` & `zipline-tej-0.0.3/zipline-tej/data/history_loader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/in_memory_daily_bars.py` & `zipline-tej-0.0.3/zipline-tej/data/in_memory_daily_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/loader.py` & `zipline-tej-0.0.3/zipline-tej/data/loader.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/minute_bars.py` & `zipline-tej-0.0.3/zipline-tej/data/minute_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/resample.py` & `zipline-tej-0.0.3/zipline-tej/data/resample.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/session_bars.py` & `zipline-tej-0.0.3/zipline-tej/data/session_bars.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/data/treasury.py` & `zipline-tej-0.0.3/zipline-tej/data/treasury.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/errors.py` & `zipline-tej-0.0.3/zipline-tej/errors.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/__init__.py` & `zipline-tej-0.0.3/zipline-tej/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/buy_and_hold.py` & `zipline-tej-0.0.3/zipline-tej/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/buyapple.py` & `zipline-tej-0.0.3/zipline-tej/examples/buyapple.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/buyapple_ide.py` & `zipline-tej-0.0.3/zipline-tej/examples/buyapple_ide.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/dual_ema_talib.py` & `zipline-tej-0.0.3/zipline-tej/examples/dual_ema_talib.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/dual_moving_average.py` & `zipline-tej-0.0.3/zipline-tej/examples/dual_moving_average.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/momentum_pipeline.py` & `zipline-tej-0.0.3/zipline-tej/examples/momentum_pipeline.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/examples/olmar.py` & `zipline-tej-0.0.3/zipline-tej/examples/olmar.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/extensions.py` & `zipline-tej-0.0.3/zipline-tej/extensions.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/__init__.py` & `zipline-tej-0.0.3/zipline-tej/finance/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/asset_restrictions.py` & `zipline-tej-0.0.3/zipline-tej/finance/asset_restrictions.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/cancel_policy.py` & `zipline-tej-0.0.3/zipline-tej/finance/cancel_policy.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/commission.py` & `zipline-tej-0.0.3/zipline-tej/finance/commission.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/constants.py` & `zipline-tej-0.0.3/zipline-tej/finance/constants.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/controls.py` & `zipline-tej-0.0.3/zipline-tej/finance/controls.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/execution.py` & `zipline-tej-0.0.3/zipline-tej/finance/execution.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/ledger.py` & `zipline-tej-0.0.3/zipline-tej/finance/ledger.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/order.py` & `zipline-tej-0.0.3/zipline-tej/finance/order.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/position.py` & `zipline-tej-0.0.3/zipline-tej/finance/position.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/shared.py` & `zipline-tej-0.0.3/zipline-tej/finance/shared.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/slippage.py` & `zipline-tej-0.0.3/zipline-tej/finance/slippage.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/trading.py` & `zipline-tej-0.0.3/zipline-tej/finance/trading.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/finance/transaction.py` & `zipline-tej-0.0.3/zipline-tej/finance/transaction.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/gens/composites.py` & `zipline-tej-0.0.3/zipline-tej/gens/composites.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/gens/tradesimulation.py` & `zipline-tej-0.0.3/zipline-tej/gens/tradesimulation.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/gens/utils.py` & `zipline-tej-0.0.3/zipline-tej/gens/utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/lib/adjusted_array.py` & `zipline-tej-0.0.3/zipline-tej/lib/adjusted_array.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/lib/labelarray.py` & `zipline-tej-0.0.3/zipline-tej/lib/labelarray.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/lib/normalize.py` & `zipline-tej-0.0.3/zipline-tej/lib/normalize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/master.py` & `zipline-tej-0.0.3/zipline-tej/master.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/__init__.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/api_utils.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/api_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/common.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/common.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/domain.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/domain.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/downsample_helpers.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/downsample_helpers.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/engine.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/engine.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/expression.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/expression.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/graph.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/graph.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/mixins.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/mixins.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/pipeline.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/term.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/term.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/pipeline/visualize.py` & `zipline-tej-0.0.3/zipline-tej/pipeline/visualize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/protocol.py` & `zipline-tej-0.0.3/zipline-tej/protocol.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/test_algorithms.py` & `zipline-tej-0.0.3/zipline-tej/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/__init__.py` & `zipline-tej-0.0.3/zipline-tej/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/core.py` & `zipline-tej-0.0.3/zipline-tej/testing/core.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/debug.py` & `zipline-tej-0.0.3/zipline-tej/testing/debug.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/fixtures.py` & `zipline-tej-0.0.3/zipline-tej/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/pipeline_terms.py` & `zipline-tej-0.0.3/zipline-tej/testing/pipeline_terms.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/predicates.py` & `zipline-tej-0.0.3/zipline-tej/testing/predicates.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/testing/slippage.py` & `zipline-tej-0.0.3/zipline-tej/testing/slippage.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/algo_instance.py` & `zipline-tej-0.0.3/zipline-tej/utils/algo_instance.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/api_support.py` & `zipline-tej-0.0.3/zipline-tej/utils/api_support.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/argcheck.py` & `zipline-tej-0.0.3/zipline-tej/utils/argcheck.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/cache.py` & `zipline-tej-0.0.3/zipline-tej/utils/cache.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/calendar_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/cli.py` & `zipline-tej-0.0.3/zipline-tej/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/compat.py` & `zipline-tej-0.0.3/zipline-tej/utils/compat.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/context_tricks.py` & `zipline-tej-0.0.3/zipline-tej/utils/context_tricks.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/data.py` & `zipline-tej-0.0.3/zipline-tej/utils/data.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/date_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/deprecate.py` & `zipline-tej-0.0.3/zipline-tej/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/events.py` & `zipline-tej-0.0.3/zipline-tej/utils/events.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/exploding_object.py` & `zipline-tej-0.0.3/zipline-tej/utils/exploding_object.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/factory.py` & `zipline-tej-0.0.3/zipline-tej/utils/factory.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/final.py` & `zipline-tej-0.0.3/zipline-tej/utils/final.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/formatting.py` & `zipline-tej-0.0.3/zipline-tej/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/functional.py` & `zipline-tej-0.0.3/zipline-tej/utils/functional.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/idbox.py` & `zipline-tej-0.0.3/zipline-tej/utils/idbox.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/input_validation.py` & `zipline-tej-0.0.3/zipline-tej/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/math_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/memoize.py` & `zipline-tej-0.0.3/zipline-tej/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/numpy_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/pandas_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/paths.py` & `zipline-tej-0.0.3/zipline-tej/utils/paths.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/preprocess.py` & `zipline-tej-0.0.3/zipline-tej/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/range.py` & `zipline-tej-0.0.3/zipline-tej/utils/range.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/run_algo.py` & `zipline-tej-0.0.3/zipline-tej/utils/run_algo.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/security_list.py` & `zipline-tej-0.0.3/zipline-tej/utils/security_list.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/sentinel.py` & `zipline-tej-0.0.3/zipline-tej/utils/sentinel.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/sharedoc.py` & `zipline-tej-0.0.3/zipline-tej/utils/sharedoc.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/utils/sqlite_utils.py` & `zipline-tej-0.0.3/zipline-tej/utils/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline-tej/zipline_warnings.py` & `zipline-tej-0.0.3/zipline-tej/zipline_warnings.py`

 * *Files identical despite different names*

### Comparing `zipline-tej-0.0.2/zipline_tej.egg-info/PKG-INFO` & `zipline-tej-0.0.3/zipline_tej.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-tej
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for stock backtesting modified by TEJ.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

