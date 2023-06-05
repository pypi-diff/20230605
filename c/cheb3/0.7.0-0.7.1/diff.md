# Comparing `tmp/cheb3-0.7.0.tar.gz` & `tmp/cheb3-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheb3-0.7.0.tar", last modified: Thu Jun  1 12:33:46 2023, max compression
+gzip compressed data, was "cheb3-0.7.1.tar", last modified: Mon Jun  5 12:22:15 2023, max compression
```

## Comparing `cheb3-0.7.0.tar` & `cheb3-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yanhui    (1000) yanhui    (1000)        0 2023-06-01 12:33:46.150231 cheb3-0.7.0/
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     1063 2023-02-26 09:01:57.000000 cheb3-0.7.0/LICENSE
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     2938 2023-06-01 12:33:46.150231 cheb3-0.7.0/PKG-INFO
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     2316 2023-05-23 14:04:18.000000 cheb3-0.7.0/README.md
-drwxrwxr-x   0 yanhui    (1000) yanhui    (1000)        0 2023-06-01 12:33:46.150231 cheb3-0.7.0/cheb3/
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)      177 2023-02-26 12:36:38.000000 cheb3-0.7.0/cheb3/__init__.py
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     3450 2023-05-15 15:36:53.000000 cheb3-0.7.0/cheb3/account.py
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     2801 2023-04-18 14:04:12.000000 cheb3-0.7.0/cheb3/connection.py
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)       61 2023-04-10 07:50:43.000000 cheb3-0.7.0/cheb3/constants.py
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     9411 2023-05-16 14:06:43.000000 cheb3-0.7.0/cheb3/contract.py
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     9207 2023-05-17 13:05:49.000000 cheb3-0.7.0/cheb3/utils.py
-drwxrwxr-x   0 yanhui    (1000) yanhui    (1000)        0 2023-06-01 12:33:46.150231 cheb3-0.7.0/cheb3.egg-info/
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)     2938 2023-06-01 12:33:46.000000 cheb3-0.7.0/cheb3.egg-info/PKG-INFO
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)      283 2023-06-01 12:33:46.000000 cheb3-0.7.0/cheb3.egg-info/SOURCES.txt
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)        1 2023-06-01 12:33:46.000000 cheb3-0.7.0/cheb3.egg-info/dependency_links.txt
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)       29 2023-06-01 12:33:46.000000 cheb3-0.7.0/cheb3.egg-info/requires.txt
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)        6 2023-06-01 12:33:46.000000 cheb3-0.7.0/cheb3.egg-info/top_level.txt
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)      734 2023-06-01 12:31:05.000000 cheb3-0.7.0/pyproject.toml
--rw-rw-r--   0 yanhui    (1000) yanhui    (1000)       38 2023-06-01 12:33:46.150231 cheb3-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:22:15.241494 cheb3-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 12:22:04.000000 cheb3-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-05 12:22:15.241494 cheb3-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-05 12:22:04.000000 cheb3-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:22:15.237494 cheb3-0.7.1/cheb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-06-05 12:22:04.000000 cheb3-0.7.1/cheb3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:22:15.241494 cheb3-0.7.1/cheb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-05 12:22:15.000000 cheb3-0.7.1/cheb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 12:22:15.000000 cheb3-0.7.1/cheb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:22:15.000000 cheb3-0.7.1/cheb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 12:22:15.000000 cheb3-0.7.1/cheb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 12:22:15.000000 cheb3-0.7.1/cheb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 12:22:04.000000 cheb3-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:22:15.241494 cheb3-0.7.1/setup.cfg
```

### Comparing `cheb3-0.7.0/LICENSE` & `cheb3-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.0/PKG-INFO` & `cheb3-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.0
+Version: 0.7.1
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="center" style="display: flex;">
-    <img width="100" src="docs/_static/img/logo.png">
-    <img src="docs/_static/img/cheb3.png">
+<p align="center">
+    <img width="300" src="https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/cheb3.png">
 </p>
 
 <p align="center">🐣 web3 CTF tool based on web3.py</p>
 
 <p align="center">
     <a href="https://cheb3.readthedocs.io/en/latest/index.html">
