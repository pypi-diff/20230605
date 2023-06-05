# Comparing `tmp/ever_playground-0.6.2.tar.gz` & `tmp/ever_playground-0.6.3.tar.gz`

## Comparing `ever_playground-0.6.2.tar` & `ever_playground-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 ever_playground-0.6.2/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.2/.gitignore
--rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.6.2/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.2/README.md
--rw-rw-r--   0     1000     1000     4831 2023-05-22 11:02:08.000000 ever_playground-0.6.2/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     5944 2023-05-22 15:35:59.000000 ever_playground-0.6.2/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.2/examples/basics.py
--rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.6.2/examples/highload/generate.fif
--rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.2/examples/highload/highload-wallet-v2.fif
--rw-rw-r--   0     1000     1000     4688 2023-05-22 21:07:18.000000 ever_playground-0.6.2/examples/highload/highload-wallet-v2.py
--rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/order-list-fift
--rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.6.2/examples/highload/order-list-py
--rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/sample.pk
--rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/sample27172.addr
--rw-rw-r--   0     1000     1000     1487 2023-05-24 13:11:36.000000 ever_playground-0.6.2/examples/ifjmp-perf-eval.py
--rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.2/examples/recover-stake.fif
--rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.2/examples/recover-stake.py
--rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.2/examples/runvm.py
--rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.2/examples/testgiver.fif
--rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.6.2/examples/testgiver.py
--rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.2/examples/validator-elect-req.fif
--rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.2/examples/validator-elect-req.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.2/pyproject.toml
--rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.6.2/run-examples.py
--rw-rw-r--   0     1000     1000    18118 2023-05-22 15:37:09.000000 ever_playground-0.6.2/src/lib.rs
--rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.6.2/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.2/src/utils.rs
--rw-rw-r--   0     1000     1000    24730 2023-05-24 13:19:21.000000 ever_playground-0.6.2/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 ever_playground-0.6.3/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.3/.gitignore
+-rw-rw-r--   0     1000     1000      230 2023-06-02 10:45:36.000000 ever_playground-0.6.3/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.3/README.md
+-rw-rw-r--   0     1000     1000     1062 2023-05-24 15:04:04.000000 ever_playground-0.6.3/create-param8.py
+-rw-rw-r--   0     1000     1000     4916 2023-06-05 17:34:16.000000 ever_playground-0.6.3/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     7420 2023-06-05 17:25:46.000000 ever_playground-0.6.3/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.3/examples/basics.py
+-rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.6.3/examples/highload/generate.fif
+-rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.3/examples/highload/highload-wallet-v2.fif
+-rw-rw-r--   0     1000     1000     4688 2023-05-22 21:07:18.000000 ever_playground-0.6.3/examples/highload/highload-wallet-v2.py
+-rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/order-list-fift
+-rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.6.3/examples/highload/order-list-py
+-rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/sample.pk
+-rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/sample27172.addr
+-rw-rw-r--   0     1000     1000     1487 2023-05-24 13:11:36.000000 ever_playground-0.6.3/examples/ifjmp-perf-eval.py
+-rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.3/examples/recover-stake.fif
+-rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.3/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.3/examples/runvm.py
+-rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.3/examples/testgiver.fif
+-rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.6.3/examples/testgiver.py
+-rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.3/examples/validator-elect-req.fif
+-rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.3/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.3/pyproject.toml
+-rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.6.3/run-examples.py
+-rw-rw-r--   0     1000     1000    18724 2023-06-02 10:13:02.000000 ever_playground-0.6.3/src/lib.rs
+-rw-rw-r--   0     1000     1000     1021 2023-06-05 17:30:59.000000 ever_playground-0.6.3/src/tests.rs
+-rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.3/src/utils.rs
+-rw-rw-r--   0     1000     1000     3036 2023-06-02 16:56:59.000000 ever_playground-0.6.3/try-catch.py
+-rw-rw-r--   0     1000     1000     3572 2023-06-05 17:22:15.000000 ever_playground-0.6.3/ttt.py
+-rw-rw-r--   0     1000     1000    24716 2023-06-05 17:36:39.000000 ever_playground-0.6.3/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.3/PKG-INFO
```

### Comparing `ever_playground-0.6.2/Cargo.toml` & `ever_playground-0.6.3/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 [package]
 name = "ever-playground"
