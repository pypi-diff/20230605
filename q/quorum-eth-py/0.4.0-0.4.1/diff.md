# Comparing `tmp/quorum_eth_py-0.4.0.tar.gz` & `tmp/quorum_eth_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.4.0.tar", last modified: Tue May 23 07:48:53 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.4.1.tar", last modified: Mon Jun  5 15:15:53 2023, max compression
```

## Comparing `quorum_eth_py-0.4.0.tar` & `quorum_eth_py-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.162515 quorum_eth_py-0.4.0/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-23 07:48:53.161519 quorum_eth_py-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.102683 quorum_eth_py-0.4.0/quorum_eth_py/
--rw-rw-rw-   0        0        0      343 2023-05-23 02:53:26.000000 quorum_eth_py-0.4.0/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1746 2023-05-17 04:45:00.000000 quorum_eth_py-0.4.0/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0      149 2023-05-22 12:44:15.000000 quorum_eth_py-0.4.0/quorum_eth_py/_constants.py
--rw-rw-rw-   0        0        0     6276 2023-05-23 07:43:44.000000 quorum_eth_py-0.4.0/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.4.0/quorum_eth_py/_gateway.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.4.0/quorum_eth_py/_http.py
--rw-rw-rw-   0        0        0     6150 2023-05-23 07:39:54.000000 quorum_eth_py-0.4.0/quorum_eth_py/_paid_group.py
--rw-rw-rw-   0        0        0     2177 2023-05-23 07:02:25.000000 quorum_eth_py-0.4.0/quorum_eth_py/_rum_erc20.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.159523 quorum_eth_py-0.4.0/quorum_eth_py/contract/
--rw-rw-rw-   0        0        0    38405 2023-05-22 11:47:48.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroup.py
--rw-rw-rw-   0        0        0    38871 2023-05-23 06:31:13.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroupV2.py
--rw-rw-rw-   0        0        0    23212 2023-05-22 10:47:15.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/RumERC20.py
--rw-rw-rw-   0        0        0      280 2023-05-22 11:47:45.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.151544 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 07:48:53.162515 quorum_eth_py-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-05-23 02:30:10.000000 quorum_eth_py-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:15:53.730208 quorum_eth_py-0.4.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-06-05 15:15:53.728248 quorum_eth_py-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:15:53.702282 quorum_eth_py-0.4.1/quorum_eth_py/
+-rw-rw-rw-   0        0        0      343 2023-06-05 15:06:21.000000 quorum_eth_py-0.4.1/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     2297 2023-06-05 15:15:39.000000 quorum_eth_py-0.4.1/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0      149 2023-05-22 12:44:15.000000 quorum_eth_py-0.4.1/quorum_eth_py/_constants.py
+-rw-rw-rw-   0        0        0     6276 2023-05-23 07:43:44.000000 quorum_eth_py-0.4.1/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.4.1/quorum_eth_py/_gateway.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.4.1/quorum_eth_py/_http.py
+-rw-rw-rw-   0        0        0     6150 2023-05-23 07:39:54.000000 quorum_eth_py-0.4.1/quorum_eth_py/_paid_group.py
+-rw-rw-rw-   0        0        0     2177 2023-05-23 07:02:25.000000 quorum_eth_py-0.4.1/quorum_eth_py/_rum_erc20.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:15:53.726220 quorum_eth_py-0.4.1/quorum_eth_py/contract/
+-rw-rw-rw-   0        0        0    38405 2023-05-22 11:47:48.000000 quorum_eth_py-0.4.1/quorum_eth_py/contract/PaidGroup.py
+-rw-rw-rw-   0        0        0    38871 2023-05-23 06:31:13.000000 quorum_eth_py-0.4.1/quorum_eth_py/contract/PaidGroupV2.py
+-rw-rw-rw-   0        0        0    23212 2023-05-22 10:47:15.000000 quorum_eth_py-0.4.1/quorum_eth_py/contract/RumERC20.py
+-rw-rw-rw-   0        0        0      280 2023-05-22 11:47:45.000000 quorum_eth_py-0.4.1/quorum_eth_py/contract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:15:53.714252 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-06-05 15:15:53.000000 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-05 15:15:53.000000 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:15:53.000000 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-05 15:15:53.000000 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 15:15:53.000000 quorum_eth_py-0.4.1/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:15:53.730208 quorum_eth_py-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2023-06-05 15:06:23.000000 quorum_eth_py-0.4.1/setup.py
```

### Comparing `quorum_eth_py-0.4.0/LICENSE` & `quorum_eth_py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/PKG-INFO` & `quorum_eth_py-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_eth_py
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/_browser.py` & `quorum_eth_py-0.4.1/quorum_eth_py/_browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,20 @@
         holders = self.contract_holders(contract_address)
         try:
             minted = self.w3.to_checksum_address(to_address) in holders
         except ValueError as err:
             minted = to_address in holders
             logger.warning("%s is_minted error: %s", to_address, err)
         return minted
+
+    def get_token_list(self, address: str):
+        """get token list of address"""
+        address = self.w3.to_checksum_address(address)
+        data = self.http.get(f"?module=account&action=tokenlist&address={address}")
+        if data.get("status") != "1":
+            logger.warning("get_token_list error: %s", data)
+            return []
+        tokens = data.get("result", [])
+        for i in tokens:
+            balance = self.w3.from_wei(int(i.get("balance")), "ether")
+            i["balance2"] = float(str(balance))
+        return tokens
```

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/_eth.py` & `quorum_eth_py-0.4.1/quorum_eth_py/_eth.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/_http.py` & `quorum_eth_py-0.4.1/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/_paid_group.py` & `quorum_eth_py-0.4.1/quorum_eth_py/_paid_group.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/_rum_erc20.py` & `quorum_eth_py-0.4.1/quorum_eth_py/_rum_erc20.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroup.py` & `quorum_eth_py-0.4.1/quorum_eth_py/contract/PaidGroup.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroupV2.py` & `quorum_eth_py-0.4.1/quorum_eth_py/contract/PaidGroupV2.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py/contract/RumERC20.py` & `quorum_eth_py-0.4.1/quorum_eth_py/contract/RumERC20.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.4.1/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-eth-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.4.0/quorum_eth_py.egg-info/SOURCES.txt` & `quorum_eth_py-0.4.1/quorum_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.4.0/setup.py` & `quorum_eth_py-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.4.0",
+    version="0.4.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

