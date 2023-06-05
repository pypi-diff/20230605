# Comparing `tmp/sports-betting-0.5.0.tar.gz` & `tmp/sports-betting-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports-betting-0.5.0.tar", last modified: Thu Apr 27 17:17:44 2023, max compression
+gzip compressed data, was "sports-betting-0.5.1.tar", last modified: Mon Jun  5 19:36:23 2023, max compression
```

## Comparing `sports-betting-0.5.0.tar` & `sports-betting-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1072 2023-04-25 16:59:22.976380 sports-betting-0.5.0/LICENSE
--rw-r--r--   0        0        0     9397 2023-04-25 17:00:49.972566 sports-betting-0.5.0/README.md
--rw-r--r--   0        0        0     5464 2023-04-27 17:17:40.274284 sports-betting-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-04-25 17:00:49.977235 sports-betting-0.5.0/src/sportsbet/__init__.py
--rw-r--r--   0        0        0      131 2023-04-25 16:59:22.992255 sports-betting-0.5.0/src/sportsbet/__main__.py
--rw-r--r--   0        0        0      124 2023-04-25 17:00:49.977635 sports-betting-0.5.0/src/sportsbet/cli/__init__.py
--rw-r--r--   0        0        0      466 2023-04-25 17:00:49.977881 sports-betting-0.5.0/src/sportsbet/cli/_cli.py
--rw-r--r--   0        0        0     3905 2023-04-25 17:00:49.978201 sports-betting-0.5.0/src/sportsbet/cli/_datasets.py
--rw-r--r--   0        0        0     3328 2023-04-25 17:00:49.978506 sports-betting-0.5.0/src/sportsbet/cli/_evaluation.py
--rw-r--r--   0        0        0      874 2023-04-25 17:00:49.978798 sports-betting-0.5.0/src/sportsbet/cli/_options.py
--rw-r--r--   0        0        0     4912 2023-04-25 17:00:49.979119 sports-betting-0.5.0/src/sportsbet/cli/_utils.py
--rw-r--r--   0        0        0      320 2023-04-25 19:18:34.131135 sports-betting-0.5.0/src/sportsbet/datasets/__init__.py
--rw-r--r--   0        0        0    18296 2023-04-25 17:00:49.980378 sports-betting-0.5.0/src/sportsbet/datasets/_base.py
--rw-r--r--   0        0        0    15883 2023-04-25 17:00:49.981171 sports-betting-0.5.0/src/sportsbet/datasets/_dummy.py
--rw-r--r--   0        0        0        0 2023-04-25 16:59:22.999739 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/__init__.py
--rw-r--r--   0        0        0    21957 2023-04-25 17:00:49.981862 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_data.py
--rw-r--r--   0        0        0    29307 2023-04-27 17:17:40.275507 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fd.py
--rw-r--r--   0        0        0     5122 2023-04-26 13:27:31.161262 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fte.py
--rw-r--r--   0        0        0     3802 2023-04-27 17:17:40.277950 sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_utils.py
--rw-r--r--   0        0        0      326 2023-04-25 17:00:49.984179 sports-betting-0.5.0/src/sportsbet/evaluation/__init__.py
--rw-r--r--   0        0        0    11881 2023-04-25 17:00:49.984882 sports-betting-0.5.0/src/sportsbet/evaluation/_base.py
--rw-r--r--   0        0        0     6783 2023-04-25 17:00:49.985439 sports-betting-0.5.0/src/sportsbet/evaluation/_classifier.py
--rw-r--r--   0        0        0     7919 2023-04-25 17:00:49.985811 sports-betting-0.5.0/src/sportsbet/evaluation/_rules.py
--rw-r--r--   0        0        0        0 2023-04-25 16:59:23.004536 sports-betting-0.5.0/src/sportsbet/py.typed
--rw-r--r--   0        0        0      162 2023-04-25 16:59:23.004826 sports-betting-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0       20 2023-04-25 17:00:49.986811 sports-betting-0.5.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      270 2023-04-25 17:00:49.987208 sports-betting-0.5.0/tests/cli/configs/bettor.py
--rw-r--r--   0        0        0      316 2023-04-25 17:00:49.987619 sports-betting-0.5.0/tests/cli/configs/dataloader.py
--rw-r--r--   0        0        0     2919 2023-04-25 17:00:49.988270 sports-betting-0.5.0/tests/cli/test_datasets.py
--rw-r--r--   0        0        0     2050 2023-04-25 17:00:49.988782 sports-betting-0.5.0/tests/cli/test_evaluation.py
--rw-r--r--   0        0        0      482 2023-04-25 17:00:49.989200 sports-betting-0.5.0/tests/cli/test_main.py
--rw-r--r--   0        0        0      310 2023-04-25 16:59:23.005092 sports-betting-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0       28 2023-04-25 16:59:23.005357 sports-betting-0.5.0/tests/datasets/__init__.py
--rw-r--r--   0        0        0    18705 2023-04-25 17:00:49.989963 sports-betting-0.5.0/tests/datasets/test_dummy.py
--rw-r--r--   0        0        0       30 2023-04-25 16:59:23.006158 sports-betting-0.5.0/tests/evaluation/__init__.py
--rw-r--r--   0        0        0     7350 2023-04-25 16:59:23.006482 sports-betting-0.5.0/tests/evaluation/test_classifier.py
--rw-r--r--   0        0        0     2897 2023-04-25 17:00:49.990754 sports-betting-0.5.0/tests/evaluation/test_rules.py
--rw-r--r--   0        0        0    10743 1970-01-01 00:00:00.000000 sports-betting-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-05 19:31:12.611168 sports-betting-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9621 2023-06-05 19:36:15.136886 sports-betting-0.5.1/README.md
+-rw-r--r--   0        0        0     5464 2023-06-05 19:31:12.626661 sports-betting-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-06-05 19:31:12.627671 sports-betting-0.5.1/src/sportsbet/__init__.py
+-rw-r--r--   0        0        0      131 2023-06-05 19:31:12.628356 sports-betting-0.5.1/src/sportsbet/__main__.py
+-rw-r--r--   0        0        0      124 2023-06-05 19:31:12.629392 sports-betting-0.5.1/src/sportsbet/cli/__init__.py
+-rw-r--r--   0        0        0      466 2023-06-05 19:31:12.629917 sports-betting-0.5.1/src/sportsbet/cli/_cli.py
+-rw-r--r--   0        0        0     4005 2023-06-05 19:36:15.137373 sports-betting-0.5.1/src/sportsbet/cli/_datasets.py
+-rw-r--r--   0        0        0     3428 2023-06-05 19:36:15.137783 sports-betting-0.5.1/src/sportsbet/cli/_evaluation.py
+-rw-r--r--   0        0        0      874 2023-06-05 19:31:12.631140 sports-betting-0.5.1/src/sportsbet/cli/_options.py
+-rw-r--r--   0        0        0     4912 2023-06-05 19:31:12.631438 sports-betting-0.5.1/src/sportsbet/cli/_utils.py
+-rw-r--r--   0        0        0      320 2023-06-05 19:31:12.631839 sports-betting-0.5.1/src/sportsbet/datasets/__init__.py
+-rw-r--r--   0        0        0    18296 2023-06-05 19:31:12.632258 sports-betting-0.5.1/src/sportsbet/datasets/_base.py
+-rw-r--r--   0        0        0    15883 2023-06-05 19:31:12.632762 sports-betting-0.5.1/src/sportsbet/datasets/_dummy.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:31:12.632869 sports-betting-0.5.1/src/sportsbet/datasets/_soccer/__init__.py
+-rw-r--r--   0        0        0    21957 2023-06-05 19:31:12.633704 sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_data.py
+-rw-r--r--   0        0        0    29307 2023-06-05 19:31:12.634605 sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_fd.py
+-rw-r--r--   0        0        0     5122 2023-06-05 19:31:12.635697 sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_fte.py
+-rw-r--r--   0        0        0     3802 2023-06-05 19:31:12.636191 sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_utils.py
+-rw-r--r--   0        0        0      326 2023-06-05 19:31:12.636871 sports-betting-0.5.1/src/sportsbet/evaluation/__init__.py
+-rw-r--r--   0        0        0    11881 2023-06-05 19:31:12.637257 sports-betting-0.5.1/src/sportsbet/evaluation/_base.py
+-rw-r--r--   0        0        0     6783 2023-06-05 19:31:12.637574 sports-betting-0.5.1/src/sportsbet/evaluation/_classifier.py
+-rw-r--r--   0        0        0     7919 2023-06-05 19:31:12.637874 sports-betting-0.5.1/src/sportsbet/evaluation/_rules.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:31:12.637954 sports-betting-0.5.1/src/sportsbet/py.typed
+-rw-r--r--   0        0        0      162 2023-06-05 19:31:12.639021 sports-betting-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0       20 2023-06-05 19:31:12.639717 sports-betting-0.5.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-05 19:31:12.640526 sports-betting-0.5.1/tests/cli/configs/bettor.py
+-rw-r--r--   0        0        0      316 2023-06-05 19:31:12.641241 sports-betting-0.5.1/tests/cli/configs/dataloader.py
+-rw-r--r--   0        0        0     2919 2023-06-05 19:31:12.641985 sports-betting-0.5.1/tests/cli/test_datasets.py
+-rw-r--r--   0        0        0     2050 2023-06-05 19:31:12.642627 sports-betting-0.5.1/tests/cli/test_evaluation.py
+-rw-r--r--   0        0        0      482 2023-06-05 19:31:12.643153 sports-betting-0.5.1/tests/cli/test_main.py
+-rw-r--r--   0        0        0      310 2023-06-05 19:31:12.643780 sports-betting-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0       28 2023-06-05 19:31:12.644427 sports-betting-0.5.1/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    18705 2023-06-05 19:31:12.644990 sports-betting-0.5.1/tests/datasets/test_dummy.py
+-rw-r--r--   0        0        0       30 2023-06-05 19:31:12.645576 sports-betting-0.5.1/tests/evaluation/__init__.py
+-rw-r--r--   0        0        0     7350 2023-06-05 19:31:12.646129 sports-betting-0.5.1/tests/evaluation/test_classifier.py
+-rw-r--r--   0        0        0     2897 2023-06-05 19:31:12.647249 sports-betting-0.5.1/tests/evaluation/test_rules.py
+-rw-r--r--   0        0        0    10967 1970-01-01 00:00:00.000000 sports-betting-0.5.1/PKG-INFO
```

### Comparing `sports-betting-0.5.0/LICENSE` & `sports-betting-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/README.md` & `sports-betting-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 git clone https://github.com/georgedouzas/sports-betting.git
 cd sports-betting
 pdm install
 ```
 
 ## Usage
 
+You can use the Python API or the CLI to access the full functionality of `sports-betting`. Nevertheless, it is recommended to be
+familiar with the Python API since it is still needed to write configuration files for the CLI.
+
 ### API
 
 The `sports-betting` package makes it easy to download sports betting data:
 
 ```python
 from sportsbet.datasets import SoccerDataLoader
 dataloader = SoccerDataLoader(param_grid={'league': ['Italy'], 'year': [2020]})