-version = "0.6.2"
+version = "0.6.3"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
 ed25519-dalek = "1"
 num-bigint = "0.4"
 pyo3 = { version = "0.18.3", features = ["extension-module", "num-bigint"] }
 rand = "0.7"
 
-ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.61" }
-ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.7" }
-ton_labs_assembler = { git = "https://github.com/tonlabs/ever-assembler", tag = "1.2.111" }
-ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.149" }
+ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.72" }
+ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.13" }
+ton_labs_assembler = { git = "https://github.com/tonlabs/ever-assembler", tag = "1.2.120" }
+ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.164" }
+
+#[patch."ssh://git@github.com/tonlabs/ever-block-private.git"]
+#ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.72" }
+#
+#[patch."ssh://git@github.com/tonlabs/ever-types-private.git"]
+#ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.13" }
```

### Comparing `ever_playground-0.6.2/README.md` & `ever_playground-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/ever_playground/__init__.py` & `ever_playground-0.6.3/ever_playground/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Tuple
+from typing import Optional, Tuple
 from fractions import Fraction
 
 from .ever_playground import Cell, Builder, Slice, Dictionary, assemble, runvm
 from .ever_playground import ed25519_new_keypair, ed25519_secret_to_public, ed25519_sign, ed25519_check_signature
 
 __all__ = [
     "Cell",
@@ -77,42 +77,42 @@
     print(f"Loading private key from file {filename}")
     with open(filename, "rb") as file:
         secret = file.read()
         public = ed25519_secret_to_public(secret)
         return public, secret
 
 class StateInit:
-    split_depth: int
+    split_depth: Optional[int]
     tick: bool
     tock: bool
-    code: Cell
-    data: Cell
-    library: Dictionary
+    code: Optional[Cell]
+    data: Optional[Cell]
+    library: Optional[Dictionary]
 
     def __init__(
             self,
-            split_depth: int = None,
+            split_depth: Optional[int] = None,
             tick: bool = False,
             tock: bool = False,
-            code: Cell = None,
-            data: Cell = None,
-            library: Dictionary = None):
+            code: Optional[Cell] = None,
+            data: Optional[Cell] = None,
+            library: Optional[Dictionary] = None):
         self.split_depth = split_depth
         self.tick = tick
         self.tock = tock
         self.code = code
         self.data = data
         self.library = library
 
     def deserialize(self, s: Slice):
         if s.u(1):
             self.split_depth = s.u(5)
         if s.u(1):
-            self.tick = s.u(1)
-            self.tock = s.u(1)
+            self.tick = bool(s.u(1))
+            self.tock = bool(s.u(1))
         else:
             self.tick = self.tock = False
         if s.u(1):
             self.code = s.r()
         if s.u(1):
             self.data = s.r()
         if s.u(1):
@@ -136,40 +136,40 @@
         if self.data is None:
             b.i(1, 0)
         else:
             b.i(1, 1).r(self.data)
         if self.library is None:
             b.i(1, 0)
         else:
-            b.i(1, 1).s(Slice(self.library.serialize()))
+            b.i(1, 1).b(self.library.serialize())
         return b
 
 class Currency:
     FACTOR = 1000000000
     value: int
 
-    def __init__(self, value: int = None):
+    def __init__(self, value: int = 0):
         if value < 0 or value.bit_length() > 128:
             raise Exception("Currency value must be non-negative and fit into 128 bits")
         self.value = value
 
-    @classmethod
-    def from_str(cls, value: str):
-        value = int(Fraction(value) * Currency.FACTOR)
-        return Currency(value)
+    @staticmethod
+    def from_str(value: str):
+        return Currency(int(Fraction(value) * Currency.FACTOR))
 
     def deserialize(self, s: Slice):
         len = s.u(4)
         if len == 0:
             self.value = 0
         else:
             self.value = s.u(len * 8)
+        return self
 
     def serialize(self) -> Builder:
         if self.value == 0:
             return Builder().i(4, 0)
         len = (self.value.bit_length() + 7) >> 3
-        assert(len <= 16)
+        assert(len < 16)
         return Builder().i(4, len).i(len * 8, self.value)
 
     def __str__(self) -> str:
         return str(float(Fraction(self.value) / self.FACTOR))
