# Comparing `tmp/bookio_fetchfox-0.1.2.tar.gz` & `tmp/bookio_fetchfox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.1.2.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.2.0.tar", max compression
```

## Comparing `bookio_fetchfox-0.1.2.tar` & `bookio_fetchfox-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0     3532 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1770 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2664 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      449 2023-06-04 20:24:00.555455 bookio_fetchfox-0.1.2/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1570 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4154 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2573 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     5680 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     1430 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0     9675 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      452 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     7647 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      453 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      178 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      463 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1177 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      362 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1239 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1677 2023-06-04 20:24:00.559455 bookio_fetchfox-0.1.2/fetchfox/rest.py
--rw-r--r--   0        0        0     1094 2023-06-04 20:24:00.571455 bookio_fetchfox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.2/setup.py
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3532 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1770 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2664 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      449 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1606 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/cardano/jpgstore.py
+-rwxr-xr-x   0        0        0      675 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4154 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2573 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     6014 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     1698 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    10257 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     7981 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      178 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     1215 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      463 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1320 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      362 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1382 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1677 2023-06-05 17:47:28.258699 bookio_fetchfox-0.2.0/fetchfox/rest.py
+-rw-r--r--   0        0        0     1116 2023-06-05 17:47:28.270699 bookio_fetchfox-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 bookio_fetchfox-0.2.0/setup.py
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 bookio_fetchfox-0.2.0/PKG-INFO
```

### Comparing `bookio_fetchfox-0.1.2/README.md` & `bookio_fetchfox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,19 +20,22 @@
 def get_listings(policy_id: str) -> Iterable[dict]:
     check_str(policy_id, "jpgstore.policy_id")
     policy_id = policy_id.strip().lower()
 
     cursor = ""
 
     while True:
+        params = {}
+
+        if cursor:
+            params["cursor"] = cursor
+
         response, status_code = get(
             f"policy/{policy_id}/listings",
-            params={
-                "cursor": cursor,
-            },
+            params=params,
         )
 
         cursor = response.get("nextPageCursor")
 
         if not cursor:  # pragma: no cover
             break
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.2.0/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from datetime import datetime
-from typing import Iterable
+from typing import Iterable, Optional
 
 import pytz
 
 from fetchfox.apis.algorand import (
     algonodecloud,
     nfdomains,
     randswapcom,
@@ -139,14 +139,25 @@
                 marketplace=ALGOXNFT_COM,
                 price=listing["price"] // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=listing["seller"],
             )
 
+    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+        floor = None
+
+        for listing in self.get_listings(collection_id):
+            if floor is None:
+                floor = listing
+            elif listing.usd < floor.usd:
+                floor = listing
+
+        return floor
+
     def get_sales(self, collection_id: str, *args, **kwargs) -> Iterable[SaleDTO]:
         venues = {
             "algoxnft": ALGOXNFT_COM,
             "randgallery": RANDGALLERY_COM,
             "shufl": SHUFL_APP,
             None: UNKNOWN,
         }
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import abstractmethod
-from typing import Iterable
+from typing import Iterable, Optional
+from fetchfox.apis import coingeckocom
 
 from fetchfox.dtos import (
     AssetDTO,
     CampaignDTO,
     HoldingDTO,
     ListingDTO,
     RankDTO,
@@ -12,14 +13,17 @@
 
 
 class Blockchain:
     def __init__(self, name: str, currency: str):
         self.name: str = name
         self.currency: str = currency
 
+    def usd(self) -> float:
+        return coingeckocom.usd(self.currency)
+
     @abstractmethod
     def get_assets(
         self, collection_id: str, fetch_metadata: bool = True, *args, **kwargs
     ) -> Iterable[AssetDTO]:
         raise NotImplementedError()
 
     @abstractmethod
@@ -33,14 +37,18 @@
     def get_holdings(self, wallet: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_listings(self, collection_id: str, *args, **kwargs) -> Iterable[ListingDTO]:
         raise NotImplementedError()
 
+    @abstractmethod
+    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+        raise NotImplementedError()
+
     def get_ranks(self, collection_id: str, *args, **kwargs) -> Iterable[RankDTO]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_snapshot(self, collection_id: str, *args, **kwargs) -> Iterable[HoldingDTO]:
         raise NotImplementedError()
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import logging
 from datetime import datetime
 from functools import lru_cache
-from typing import Iterable
+from typing import Iterable, Optional
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.cardano import blockfrostio, cnfttools, handleme, jpgstore
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import CARDANO
@@ -182,14 +182,17 @@
                 address=stake_address,
                 quantity=holding["amount"],
             )
 
     def get_listings(
         self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
     ) -> Iterable[ListingDTO]:
+        if collection_discriminator:
+            collection_discriminator = collection_discriminator.lower()
+
         for listing in jpgstore.get_listings(collection_id):
             asset_id = listing["asset_id"]
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
             if collection_discriminator:
                 if collection_discriminator not in asset_name.lower():
@@ -223,14 +226,30 @@
                 price=int(listing["price_lovelace"]) // 10**6,
                 currency=self.currency,
                 listed_at=listed_at,
                 listed_by=None,
                 tx_hash=listing["tx_hash"],
             )
 