@@ -209,9 +212,9 @@
 ```bash
 sportsbet bettor backtest -b bettor_config.py -d dataloader_config.py
 ```
 
 Get the value bets:
 
 ```bash
-sportsbet bettor bettor -b bettor_config.py -d dataloader_config.py
+sportsbet bettor bet -b bettor_config.py -d dataloader_config.py
 ```
```

### Comparing `sports-betting-0.5.0/pyproject.toml` & `sports-betting-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "vectorbt>=0.24.5",
     "QuantStats>=0.0.47",
     "typing-extensions>=4.5.0",
     "click>=8.1.3",
     "rich>=13.3.3",
     "aiohttp>=3.8.4",
 ]
-version = "0.5.0"
+version = "0.5.1"
 
 [project.urls]
 Homepage = "https://georgedouzas.github.io/sports-betting"
 Documentation = "https://georgedouzas.github.io/sports-betting"
 Changelog = "https://georgedouzas.github.io/sports-betting/changelog"
 Repository = "https://github.com/georgedouzas/sports-betting"
 Issues = "https://github.com/georgedouzas/sports-betting/issues"
```

### Comparing `sports-betting-0.5.0/src/sportsbet/__init__.py` & `sports-betting-0.5.1/src/sportsbet/__init__.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/cli/_datasets.py` & `sports-betting-0.5.1/src/sportsbet/cli/_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     mod = get_module(dataloader_config_path)
     dataloader = get_dataloader(mod)
     if dataloader is None:
         return
     train_params = get_train_params(mod)
     X_train, Y_train, O_train = dataloader.extract_train_data(**train_params)
     if mod is not None:
-        path = str(Path(dataloader_config_path).parent / mod.MAIN.get('path'))
+        path = Path(dataloader_config_path).parent / mod.MAIN.get('path')
+        path.parent.mkdir(parents=True, exist_ok=True)
         dataloader.save(path)
         print_console(
             [X_train, Y_train] + ([O_train] if O_train is not None else []),
             ['Training input data', 'Training output data'] + (['Training odds data'] if O_train is not None else []),
         )
 
 
@@ -92,15 +93,16 @@
             warning = Panel.fit(
                 '[bold red]Configuration file has been modified. Extract again the training data.',
             )
             console.print(warning)
             return
     X_fix, _, O_fix = dataloader.extract_fixtures_data()
     if mod is not None:
-        path = str(Path(dataloader_config_path).parent / mod.MAIN.get('path'))
+        path = Path(dataloader_config_path).parent / mod.MAIN.get('path')
+        path.parent.mkdir(parents=True, exist_ok=True)
         dataloader.save(path)
     if not X_fix.empty:
         print_console([X_fix], ['Fixtures input data'])
         if O_fix is not None and not O_fix.empty:
             print_console([O_fix], ['Fixtures odds data'])
     else:
         warning = Panel.fit(
```

### Comparing `sports-betting-0.5.0/src/sportsbet/cli/_evaluation.py` & `sports-betting-0.5.1/src/sportsbet/cli/_evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,16 @@
             '[bold red]Dataloader does not support odds data. Backtesting of bettor is not possible.',
         )
         console.print(warning)
         return
     backtesting_params = get_backtesting_params(bettor_mod)
     bettor.backtest(X, Y, O, **backtesting_params, refit=True)
     if bettor_mod is not None:
