# Comparing `tmp/rqsdk-1.4.9.tar.gz` & `tmp/rqsdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rqsdk-1.4.9.tar", last modified: Fri Nov 11 08:11:12 2022, max compression
+gzip compressed data, was "dist/rqsdk-1.5.0.tar", last modified: Mon Jun  5 02:40:19 2023, max compression
```

## Comparing `rqsdk-1.4.9.tar` & `rqsdk-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.621627 rqsdk-1.4.9/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2022-11-11 08:11:07.000000 rqsdk-1.4.9/HISTORY.md
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2022-11-11 08:11:07.000000 rqsdk-1.4.9/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-11-11 08:11:12.621627 rqsdk-1.4.9/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2022-11-11 08:11:07.000000 rqsdk-1.4.9/README.md
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.622627 rqsdk-1.4.9/rqsdk/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/__main__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2022-11-11 08:11:12.622627 rqsdk-1.4.9/rqsdk/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    12452 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/cmds.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1719 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/const.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/license_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/proxy_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/script_update.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/testing.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.621627 rqsdk-1.4.9/rqsdk.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2994 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2022-11-11 08:11:12.622627 rqsdk-1.4.9/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3258 2022-11-11 08:11:07.000000 rqsdk-1.4.9/setup.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79815 2022-11-11 08:11:07.000000 rqsdk-1.4.9/versioneer.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.009682 rqsdk-1.5.0/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-06-05 02:40:04.000000 rqsdk-1.5.0/HISTORY.md
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-06-05 02:40:04.000000 rqsdk-1.5.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-05 02:40:19.009682 rqsdk-1.5.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-06-05 02:40:04.000000 rqsdk-1.5.0/README.md
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.011682 rqsdk-1.5.0/rqsdk/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/__main__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-06-05 02:40:19.011682 rqsdk-1.5.0/rqsdk/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    12905 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/cmds.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/const.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/license_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/proxy_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/script_update.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/testing.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.008682 rqsdk-1.5.0/rqsdk.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3363 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-06-05 02:40:19.010682 rqsdk-1.5.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3129 2023-06-05 02:40:04.000000 rqsdk-1.5.0/setup.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79815 2023-06-05 02:40:04.000000 rqsdk-1.5.0/versioneer.py
```

### Comparing `rqsdk-1.4.9/PKG-INFO` & `rqsdk-1.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.4.9
+Version: 1.5.0
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
@@ -17,10 +17,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.6.1
 Provides-Extra: rqdatac
 Provides-Extra: rqfactor
 Provides-Extra: rqoptimizer
 Provides-Extra: rqalpha_plus
+Provides-Extra: rqpattr
 
 UNKNOWN
```

### Comparing `rqsdk-1.4.9/README.md` & `rqsdk-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk/__init__.py` & `rqsdk-1.5.0/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk/__main__.py` & `rqsdk-1.5.0/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk/cmds.py` & `rqsdk-1.5.0/rqsdk/cmds.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     <PRODUCT> 可选: rqdatac | rqfactor | rqoptimizer | rqalpha_plus
 
     \b
     * rqdatac - 金融数据API（默认已安装）
     * rqalpha_plus - 多资产回测引擎
     * rqoptimizer - 股票优化器
     * rqfactor - 因子投研和检验
+    * rqpattr - 绩效归因计算
     """
     if product != "":
         if product not in PRODUCTS:
             click.echo("PRODUCT可选为:{}\n,当前为{}。".format(PRODUCTS, product))
             return
         key = [product]
     else:
@@ -181,14 +182,19 @@
             except ImportError:
                 pass
             try:
                 import rqoptimizer2
                 key.append('rqoptimizer')
             except ImportError:
                 pass
+            try:
+                import rqpattr
+                key.append('rqpattr')
+            except ImportError:
+                pass
 
     full_name = "rqsdk[{}]".format(",".join(key))
     click.echo("开始更新 {} 请稍后...".format(full_name))
     return pip_install(full_name, index_url)
 
 
 @cli.command()
@@ -205,14 +211,15 @@
     <PRODUCT> 可选: rqdatac | rqfactor | rqoptimizer | rqalpha_plus
 
     \b
     * rqdatac - 金融数据API（默认已安装）
     * rqalpha_plus - 多资产回测引擎
     * rqoptimizer - 股票优化器
     * rqfactor - 因子投研和检验
+    * rqpattr - 绩效归因计算
     """
 
     if product == 'rqsdk':
         full_name = product
     elif product in PRODUCTS:
         from rqsdk import __version__
         full_name = "rqsdk[{}]=={}".format(product, __version__)
