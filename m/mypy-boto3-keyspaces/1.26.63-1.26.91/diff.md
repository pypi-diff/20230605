# Comparing `tmp/mypy-boto3-keyspaces-1.26.63.tar.gz` & `tmp/mypy-boto3-keyspaces-1.26.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-keyspaces-1.26.63.tar", last modified: Thu Feb  2 20:49:28 2023, max compression
+gzip compressed data, was "mypy-boto3-keyspaces-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
```

## Comparing `mypy-boto3-keyspaces-1.26.63.tar` & `mypy-boto3-keyspaces-1.26.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.110372 mypy-boto3-keyspaces-1.26.63/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-02-02 20:49:28.110372 mypy-boto3-keyspaces-1.26.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.110372 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.110372 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-02 20:49:27.000000 mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 20:49:28.110372 mypy-boto3-keyspaces-1.26.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-02 20:47:48.000000 mypy-boto3-keyspaces-1.26.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-03-14 19:47:50.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 19:48:00.000000 mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.357219 mypy-boto3-keyspaces-1.26.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-14 19:47:49.000000 mypy-boto3-keyspaces-1.26.91/setup.py
```

### Comparing `mypy-boto3-keyspaces-1.26.63/LICENSE` & `mypy-boto3-keyspaces-1.26.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/PKG-INFO` & `mypy-boto3-keyspaces-1.26.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.26.63
-Summary: Type annotations for boto3.Keyspaces 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.91
+Summary: Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,14 +304,15 @@
 ### Literals
 
 `mypy_boto3_keyspaces.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_keyspaces.literals import (
+    ClientSideTimestampsStatusType,
     EncryptionTypeType,
     ListKeyspacesPaginatorName,
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
@@ -321,29 +322,30 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: EncryptionTypeType) -> bool:
+def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
```