-        path = str(Path(bettor_config_path).parent / bettor_mod.MAIN.get('path'))
+        path = Path(bettor_config_path).parent / bettor_mod.MAIN.get('path')
+        path.parent.mkdir(parents=True, exist_ok=True)
         bettor.save(path)
         print_console([bettor.backtest_results_], ['Backtesting results'])
 
 
 @bettor.command()
 @get_bettor_config_path_option()
 @get_dataloader_config_path_option()
@@ -89,10 +90,11 @@
         return
     try:
         check_is_fitted(bettor)
     except NotFittedError:
         bettor.fit(*dataloader.train_data_[:-1])
     value_bets = bettor.bet(X, O)
     if bettor_mod is not None:
-        path = str(Path(bettor_config_path).parent / bettor_mod.MAIN.get('path'))
+        path = Path(bettor_config_path).parent / bettor_mod.MAIN.get('path')
+        path.parent.mkdir(parents=True, exist_ok=True)
         bettor.save(path)
         print_console([value_bets], ['Value bets'])
```

### Comparing `sports-betting-0.5.0/src/sportsbet/cli/_options.py` & `sports-betting-0.5.1/src/sportsbet/cli/_options.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/cli/_utils.py` & `sports-betting-0.5.1/src/sportsbet/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_base.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_dummy.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_data.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_data.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fd.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_fd.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_fte.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_fte.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/datasets/_soccer/_utils.py` & `sports-betting-0.5.1/src/sportsbet/datasets/_soccer/_utils.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/evaluation/_base.py` & `sports-betting-0.5.1/src/sportsbet/evaluation/_base.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/evaluation/_classifier.py` & `sports-betting-0.5.1/src/sportsbet/evaluation/_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/src/sportsbet/evaluation/_rules.py` & `sports-betting-0.5.1/src/sportsbet/evaluation/_rules.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/tests/cli/test_datasets.py` & `sports-betting-0.5.1/tests/cli/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/tests/cli/test_evaluation.py` & `sports-betting-0.5.1/tests/cli/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/tests/datasets/test_dummy.py` & `sports-betting-0.5.1/tests/datasets/test_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/tests/evaluation/test_classifier.py` & `sports-betting-0.5.1/tests/evaluation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/tests/evaluation/test_rules.py` & `sports-betting-0.5.1/tests/evaluation/test_rules.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.5.0/PKG-INFO` & `sports-betting-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports-betting
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python sports betting toolbox.
 License: MIT
 Keywords: sports betting,sports analytics,machine learning
 Author-email: Georgios Douzas <gdouzas@icloud.com>
 Requires-Python: >=3.9, <3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -141,14 +141,17 @@
 git clone https://github.com/georgedouzas/sports-betting.git
 cd sports-betting
 pdm install
 ```
 
 ## Usage
 
+You can use the Python API or the CLI to access the full functionality of `sports-betting`. Nevertheless, it is recommended to be
+familiar with the Python API since it is still needed to write configuration files for the CLI.
+
 ### API
 
 The `sports-betting` package makes it easy to download sports betting data:
 
 ```python
 from sportsbet.datasets import SoccerDataLoader
 dataloader = SoccerDataLoader(param_grid={'league': ['Italy'], 'year': [2020]})
@@ -238,10 +241,10 @@
 ```bash
 sportsbet bettor backtest -b bettor_config.py -d dataloader_config.py
 ```
 
 Get the value bets:
 
 ```bash
-sportsbet bettor bettor -b bettor_config.py -d dataloader_config.py
+sportsbet bettor bet -b bettor_config.py -d dataloader_config.py
 ```
```