+    def get_floor(
+        self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
+    ) -> Optional[ListingDTO]:
+        floor = None
+
+        for listing in self.get_listings(
+            collection_id,
+            collection_discriminator=collection_discriminator,
+        ):
+            if floor is None:
+                floor = listing
+            elif listing.usd < floor.usd:
+                floor = listing
+
+        return floor
+
     def get_sales(
         self, collection_id: str, collection_discriminator: str = None, *args, **kwargs
     ) -> Iterable[SaleDTO]:
         for sale in jpgstore.get_sales(collection_id):
             asset_id = sale["asset_id"]
             policy_id, asset_name = utils.split_asset_id(asset_id)
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from datetime import datetime
-from typing import Iterable
+from typing import Iterable, Optional
 
 import pytz
 
 from fetchfox.apis import bookio
 from fetchfox.apis.evm import moralisio, ensideascom, openseaio
 from fetchfox.blockchains.base import Blockchain
 from fetchfox.constants.blockchains import ETHEREUM
@@ -190,14 +190,25 @@
                 price=float(int(price["value"]) / 10 ** price["decimals"]),
                 currency=price["currency"].replace("WETH", "ETH"),
                 listed_at=listed_at,
                 listed_by=parameters["offerer"],
                 tx_hash=listing["order_hash"],
             )
 
+    def get_floor(self, collection_id: str, *args, **kwargs) -> Optional[ListingDTO]:
+        floor = None
+
+        for listing in self.get_listings(collection_id):
+            if floor is None:
+                floor = listing
+            elif listing.usd < floor.usd:
+                floor = listing
+
+        return floor
+
     def get_sales(
         self, collection_id: str, slug: str = None, *args, **kwargs
     ) -> Iterable[SaleDTO]:
         sales = openseaio.get_sales(
             collection_id,
             api_key=self.openseaio_api_key,
             slug=slug,
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.2.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.2.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.2.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.2.0/fetchfox/dtos/sale.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from datetime import datetime
 from typing import List
 
+from fetchfox.apis import coingeckocom
 
-class ListingDTO:
+
+class SaleDTO:
     def __init__(
         self,
         identifier: str,
         collection_id: str,
         asset_ids: List[str],
         asset_names: List[str],
-        listing_id: str,
+        tx_hash: str,
         marketplace: str,
         price: float,
         currency: str,
-        listed_at: datetime,
-        listed_by: str = None,
-        tx_hash: str = None,
+        confirmed_at: datetime,
+        sale_id: str = None,
+        sold_by: str = None,
+        bought_by: str = None,
     ):
         self.identifier: str = identifier
         self.collection_id: str = collection_id
         self.asset_ids: List[str] = asset_ids
         self.asset_names: List[str] = asset_names
-        self.listing_id: str = listing_id
+        self.tx_hash: str = tx_hash
         self.marketplace: str = marketplace
         self.price: float = price
         self.currency: str = currency
-        self.listed_at: datetime = listed_at
-        self.listed_by: str = listed_by
-        self.tx_hash: str = tx_hash
+        self.confirmed_at: datetime = confirmed_at
+        self.sale_id: str = sale_id
+        self.sold_by: str = sold_by
+        self.bought_by: str = bought_by
+
+    @property
+    def usd(self) -> float:
+        return self.price * coingeckocom.usd(self.currency)
 
     @property
     def first(self) -> str:
         return self.asset_ids[0]
 
     @property
     def is_bundle(self) -> bool:
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.2.0/fetchfox/dtos/listing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from datetime import datetime
 from typing import List
 
+from fetchfox.apis import coingeckocom
 
-class SaleDTO:
+
+class ListingDTO:
     def __init__(
         self,
         identifier: str,
         collection_id: str,
         asset_ids: List[str],
         asset_names: List[str],
-        tx_hash: str,
+        listing_id: str,
         marketplace: str,
         price: float,
         currency: str,
-        confirmed_at: datetime,
-        sale_id: str = None,
-        sold_by: str = None,
-        bought_by: str = None,
+        listed_at: datetime,
+        listed_by: str = None,
+        tx_hash: str = None,
     ):
         self.identifier: str = identifier
         self.collection_id: str = collection_id
         self.asset_ids: List[str] = asset_ids
         self.asset_names: List[str] = asset_names
-        self.tx_hash: str = tx_hash
+        self.listing_id: str = listing_id
         self.marketplace: str = marketplace
         self.price: float = price
         self.currency: str = currency
-        self.confirmed_at: datetime = confirmed_at
-        self.sale_id: str = sale_id
-        self.sold_by: str = sold_by
-        self.bought_by: str = bought_by
+        self.listed_at: datetime = listed_at
+        self.listed_by: str = listed_by
+        self.tx_hash: str = tx_hash
+
+    @property
+    def usd(self) -> float:
+        return self.price * coingeckocom.usd(self.currency)
 
     @property
     def first(self) -> str:
         return self.asset_ids[0]
 
     @property
     def is_bundle(self) -> bool:
```

### Comparing `bookio_fetchfox-0.1.2/fetchfox/rest.py` & `bookio_fetchfox-0.2.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.2/pyproject.toml` & `bookio_fetchfox-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.1.2"
+version = "0.2.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
@@ -33,14 +33,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 backoff = "^2.2.1"
 asyncio = "^3.4.3"
 aiohttp = "^3.8.4"
 pytz = "^2023.3"
+cachetools = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 coverage = "^7.2.7"
 ddt = "^1.6.0"
 
 [build-system]
```

### Comparing `bookio_fetchfox-0.1.2/setup.py` & `bookio_fetchfox-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
+ 'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-0.1.2/PKG-INFO` & `bookio_fetchfox-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Documentation, https://github.com/book-io/fetchfox/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # book.io / fetchfox
 
 > Collection of API services to fetch information from several blockchains.
```

