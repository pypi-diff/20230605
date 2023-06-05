# Comparing `tmp/vnpy_ctastrategy-1.1.4.tar.gz` & `tmp/vnpy_ctastrategy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_ctastrategy-1.1.4.tar", last modified: Sun Apr 23 03:38:22 2023, max compression
+gzip compressed data, was "vnpy_ctastrategy-1.1.5.tar", last modified: Mon Jun  5 13:44:01 2023, max compression
```

## Comparing `vnpy_ctastrategy-1.1.4.tar` & `vnpy_ctastrategy-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.392650 vnpy_ctastrategy-1.1.4/
--rw-rw-rw-   0        0        0     1107 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     1969 2023-04-23 03:38:22.392650 vnpy_ctastrategy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      946 2023-04-23 03:37:50.000000 vnpy_ctastrategy-1.1.4/README.md
--rw-rw-rw-   0        0        0     1088 2023-04-23 03:38:22.395653 vnpy_ctastrategy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.296113 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/
--rw-rw-rw-   0        0        0     2072 2023-04-23 02:03:30.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/__init__.py
--rw-rw-rw-   0        0        0    37582 2023-02-13 09:22:23.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/backtesting.py
--rw-rw-rw-   0        0        0     1274 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/base.py
--rw-rw-rw-   0        0        0    32778 2023-04-23 02:01:58.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/engine.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.375373 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/
--rw-rw-rw-   0        0        0        0 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/__init__.py
--rw-rw-rw-   0        0        0     3764 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/atr_rsi_strategy.py
--rw-rw-rw-   0        0        0     3701 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/boll_channel_strategy.py
--rw-rw-rw-   0        0        0     2919 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/double_ma_strategy.py
--rw-rw-rw-   0        0        0     4192 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/dual_thrust_strategy.py
--rw-rw-rw-   0        0        0     4185 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/king_keltner_strategy.py
--rw-rw-rw-   0        0        0     6118 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_signal_strategy.py
--rw-rw-rw-   0        0        0     3667 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py
--rw-rw-rw-   0        0        0     3044 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/test_strategy.py
--rw-rw-rw-   0        0        0     4381 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/turtle_signal_strategy.py
--rw-rw-rw-   0        0        0    13503 2023-01-06 11:08:07.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/template.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.389650 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/
--rw-rw-rw-   0        0        0       32 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/cta.ico
--rw-rw-rw-   0        0        0     9024 2023-03-08 14:40:08.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/rollover.py
--rw-rw-rw-   0        0        0    17453 2023-03-09 07:35:44.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:38:22.338937 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/
--rw-rw-rw-   0        0        0     1969 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 03:38:22.000000 vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 13:44:01.813995 vnpy_ctastrategy-1.1.5/
+-rw-rw-rw-   0        0        0     1107 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1969 2023-06-05 13:44:01.814991 vnpy_ctastrategy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2023-04-23 03:37:50.000000 vnpy_ctastrategy-1.1.5/README.md
+-rw-rw-rw-   0        0        0     1088 2023-06-05 13:44:01.816992 vnpy_ctastrategy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:44:01.622666 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/
+-rw-rw-rw-   0        0        0     2072 2023-04-23 02:03:30.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/__init__.py
+-rw-rw-rw-   0        0        0    37530 2023-06-05 13:34:26.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/backtesting.py
+-rw-rw-rw-   0        0        0     1274 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/base.py
+-rw-rw-rw-   0        0        0    32778 2023-04-23 02:01:58.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:44:01.775588 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/
+-rw-rw-rw-   0        0        0        0 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/__init__.py
+-rw-rw-rw-   0        0        0     3764 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/atr_rsi_strategy.py
+-rw-rw-rw-   0        0        0     3701 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/boll_channel_strategy.py
+-rw-rw-rw-   0        0        0     2919 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/double_ma_strategy.py
+-rw-rw-rw-   0        0        0     4192 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/dual_thrust_strategy.py
+-rw-rw-rw-   0        0        0     4185 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/king_keltner_strategy.py
+-rw-rw-rw-   0        0        0     6118 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/multi_signal_strategy.py
+-rw-rw-rw-   0        0        0     3667 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py
+-rw-rw-rw-   0        0        0     3044 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/test_strategy.py
+-rw-rw-rw-   0        0        0     4381 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/turtle_signal_strategy.py
+-rw-rw-rw-   0        0        0    13503 2023-01-06 11:08:07.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/template.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:44:01.812000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/
+-rw-rw-rw-   0        0        0       32 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2023-01-06 11:03:46.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/cta.ico
+-rw-rw-rw-   0        0        0     9024 2023-03-08 14:40:08.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/rollover.py
+-rw-rw-rw-   0        0        0    17453 2023-03-09 07:35:44.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:44:01.675204 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/
+-rw-rw-rw-   0        0        0     1969 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-05 13:44:01.000000 vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/top_level.txt
```

### Comparing `vnpy_ctastrategy-1.1.4/LICENSE` & `vnpy_ctastrategy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/PKG-INFO` & `vnpy_ctastrategy-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_ctastrategy
-Version: 1.1.4
+Version: 1.1.5
 Summary: CTA strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