```

### Comparing `ever_playground-0.6.2/ever_playground/ever_playground.pyi` & `ever_playground-0.6.3/ever_playground/ever_playground.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,252 @@
+from typing import Optional
+
 class Cell:
     """
     A TVM cell consists of at most 1023 bits of data, and of at
     most four references to other cells. All persistent data (including TVM
     code) in the TON Blockchain is represented as a collection of TVM
     cells.
     """
 
     def write(self, flags: int) -> bytes:
         """
-        Writes the Cell to a boc bytestream.
+        Writes the cell to boc bytes.
 
-        Bits of the flags parameter have the following effect:
+        Bits of the ``flags`` parameter have the following effect:
         - +1 enables bag-of-cells index creation (useful for lazy deserialization of large bags of cells).
         - +2 includes the CRC32-C of all data into the serialization (useful for checking data integrity).
         """
 
     @staticmethod
     def read(bytes: bytes) -> Cell:
         """
-        Reads a Cell from a boc bytestream.
+        Reads a Cell from the boc ``bytes``.
         """
 
     def repr_hash(self) -> int:
         """
-        Returns representation hash of the Cell.
+        Returns the representation hash of the cell.
+        """
+
+    def cells_count(self) -> int:
+        """
+        Returns the total cells count.
+        """
+
+    def unique_cells_count(self) -> int:
+        """
+        Returns the unique cells count.
         """
 
 class Slice:
     """
     A TVM cell slice, or slice for short, is a contiguous “sub-cell”
     of an existing cell, containing some of its bits of data and some of its
     references. Essentially, a slice is a read-only view for a subcell of a cell.
     Slices are used for unpacking data previously stored (or serialized) in a
     cell or a tree of cells.
     """
 
-    def __init__(self, cell: Cell) -> Slice: ...
+    def __init__(self, cell: Cell) -> None: ...
 
     def i(self, bits: int) -> int:
         """
-        Reads a signed integer out from the Slice and shifts internal data pointer.
+        Reads a signed integer of bit length ``bits`` and advances the internal data pointer.
         """
 
     def u(self, bits: int) -> int:
         """
-        Reads an unsigned integer out from the Slice and shifts internal data pointer.
+        Reads an unsigned integer of bit length ``bits`` and advances the internal data pointer.
         """
 
     def refs(self) -> int:
         """
-        Returns remaining references count.
+        Returns the remaining children cells (aka references) count.
         """
 
     def r(self) -> Cell:
         """
-        Reads a Cell out from the Slice and shifts internal refs pointer.
+        Reads the next children cell (aka reference) and advances the internal refs pointer.
         """
 
     def is_empty(self) -> bool:
         """
-        Returns whether the Slice data is empty.
+        Returns whether the data of the slice is empty.
         """
 
 class Builder:
     """
     A TVM cell builder, or builder for short, is an “incomplete”
     cell that supports fast operations of appending bitstrings and cell references
     at its end. Builders are used for packing (or serializing) data
     from the top of the stack into new cells (e.g., before transferring them
     to persistent storage).
     """
 
     def s(self, slice: Slice) -> Builder:
         """
-        Appends a Builder with a Slice.
+        Appends Builder with ``slice``.
         """
 
     def b(self, builder: Builder) -> Builder:
         """
-        Appends a Builder with another Builder.
+        Appends Builder with another ``builder``.
         """
 
     def i(self, bits: int, integer: int) -> Builder:
         """
-        Appends a Builder with an integer of specified length.
+        Appends Builder with ``integer`` of specified bit length ``bits``.
         """
 
     def ib(self, bin: str) -> Builder:
         """
-        Appends a Builder with an integer from binary string.
+        Appends Builder with an integer from the binary string ``bin``.
         """
 
     def x(self, bitstring: str) -> Builder:
         """
-        Appends a Builder with a bitstring.
+        Appends Builder with ``bitstring``.
 
-        TODO describe what TVM bitstring is
+        Bitstrings provide a way to represent a sequence of bits as a hexadecimal string.
+        If the sequence has the bit length multiple of 4, then the hexadecimal string
+        contains just length/4 count of hexadecimal digits. Otherwise, the representation
+        uses a completion tag ``_`` in the end of the hexstring, which means that
+        the rightmost ``0`` bits and the first ``1`` bit are trimmed. For more details,
+        see chapter 1.0 of the TVM whitepaper.
         """
 
     def y(self, data: bytes) -> Builder:
         """
-        Appends a Builder with bytes.
+        Appends Builder with the ``data`` bytes.
         """
 
     def r(self, cell: Cell) -> Builder:
         """
-        Appends a Builder with a Cell.
+        Appends Builder with ``cell``.
         """
 
     def fits(self, slice: Slice, extra_bits: int, extra_refs: int) -> bool:
         """
-        TODO
+        Checks whether Builder can be appended with ``slice``, some extra data of the
+        ``extra_bits`` length, and some extra children cells ``extra_refs``. 
         """
 
     def finalize(self) -> Cell:
         """
-        Converts a Builder into an ordinary Cell.
+        Converts (finalizes) Builder into an ordinary Cell.
         """
 
     def slice(self) -> Slice:
         """
-        Converts a Builder into a Slice.
+        Converts Builder into Slice.
 
         This is a shortcut for doing Builder.finalize().slice()
         """
 
 class Dictionary:
     """
     Hashmaps, or dictionaries, are a specific data structure represented by a tree
     of cells. Essentially, a hashmap represents a map from keys, which are bitstrings
     of either fixed or variable length, into values of an arbitrary type X,
     in such a way that fast lookups and modifications be possible.
     """
 
     def __init__(self, bit_len: int) -> None: ...
 