+        <a href="https://pypi.python.org/pypi/cheb3"><img alt="PyPI" src="https://img.shields.io/pypi/v/cheb3.svg"></a>
         <img alt="Documentation" src="https://img.shields.io/readthedocs/cheb3.svg">
     </a>
 </p>
 
 ## Install
 
 ```bash
-pip3 install -U git+https://github.com/YanhuiJessica/cheb3.git#egg=cheb3
+pip3 install -U cheb3
 ```
 
 ## Quick Start
 
 ```py
 >>> from cheb3 import Connection
 >>> from cheb3.utils import compile_sol
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.0 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.1 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
-           [docs/_static/img/logo.png] [docs/_static/img/cheb3.png]
+ [https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/
+                                  cheb3.png]
                       ð£ web3 CTF tool based on web3.py
-                                [Documentation]
-## Install ```bash pip3 install -U git+https://github.com/YanhuiJessica/
-cheb3.git#egg=cheb3 ``` ## Quick Start ```py >>> from cheb3 import Connection
->>> from cheb3.utils import compile_sol >>> >>> conn = Connection("http://
-localhost:8545") >>> account = conn.account("") >>> abi, bytecode = compile_sol
-(''' // SPDX-License-Identifier: MIT pragma solidity ^0.8.0; import
-"@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract Cheb3Token is ERC20
-{ constructor(string memory _name, string memory _symbol) ERC20(_name, _symbol)
-{ _mint(msg.sender, 100); } } ''', solc_version="0.8.17", # choose the version
-of the compiler base_path="node_modules/" # to include @openzeppelin contracts
-)['Cheb3Token'] ``` ### Interacting with existing contracts #### Using ABI
-```py >>> to_addr = "0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract =
-conn.contract( account, # specified the signer address="", abi=abi ) >>> print
+                            [PyPI]_[Documentation]
+## Install ```bash pip3 install -U cheb3 ``` ## Quick Start ```py >>> from
+cheb3 import Connection >>> from cheb3.utils import compile_sol >>> >>> conn =
+Connection("http://localhost:8545") >>> account = conn.account("") >>> abi,
+bytecode = compile_sol(''' // SPDX-License-Identifier: MIT pragma solidity
+^0.8.0; import "@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract
+Cheb3Token is ERC20 { constructor(string memory _name, string memory _symbol)
+ERC20(_name, _symbol) { _mint(msg.sender, 100); } } ''', solc_version="0.8.17",
+# choose the version of the compiler base_path="node_modules/" # to include
+@openzeppelin contracts )['Cheb3Token'] ``` ### Interacting with existing
+contracts #### Using ABI ```py >>> to_addr =
+"0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract = conn.contract
+( account, # specified the signer address="", abi=abi ) >>> print
 (contract.functions.balanceOf(account.address).call()) >>>
 contract.functions.transfer(to_addr, 10).send_transaction() >>> print
 (contract.caller.balanceOf(to_addr)) # is equivalent to
 `contract.functions.balanceOf(to_addr).call()` ``` #### Using function
 signatures ```py >>> from cheb3.utils import encode_with_signature >>> >>>
 contract_addr = contract.address >>> account.send_transaction(contract_addr,
 data=encode_with_signature("transfer(address,uint256)", to_addr, 10)) >>> print
```

### Comparing `cheb3-0.7.0/README.md` & `cheb3-0.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-<p align="center" style="display: flex;">
-    <img width="100" src="docs/_static/img/logo.png">
-    <img src="docs/_static/img/cheb3.png">
+<p align="center">
+    <img width="300" src="https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/cheb3.png">
 </p>
 
 <p align="center">🐣 web3 CTF tool based on web3.py</p>
 
 <p align="center">
     <a href="https://cheb3.readthedocs.io/en/latest/index.html">
+        <a href="https://pypi.python.org/pypi/cheb3"><img alt="PyPI" src="https://img.shields.io/pypi/v/cheb3.svg"></a>
         <img alt="Documentation" src="https://img.shields.io/readthedocs/cheb3.svg">
     </a>
 </p>
 
 ## Install
 
 ```bash
-pip3 install -U git+https://github.com/YanhuiJessica/cheb3.git#egg=cheb3
+pip3 install -U cheb3
 ```
 
 ## Quick Start
 
 ```py
 >>> from cheb3 import Connection
 >>> from cheb3.utils import compile_sol
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-           [docs/_static/img/logo.png] [docs/_static/img/cheb3.png]
+ [https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/
+                                  cheb3.png]
                       ð£ web3 CTF tool based on web3.py
-                                [Documentation]
-## Install ```bash pip3 install -U git+https://github.com/YanhuiJessica/
-cheb3.git#egg=cheb3 ``` ## Quick Start ```py >>> from cheb3 import Connection
->>> from cheb3.utils import compile_sol >>> >>> conn = Connection("http://
-localhost:8545") >>> account = conn.account("") >>> abi, bytecode = compile_sol
-(''' // SPDX-License-Identifier: MIT pragma solidity ^0.8.0; import
-"@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract Cheb3Token is ERC20
-{ constructor(string memory _name, string memory _symbol) ERC20(_name, _symbol)
-{ _mint(msg.sender, 100); } } ''', solc_version="0.8.17", # choose the version
-of the compiler base_path="node_modules/" # to include @openzeppelin contracts
-)['Cheb3Token'] ``` ### Interacting with existing contracts #### Using ABI
-```py >>> to_addr = "0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract =
-conn.contract( account, # specified the signer address="", abi=abi ) >>> print
+                            [PyPI]_[Documentation]
+## Install ```bash pip3 install -U cheb3 ``` ## Quick Start ```py >>> from
+cheb3 import Connection >>> from cheb3.utils import compile_sol >>> >>> conn =
+Connection("http://localhost:8545") >>> account = conn.account("") >>> abi,
+bytecode = compile_sol(''' // SPDX-License-Identifier: MIT pragma solidity
+^0.8.0; import "@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract
+Cheb3Token is ERC20 { constructor(string memory _name, string memory _symbol)
+ERC20(_name, _symbol) { _mint(msg.sender, 100); } } ''', solc_version="0.8.17",
+# choose the version of the compiler base_path="node_modules/" # to include
+@openzeppelin contracts )['Cheb3Token'] ``` ### Interacting with existing
+contracts #### Using ABI ```py >>> to_addr =
+"0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract = conn.contract
+( account, # specified the signer address="", abi=abi ) >>> print
 (contract.functions.balanceOf(account.address).call()) >>>
 contract.functions.transfer(to_addr, 10).send_transaction() >>> print
 (contract.caller.balanceOf(to_addr)) # is equivalent to
 `contract.functions.balanceOf(to_addr).call()` ``` #### Using function
 signatures ```py >>> from cheb3.utils import encode_with_signature >>> >>>
 contract_addr = contract.address >>> account.send_transaction(contract_addr,
 data=encode_with_signature("transfer(address,uint256)", to_addr, 10)) >>> print
```

### Comparing `cheb3-0.7.0/cheb3/account.py` & `cheb3-0.7.1/cheb3/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def send_transaction(
         self, to: HexStr, value: int = 0, data: HexStr = "0x", **kwargs
     ) -> TxReceipt:
         """Transfer ETH or interact with a smart contract.
 
         :param to: The address of the receiver.
         :type to: HexStr
-        :param value: The amount to transfer, defaults to 0.
+        :param value: The amount to transfer, defaults to 0 (wei).
         :type value: int
         :param data: The transaction data, defaults to `0x`.
         :type data: HexStr
 
         Keyword Args:
             gas_price (int): Specify the gas price for the transaction.
             gas_limit (int): Specify the maximum gas the transaction can use.
```

### Comparing `cheb3-0.7.0/cheb3/connection.py` & `cheb3-0.7.1/cheb3/connection.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.0/cheb3/contract.py` & `cheb3-0.7.1/cheb3/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,40 +57,36 @@
 
     def deploy(self, *constructor_args, **kwargs) -> None:
         """Deploys the contract.
 
         :param constructor_args: Constructor arguments.
 
         Keyword Args:
-            value (int): The amount to transfer, defaults to 0.
+            value (int): The amount to transfer, defaults to 0 (wei).
             gas_price (int): Specifies the gas price for the deployment.
             gas_limit (int): Specifies the maximum gas the deployment can use.
             proxy (bool): A minimal proxy contract (ERC-1167) will be deployed
                 and connected to the logic contract if set to :const:`True`,
                 defaults to :const:`False`.
         """
         if not self.signer:
             raise AttributeError("The `signer` is missing.")
 
         if self.address:
-            logger.info(
-                f"Contract {type(self).__name__} has already been deployed at {self.address}."
-            )
+            logger.info(f"Contract {type(self).__name__} has already been deployed at {self.address}.")
             return
 
         tx = self.signer.sign_transaction(
             self.instance.constructor(*constructor_args).build_transaction(
                 {
                     "chainId": self.w3.eth.chain_id,
                     "nonce": self.w3.eth.get_transaction_count(self.signer.address),
                     "gas": kwargs.get(
                         "gas_limit",
-                        self.instance.constructor(*constructor_args).estimate_gas(
-                            {"from": self.signer.address}
-                        ),
+                        self.instance.constructor(*constructor_args).estimate_gas({"from": self.signer.address}),
                     ),
                     "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
                     "value": kwargs.get("value", 0),
                 }
             )
         ).rawTransaction
         logger.debug(f"Deploying {type(self).__name__} ...")
@@ -123,65 +119,53 @@
             logger.info(f"The proxy is deployed at {receipt.contractAddress}")
             self.address = receipt.contractAddress
 
         self.instance = self.w3.eth.contract(self.address, abi=self.instance.abi)
         self._init_functions()
 
     @staticmethod
-    def get_fallback_function(
-        abi: ABI, w3: Web3, signer: eth_account.Account, address: str
-    ):
+    def get_fallback_function(abi: ABI, w3: Web3, signer: eth_account.Account, address: str):
         if abi and fallback_func_abi_exists(abi):
             return ContractFunctionWrapper.factory(
                 "fallback",
                 w3=w3,
                 signer=signer,
                 contract_abi=abi,
                 address=address,
                 function_identifier=FallbackFn,
             )()
         else:
             return cast(ContractFunctionWrapper, NonExistentFallbackFunction())
 
     @staticmethod
-    def get_receive_function(
-        abi: ABI, w3: Web3, signer: eth_account.Account, address: str
-    ):
+    def get_receive_function(abi: ABI, w3: Web3, signer: eth_account.Account, address: str):
         if abi and receive_func_abi_exists(abi):
             return ContractFunctionWrapper.factory(
                 "receive",
                 w3=w3,
                 signer=signer,
                 contract_abi=abi,
                 address=address,
                 function_identifier=ReceiveFn,
             )()
         else:
             return cast(ContractFunctionWrapper, NonExistentReceiveFunction())
 
     def _init_functions(self) -> None:
-        self.functions = ContractFunctionsWrapper(
-            self.signer, self.instance.abi, self.w3, self.address
-        )
+        self.functions = ContractFunctionsWrapper(self.signer, self.instance.abi, self.w3, self.address)
         self.caller = ContractCaller(self.instance.abi, self.w3, self.address)
 
-        self.fallback = self.get_fallback_function(
-            self.instance.abi, self.w3, self.signer, self.address
-        )
-        self.receive = self.get_receive_function(
-            self.instance.abi, self.w3, self.signer, self.address
-        )
+        self.fallback = self.get_fallback_function(self.instance.abi, self.w3, self.signer, self.address)
+        self.receive = self.get_receive_function(self.instance.abi, self.w3, self.signer, self.address)
 
     @classmethod
     def factory(cls, w3: Web3, contract_name: str = "") -> "Contract":
         contract = cast(
             Contract,
-            PropertyCheckingFactory(
-                contract_name or cls.__name__.lower(), (cls,), {"w3": w3}
-            ),
+            PropertyCheckingFactory(contract_name or cls.__name__.lower(), (cls,), {"w3": w3}),
         )
         return contract
 
     def get_balance(self) -> int:
         """Returns the balance of the contract instance."""
         return self.w3.eth.get_balance(self.address)
 
@@ -229,26 +213,24 @@
 class ContractFunctionWrapper(ContractFunction):
     signer: eth_account.Account = None
 
     def send_transaction(self, **kwargs) -> TxReceipt:
         if not self.signer:
             raise AttributeError("The `signer` is missing.")
 
-        tx = {
-            "chainId": self.w3.eth.chain_id,
-            "nonce": self.w3.eth.get_transaction_count(self.signer.address),
-            "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
-            "value": kwargs.get("value", 0),
-        }
+        tx = self.build_transaction(
+            {
+                "chainId": self.w3.eth.chain_id,
+                "nonce": self.w3.eth.get_transaction_count(self.signer.address),
+                "gasPrice": kwargs.get("gas_price", self.w3.eth.gas_price),
+                "value": kwargs.get("value", 0),
+            }
+        )
         tx["gas"] = kwargs.get("gas_limit", self.w3.eth.estimate_gas(tx))
-        tx = self.signer.sign_transaction(self.build_transaction(tx)).rawTransaction
+        tx = self.signer.sign_transaction(tx).rawTransaction
         tx_hash = self.w3.eth.send_raw_transaction(tx).hex()
-        func_name = (
-            self.function_identifier
-            if isinstance(self.function_identifier, str)
-            else self.function_identifier.__name__
-        )
+        func_name = self.function_identifier if isinstance(self.function_identifier, str) else self.function_identifier.__name__
         logger.info(f"({self.address}).{func_name} transaction hash: {tx_hash}")
         receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         if not receipt.status:
             raise Exception(f"Transact to ({self.address}).{func_name} errored.")
         return receipt
```

### Comparing `cheb3-0.7.0/cheb3/utils.py` & `cheb3-0.7.1/cheb3/utils.py`

 * *Files identical despite different names*

### Comparing `cheb3-0.7.0/cheb3.egg-info/PKG-INFO` & `cheb3-0.7.1/cheb3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: cheb3
-Version: 0.7.0
+Version: 0.7.1
 Summary: Web3 CTF tool based on web3.py
 Author-email: YanhuiJessica <y4nhv1@gmail.com>
 Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/YanhuiJessica/cheb3
 Project-URL: Bug Reports, https://github.com/YanhuiJessica/cheb3/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="center" style="display: flex;">
-    <img width="100" src="docs/_static/img/logo.png">
-    <img src="docs/_static/img/cheb3.png">
+<p align="center">
+    <img width="300" src="https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/cheb3.png">
 </p>
 
 <p align="center">🐣 web3 CTF tool based on web3.py</p>
 
 <p align="center">
     <a href="https://cheb3.readthedocs.io/en/latest/index.html">
+        <a href="https://pypi.python.org/pypi/cheb3"><img alt="PyPI" src="https://img.shields.io/pypi/v/cheb3.svg"></a>
         <img alt="Documentation" src="https://img.shields.io/readthedocs/cheb3.svg">
     </a>
 </p>
 
 ## Install
 
 ```bash
-pip3 install -U git+https://github.com/YanhuiJessica/cheb3.git#egg=cheb3
+pip3 install -U cheb3
 ```
 
 ## Quick Start
 
 ```py
 >>> from cheb3 import Connection
 >>> from cheb3.utils import compile_sol
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: cheb3 Version: 0.7.0 Summary: Web3 CTF tool based
+Metadata-Version: 2.1 Name: cheb3 Version: 0.7.1 Summary: Web3 CTF tool based
 on web3.py Author-email: YanhuiJessica
 gmail.com> Project-URL: Homepage, https://github.com/YanhuiJessica/cheb3
 Project-URL: Documentation, https://cheb3.readthedocs.io/en/latest/ Project-
 URL: Source, https://github.com/YanhuiJessica/cheb3 Project-URL: Bug Reports,
 https://github.com/YanhuiJessica/cheb3/issues Classifier: Development Status ::
 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
-           [docs/_static/img/logo.png] [docs/_static/img/cheb3.png]
+ [https://raw.githubusercontent.com/YanhuiJessica/cheb3/main/docs/_static/img/
+                                  cheb3.png]
                       ð£ web3 CTF tool based on web3.py
-                                [Documentation]
-## Install ```bash pip3 install -U git+https://github.com/YanhuiJessica/
-cheb3.git#egg=cheb3 ``` ## Quick Start ```py >>> from cheb3 import Connection
->>> from cheb3.utils import compile_sol >>> >>> conn = Connection("http://
-localhost:8545") >>> account = conn.account("") >>> abi, bytecode = compile_sol
-(''' // SPDX-License-Identifier: MIT pragma solidity ^0.8.0; import
-"@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract Cheb3Token is ERC20
-{ constructor(string memory _name, string memory _symbol) ERC20(_name, _symbol)
-{ _mint(msg.sender, 100); } } ''', solc_version="0.8.17", # choose the version
-of the compiler base_path="node_modules/" # to include @openzeppelin contracts
-)['Cheb3Token'] ``` ### Interacting with existing contracts #### Using ABI
-```py >>> to_addr = "0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract =
-conn.contract( account, # specified the signer address="", abi=abi ) >>> print
+                            [PyPI]_[Documentation]
+## Install ```bash pip3 install -U cheb3 ``` ## Quick Start ```py >>> from
+cheb3 import Connection >>> from cheb3.utils import compile_sol >>> >>> conn =
+Connection("http://localhost:8545") >>> account = conn.account("") >>> abi,
+bytecode = compile_sol(''' // SPDX-License-Identifier: MIT pragma solidity
+^0.8.0; import "@openzeppelin/contracts/token/ERC20/ERC20.sol"; contract
+Cheb3Token is ERC20 { constructor(string memory _name, string memory _symbol)
+ERC20(_name, _symbol) { _mint(msg.sender, 100); } } ''', solc_version="0.8.17",
+# choose the version of the compiler base_path="node_modules/" # to include
+@openzeppelin contracts )['Cheb3Token'] ``` ### Interacting with existing
+contracts #### Using ABI ```py >>> to_addr =
+"0xAcF2f2575dFe641B350fE671f2Eb7E796A4ba402" >>> contract = conn.contract
+( account, # specified the signer address="", abi=abi ) >>> print
 (contract.functions.balanceOf(account.address).call()) >>>
 contract.functions.transfer(to_addr, 10).send_transaction() >>> print
 (contract.caller.balanceOf(to_addr)) # is equivalent to
 `contract.functions.balanceOf(to_addr).call()` ``` #### Using function
 signatures ```py >>> from cheb3.utils import encode_with_signature >>> >>>
 contract_addr = contract.address >>> account.send_transaction(contract_addr,
 data=encode_with_signature("transfer(address,uint256)", to_addr, 10)) >>> print
```

### Comparing `cheb3-0.7.0/pyproject.toml` & `cheb3-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cheb3"
-version = "0.7.0"
+version = "0.7.1"
 authors = [{name = "YanhuiJessica",email = "y4nhv1@gmail.com"}]
 description = "Web3 CTF tool based on web3.py"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "web3>=6.0.0",
   "py-solc-x",
```

