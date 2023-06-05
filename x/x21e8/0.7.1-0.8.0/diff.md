# Comparing `tmp/x21e8-0.7.1.tar.gz` & `tmp/x21e8-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.7.1.tar", max compression
+gzip compressed data, was "x21e8-0.8.0.tar", max compression
```

## Comparing `x21e8-0.7.1.tar` & `x21e8-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5126 2023-06-02 15:02:32.985456 x21e8-0.7.1/README.md
--rw-r--r--   0        0        0      794 2023-06-02 15:02:32.989456 x21e8-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6082 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2409 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/token.py
--rw-r--r--   0        0        0      765 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/config.py
--rw-r--r--   0        0        0     1096 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/data.py
--rw-r--r--   0        0        0     3885 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/utils.py
--rw-r--r--   0        0        0      619 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1035 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     2237 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4367 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6174 1970-01-01 00:00:00.000000 x21e8-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     5126 2023-06-05 07:40:44.116080 x21e8-0.8.0/README.md
+-rw-r--r--   0        0        0      794 2023-06-05 07:40:44.124084 x21e8-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6153 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2409 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/application/token.py
+-rw-r--r--   0        0        0      765 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1096 2023-06-05 07:40:44.124084 x21e8-0.8.0/x21e8/routers/data.py
+-rw-r--r--   0        0        0     4145 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      997 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1035 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2237 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4781 2023-06-05 07:40:44.128086 x21e8-0.8.0/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6174 1970-01-01 00:00:00.000000 x21e8-0.8.0/PKG-INFO
```

### Comparing `x21e8-0.7.1/README.md` & `x21e8-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/pyproject.toml` & `x21e8-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.7.1"
+version = "0.8.0"
 description = "x21e8 service to manage RDDL network identities on TrustAnchors and workflows."
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*"
```

### Comparing `x21e8-0.7.1/x21e8/application/liquid.py` & `x21e8-0.8.0/x21e8/application/liquid.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         (contract, contract_hash_rev) = self._create_contract(issue_request, nft_token, cid, pubkey)
 
         rpc_connection.settxfee(FEE_RATE)
         raw_tx = rpc_connection.createrawtransaction([], [{"data": "00"}])
         print(raw_tx)
 
         # get funded raw transaction