-    def get(self, key: Slice) -> Slice:
+    def get(self, key: Slice) -> Optional[Slice]:
         """
-        Searches for a given key and returns corresponding value. None is returned when key is not found.
+        Gets a value for the given ``key``.
         """
 
     def add(self, key: Slice, value: Slice) -> Dictionary:
         """
-        TODO
+        Sets ``value`` for the given ``key``.
         """
 
     def add_kv_slice(self, key_len: int, slice: Slice) -> Dictionary:
         """
-        Adds a new key-value pair from the slice. The first key_len data bits are used as a key,
+        Adds a new key-value pair from ``slice``. The first ``key_len`` data bits are used as a key,
         and all the rest as a value.
         """
 
     def cell(self) -> Cell:
         """
         Returns underlying cell.
         """
 
     def serialize(self) -> Builder:
         """
-        Serializes a Dictionary into a Builder as defined in the TL-B scheme of HashmapE.
+        Serializes Dictionary into Builder as defined in the TL-B scheme of HashmapE.
         """
 
-    def deserialize(self, slice: Slice) -> Dictionary:
+    @staticmethod
+    def deserialize(bits: int, slice: Slice) -> Dictionary:
         """
-        Deserializes a Dictionary from a Slice.
+        Deserializes Dictionary from ``slice`` with the ``bits`` key length.
         """
 
 class NaN:
     """
     Opaque type representing a special case of the TVM Integer type.
     """
 
 class Continuation:
     """
-    Opaque type representing Contination value on the output stack of TVM invocation.
+    Opaque type representing a Continuation value in the output stack of TVM invocation.
     """
 
 def runvm(code: Slice, stack: list, **kwargs) -> VmResult:
     """
-    Invokes a new instance of TVM with the current continuation cc initialized from Slice code.
-    A stack of values is passed to the instance before execution.
+    Invokes TVM with the current continuation cc initialized from the ``code`` slice and
+    the ``stack`` of values.
 
     Optional parameters:
      - capabilities: int
      - c4: Cell
      - c7: list
      - gas_limit: int
      - gas_credit: int
      - trace: bool
+
+    Returns VmResult.    
     """
 
 class VmResult:
     stack: list
     exit_code: int
     exception_value: object
     steps: int
     gas_used: int
 
 def assemble(code: str) -> Cell:
     """
-    Translates a code string in assembler language to a Cell of TVM bytecode.
+    Translates the ``code`` string in assembler language to a Cell of TVM bytecode.
     """
 
 from typing import Tuple
 
 def ed25519_new_keypair() -> Tuple[bytes, bytes]:
     """
+    Generates a new Ed25519 private/public key pair, and returns both the private key
+    and the public key as 32-byte values.
+
+    Example:
+    ```
+        secret, public = ed25519_new_keypair()
+    ```
     """
 
 def ed25519_secret_to_public(secret: bytes) -> bytes:
     """
+    Computes the public key corresponding to the private Ed25519 key ``secret``.
     """
 
 def ed25519_sign(data: bytes, secret: bytes) -> bytes:
     """
+    Signs ``data`` with the Ed25519 private key ``secret`` (a 32-byte value) and returns the signature as a 64-byte value.
     """
 
 def ed25519_check_signature(data: bytes, signature: bytes, public: bytes) -> bool:
     """
+    Checks whether ``signature`` is a valid Ed25519 signature of ``data`` with the public key ``public``.
     """
