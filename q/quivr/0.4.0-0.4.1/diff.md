# Comparing `tmp/quivr-0.4.0.tar.gz` & `tmp/quivr-0.4.1.tar.gz`

## Comparing `quivr-0.4.0.tar` & `quivr-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/__version__.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/attributes.py
--rw-r--r--   0        0        0    26085 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/columns.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/errors.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/streaming.py
--rw-r--r--   0        0        0    27596 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.0/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.0/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/__version__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/attributes.py
+-rw-r--r--   0        0        0    27573 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/columns.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/errors.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/schemagraph.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/streaming.py
+-rw-r--r--   0        0        0    27596 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/tables.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.1/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.1/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.1/README.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.1/PKG-INFO
```

### Comparing `quivr-0.4.0/quivr/__init__.py` & `quivr-0.4.1/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/attributes.py` & `quivr-0.4.1/quivr/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     """
 
     def __init__(self, default: Any = None):
         self.default = default
         self.name = "__ERR_UNSET_NAME"
 
     def __get__(self, instance: "Table", owner):
+        if instance is None:
+            return self
         if instance.table.schema.metadata is None:
             return self.default
         name = self.name.encode("utf8")
         if name not in instance.table.schema.metadata:
             return self.default
         raw = instance.table.schema.metadata[name]
         return self.from_bytes(raw)
```

### Comparing `quivr-0.4.0/quivr/columns.py` & `quivr-0.4.1/quivr/columns.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     ):
         self.dtype = dtype
         self.nullable = nullable
         self.metadata = metadata
         self.validator = validator
 
     def __get__(self, obj: "Table", objtype: type):
+        if obj is None:
+            return self
         return obj.table.column(self.name)
 
     def __set__(self, obj: "Table", value):
         idx = obj.table.schema.get_field_index(self.name)
         obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value])
 
     def __set_name__(self, owner: type, name: str):
@@ -59,14 +61,16 @@
     def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> T:
+        if obj is None:
+            return self
         array = obj.table.column(self.name)
 
         metadata = self.metadata
         if metadata is None:
             metadata = {}
         metadata.update(obj._metadata_for_column(self.name))
 
@@ -86,14 +90,16 @@
         nullable: bool = True,
         validator: Optional[validators.Validator] = None,
         metadata: Optional[MetadataDict] = None,
     ):
         super().__init__(pa.int8(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int8Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int16Column(Column):
     """
     A column for storing 16-bit integers.
     """
@@ -103,92 +109,106 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int16Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int32Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int64Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt8Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint8(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt8Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt16Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt16Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt32Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt64Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float16Column(Column):
     """
     A column for storing 16-bit floating point numbers.
     """
@@ -198,14 +218,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.HalfFloatArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float32Column(Column):
     """
     A column for storing 32-bit floating point numbers.
     """
@@ -215,14 +237,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.FloatArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float64Column(Column):
     """
     A column for storing 64-bit floating point numbers.
     """
@@ -232,14 +256,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.DoubleArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class StringColumn(Column):
     """A column for storing strings.
 
     This can be used to store strings of any length, but it is not
@@ -253,14 +279,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.string(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.StringArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeBinaryColumn(Column):
     """
     A column for storing large binary objects. Large binary data is stored in
     variable-length chunks.
@@ -271,14 +299,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeBinaryArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeStringColumn(Column):
     """
     A column for storing large strings. Large string data is stored in
     variable-length chunks.
@@ -289,14 +319,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.large_string(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeStringArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date32Column(Column):
     """A column for storing dates.
 
     Internally, this column stores dates as 32-bit integers which
@@ -309,14 +341,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Date32Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date64Column(Column):
     """A column for storing dates.
 
     Internally, this column stores dates as 64-bit integers which
@@ -329,14 +363,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Date64Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class TimestampColumn(Column):
     """A column for storing timestamps.
 
     Timestamp data can be stored in one of four units:
@@ -360,14 +396,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.TimestampArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time32Column(Column):
     """
     A column for storing time values.
 
@@ -384,14 +422,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Time32Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time64Column(Column):
     """
     A column for storing time values with high precision.
 
@@ -408,14 +448,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Time64Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class DurationColumn(Column):
     """
     An absolute length of time unrelated to any calendar artifacts.
 
@@ -432,14 +474,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.DurationArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class MonthDayNanoIntervalColumn(Column):
     """A column for storing calendar intervals (an elapsed number of months,
     days, and nanoseconds).
 
@@ -458,14 +502,16 @@
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(
             pa.month_day_nano_interval(), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.MonthDayNanoIntervalArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class BinaryColumn(Column):
     """A column for storing opaque binary data.
 
     The data can be either variable-length or fixed-length, depending
@@ -483,14 +529,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.binary(length), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.BinaryArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal128Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
@@ -514,14 +562,16 @@
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal128(precision, scale), nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal128Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal256Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
@@ -534,14 +584,16 @@
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal256(precision, scale), nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal256Array:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class NullColumn(Column):
     """A column for storing null values.
 
     Nulls are represented as a single bit, and do not take up any
@@ -554,14 +606,16 @@
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.null(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.NullArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 # Complex types follow
 
 
 class ListColumn(Column):
@@ -605,14 +659,16 @@
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.list_(value_type, list_size), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.ListArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeListColumn(Column):
     """A column for storing large lists of values.
 
     Unless you need to represent data with more than 2**31 elements,
@@ -647,14 +703,16 @@
             A validator to run against the column's values.
         """
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeListArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class MapColumn(Column):
     """A column for storing maps of key-value pairs.
 
     The keys and values can be of any type, as long as the keys are
@@ -692,14 +750,16 @@
         if isinstance(item_type, Column):
             item_type = item_type.dtype
         super().__init__(
             pa.map_(key_type, item_type), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.MapArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class DictionaryColumn(Column):
     """A column for storing dictionary-encoded values.
 
     This is intended for use with categorical data. See MapColumn for a
@@ -744,14 +804,16 @@
             pa.dictionary(index_type, value_type, ordered=ordered),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.DictionaryArray:
+        if obj is None:
+            return self
         return obj.table[self.name].combine_chunks()
 
 
 class StructColumn(Column):
     """A column for storing structured data.
 
     In general, prefer to define Tables and use their as_column method
```

### Comparing `quivr-0.4.0/quivr/concat.py` & `quivr-0.4.1/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/indexing.py` & `quivr-0.4.1/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/matrix.py` & `quivr-0.4.1/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/schemagraph.py` & `quivr-0.4.1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/tables.py` & `quivr-0.4.1/quivr/tables.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/quivr/validators.py` & `quivr-0.4.1/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/LICENSE` & `quivr-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/README.md` & `quivr-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/pyproject.toml` & `quivr-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.4.0/PKG-INFO` & `quivr-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.4.0
+Version: 0.4.1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