+        # this call troughs an exception if there are not enough funds
         frt = rpc_connection.fundrawtransaction(raw_tx, {"feeRate": FEE_RATE})
         print(frt)
         hex_frt = frt["hex"]
         print(hex_frt)
 
         ria = rpc_connection.rawissueasset(
             hex_frt,
```

### Comparing `x21e8-0.7.1/x21e8/application/planetmint.py` & `x21e8-0.8.0/x21e8/application/planetmint.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/application/token.py` & `x21e8-0.8.0/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/config.py` & `x21e8-0.8.0/x21e8/config.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/main.py` & `x21e8-0.8.0/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/network/liquid/__init__.py` & `x21e8-0.8.0/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/network/liquid/util.py` & `x21e8-0.8.0/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/routers/assets.py` & `x21e8-0.8.0/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/routers/data.py` & `x21e8-0.8.0/x21e8/routers/data.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/routers/machine.py` & `x21e8-0.8.0/x21e8/routers/machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.error import URLError
 
 from fastapi import APIRouter, HTTPException
-from planetmint_driver.exceptions import PlanetmintException
+from bitcoinrpc.authproxy import JSONRPCException
 
+from planetmint_driver.exceptions import PlanetmintException
 
 from x21e8.application.liquid import LiquidNode
 from x21e8.config import RDDL_ASSET_REG_ENDPOINT
 from x21e8.models.issuing_request import IssuingRequest
 from x21e8.models.nft_asset import NftAsset
 from x21e8.application.rddl import resolve_nft_cid
 from x21e8.utils.storage import store_asset
@@ -56,16 +57,21 @@
         print(f"The Planetmint server configured does not support the given transaction. {e}")
         raise HTTPException(
             status_code=423,
             detail=f"The Planetmint server configured does not support the given transaction. {e}",
         )
 
     if check_if_tokens_should_be_issued(issuing_request_input):
-        asset, asset_id, contract = LiquidNode().issue_tokens(issuing_request_input, token_nft["id"], nft_cid)
-        print(f"Liquid issued token: {asset_id}  - {contract}")
+        try:
+            asset, asset_id, contract = LiquidNode().issue_tokens(issuing_request_input, token_nft["id"], nft_cid)
+            print(f"Liquid issued token: {asset_id}  - {contract}")
+        except JSONRPCException as e:
+            print(f"Exception Token issuance : {e}")
+            raise HTTPException(status_code=425, detail=f"Exception: RDDL token issuance - {e}")
+
         try:
             response = LiquidNode.register_asset(asset, contract, RDDL_ASSET_REG_ENDPOINT)
             print(f"RDDL asset registration: {response}")
         except Exception as e:
             print(f"Exception: RDDL asset registration - {e}")
             raise HTTPException(status_code=425, detail=f"Exception: RDDL asset registration - {e}")
```

### Comparing `x21e8-0.7.1/x21e8/routers/seed.py` & `x21e8-0.8.0/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/routers/utils.py` & `x21e8-0.8.0/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/utils/encryption.py` & `x21e8-0.8.0/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/utils/storage.py` & `x21e8-0.8.0/x21e8/utils/storage.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/wallet/base_wallet.py` & `x21e8-0.8.0/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.8.0/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.8.0/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/wallet/seed.py` & `x21e8-0.8.0/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.1/x21e8/wallet/sw_wallet.py` & `x21e8-0.8.0/x21e8/wallet/sw_wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import TrezorCrypto
 
-from nacl.signing import SigningKey
+from planetmint_cryptoconditions.crypto import Ed25519SigningKey
 from x21e8.network import liquid
 from x21e8.wallet.base_wallet import BaseWallet
 
 HARDENED = 0x80000000
 PLANET_VERSION_PUBLIC = 0x02D41400
 PLANET_VERSION_PRIVATE = 0x02D40FC0
 
 
 class SoftwareWallet(BaseWallet):
     def __init__(self):
         self.seed = None
         self.private_key = None
         self.public_key = None
+        self.planetmint_address = None
         self.liquid_address = None
+        self.liquid_derived_key = None
         self._init_wallet()
 
     def planetmint_sign_digest(self, input, message: bytes):
-        ncal_sk = SigningKey(self.private_key)
-        res = ncal_sk.sign(message)
-        return res.signature  # signature matches signature from other schemes
+        cc_key = Ed25519SigningKey(self.private_key, "bytes")
+        signature = cc_key.sign(message, encoding="bytes")
+        return signature  # signature matches signature from other schemes
 
     def liquid_sign_digest(self, message: bytes):
         pass
 
     def get_liquid_pubkey(self) -> bytes:
-        pass
+        return self.liquid_address
 
     def get_liquid_address(self) -> bytes:
         return self.liquid_address
 
     def get_confidential_liquid_address(self) -> bytes:
         master_blinding_key = wally.asset_blinding_key_from_seed(self.seed)
         script_pubkey = wally.address_to_scriptpubkey(self.liquid_address, x21e8.network.liquid.WALLY_NETWORK_LIQUID)
@@ -44,14 +46,19 @@
         )
         return confidential_address
         # end-create_conf_address
 
     def get_planetmint_pubkey(self) -> bytes:
         return self.public_key
 
+    def get_planetmint_address(self) -> str:
+        cc_key = Ed25519SigningKey(self.private_key, "bytes")
+        encoded_vk = cc_key.get_verifying_key().encode().decode()
+        return encoded_vk
+
     def _get_planetmint_keys_tc(self, id: int):
         self._read_seed()
         node = TrezorCrypto.from_seed(self.seed, TrezorCrypto.ED25519_NAME)
         # [Chain m/0'] check tests/bip32_tests.py for more derivation path examples
         node.derive(HARDENED | 0)
         self.private_key = node.private_key()
         self.public_key = node.public_key()[1:]
@@ -70,16 +77,17 @@
 
         liquid.liquid_api.bip32_key_from_seed(
             self.seed, len(self.seed), liquid.VER_TEST_PRIVATE, 0, liquid.liquid_api.byref(master)
         )
         liquid.liquid_api.bip32_key_from_parent_path_str_n(
             master, derivation_path, len(derivation_path), 0, liquid.BIP32_FLAG_KEY_PRIVATE, derived_key
         )
+        self.liquid_derived_key = derived_key
         _, derived_key_address = liquid.liquid_api.wally_bip32_key_to_address(
-            master, liquid.WALLY_ADDRESS_TYPE_P2PKH, liquid.WALLY_ADDRESS_VERSION_P2PKH_LIQUID_TESTNET
+            derived_key, liquid.WALLY_ADDRESS_TYPE_P2PKH, liquid.WALLY_ADDRESS_VERSION_P2PKH_LIQUID_TESTNET
         )
         return derived_key_address
 
     def make_cbuffer(hex_in):
         from binascii import unhexlify
 
         if hex_in is None:
```

### Comparing `x21e8-0.7.1/PKG-INFO` & `x21e8-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.7.1
+Version: 0.8.0
 Summary: x21e8 service to manage RDDL network identities on TrustAnchors and workflows.
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