```

### Comparing `ever_playground-0.6.2/examples/basics.py` & `ever_playground-0.6.3/examples/basics.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/highload/generate.fif` & `ever_playground-0.6.3/examples/highload/generate.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/highload/highload-wallet-v2.fif` & `ever_playground-0.6.3/examples/highload/highload-wallet-v2.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/highload/highload-wallet-v2.py` & `ever_playground-0.6.3/examples/highload/highload-wallet-v2.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/ifjmp-perf-eval.py` & `ever_playground-0.6.3/examples/ifjmp-perf-eval.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/recover-stake.fif` & `ever_playground-0.6.3/examples/recover-stake.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/recover-stake.py` & `ever_playground-0.6.3/examples/recover-stake.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/runvm.py` & `ever_playground-0.6.3/examples/runvm.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/testgiver.fif` & `ever_playground-0.6.3/examples/testgiver.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/testgiver.py` & `ever_playground-0.6.3/examples/testgiver.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/validator-elect-req.fif` & `ever_playground-0.6.3/examples/validator-elect-req.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/examples/validator-elect-req.py` & `ever_playground-0.6.3/examples/validator-elect-req.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/pyproject.toml` & `ever_playground-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/run-examples.py` & `ever_playground-0.6.3/run-examples.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/src/lib.rs` & `ever_playground-0.6.3/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mod tests;
 mod utils;
 
-use std::sync::Arc;
+use std::{sync::Arc, collections::HashSet};
 
 use ed25519_dalek::Signer;
 use utils::*;
 
 use num_bigint::{BigInt, BigUint, Sign};
 use pyo3::{
     prelude::*,
@@ -37,15 +37,15 @@
     #[pyo3(signature = (bitstring, *args))]
     fn new(bitstring: String, args: &PyTuple) -> PyResult<Self> {
         if args.len() > 4 {
             return err!("cell can't contain more than 4 references")
         }
         let slice = SliceData::from_string(&bitstring)
             .map_err(|_| PyRuntimeError::new_err(format!("invalid bitstring \"{}\"", bitstring)))?;
-        let mut b = BuilderData::from_slice(&slice);
+        let mut b = slice.as_builder();
         for arg in args.iter() {
             let cell = arg.extract::<Cell>()?;
             b.checked_append_reference(cell.cell).map_err(runtime_err)?;
         }
         let cell = b.into_cell().map_err(runtime_err)?;
         Ok(Self { cell })
     }
@@ -71,17 +71,35 @@
             .map(|cell| Self { cell })
             .map_err(runtime_err)
     }
     fn repr_hash(&self) -> BigUint {
         let hash = self.cell.repr_hash();
         BigUint::from_bytes_be(hash.as_slice())
     }