@@ -315,25 +322,28 @@
 
 @cli.command()
 @click.option(
     '-d', '--data-bundle-path', default=DEFAULT_BUNDLE_PATH, type=click.Path(file_okay=False),
     help="bundle 目录，默认为 {}".format(DEFAULT_BUNDLE_PATH)
 )
 @click.option('--minbar', help="检查分钟数据是否异常", default=False, is_flag=True)
-def check_data(data_bundle_path, minbar):
+@click.option('--daybar', help="检查日线数据是否异常", default=False, is_flag=True)
+def check_data(data_bundle_path, minbar, daybar):
     """
         检查bundle中的数据是否正确
     """
+    check_all = not any([minbar, daybar])
     try:
         from rqalpha_plus.bundle import check_min_bar_data
-        if not all([minbar]):
-            print("请选择品种:[--minbar]")
-        elif minbar:
+        from rqalpha.cmds.bundle import check_bundle_data
+        if minbar or check_all:
             check_min_bar_data(data_bundle_path)
-    except ImportError:
+        if daybar or check_all:
+            check_bundle_data(os.path.join(data_bundle_path, "bundle"))
+    except ImportError as e:
         click.echo("""请先使用'rqsdk install rqalpha_plus'安装rqalpha_plus""")
 
 
 @cli.command()
 @click.option(
     '-d', '--data-bundle-path', default=DEFAULT_BUNDLE_PATH, type=click.Path(file_okay=False),
     help="bundle 目录，默认为 {}".format(DEFAULT_BUNDLE_PATH)
```

### Comparing `rqsdk-1.4.9/rqsdk/const.py` & `rqsdk-1.5.0/rqsdk/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 RQDATAC_DEFAULT_ADDRESS = "rqdatad-pro.ricequant.com:16011"
 PERMISSIONS_INFO_URL = "https://www.ricequant.com/api/rqlicense/get_permissions_readable_info"
 EXTRA_INDEX_URL = "https://rquser:Ricequant8@pypi2.ricequant.com/simple/"
 BASH_FILE = [".bash_profile", ".bashrc", ".bash_profile", ".zshrc"]
 TAG_MAP = ["stock", "futures", "fund", "index", "option", "convertible", ]
 DEFAULT_BUNDLE_PATH = os.path.join(os.path.expanduser('~'), ".rqalpha-plus")
 
-PRODUCTS = ["rqalpha_plus", "rqdatac", "rqfactor", "rqoptimizer"]
+PRODUCTS = ["rqalpha_plus", "rqdatac", "rqfactor", "rqoptimizer", "rqpattr"]
 CONCERNED_PACKAGES = [
     "rqsdk",
 
     "rqdatac", "wcwidth", "tabulate", 'requests', "cryptography", "click", "jwt", "patsy", "statsmodels",
     "scipy", "numpy", "pandas", "rapidjson", "rqdatac_fund",
-    
+
     "rqfactor", "talib",
 
     "rqoptimizer", "ecos", "scs", "cvxpy", "osqp", "rqoptimizer2",
-    
+
     "rqalpha_plus", "rqalpha", "rqalpha_mod_option", "rqalpha_mod_optimizer2", "rqalpha_mod_convertible",
     "rqalpha_mod_ricequant_data", "rqalpha_mod_rqfactor", "rqalpha_mod_spot",  "rqalpha_mod_fund",
-    "rqalpha_mod_incremental", "rqrisk", "h5py", "hdf5plugin"
+    "rqalpha_mod_incremental", "rqrisk", "h5py", "hdf5plugin",
+
+    "rqpattr"
 ]
```

### Comparing `rqsdk-1.4.9/rqsdk/license_helper.py` & `rqsdk-1.5.0/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk/script_update.py` & `rqsdk-1.5.0/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk/testing.py` & `rqsdk-1.5.0/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.9/rqsdk.egg-info/PKG-INFO` & `rqsdk-1.5.0/rqsdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.4.9
+Version: 1.5.0
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
@@ -17,10 +17,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.6.1
 Provides-Extra: rqdatac
 Provides-Extra: rqfactor
 Provides-Extra: rqoptimizer
 Provides-Extra: rqalpha_plus
+Provides-Extra: rqpattr
 
 UNKNOWN
```

### Comparing `rqsdk-1.4.9/rqsdk.egg-info/requires.txt` & `rqsdk-1.5.0/rqsdk.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-tabulate
-patsy>=0.5.1
 rqdatac>=2.9.44
-click>=7.0
-statsmodels>=0.12.1
+pyjwt==1.7.1
 pandas>=0.24.2
+tabulate
 requests
-pyjwt==1.7.1
+click>=7.0
+patsy>=0.5.1
+statsmodels>=0.12.1
 rqdatac_fund==1.0.*,>=1.0.18
 wcwidth
 
 [:python_version <= "3.6"]
 cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
@@ -17,75 +17,75 @@
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
 [:python_version > "3.7"]
-cryptography<=36.0.2,>=2.9.2
+pyopenssl>22.0.0
 
 [:python_version >= "3.8"]
 numpy>=1.23.0
 scipy>=1.8.0
 
 [rqalpha_plus]
-matplotlib<=3.5.0
-tabulate
-rqalpha-mod-optimizer2==1.0.*,>=1.0.8
+rqdatac>=2.9.44
+rqalpha-mod-fund==0.0.12
+rqalpha-mod-incremental==0.0.8
+rqrisk==1.0.7
 rqalpha-mod-rqfactor==1.0.10
-rqrisk==1.0.3
-rqalpha-plus==4.2.2
+tabulate
 click>=7.0
-rqalpha-mod-option==1.1.*,>=1.1.19
-requests
+rqalpha==5.0.0
+ta-lib>=0.4.20
 hdf5plugin
-rqdatac_fund==1.0.*,>=1.0.18
-patsy>=0.5.1
+rqalpha-mod-ricequant-data==2.4.0
+rqalpha-mod-convertible==1.2.15
 wcwidth
-rqalpha-mod-incremental==0.0.7
-rqalpha==4.13.0
-rqalpha-mod-convertible==1.2.*,>=1.2.14
-rqalpha-mod-spot==1.0.*,>=1.0.8
-rqalpha-mod-fund==0.0.11
-rqalpha-mod-ricequant-data==2.3.*,>=2.3.8
-rqdatac>=2.9.44
-ta-lib==0.4.20
-statsmodels>=0.12.1
+rqalpha-mod-optimizer2==1.0.8
 pandas>=0.24.2
-h5py>=3.0.0
 pyjwt==1.7.1
+rqalpha-mod-option==1.1.23
+matplotlib>=3.1.0
+rqalpha-plus==4.2.4
+requests
+patsy>=0.5.1
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
 rqfactor==1.3.*,>=1.3.1
+rqalpha-mod-spot==1.0.9
+h5py>=3.0.0
 
 [rqalpha_plus:python_version <= "3.6"]
 python-rapidjson<=1.5
-numpy>=1.19.5
 cryptography==2.9.2
+numpy>=1.19.5
 
 [rqalpha_plus:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
-cryptography<=36.0.2,>=2.9.2
+pyopenssl>22.0.0
 
 [rqalpha_plus:python_version >= "3.8"]
 numpy>=1.23.0
 scipy>=1.8.0
 
 [rqdatac]
-tabulate
-patsy>=0.5.1
 rqdatac>=2.9.44
-click>=7.0
-statsmodels>=0.12.1
+pyjwt==1.7.1
 pandas>=0.24.2
+tabulate
 requests
-pyjwt==1.7.1
+click>=7.0
+patsy>=0.5.1
+statsmodels>=0.12.1
 rqdatac_fund==1.0.*,>=1.0.18
 wcwidth
 
 [rqdatac:python_version <= "3.6"]
 cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
@@ -93,85 +93,116 @@
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqdatac:python_version > "3.7"]
-cryptography<=36.0.2,>=2.9.2
+pyopenssl>22.0.0
 
 [rqdatac:python_version >= "3.8"]
 numpy>=1.23.0
 scipy>=1.8.0
 
 [rqfactor]
+rqdatac>=2.9.44
 tabulate
 click>=7.0
-requests
-rqdatac_fund==1.0.*,>=1.0.18
-patsy>=0.5.1
+ta-lib>=0.4.20
 wcwidth
-rqdatac>=2.9.44
-ta-lib==0.4.20
-statsmodels>=0.12.1
 pandas>=0.24.2
 pyjwt==1.7.1
+requests
+patsy>=0.5.1
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
 rqfactor==1.3.*,>=1.3.1
 
 [rqfactor:python_version <= "3.6"]
 python-rapidjson<=1.5
-numpy>=1.19.5
 cryptography==2.9.2
+numpy>=1.19.5
 
 [rqfactor:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
-cryptography<=36.0.2,>=2.9.2
+pyopenssl>22.0.0
 
 [rqfactor:python_version >= "3.8"]
 numpy>=1.23.0
 scipy>=1.8.0
 
 [rqoptimizer]
+rqdatac>=2.9.44
+osqp==0.6.2.post5
 tabulate
 click>=7.0
+rqoptimizer==1.2.*,>=1.2.17
+ecos==2.0.10
 rqoptimizer2==1.2.*,>=1.2.17
-requests
-osqp==0.6.2.post5
-rqdatac_fund==1.0.*,>=1.0.18
-patsy>=0.5.1
 wcwidth
-scs==2.1.4
-rqdatac>=2.9.44
-rqoptimizer==1.2.*,>=1.2.17
-statsmodels>=0.12.1
 pandas>=0.24.2
 pyjwt==1.7.1
-ecos==2.0.10
+requests
+patsy>=0.5.1
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
+scs==2.1.4
 
 [rqoptimizer:python_version <= "3.6"]
 python-rapidjson<=1.5
-numpy>=1.19.5
 cryptography==2.9.2
+numpy>=1.19.5
 
 [rqoptimizer:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqoptimizer:python_version == "3.6"]
 cvxpy==1.1.18
 
 [rqoptimizer:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqoptimizer:python_version > "3.7"]
-cryptography<=36.0.2,>=2.9.2
+pyopenssl>22.0.0
 
 [rqoptimizer:python_version >= "3.7"]
 cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
 numpy>=1.23.0
 scipy>=1.8.0
+
+[rqpattr]
+rqdatac>=2.9.44
+tabulate
+click>=7.0
+wcwidth
+rqpattr>=0.0.2
+pandas>=0.24.2
+pyjwt==1.7.1
+requests
+patsy>=0.5.1
+statsmodels>=0.12.1
+rqdatac_fund==1.0.*,>=1.0.18
+
+[rqpattr:python_version <= "3.6"]
+python-rapidjson<=1.5
+cryptography==2.9.2
+numpy>=1.19.5
+
+[rqpattr:python_version <= "3.7"]
+scipy<=1.7.3
+
+[rqpattr:python_version == "3.7"]
+numpy>=1.20.0
+
+[rqpattr:python_version > "3.7"]
+pyopenssl>22.0.0
+
+[rqpattr:python_version >= "3.8"]
+numpy>=1.23.0
+scipy>=1.8.0
```

### Comparing `rqsdk-1.4.9/setup.py` & `rqsdk-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import versioneer
 
 version_map = {}
 version_map["rqdatac"] = {
     "wcwidth",
     "tabulate",
     "requests",
-    "cryptography>=2.9.2, <=36.0.2; python_version > '3.7'",
+    "pyopenssl>22.0.0; python_version > '3.7'",  #  cryptography 的版本由 pyopenssl 来指定
     "cryptography==2.9.2; python_version <= '3.6'",  # python 3.6.0有点过分,pip更新报错，cryptography版本太高也报错
     "click>=7.0",
     "pyjwt==1.7.1",
     "patsy>=0.5.1",
     "statsmodels>=0.12.1",
     "scipy <= 1.7.3; python_version <= '3.7'",
     "scipy >= 1.8.0; python_version >= '3.8'",
@@ -21,44 +21,44 @@
     "numpy>=1.23.0; python_version >= '3.8'",  # numpy 1.23.0 修改了类型大小
     "pandas >= 0.24.2",
     "python-rapidjson <= 1.5; python_version <= '3.6'",  # rapidjson 1.6 开始不再提供 python 3.6 的 whl 包
     "rqdatac>=2.9.44",
     "rqdatac_fund==1.0.*,>=1.0.18"
 }
 version_map["rqfactor"] = version_map["rqdatac"] | {
-    "ta-lib==0.4.20",
+    "ta-lib>=0.4.20",
     "rqfactor==1.3.*,>=1.3.1",
 }
 version_map["rqoptimizer"] = version_map["rqdatac"] | {
     "ecos==2.0.10",
     "scs==2.1.4",
     "cvxpy==1.1.18 ; python_version == '3.6'",
     "cvxpy==1.2.0 ; python_version >= '3.7'",
     "osqp==0.6.2.post5",
     "rqoptimizer==1.2.*,>=1.2.17",
     "rqoptimizer2==1.2.*,>=1.2.17",
 }
 version_map["rqalpha_plus"] = version_map["rqfactor"] | {
-    "rqalpha==4.13.0",
-    "rqalpha-mod-option==1.1.*,>=1.1.19",
-    "rqalpha-mod-optimizer2==1.0.*, >=1.0.8",
-    "rqalpha-mod-convertible==1.2.*,>=1.2.14",
-    "rqalpha-mod-ricequant-data==2.3.*,>=2.3.8",
+    "rqalpha==5.0.0",
+    "rqalpha-mod-option==1.1.23",
+    "rqalpha-mod-optimizer2==1.0.8",
+    "rqalpha-mod-convertible==1.2.15",
+    "rqalpha-mod-ricequant-data==2.4.0",
     "rqalpha-mod-rqfactor==1.0.10",
-    "rqalpha-mod-spot==1.0.*,>=1.0.8",
-    "rqalpha-mod-fund==0.0.11",
-    "rqalpha-mod-incremental==0.0.7",
-    "rqalpha-plus==4.2.2",
-    "rqrisk==1.0.3",
+    "rqalpha-mod-spot==1.0.9",
+    "rqalpha-mod-fund==0.0.12",
+    "rqalpha-mod-incremental==0.0.8",
+    "rqalpha-plus==4.2.4",
+    "rqrisk==1.0.7",
     "h5py>=3.0.0",
     "hdf5plugin",
-    # 3.6.0 在 pycharm 中画图存在问题，待 3.6.1 发布后可移除这一限制
-    # https://youtrack.jetbrains.com/issue/PY-56370
-    # https://github.com/matplotlib/matplotlib/pull/23912
-    "matplotlib<=3.5.0",
+    "matplotlib>=3.1.0",
+}
+version_map["rqpattr"] = version_map["rqdatac"] | {
+    "rqpattr>=0.0.2"
 }
 
 extras_require = {k: list(v) for k, v in version_map.items()}
 
 with open('README.md', encoding="utf8") as f:
     readme = f.read()
```

### Comparing `rqsdk-1.4.9/versioneer.py` & `rqsdk-1.5.0/versioneer.py`

 * *Files identical despite different names*