```

### Comparing `vnpy_ctastrategy-1.1.4/README.md` & `vnpy_ctastrategy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/setup.cfg` & `vnpy_ctastrategy-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6374 6173 7472 6174   = vnpy_ctastrat
 00000020: 6567 790d 0a76 6572 7369 6f6e 203d 2031  egy..version = 1
-00000030: 2e31 2e34 0d0a 7572 6c20 3d20 6874 7470  .1.4..url = http
+00000030: 2e31 2e35 0d0a 7572 6c20 3d20 6874 7470  .1.5..url = http
 00000040: 733a 2f2f 7777 772e 766e 7079 2e63 6f6d  s://www.vnpy.com
 00000050: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
 00000060: 0a61 7574 686f 7220 3d20 5869 616f 796f  .author = Xiaoyo
 00000070: 7520 4368 656e 0d0a 6175 7468 6f72 5f65  u Chen..author_e
 00000080: 6d61 696c 203d 2078 6961 6f79 6f75 2e63  mail = xiaoyou.c
 00000090: 6865 6e40 6d61 696c 2e76 6e70 792e 636f  hen@mail.vnpy.co
 000000a0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
```

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/__init__.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/backtesting.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/backtesting.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 import traceback
 
 import numpy as np
 from pandas import DataFrame, Series
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from vnpy.trader.constant import (Direction, Offset, Exchange,
-                                  Interval, Status)
+from vnpy.trader.constant import (
+    Direction,
+    Offset,
+    Exchange,
+    Interval,
+    Status
+)
 from vnpy.trader.database import get_database, BaseDatabase
 from vnpy.trader.object import OrderData, TradeData, BarData, TickData
-from vnpy.trader.utility import round_to
+from vnpy.trader.utility import round_to, extract_vt_symbol
 from vnpy.trader.optimize import (
     OptimizationSetting,
     check_optimization_setting,
     run_bf_optimization,
     run_ga_optimization
 )
 
@@ -129,15 +134,19 @@
         self.pricetick = pricetick
         self.start = start
 
         self.symbol, exchange_str = self.vt_symbol.split(".")
         self.exchange = Exchange(exchange_str)
 
         self.capital = capital
-        self.end = end
+
+        if not end:
+            end = datetime.now()
+        self.end = end.replace(hour=23, minute=59, second=59)
+
         self.mode = mode
         self.risk_free = risk_free
         self.annual_days = annual_days
 
     def add_strategy(self, strategy_class: Type[CtaTemplate], setting: dict) -> None:
         """"""
         self.strategy_class = strategy_class
@@ -204,52 +213,26 @@
         """"""
         if self.mode == BacktestingMode.BAR:
             func = self.new_bar
         else:
             func = self.new_tick
 
         self.strategy.on_init()
-
-        # Use the first [days] of history data for initializing strategy
-        day_count: int = 0
-        ix: int = 0
-
-        for ix, data in enumerate(self.history_data):
-            if self.datetime and data.datetime.day != self.datetime.day:
-                day_count += 1
-                if day_count >= self.days:
-                    break
-
-            self.datetime = data.datetime
-
-            try:
-                self.callback(data)
-            except Exception:
-                self.output("触发异常，回测终止")
-                self.output(traceback.format_exc())
-                return
-
         self.strategy.inited = True
         self.output("策略初始化完成")
 
         self.strategy.on_start()
         self.strategy.trading = True
         self.output("开始回放历史数据")
 
-        # Use the rest of history data for running backtesting
-        backtesting_data: list = self.history_data[ix:]
-        if len(backtesting_data) <= 1:
-            self.output("历史数据不足，回测终止")
-            return
-
-        total_size: int = len(backtesting_data)
+        total_size: int = len(self.history_data)
         batch_size: int = max(int(total_size / 10), 1)
 
         for ix, i in enumerate(range(0, total_size, batch_size)):
-            batch_data: list = backtesting_data[i: i + batch_size]
+            batch_data: list = self.history_data[i: i + batch_size]
             for data in batch_data:
                 try:
                     func(data)
                 except Exception:
                     self.output("触发异常，回测终止")
                     self.output(traceback.format_exc())
                     return
@@ -262,16 +245,15 @@
         self.output("历史数据回放结束")
 
     def calculate_result(self) -> DataFrame:
         """"""
         self.output("开始计算逐日盯市盈亏")
 
         if not self.trades:
-            self.output("成交记录为空，无法计算")
-            return
+            self.output("回测成交记录为空")
 
         # Add trade data into daily reuslt.
         for trade in self.trades.values():
             d: date = trade.datetime.date()
             daily_result: DailyResult = self.daily_results[d]
             daily_result.add_trade(trade)
 
@@ -785,23 +767,54 @@
         vt_symbol: str,
         days: int,
         interval: Interval,
         callback: Callable,
         use_database: bool
     ) -> List[BarData]:
         """"""
-        self.days = days
         self.callback = callback
-        return []
+
+        init_end = self.start - INTERVAL_DELTA_MAP[interval]
+        init_start = self.start - timedelta(days=days)
+
+        symbol, exchange = extract_vt_symbol(vt_symbol)
+
+        bars: List[BarData] = load_bar_data(
+            symbol,
+            exchange,
+            interval,
+            init_start,
+            init_end
+        )
+
+        for bar in bars:
+            callback(bar)
+
+        return bars
 
     def load_tick(self, vt_symbol: str, days: int, callback: Callable) -> List[TickData]:
         """"""
-        self.days = days
         self.callback = callback
-        return []
+
+        init_end = self.start - timedelta(seconds=1)
+        init_start = self.start - timedelta(days=days)
+
+        symbol, exchange = extract_vt_symbol(vt_symbol)
+
+        ticks: List[TickData] = load_tick_data(
+            symbol,
+            exchange,
+            init_start,
+            init_end
+        )
+
+        for tick in ticks:
+            callback(tick)
+
+        return ticks
 
     def send_order(
         self,
         strategy: CtaTemplate,
         direction: Direction,
         offset: Offset,
         price: float,
@@ -1120,15 +1133,15 @@
     engine.add_strategy(strategy_class, setting)
     engine.load_data()
     engine.run_backtesting()
     engine.calculate_result()
     statistics: dict = engine.calculate_statistics(output=False)
 
     target_value: float = statistics[target_name]
-    return (str(setting), target_value, statistics)
+    return (setting, target_value, statistics)
 
 
 def wrap_evaluate(engine: BacktestingEngine, target_name: str) -> callable:
     """
     Wrap evaluate function with given setting from backtesting engine.
     """
     func: callable = partial(
```

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/base.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/base.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/engine.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/engine.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/atr_rsi_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/atr_rsi_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/boll_channel_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/boll_channel_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/double_ma_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/double_ma_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/dual_thrust_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/dual_thrust_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/king_keltner_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/king_keltner_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_signal_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/multi_signal_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/multi_timeframe_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/test_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/test_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/strategies/turtle_signal_strategy.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/strategies/turtle_signal_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/template.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/template.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/cta.ico` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/cta.ico`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/rollover.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/rollover.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy/ui/widget.py` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/PKG-INFO` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-ctastrategy
-Version: 1.1.4
+Version: 1.1.5
 Summary: CTA strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Platform: UNKNOWN
```

### Comparing `vnpy_ctastrategy-1.1.4/vnpy_ctastrategy.egg-info/SOURCES.txt` & `vnpy_ctastrategy-1.1.5/vnpy_ctastrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

