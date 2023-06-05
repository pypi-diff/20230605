# Comparing `tmp/bookio_fetchfox-0.2.0.tar.gz` & `tmp/bookio_fetchfox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.2.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.3.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.2.0.tar` & `bookio_fetchfox-0.3.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     3532 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1770 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2664 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      449 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1606 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/jpgstore.py
--rwxr-xr-x   0        0        0      675 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4154 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2573 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     6014 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     1698 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    10257 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      452 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     7981 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      453 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      178 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      463 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1320 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      362 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1382 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1677 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1116 2023-06-05 17:47:28.270699 bookio_fetchfox-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 bookio_fetchfox-0.2.0/setup.py
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 bookio_fetchfox-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3723 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1764 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      449 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-05 21:22:29.771875 bookio_fetchfox-0.3.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4147 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2555 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     6862 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     1996 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    10727 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     8690 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      178 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2263 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     1215 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      463 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1320 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      362 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1382 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1677 2023-06-05 21:22:29.775875 bookio_fetchfox-0.3.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1148 2023-06-05 21:22:29.787876 bookio_fetchfox-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 bookio_fetchfox-0.3.0/setup.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 bookio_fetchfox-0.3.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.2.0/README.md` & `bookio_fetchfox-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 * get_asset ([algonode.cloud](https://algonode.cloud))
 * get_assets ([algonode.cloud](https://algonode.cloud))
 * get_holdings ([algonode.cloud](https://algonode.cloud))
 * get_snapshot ([algonode.cloud](https://algonode.cloud))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))
+* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))
 * get_sales ([nftexplorer.app¹](https://nftexplorer.app))
 
 
 ### Cardano
 
 ```python
 import os
@@ -59,14 +60,15 @@
 
 * get_asset ([blockfrost.io²](https://blockfrost.io))
 * get_assets ([blockfrost.io²](https://blockfrost.io))
 * get_holdings ([blockfrost.io²](https://blockfrost.io))
 * get_campaigns ([book.io](https://book.io))
 * get_snapshot ([blockfrost.io²](https://blockfrost.io))
 * get_listings ([jpg.store](https://jpg.store))
+* get_floor ([jpg.store](https://jpg.store))
 * get_sales ([jpg.store](https://jpg.store))
 * get_ranks ([cnft.tools](https://cnft.tools))
 
 
 ### EVM (Ethereum and Polygon)
 
 ```python
@@ -103,14 +105,15 @@
 
 * get_asset ([moralis.io³](https://moralis.io))
 * get_assets ([moralis.io³](https://moralis.io))
 * get_holdings ([moralis.io³](https://moralis.io))
 * get_snapshot ([moralis.io³](https://moralis.io))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([opensea.io⁴](https://opensea.io))
+* get_floor ([opensea.io⁴](https://opensea.io))
 * get_sales ([opensea.io⁴](https://opensea.io))
 
 
 > ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).
 > 
 > ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).
 >
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
 BASE_URL = "https://api.nftexplorer.app"
 
 
-def get(
-    service: str, api_key: str, params: dict = None, version: int = 1
-) -> Tuple[dict, int]:
+def get(service: str, api_key: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     check_str(api_key, "nftexplorerapp.api_key")
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         headers={
             "Authorization": api_key,
         },
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
 BASE_URL = "https://cardano-mainnet.blockfrost.io/api"
 
 
-def get(
-    service: str, project_id: str, params: dict = None, version: int = 0
-) -> Tuple[dict, int]:
+def get(service: str, project_id: str, params: dict = None, version: int = 0) -> Tuple[dict, int]:
     check_str(project_id, "blockfrost.project_id")
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params or {},
         headers={
             "project_id": project_id,
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/evm/moralisio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import logging
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-
 BASE_URL = "https://deep-index.moralis.io/api"
 
 logger = logging.getLogger(__name__)
 
 
-def get(
-    service: str, blockchain: str, api_key: str, params: dict = None, version: int = 2
-) -> Tuple[dict, int]:
+def get(service: str, blockchain: str, api_key: str, params: dict = None, version: int = 2) -> Tuple[dict, int]:
     check_str(blockchain, "moralisio.blockchain")
     check_str(api_key, "moralisio.api_key")
 
     params = params or {}
     params["chain"] = "eth" if blockchain == "ethereum" else blockchain
 
     return rest.get(
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.3.0/fetchfox/apis/evm/openseaio.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from fetchfox.checks import check_str
 
 BASE_URL = "https://api.opensea.io"
 
 logger = logging.getLogger(__name__)
 
 
-def get(
-    service: str, api_key: str, params: dict = None, version: int = 2
-) -> Tuple[dict, int]:
+def get(service: str, api_key: str, params: dict = None, version: int = 2) -> Tuple[dict, int]:
     check_str(api_key, "openseaio.api_key")
 
     if version == 1:
         url = f"{BASE_URL}/api/v{version}/{service}"
     else:
         url = f"{BASE_URL}/v{version}/{service}"
 
@@ -46,17 +44,15 @@
         version=1,
         api_key=api_key,
     )
 
     return response["asset_events"][0]["collection_slug"]
 
 
-def get_events(
-    contract_address: str, event_type: str, api_key: str, slug: str = None
-) -> Iterable[dict]:
+def get_events(contract_address: str, event_type: str, api_key: str, slug: str = None) -> Iterable[dict]:
     if not slug:
         slug = get_slug(contract_address, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
@@ -84,17 +80,15 @@
         contract_address,
         event_type="successful",
         api_key=api_key,
         slug=slug,
     )
 
 
-def get_listings(
-    contract_address: str, api_key: str, slug: str = None
-) -> Iterable[dict]:
+def get_listings(contract_address: str, api_key: str, slug: str = None) -> Iterable[dict]:
     if not slug:
         slug = get_slug(contract_address, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,46 +28,59 @@
 
 class Algorand(Blockchain):
     def __init__(self, nftexplorerapp_api_key: str = None):
         super().__init__(ALGORAND, ALGO)
 
         self.nftexplorerapp_api_key: str = nftexplorerapp_api_key
 
-    def get_assets(
-        self,
-        collection_id: str,
-        fetch_metadata: bool = True,
-        *args,
-        **kwargs,
-    ) -> Iterable[AssetDTO]:
+    def check_collection_id(self, collection_id: str):
+        if not utils.is_address(collection_id):
+            raise ValueError(f"{collection_id} is not a valid algorand creator address")
+
+    def check_asset_id(self, asset_id: str):
+        if not utils.is_asset_id(asset_id):
+            raise ValueError(f"{asset_id} is not a valid algorand asset id")
+
+    def check_wallet(self, wallet: str):
+        if not utils.is_wallet(wallet):
+            raise ValueError(f"{wallet} is not a valid algorand address or nfdomain")
+
+    def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
+        self.check_collection_id(collection_id)
+
         for asset_id in algonodecloud.get_assets(collection_id):
             if fetch_metadata:
                 yield self.get_asset(
                     collection_id=collection_id,
                     asset_id=str(asset_id),
                 )
             else:
                 yield AssetDTO(
                     collection_id=collection_id,
                     asset_id=str(asset_id),
                     metadata={},
                 )
 
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
         data = algonodecloud.get_asset_data(asset_id)
         metadata = algonodecloud.get_asset_metadata(asset_id)
         metadata["name"] = data["name"]
 
         return AssetDTO(
             collection_id=collection_id,
             asset_id=asset_id,
             metadata=metadata,
         )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_wallet(wallet)
+
         if utils.is_nf_domain(wallet):
             wallet = nfdomains.resolve_nf_domain(wallet)
 
         holdings = algonodecloud.get_holdings(wallet)
 
         for holding in holdings:
             asset_id = holding["asset-id"]
@@ -80,27 +93,31 @@
                 collection_id=None,
                 asset_id=asset_id,
                 address=wallet,
                 quantity=quantity,
             )
 
     def get_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_collection_id(collection_id)
+
         for asset in self.get_assets(collection_id, fetch_metadata=False):
             holding = algonodecloud.get_owner(
                 str(asset.asset_id),
             )
 
             yield HoldingDTO(
                 collection_id=asset.collection_id,
                 asset_id=holding["asset_id"],
                 address=holding["address"],
                 quantity=holding["amount"],
             )
 
     def get_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
+        self.check_collection_id(collection_id)
+
         listings = randswapcom.get_listings(collection_id)
 
         for listing in listings:
             asset_ids = [str(listing["assetId"])]
             asset_names = [""]
 
             listed_at = datetime.fromtimestamp(
@@ -140,25 +157,29 @@
                 price=listing["price"] // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=listing["seller"],
             )
 
     def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+        self.check_collection_id(collection_id)
+
         floor = None
 
         for listing in self.get_listings(collection_id):
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
         return floor
 
     def get_sales(self, collection_id: str, *args, **kwargs) -> Iterable[SaleDTO]:
+        self.check_collection_id(collection_id)
+
         venues = {
             "algoxnft": ALGOXNFT_COM,
             "randgallery": RANDGALLERY_COM,
             "shufl": SHUFL_APP,
             None: UNKNOWN,
         }
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import Iterable, Optional
-from fetchfox.apis import coingeckocom
 
+from fetchfox.apis import coingeckocom
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     HoldingDTO,
     ListingDTO,
     RankDTO,
     SaleDTO,
@@ -17,17 +17,27 @@
         self.name: str = name
         self.currency: str = currency
 
     def usd(self) -> float:
         return coingeckocom.usd(self.currency)
 
     @abstractmethod
-    def get_assets(
-        self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs
-    ) -> Iterable[AssetDTO]:
+    def check_collection_id(self, collection_id: str):
+        raise NotImplementedError()
+
+    @abstractmethod
+    def check_asset_id(self, asset_id: str):
+        raise NotImplementedError()
+
+    @abstractmethod
+    def check_wallet(self, wallet: str):
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
         raise NotImplementedError()
 
     def get_campaigns(self) -> Iterable[CampaignDTO]:
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,49 +28,58 @@
 
 class Cardano(Blockchain):
     def __init__(self, blockfrostio_project_id: str = None):
         super().__init__(CARDANO, ADA)
 
         self.blockfrostio_project_id: str = blockfrostio_project_id
 
+    def check_collection_id(self, collection_id: str):
+        if not utils.is_policy_id(collection_id):
+            raise ValueError(f"{collection_id} is not a valid cardano policy id")
+
+    def check_asset_id(self, asset_id: str):
+        if not utils.is_asset_id(asset_id):
+            raise ValueError(f"{asset_id} is not a valid cardano asset id")
+
+    def check_wallet(self, wallet: str):
+        if not utils.is_wallet(wallet):
+            raise ValueError(f"{wallet} is not a valid cardano address, stake key or ada handle")
+
     @lru_cache
-    def get_stake_address(self, wallet: str) -> str:
+    def get_stake_key(self, wallet: str) -> str:
+        self.check_wallet(wallet)
+
         if utils.is_stake_key(wallet):
             return wallet
 
         if utils.is_address(wallet):
             return blockfrostio.get_stake_address(
                 wallet,
                 project_id=self.blockfrostio_project_id,
             )
 
         if utils.is_ada_handle(wallet):
             return handleme.resolve_handle(wallet)
 
         return None
 
-    def get_assets(
-        self,
-        collection_id: str,
-        collection_discriminator: str = None,
-        fetch_metadata: bool = True,
-        *args,
-        **kwargs,
-    ) -> Iterable[AssetDTO]:
+    def get_assets(self, collection_id: str, discriminator: str = None, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
+        self.check_collection_id(collection_id)
+
         response = blockfrostio.get_assets(
             collection_id,
             project_id=self.blockfrostio_project_id,
         )
 
         for asset_id in response:
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
-            if collection_discriminator:
-                if collection_discriminator not in asset_name.lower():
+            if discriminator:
+                if discriminator not in asset_name.lower():
                     continue
 
             if fetch_metadata:
                 yield self.get_asset(
                     collection_id=collection_id,
                     asset_id=asset_id,
                 )
@@ -78,14 +87,17 @@
                 yield AssetDTO(
                     collection_id=collection_id,
                     asset_id=asset_id,
                     metadata={},
                 )
 
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
         response = blockfrostio.get_asset_data(
             asset_id,
             project_id=self.blockfrostio_project_id,
         )
 
         metadata = response.get("onchain_metadata", {})
 
@@ -97,34 +109,36 @@
 
     def get_campaigns(self) -> Iterable[CampaignDTO]:
         for campaign in bookio.campaigns():
             if campaign["blockchain"] != CARDANO:
                 continue
 
             landing = campaign["landing"]
+            pricing = landing["price_description"].replace(" (+2 ADA that will be returned with your eBook)", "").strip()
+
             start_at = campaign["start_at"]
 
             yield CampaignDTO(
                 blockchain=CARDANO,
                 parlamint_id=campaign["id"],
                 collection_id=landing["lottery"]["collection_id"],
                 name=campaign["display_name"],
                 description=campaign["landing"]["opener"],
                 supply=campaign["total_deas"],
                 limit=campaign["max_quantity"],
                 price=landing["price"],
-                pricing=landing["price_description"]
-                .replace(" (+2 ADA that will be returned with your eBook)", "")
-                .strip(),
+                pricing=pricing,
                 rarity_chart_url=landing["rarity_chart_url"],
                 start_at=formatters.timestamp(start_at["start_at"]),
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
-        stake_address = self.get_stake_address(wallet)
+        self.check_wallet(wallet)
+
+        stake_address = self.get_stake_key(wallet)
 
         holdings = blockfrostio.get_holdings(
             stake_address,
             project_id=self.blockfrostio_project_id,
         )
 
         for holding in holdings:
@@ -141,82 +155,74 @@
                 collection_id=policy_id,
                 asset_id=asset_id,
                 address=stake_address,
                 quantity=quantity,
             )
 
     def get_ranks(self, collection_id: str, *args, **kwargs) -> Iterable[RankDTO]:
+        self.check_collection_id(collection_id)
+
         for asset_name, rank in cnfttools.get_ranks(collection_id):
             asset_name_bytes = asset_name.encode()
             asset_name_base16 = base64.b16encode(asset_name_bytes).decode("utf-8")
             asset_id = f"{collection_id}{asset_name_base16}"
 
             yield RankDTO(
                 collection_id=collection_id,
                 asset_id=asset_id.lower(),
                 asset_name=asset_name,
                 rank=int(rank),
             )
 
-    def get_snapshot(
-        self,
-        collection_id: str,
-        collection_discriminator: str = None,
-        *args,
-        **kwargs,
-    ) -> Iterable[HoldingDTO]:
-        for asset in self.get_assets(
-            collection_id,
-            collection_discriminator=collection_discriminator,
-            fetch_metadata=False,
-        ):
+    def get_snapshot(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_collection_id(collection_id)
+
+        for asset in self.get_assets(collection_id, discriminator=discriminator, fetch_metadata=False):
             holding = blockfrostio.get_owner(
                 asset.asset_id,
                 project_id=self.blockfrostio_project_id,
             )
 
-            stake_address = self.get_stake_address(holding["address"])
+            stake_address = self.get_stake_key(holding["address"])
 
             yield HoldingDTO(
                 collection_id=collection_id,
                 asset_id=holding["asset_id"],
                 address=stake_address,
                 quantity=holding["amount"],
             )
 
-    def get_listings(
-        self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
-    ) -> Iterable[ListingDTO]:
-        if collection_discriminator:
-            collection_discriminator = collection_discriminator.lower()
+    def get_listings(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[ListingDTO]:
+        self.check_collection_id(collection_id)
+
+        if discriminator:
+            discriminator = discriminator.lower()
 
         for listing in jpgstore.get_listings(collection_id):
             asset_id = listing["asset_id"]
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
-            if collection_discriminator:
-                if collection_discriminator not in asset_name.lower():
+            if discriminator:
+                if discriminator not in asset_name.lower():
                     continue
 
             asset_ids = []
             asset_names = []
 
             if listing["listing_type"] == "BUNDLE":
                 for bundled_asset in listing["bundled_assets"]:
                     asset_ids.append(bundled_asset["asset_id"])
                     asset_names.append(bundled_asset["display_name"])
             else:
                 asset_ids.append(listing["asset_id"])
                 asset_names.append(listing["display_name"])
 
             if listing.get("confirmed_at"):
-                listed_at = datetime.fromisoformat(
-                    listing["confirmed_at"].replace("Z", "+00:00")
-                )
+                listed_at = datetime.fromisoformat(listing["confirmed_at"].replace("Z", "+00:00"))
             else:
                 listed_at = datetime.now(tz=pytz.utc)
 
             yield ListingDTO(
                 identifier=listing["tx_hash"],
                 collection_id=policy_id,
                 asset_ids=asset_ids,
@@ -226,40 +232,37 @@
                 price=int(listing["price_lovelace"]) // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=None,
                 tx_hash=listing["tx_hash"],
             )
 
-    def get_floor(
-        self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
-    ) -> Optional[ListingDTO]:
+    def get_floor(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Optional[ListingDTO]:
+        self.check_collection_id(collection_id)
+
         floor = None
 
-        for listing in self.get_listings(
-            collection_id,
-            collection_discriminator=collection_discriminator,
-        ):
+        for listing in self.get_listings(collection_id, discriminator=discriminator):
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
         return floor
 
-    def get_sales(
-        self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
-    ) -> Iterable[SaleDTO]:
+    def get_sales(self, collection_id: str, discriminator: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
+        self.check_collection_id(collection_id)
+
         for sale in jpgstore.get_sales(collection_id):
             asset_id = sale["asset_id"]
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
-            if collection_discriminator:
-                if collection_discriminator not in asset_name.lower():
+            if discriminator:
+                if discriminator not in asset_name.lower():
                     continue
 
             if sale["action"] == "ACCEPT_OFFER":
                 buyer = sale["seller_address"]
                 seller = sale["signer_address"]
             elif sale["action"] == "ACCEPT_COLLECTION_OFFER":
                 buyer = sale["signer_address"]
@@ -276,17 +279,15 @@
                     asset_ids.append(bundled_asset["asset_id"])
                     asset_names.append(bundled_asset["display_name"])
             else:
                 asset_ids.append(sale["asset_id"])
                 asset_names.append(sale["display_name"])
 
             if sale.get("confirmed_at"):
-                confirmed_at = datetime.fromisoformat(
-                    sale["confirmed_at"].replace("Z", "+00:00")
-                )
+                confirmed_at = datetime.fromisoformat(sale["confirmed_at"].replace("Z", "+00:00"))
             else:
                 confirmed_at = datetime.now(tz=pytz.utc)
 
             yield SaleDTO(
                 identifier=sale["tx_hash"],
                 collection_id=policy_id,
                 asset_ids=asset_ids,
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,33 +14,35 @@
 from fetchfox.helpers import formatters
 from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 class Evm(Blockchain):
-    def __init__(
-        self,
-        name: str,
-        currency: str,
-        moralisio_api_key: str = None,
-        openseaio_api_key: str = None,
-    ):
+    def __init__(self, name: str, currency: str, moralisio_api_key: str = None, openseaio_api_key: str = None):
         super().__init__(name, currency)
 
         self.moralisio_api_key: str = moralisio_api_key
         self.openseaio_api_key: str = openseaio_api_key
 
-    def get_assets(
-        self,
-        collection_id: str,
-        fetch_metadata: bool = True,
-        *args,
-        **kwargs,
-    ) -> Iterable[AssetDTO]:
+    def check_collection_id(self, collection_id: str):
+        if not utils.is_address(collection_id):
+            raise ValueError(f"{collection_id} is not a valid {self.name} contract address")
+
+    def check_asset_id(self, asset_id: str):
+        if not utils.is_asset_id(asset_id):
+            raise ValueError(f"{asset_id} is not a valid {self.name} asset id")
+
+    def check_wallet(self, wallet: str):
+        if not utils.is_wallet(wallet):
+            raise ValueError(f"{wallet} is not a valid {self.name} address or ens domain")
+
+    def get_assets(self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs) -> Iterable[AssetDTO]:
+        self.check_collection_id(collection_id)
+
         if fetch_metadata:
             asset_id = -1
 
             while True:
                 try:
                     asset_id += 1
 
@@ -63,14 +65,17 @@
                 yield AssetDTO(
                     collection_id=collection_id,
                     asset_id=asset_id,
                     metadata={},
                 )
 
     def get_asset(self, collection_id: str, asset_id: str, *args, **kwargs) -> AssetDTO:
+        self.check_collection_id(collection_id)
+        self.check_asset_id(asset_id)
+
         data = moralisio.get_asset_data(
             contract_address=collection_id,
             asset_id=asset_id,
             blockchain=self.name,
             api_key=self.moralisio_api_key,
         )
 
@@ -111,14 +116,16 @@
                 limit=campaign["max_quantity"],
                 pricing=landing["price_description"],
                 rarity_chart_url=landing["rarity_chart_url"],
                 start_at=formatters.timestamp(start_at["start_at"]),
             )
 
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_wallet(wallet)
+
         if utils.is_ens_domain(wallet):
             wallet = ensideascom.resolve_ens_domain(wallet)
 
         holdings = moralisio.get_holdings(
             wallet,
             blockchain=self.name,
             api_key=self.moralisio_api_key,
@@ -133,31 +140,33 @@
                 collection_id=contract_address,
                 asset_id=asset_id,
                 address=wallet,
                 quantity=quantity,
             )
 
     def get_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
+        self.check_collection_id(collection_id)
+
         assets = moralisio.get_owners(
             collection_id,
             blockchain=self.name,
             api_key=self.moralisio_api_key,
         )
 
         for asset in assets:
             yield HoldingDTO(
                 collection_id=asset["contract_address"],
                 asset_id=asset["asset_id"],
                 address=asset["address"],
                 quantity=asset["amount"],
             )
 
-    def get_listings(
-        self, collection_id: str, slug: str = None, *args, **kwargs
-    ) -> Iterable[ListingDTO]:
+    def get_listings(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[ListingDTO]:
+        self.check_collection_id(collection_id)
+
         listings = openseaio.get_listings(
             collection_id,
             api_key=self.openseaio_api_key,
             slug=slug,
         )
 
         for listing in listings:
@@ -191,55 +200,53 @@
                 currency=price["currency"].replace("WETH", "ETH"),
                 listed_at=listed_at,
                 listed_by=parameters["offerer"],
                 tx_hash=listing["order_hash"],
             )
 
     def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+        self.check_collection_id(collection_id)
+
         floor = None
 
         for listing in self.get_listings(collection_id):
             if floor is None:
                 floor = listing
             elif listing.usd < floor.usd:
                 floor = listing
 
         return floor
 
-    def get_sales(
-        self, collection_id: str, slug: str = None, *args, **kwargs
-    ) -> Iterable[SaleDTO]:
+    def get_sales(self, collection_id: str, slug: str = None, *args, **kwargs) -> Iterable[SaleDTO]:
+        self.check_collection_id(collection_id)
+
         sales = openseaio.get_sales(
             collection_id,
             api_key=self.openseaio_api_key,
             slug=slug,
         )
 
         for sale in sales:
             asset = sale["asset"]
 
             asset_ids = [asset["token_id"]]
             asset_names = [asset["name"]]
 
             if sale.get("event_timestamp"):
-                confirmed_at = datetime.fromisoformat(
-                    sale["event_timestamp"] + "+00:00"
-                )
+                confirmed_at = datetime.fromisoformat(sale["event_timestamp"] + "+00:00")
             else:
                 confirmed_at = datetime.now(tz=pytz.utc)
 
             yield SaleDTO(
                 identifier=sale["id"],
                 collection_id=collection_id,
                 asset_ids=asset_ids,
                 asset_names=asset_names,
                 tx_hash=sale["transaction"]["transaction_hash"],
                 marketplace=OPENSEA_IO,
-                price=float(
-                    int(sale["total_price"]) / 10 ** sale["payment_token"]["decimals"]
-                ),
+                price=float(int(sale["total_price"]) / 10 ** sale["payment_token"]["decimals"]),
                 currency=sale["payment_token"]["symbol"].replace("WETH", "ETH"),
                 confirmed_at=confirmed_at,
                 sold_by=sale["transaction"]["from_account"]["address"],
                 bought_by=sale["transaction"]["to_account"]["address"],
                 sale_id=sale["id"],
             )
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.3.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.3.0/fetchfox/dtos/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
     @property
     def quantity(self) -> int:
         return int(self.metadata.get("quantity", "1"))
 
     @property
     def cover_theme(self) -> str:
-        attributes = (
-            self.metadata.get("attributes") or self.metadata.get("properties") or {}
-        )
+        attributes = self.metadata.get("attributes") or self.metadata.get("properties") or {}
 
         if not attributes:
             return "none"
 
         if "Cover Theme" in attributes:
             return attributes["Cover Theme"].split(" / ")[-1]
 
@@ -48,40 +46,34 @@
             elif isinstance(attribute, list):
                 trait_count += len(attribute)
 
         return f"Traits: {trait_count}"
 
     @property
     def cover_variation(self) -> str:
-        attributes = (
-            self.metadata.get("attributes") or self.metadata.get("properties") or {}
-        )
+        attributes = self.metadata.get("attributes") or self.metadata.get("properties") or {}
 
         if not attributes:
             return None
 
         try:
             return int(attributes["Variation"].split(" / ")[-1])
         except:
             return None
 
     @property
     def special(self) -> str:
-        attributes = (
-            self.metadata.get("attributes") or self.metadata.get("properties") or {}
-        )
+        attributes = self.metadata.get("attributes") or self.metadata.get("properties") or {}
 
         if not attributes:
             return None
 
         if self.metadata["name"].startswith("Gutenberg Bible"):
             dots = attributes.get("Dots", [])
 
             if "Dots_Middle" in dots and "Dots_ADA" not in dots:
                 return GHOST_BIBLE
 
         return attributes.get("Special")
 
     def __repr__(self) -> str:
-        return (
-            f"{self.title} {self.number} [{self.cover_theme} / {self.cover_variation}]"
-        )
+        return f"{self.title} {self.number} [{self.cover_theme} / {self.cover_variation}]"
```

### Comparing `bookio_fetchfox-0.2.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.3.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.3.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.3.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/fetchfox/rest.py` & `bookio_fetchfox-0.3.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.2.0/pyproject.toml` & `bookio_fetchfox-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.2.0"
+version = "0.3.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
@@ -40,10 +40,13 @@
 cachetools = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 coverage = "^7.2.7"
 ddt = "^1.6.0"
 
+[tool.black]
+line-length = 150
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bookio_fetchfox-0.2.0/setup.py` & `bookio_fetchfox-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
-    'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
+    'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bookio_fetchfox-0.2.0/PKG-INFO` & `bookio_fetchfox-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
@@ -60,14 +60,15 @@
 
 * get_asset ([algonode.cloud](https://algonode.cloud))
 * get_assets ([algonode.cloud](https://algonode.cloud))
 * get_holdings ([algonode.cloud](https://algonode.cloud))
 * get_snapshot ([algonode.cloud](https://algonode.cloud))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))
+* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))
 * get_sales ([nftexplorer.app¹](https://nftexplorer.app))
 
 
 ### Cardano
 
 ```python
 import os
@@ -88,14 +89,15 @@
 
 * get_asset ([blockfrost.io²](https://blockfrost.io))
 * get_assets ([blockfrost.io²](https://blockfrost.io))
 * get_holdings ([blockfrost.io²](https://blockfrost.io))
 * get_campaigns ([book.io](https://book.io))
 * get_snapshot ([blockfrost.io²](https://blockfrost.io))
 * get_listings ([jpg.store](https://jpg.store))
+* get_floor ([jpg.store](https://jpg.store))
 * get_sales ([jpg.store](https://jpg.store))
 * get_ranks ([cnft.tools](https://cnft.tools))
 
 
 ### EVM (Ethereum and Polygon)
 
 ```python
@@ -132,14 +134,15 @@
 
 * get_asset ([moralis.io³](https://moralis.io))
 * get_assets ([moralis.io³](https://moralis.io))
 * get_holdings ([moralis.io³](https://moralis.io))
 * get_snapshot ([moralis.io³](https://moralis.io))
 * get_campaigns ([book.io](https://book.io))
 * get_listings ([opensea.io⁴](https://opensea.io))
+* get_floor ([opensea.io⁴](https://opensea.io))
 * get_sales ([opensea.io⁴](https://opensea.io))
 
 
 > ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).
 > 
 > ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).
 >
```