-    fn __len__(&self) -> PyResult<usize> {
+    fn cells_count(&self) -> PyResult<usize> {
         self.cell.count_cells(usize::MAX).map_err(runtime_err)
     }
+    fn unique_cells_count(&self) -> PyResult<usize> {
+        let mut set = HashSet::new();
+        let mut stack = Vec::new();
+        let mut unique_count = 0;
+        stack.push(self.cell.clone());
+        while let Some(cell) = stack.pop() {
+            if set.insert(cell.repr_hash()) {
+                unique_count += 1;
+                for i in 0..cell.references_count() {
+                    stack.push(cell.reference(i).unwrap())
+                }
+            }
+        }
+        Ok(unique_count)
+    }
+    fn __len__(&self) -> PyResult<usize> {
+        self.cells_count()
+    }
     fn __str__(&self) -> PyResult<String> {
         PyResult::Ok(dump_cell(self.cell.clone()))
     }
     fn __bytes__<'a>(&'a self, py: Python<'a>) -> PyResult<&PyBytes> {
         self.write(py, 0)
     }
     fn __richcmp__(&self, other: Self, op: CompareOp, py: Python<'_>) -> PyObject {
@@ -403,15 +421,15 @@
 }
 
 fn trace_callback(_engine: &Engine, info: &EngineTraceInfo) {
     use ton_vm::executor::EngineTraceInfoType::*;
     match info.info_type {
         Start => { }
         Dump =>  println!("DUMP {}", info.cmd_str),
-        Exception => println!("EXCEPTION"),
+        //Exception => println!("EXCEPTION"),
         _ => {
             println!("STEP {} {}", info.step, info.cmd_str);
             println!("GAS {} in total, {} by insn", info.gas_used, info.gas_cmd);
             if info.stack.is_empty() {
                 println!("STACK <empty>")
             } else {
                 for item in info.stack.iter() {
```

### Comparing `ever_playground-0.6.2/src/tests.rs` & `ever_playground-0.6.3/src/tests.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #![cfg(test)]
 
 use crate::{InternalCell, dump_cell};
-use ton_types::{BuilderData, SliceData};
+use ton_types::SliceData;
 
 fn __(data: &str, refs: Vec<InternalCell>) -> ton_types::Result<InternalCell> {
-    let s = SliceData::from_string(data)?;
-    let mut b = BuilderData::from_slice(&s);
+    let mut b = SliceData::from_string(data)?.as_builder();
     for r in refs {
         b.checked_append_reference(r)?;
     }
     b.into_cell()
 }
 
 macro_rules! __ {
```

### Comparing `ever_playground-0.6.2/src/utils.rs` & `ever_playground-0.6.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.2/Cargo.lock` & `ever_playground-0.6.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -190,17 +190,17 @@
 checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer 0.10.4",
  "crypto-common",
 ]
 
 [[package]]
 name = "ed25519"
@@ -223,15 +223,15 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.6.2"
+version = "0.6.3"
 dependencies = [
  "ed25519-dalek",
  "num-bigint",
  "pyo3",
  "rand",
  "ton_block",
  "ton_labs_assembler",
@@ -510,17 +510,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -580,17 +580,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -657,30 +657,30 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.17",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -707,15 +707,15 @@
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
- "digest 0.10.6",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "signature"
 version = "1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
@@ -741,17 +741,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "45b6ddbb36c5b969c182aec3c4a0bce7df3fbad4b77114706a49aacc80567388"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -770,16 +770,16 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "ton_block"
-version = "1.9.61"
-source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.61#3870fa91ec28902eaf10795a9cc08ca08465578e"
+version = "1.9.72"
+source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.72#9350ea08938d8ff5d4490defe78446d6de08ed7e"
 dependencies = [
  "base64",
  "crc",
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
@@ -788,31 +788,31 @@
  "num-traits",
  "sha2 0.10.6",
  "ton_types",
 ]
 
 [[package]]
 name = "ton_labs_assembler"
-version = "1.2.111"
-source = "git+https://github.com/tonlabs/ever-assembler?tag=1.2.111#c7febf00f6e77a2e77984ee6f9ebaac40cefeaef"
+version = "1.2.120"
+source = "git+https://github.com/tonlabs/ever-assembler?tag=1.2.120#7e6a005463cf601188a66aec3c7cd825a90a32c1"
 dependencies = [
  "failure",
  "hex",
  "log",
  "num",
  "num-traits",
  "serde",
  "serde_json",
  "ton_types",
 ]
 
 [[package]]
 name = "ton_types"
-version = "2.0.7"
-source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.7#5815cc3cb53f7dc3cf91a32616159c595f81d0ff"
+version = "2.0.13"
+source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.13#c1dfeb2596b8226c0ef6e56ff4ff9b7d0d98aeae"
 dependencies = [
  "aes-ctr",
  "base64",
  "crc",
  "curve25519-dalek",
  "ed25519",
  "ed25519-dalek",
@@ -830,42 +830,41 @@
  "sha2 0.10.6",
  "smallvec",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "ton_vm"
-version = "1.8.149"
-source = "git+https://github.com/tonlabs/ever-vm.git?tag=1.8.149#e867fffddd6aecd2d7f846cdf6e19dcb09f80778"
+version = "1.8.164"
+source = "git+https://github.com/tonlabs/ever-vm.git?tag=1.8.164#3e32cbfa36fd4e5ce0a059b24b023aa62caee84b"
 dependencies = [
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
  "lazy_static",
  "log",
  "num",
  "num-traits",
  "rand",
- "sha2 0.10.6",
  "ton_block",
  "ton_types",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
@@ -977,9 +976,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.17",
 ]
```

### Comparing `ever_playground-0.6.2/PKG-INFO` & `ever_playground-0.6.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.6.2
+Version: 0.6.3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

