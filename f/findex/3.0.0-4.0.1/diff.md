# Comparing `tmp/findex-3.0.0-cp37-abi3-win_amd64.whl.zip` & `tmp/findex-4.0.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1803174 bytes, number of entries: 7
--rw-r--r--  4.6 unx      462 b- defN 23-Mar-07 16:55 findex-3.0.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Mar-07 16:55 findex-3.0.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       27 b- defN 23-Mar-07 16:55 cloudproof_findex/py.typed
--rw-r--r--  4.6 unx      462 b- defN 23-Mar-07 16:55 cloudproof_findex/__init__.py
--rw-r--r--  4.6 unx     6976 b- defN 23-Mar-07 16:55 cloudproof_findex/__init__.pyi
--rwxr-xr-x  4.6 unx  3542016 b- defN 23-Mar-07 16:55 cloudproof_findex/cloudproof_findex.pyd
--rw-r--r--  4.6 unx      554 b- defN 23-Mar-07 16:55 findex-3.0.0.dist-info/RECORD
-7 files, 3550593 bytes uncompressed, 1802196 bytes compressed:  49.3%
+Zip file size: 1855146 bytes, number of entries: 7
+-rw-r--r--  4.6 unx      462 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     6630 b- defN 23-Jun-05 10:00 cloudproof_findex/__init__.pyi
+-rw-r--r--  4.6 unx       27 b- defN 23-Jun-05 10:00 cloudproof_findex/py.typed
+-rw-r--r--  4.6 unx      462 b- defN 23-Jun-05 10:00 cloudproof_findex/__init__.py
+-rwxr-xr-x  4.6 unx  3670528 b- defN 23-Jun-05 10:00 cloudproof_findex/cloudproof_findex.pyd
+-rw-r--r--  4.6 unx      554 b- defN 23-Jun-05 10:00 findex-4.0.1.dist-info/RECORD
+7 files, 3678757 bytes uncompressed, 1854168 bytes compressed:  49.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: findex-3.0.0.dist-info/METADATA
+Filename: findex-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: findex-3.0.0.dist-info/WHEEL
+Filename: findex-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: cloudproof_findex/py.typed
+Filename: cloudproof_findex/__init__.pyi
 Comment: 
 
-Filename: cloudproof_findex/__init__.py
+Filename: cloudproof_findex/py.typed
 Comment: 
 
-Filename: cloudproof_findex/__init__.pyi
+Filename: cloudproof_findex/__init__.py
 Comment: 
 
 Filename: cloudproof_findex/cloudproof_findex.pyd
 Comment: 
 
-Filename: findex-3.0.0.dist-info/RECORD
+Filename: findex-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudproof_findex/__init__.pyi

```diff
@@ -173,47 +173,44 @@
         """
 
 class FindexCloud:
     """Ready to use Findex with a backend powered by Cosmian."""
 
     @staticmethod
     def upsert(
-        indexed_values_and_keywords: IndexedValuesAndKeywords,
         token: str,
         label: Label,
+        additions: IndexedValuesAndKeywords,
+        deletions: IndexedValuesAndKeywords,
         base_url: Optional[str] = None,
     ) -> None:
         """Upserts the given relations between `IndexedValue` and `Keyword` into Findex tables.
 
         Args:
-            indexed_values_and_keywords (Dict[Location | Keyword, List[Keyword | str]]):
-                map of `IndexedValue` to a list of `Keyword`.
             token (str): Findex token.
             label (Label): label used to allow versioning.
+            additions (Dict[Location | Keyword, List[Keyword | str]]):
+                map of `IndexedValue` to a list of `Keyword`.
+            deletions (Dict[Location | Keyword, List[Keyword | str]]):
+                map of `IndexedValue` to a list of `Keyword`.
             base_url (str, optional): url of Findex backend.
         """
     @staticmethod
     def search(
-        keywords: Sequence[Union[Keyword, str]],
         token: str,
         label: Label,
-        max_result_per_keyword: int = 2**32 - 1,
-        max_depth: int = 100,
-        fetch_chains_batch_size: int = 0,
+        keywords: Sequence[Union[Keyword, str]],
         base_url: Optional[str] = None,
     ) -> SearchResults:
         """Recursively search Findex graphs for `Locations` corresponding to the given `Keyword`.
 
         Args:
-            keywords (List[Keyword | str]): keywords to search using Findex.
             token (str): Findex token.
             label (Label): public label used in keyword hashing.
-            max_result_per_keyword (int, optional): maximum number of results to fetch per keyword.
-            max_depth (int, optional): maximum recursion level allowed. Defaults to 100.
-            fetch_chains_batch_size (int, optional): batch size during fetch chain.
+            keywords (List[Keyword | str]): keywords to search using Findex.
             base_url (str, optional): url of Findex backend.
 
         Returns:
             Dict[Keyword, List[Location]]: `Locations` found by `Keyword`
         """
     @staticmethod
     def derive_new_token(token: str, search: bool, index: bool) -> str: ...
@@ -246,28 +243,26 @@
         fetch_chain_table: Callable,
         update_lines: Callable,
         list_removed_locations: Callable,
         fetch_all_entry_table_uids: Callable,
     ) -> None: ...
     def upsert_wrapper(
         self,
-        indexed_values_and_keywords: IndexedValuesAndKeywords,
         master_key: MasterKey,
         label: Label,
+        additions: IndexedValuesAndKeywords,
+        deletions: IndexedValuesAndKeywords,
     ) -> None: ...
     def search_wrapper(
         self,
-        keywords: Sequence[Union[Keyword, str]],
         msk: MasterKey,
         label: Label,
-        max_result_per_keyword: int = 2**32 - 1,
-        max_depth: int = 100,
-        fetch_chains_batch_size: int = 0,
+        keywords: Sequence[Union[Keyword, str]],
         progress_callback: Optional[Callable] = None,
     ) -> SearchResults: ...
     def compact_wrapper(
         self,
-        num_reindexing_before_full_set: int,
         master_key: MasterKey,
         new_master_key: MasterKey,
         new_label: Label,
+        num_reindexing_before_full_set: int,
     ) -> None: ...
```