### Comparing `mypy-boto3-keyspaces-1.26.63/README.md` & `mypy-boto3-keyspaces-1.26.91/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,14 +272,15 @@
 ### Literals
 
 `mypy_boto3_keyspaces.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_keyspaces.literals import (
+    ClientSideTimestampsStatusType,
     EncryptionTypeType,
     ListKeyspacesPaginatorName,
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
@@ -289,29 +290,30 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: EncryptionTypeType) -> bool:
+def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__init__.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__init__.pyi` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/__main__.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Keyspaces 1.26.63\nVersion:         1.26.63\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Keyspaces 1.26.91\nVersion:         1.26.91\nBuilder version:"
+        " 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.63")
+    print("1.26.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/client.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListKeyspacesPaginator, ListTablesPaginator, ListTagsForResourcePaginator
 from .type_defs import (
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
     CreateKeyspaceResponseTypeDef,
     CreateTableResponseTypeDef,
     EncryptionSpecificationTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableResponseTypeDef,
@@ -118,15 +119,16 @@
         schemaDefinition: SchemaDefinitionTypeDef,
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         The `CreateTable` operation adds a new table to the specified keyspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#create_table)
         """
@@ -252,15 +254,16 @@
         keyspaceName: str,
         tableName: str,
         addColumns: Sequence[ColumnDefinitionTypeDef] = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
-        defaultTimeToLive: int = ...
+        defaultTimeToLive: int = ...,
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Adds new columns to the table or updates one of the table's settings, for
         example capacity mode, encryption, point-in-time recovery, or ttl settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#update_table)
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/client.pyi` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListKeyspacesPaginator, ListTablesPaginator, ListTagsForResourcePaginator
 from .type_defs import (
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
     CreateKeyspaceResponseTypeDef,
     CreateTableResponseTypeDef,
     EncryptionSpecificationTypeDef,
     GetKeyspaceResponseTypeDef,
     GetTableResponseTypeDef,
@@ -110,15 +111,16 @@
         schemaDefinition: SchemaDefinitionTypeDef,
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         The `CreateTable` operation adds a new table to the specified keyspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#create_table)
         """
@@ -232,15 +234,16 @@
         keyspaceName: str,
         tableName: str,
         addColumns: Sequence[ColumnDefinitionTypeDef] = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
-        defaultTimeToLive: int = ...
+        defaultTimeToLive: int = ...,
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Adds new columns to the table or updates one of the table's settings, for
         example capacity mode, encryption, point-in-time recovery, or ttl settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/client/#update_table)
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/literals.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for keyspaces service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_keyspaces.literals import EncryptionTypeType
+    from mypy_boto3_keyspaces.literals import ClientSideTimestampsStatusType
 
-    data: EncryptionTypeType = "AWS_OWNED_KMS_KEY"
+    data: ClientSideTimestampsStatusType = "ENABLED"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ClientSideTimestampsStatusType",
     "EncryptionTypeType",
     "ListKeyspacesPaginatorName",
     "ListTablesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "PointInTimeRecoveryStatusType",
     "SortOrderType",
     "TableStatusType",
@@ -33,14 +34,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+ClientSideTimestampsStatusType = Literal["ENABLED"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 ListKeyspacesPaginatorName = Literal["list_keyspaces"]
 ListTablesPaginatorName = Literal["list_tables"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 PointInTimeRecoveryStatusType = Literal["DISABLED", "ENABLED"]
 SortOrderType = Literal["ASC", "DESC"]
 TableStatusType = Literal[
@@ -199,14 +201,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -375,14 +378,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/literals.pyi` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 Type annotations for keyspaces service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_keyspaces.literals import EncryptionTypeType
+    from mypy_boto3_keyspaces.literals import ClientSideTimestampsStatusType
 
-    data: EncryptionTypeType = "AWS_OWNED_KMS_KEY"
+    data: ClientSideTimestampsStatusType = "ENABLED"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ClientSideTimestampsStatusType",
     "EncryptionTypeType",
     "ListKeyspacesPaginatorName",
     "ListTablesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "PointInTimeRecoveryStatusType",
     "SortOrderType",
     "TableStatusType",
@@ -31,14 +32,15 @@
     "KeyspacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+ClientSideTimestampsStatusType = Literal["ENABLED"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 ListKeyspacesPaginatorName = Literal["list_keyspaces"]
 ListTablesPaginatorName = Literal["list_tables"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 PointInTimeRecoveryStatusType = Literal["DISABLED", "ENABLED"]
 SortOrderType = Literal["ASC", "DESC"]
 TableStatusType = Literal[
@@ -197,14 +199,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -373,14 +376,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/paginator.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/paginator.pyi` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/type_defs.py` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
+    "ClientSideTimestampsTypeDef",
     "ClusteringKeyTypeDef",
     "ColumnDefinitionTypeDef",
     "CommentTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
@@ -119,14 +120,21 @@
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
 
+ClientSideTimestampsTypeDef = TypedDict(
+    "ClientSideTimestampsTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
@@ -473,14 +481,15 @@
     {
         "addColumns": Sequence[ColumnDefinitionTypeDef],
         "capacitySpecification": CapacitySpecificationTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoveryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
     },
     total=False,
 )
 
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
@@ -593,14 +602,15 @@
         "comment": CommentTypeDef,
         "capacitySpecification": CapacitySpecificationTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoveryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "tags": Sequence[TagTypeDef],
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
     },
     total=False,
 )
 
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
@@ -619,10 +629,11 @@
         "schemaDefinition": SchemaDefinitionTypeDef,
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "comment": CommentTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces/type_defs.pyi` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
+    "ClientSideTimestampsTypeDef",
     "ClusteringKeyTypeDef",
     "ColumnDefinitionTypeDef",
     "CommentTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
@@ -114,14 +115,21 @@
 )
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
+ClientSideTimestampsTypeDef = TypedDict(
+    "ClientSideTimestampsTypeDef",
+    {
+        "status": Literal["ENABLED"],
+    },
+)
+
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
@@ -456,14 +464,15 @@
     {
         "addColumns": Sequence[ColumnDefinitionTypeDef],
         "capacitySpecification": CapacitySpecificationTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoveryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
     },
     total=False,
 )
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
@@ -568,14 +577,15 @@
         "comment": CommentTypeDef,
         "capacitySpecification": CapacitySpecificationTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoveryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "tags": Sequence[TagTypeDef],
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
     },
     total=False,
 )
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
@@ -592,10 +602,11 @@
         "schemaDefinition": SchemaDefinitionTypeDef,
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
         "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
         "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
         "comment": CommentTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/PKG-INFO` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.26.63
-Summary: Type annotations for boto3.Keyspaces 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.91
+Summary: Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-keyspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,14 +304,15 @@
 ### Literals
 
 `mypy_boto3_keyspaces.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_keyspaces.literals import (
+    ClientSideTimestampsStatusType,
     EncryptionTypeType,
     ListKeyspacesPaginatorName,
     ListTablesPaginatorName,
     ListTagsForResourcePaginatorName,
     PointInTimeRecoveryStatusType,
     SortOrderType,
     TableStatusType,
@@ -321,29 +322,30 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: EncryptionTypeType) -> bool:
+def check_value(value: ClientSideTimestampsStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
+    ClientSideTimestampsTypeDef,
     ClusteringKeyTypeDef,
     ColumnDefinitionTypeDef,
     CommentTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
```

### Comparing `mypy-boto3-keyspaces-1.26.63/mypy_boto3_keyspaces.egg-info/SOURCES.txt` & `mypy-boto3-keyspaces-1.26.91/mypy_boto3_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.26.63/setup.py` & `mypy-boto3-keyspaces-1.26.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-keyspaces",
-    version="1.26.63",
+    version="1.26.91",
     packages=["mypy_boto3_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Keyspaces 1.26.63 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Keyspaces 1.26.91 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

