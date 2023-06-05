# Comparing `tmp/quivr-0.3.4.tar.gz` & `tmp/quivr-0.4.0.tar.gz`

## Comparing `quivr-0.3.4.tar` & `quivr-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/__version__.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/attributes.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/errors.py
--rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/fields.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/streaming.py
--rw-r--r--   0        0        0    27561 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.3.4/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.3.4/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.3.4/LICENSE
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 quivr-0.3.4/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 quivr-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/__version__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/attributes.py
+-rw-r--r--   0        0        0    26085 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/columns.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/errors.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/indexing.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/py.typed
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/schemagraph.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/streaming.py
+-rw-r--r--   0        0        0    27596 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/tables.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.0/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.0/README.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.0/PKG-INFO
```

### Comparing `quivr-0.3.4/quivr/attributes.py` & `quivr-0.4.0/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/quivr/concat.py` & `quivr-0.4.0/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/quivr/fields.py` & `quivr-0.4.0/quivr/columns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Union
 
 import pyarrow as pa
@@ -12,17 +13,17 @@
 if TYPE_CHECKING:
     from .tables import Table
 
 Byteslike: TypeAlias = Union[bytes, bytearray, memoryview, str]
 MetadataDict: TypeAlias = dict[Byteslike, Byteslike]
 
 
-class Field:
+class Column:
     """
-    A Field is an accessor for data in a Table, and also a descriptor for the Table's structure.
+    A Column is an accessor for data in a Table, and also a descriptor for the Table's structure.
     """
 
     def __init__(
         self,
         dtype: pa.DataType,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -46,208 +47,208 @@
     def pyarrow_field(self):
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
 
 
 T = TypeVar("T", bound="Table")
 
 
-class SubTableField(Field, Generic[T]):
+class SubTableColumn(Column, Generic[T]):
     """
-    A field which represents an embedded Quivr table.
+    A column which represents an embedded Quivr table.
     """
 
     def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> T:
         array = obj.table.column(self.name)
 
         metadata = self.metadata
         if metadata is None:
             metadata = {}
-        metadata.update(obj._metadata_for_field(self.name))
+        metadata.update(obj._metadata_for_column(self.name))
 
         schema = self.schema.with_metadata(metadata)
 
         subtable = pa.Table.from_arrays(array.flatten(), schema=schema)
         return self.table_type(subtable)
 
 
-class Int8Field(Field):
+class Int8Column(Column):
     """
-    A field for storing 8-bit integers.
+    A column for storing 8-bit integers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         validator: Optional[validators.Validator] = None,
         metadata: Optional[MetadataDict] = None,
     ):
         super().__init__(pa.int8(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int8Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Int16Field(Field):
+class Int16Column(Column):
     """
-    A field for storing 16-bit integers.
+    A column for storing 16-bit integers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int16Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Int32Field(Field):
+class Int32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int32Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Int64Field(Field):
+class Int64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Int64Array:
         return obj.table[self.name].combine_chunks()
 
 
-class UInt8Field(Field):
+class UInt8Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint8(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt8Array:
         return obj.table[self.name].combine_chunks()
 
 
-class UInt16Field(Field):
+class UInt16Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt16Array:
         return obj.table[self.name].combine_chunks()
 
 
-class UInt32Field(Field):
+class UInt32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt32Array:
         return obj.table[self.name].combine_chunks()
 
 
-class UInt64Field(Field):
+class UInt64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt64Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Float16Field(Field):
+class Float16Column(Column):
     """
-    A field for storing 16-bit floating point numbers.
+    A column for storing 16-bit floating point numbers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.HalfFloatArray:
         return obj.table[self.name].combine_chunks()
 
 
-class Float32Field(Field):
+class Float32Column(Column):
     """
-    A field for storing 32-bit floating point numbers.
+    A column for storing 32-bit floating point numbers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.FloatArray:
         return obj.table[self.name].combine_chunks()
 
 
-class Float64Field(Field):
+class Float64Column(Column):
     """
-    A field for storing 64-bit floating point numbers.
+    A column for storing 64-bit floating point numbers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.DoubleArray:
         return obj.table[self.name].combine_chunks()
 
 
-class StringField(Field):
-    """A field for storing strings.
+class StringColumn(Column):
+    """A column for storing strings.
 
     This can be used to store strings of any length, but it is not
     recommended for storing very long strings (over 2GB, for
-    example). For long strings, use LargeStringField instead.
+    example). For long strings, use LargeStringColumn instead.
 
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -255,17 +256,17 @@
     ):
         super().__init__(pa.string(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.StringArray:
         return obj.table[self.name].combine_chunks()
 
 
-class LargeBinaryField(Field):
+class LargeBinaryColumn(Column):
     """
-    A field for storing large binary objects. Large binary data is stored in
+    A column for storing large binary objects. Large binary data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -273,17 +274,17 @@
     ):
         super().__init__(pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeBinaryArray:
         return obj.table[self.name].combine_chunks()
 
 
-class LargeStringField(Field):
+class LargeStringColumn(Column):
     """
-    A field for storing large strings. Large string data is stored in
+    A column for storing large strings. Large string data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -291,18 +292,18 @@
     ):
         super().__init__(pa.large_string(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeStringArray:
         return obj.table[self.name].combine_chunks()
 
 
-class Date32Field(Field):
-    """A field for storing dates.
+class Date32Column(Column):
+    """A column for storing dates.
 
-    Internally, this field stores dates as 32-bit integers which
+    Internally, this column stores dates as 32-bit integers which
     represent time since the UNIX epoch.
 
     """
 
     def __init__(
         self,
         nullable: bool = True,
@@ -311,18 +312,18 @@
     ):
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Date32Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Date64Field(Field):
-    """A field for storing dates.
+class Date64Column(Column):
+    """A column for storing dates.
 
-    Internally, this field stores dates as 64-bit integers which
+    Internally, this column stores dates as 64-bit integers which
     represent time since the UNIX epoch in milliseconds, where the
     values are evenly divisible by 86,400,000.
     """
 
     def __init__(
         self,
         nullable: bool = True,
@@ -331,16 +332,16 @@
     ):
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Date64Array:
         return obj.table[self.name].combine_chunks()
 
 
-class TimestampField(Field):
-    """A field for storing timestamps.
+class TimestampColumn(Column):
+    """A column for storing timestamps.
 
     Timestamp data can be stored in one of four units:
       - seconds
       - milliseconds
       - microseconds
       - nanoseconds
 
@@ -362,17 +363,17 @@
     ):
         super().__init__(pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.TimestampArray:
         return obj.table[self.name].combine_chunks()
 
 
-class Time32Field(Field):
+class Time32Column(Column):
     """
-    A field for storing time values.
+    A column for storing time values.
 
     Time data can be stored in one of two units for this 32-bit type:
         - seconds
         - milliseconds
 
     Internally, a time32 value is a 32-bit integer which an elapsed time since midnight.
     """
@@ -386,17 +387,17 @@
     ):
         super().__init__(pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Time32Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Time64Field(Field):
+class Time64Column(Column):
     """
-    A field for storing time values with high precision.
+    A column for storing time values with high precision.
 
     Time data can be stored in one of two units for this 64-bit type:
         - microseconds
         - nanoseconds
 
     Internally, a time64 value is a 64-bit integer which an elapsed time since midnight.
     """
@@ -410,15 +411,15 @@
     ):
         super().__init__(pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Time64Array:
         return obj.table[self.name].combine_chunks()
 
 
-class DurationField(Field):
+class DurationColumn(Column):
     """
     An absolute length of time unrelated to any calendar artifacts.
 
     The resolution defaults to millisecond, but can be any of the other
     supported time unit values (seconds, milliseconds, microseconds,
     nanoseconds).
 
@@ -434,16 +435,16 @@
     ):
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.DurationArray:
         return obj.table[self.name].combine_chunks()
 
 
-class MonthDayNanoIntervalField(Field):
-    """A field for storing calendar intervals (an elapsed number of months,
+class MonthDayNanoIntervalColumn(Column):
+    """A column for storing calendar intervals (an elapsed number of months,
     days, and nanoseconds).
 
     Internally, a month_day_nano_interval value is a 96-bit
     integer. 32 bits are devoted to months and days, and 64 bits are
     devoted to nanoseconds.
 
     Leap seconds are ignored.
@@ -460,16 +461,16 @@
             pa.month_day_nano_interval(), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.MonthDayNanoIntervalArray:
         return obj.table[self.name].combine_chunks()
 
 
-class BinaryField(Field):
-    """A field for storing opaque binary data.
+class BinaryColumn(Column):
+    """A column for storing opaque binary data.
 
     The data can be either variable-length or fixed-length, depending
     on the 'length' parameter passed in the initializer.
 
     If length is -1 (the default) then the data is variable-length. If
     length is greater than or equal to 0, then the data is
     fixed-length.
@@ -485,47 +486,47 @@
     ):
         super().__init__(pa.binary(length), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.BinaryArray:
         return obj.table[self.name].combine_chunks()
 
 
-class Decimal128Field(Field):
-    """A field for storing arbitrary-precision decimal numbers.
+class Decimal128Column(Column):
+    """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
     integer. The precision is the number of significant digits that the
     decimal type can represent; the scale is the number of digits after
     the decimal point (note the scale can be negative).
 
-    As an example, Decimal128Field(7, 3) can exactly represent the numbers
+    As an example, Decimal128Column(7, 3) can exactly represent the numbers
     1234.567 and -1234.567 (encoded internally as the 128-bit integers
     1234567 and -1234567, respectively), but neither 12345.67 nor
     123.4567.
 
-    DecimalField(5, -3) can exactly represent the number 12345000
+    DecimalColumn(5, -3) can exactly represent the number 12345000
     (encoded internally as the 128-bit integer 12345), but neither
     123450000 nor 1234500.
 
     If you need a precision higher than 38 significant digits,
-    consider using Decimal256Field.
+    consider using Decimal256Column.
 
     """
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal128(precision, scale), nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal128Array:
         return obj.table[self.name].combine_chunks()
 
 
-class Decimal256Field(Field):
-    """A field for storing arbitrary-precision decimal numbers.
+class Decimal256Column(Column):
+    """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
     integer. The precision is the number of significant digits that the
     decimal type can represent; the scale is the number of digits after
     the decimal point (note the scale can be negative).
 
     Values are stored as 256-bit integers.
@@ -536,16 +537,16 @@
     ):
         super().__init__(pa.decimal256(precision, scale), nullable=nullable, metadata=metadata)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal256Array:
         return obj.table[self.name].combine_chunks()
 
 
-class NullField(Field):
-    """A field for storing null values.
+class NullColumn(Column):
+    """A column for storing null values.
 
     Nulls are represented as a single bit, and do not take up any
     memory space.
 
     """
 
     def __init__(
@@ -559,206 +560,206 @@
     def __get__(self, obj: "Table", objtype: type) -> pa.NullArray:
         return obj.table[self.name].combine_chunks()
 
 
 # Complex types follow
 
 
-class ListField(Field):
-    """A field for storing lists of values.
+class ListColumn(Column):
+    """A column for storing lists of values.
 
     The values in the list can be of any type.
 
     Note that all quivr Tables are storing lists of values, so this
-    field type is only useful for storing lists of lists.
+    column type is only useful for storing lists of lists.
 
 
 
     """
 
     def __init__(
         self,
-        value_type: Union[pa.DataType, pa.Field, Field],
+        value_type: Union[pa.DataType, pa.Field, Column],
         list_size: int = -1,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         """
         Parameters
         ----------
-        value_type : Union[pa.DataType, pa.Field, Field]
+        value_type : Union[pa.DataType, pa.Field, Column]
             The type of the values in the list.
 
         list_size : int
             The size of the list. If -1, then the list is variable-length.
 
         nullable : bool
             Whether the list can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
-        if isinstance(value_type, Field):
+        if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.list_(value_type, list_size), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.ListArray:
         return obj.table[self.name].combine_chunks()
 
 
-class LargeListField(Field):
-    """A field for storing large lists of values.
+class LargeListColumn(Column):
+    """A column for storing large lists of values.
 
     Unless you need to represent data with more than 2**31 elements,
-    prefer ListField.
+    prefer ListColumn.
 
     The values in the list can be of any type.
 
     Note that all quivr Tables are storing lists of values, so this
-    field type is only useful for storing lists of lists.
+    column type is only useful for storing lists of lists.
     """
 
     def __init__(
         self,
-        value_type: Union[pa.DataType, pa.Field, Field],
+        value_type: Union[pa.DataType, pa.Field, Column],
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         """
         Parameters
         ----------
-        value_type : Union[pa.DataType, pa.Field, Field]
+        value_type : Union[pa.DataType, pa.Field, Column]
             The type of the values in the list.
 
         nullable : bool
             Whether the list can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
-        if isinstance(value_type, Field):
+        if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeListArray:
         return obj.table[self.name].combine_chunks()
 
 
-class MapField(Field):
-    """A field for storing maps of key-value pairs.
+class MapColumn(Column):
+    """A column for storing maps of key-value pairs.
 
     The keys and values can be of any type, as long as the keys are
     hashable and unique.
     """
 
     def __init__(
         self,
-        key_type: Union[pa.DataType, pa.Field, Field],
-        item_type: Union[pa.DataType, pa.Field, Field],
+        key_type: Union[pa.DataType, pa.Field, Column],
+        item_type: Union[pa.DataType, pa.Field, Column],
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         """
         Parameters
         ----------
-        key_type : Union[pa.DataType, pa.Field, Field]
+        key_type : Union[pa.DataType, pa.Field, Column]
             The type of the keys in the map.
 
-        item_type : Union[pa.DataType, pa.Field, Field]
+        item_type : Union[pa.DataType, pa.Field, Column]
             The type of the values in the map.
 
         nullable : bool
             Whether the map can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
-        if isinstance(key_type, Field):
+        if isinstance(key_type, Column):
             key_type = key_type.dtype
-        if isinstance(item_type, Field):
+        if isinstance(item_type, Column):
             item_type = item_type.dtype
         super().__init__(
             pa.map_(key_type, item_type), nullable=nullable, metadata=metadata, validator=validator
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.MapArray:
         return obj.table[self.name].combine_chunks()
 
 
-class DictionaryField(Field):
-    """A field for storing dictionary-encoded values.
+class DictionaryColumn(Column):
+    """A column for storing dictionary-encoded values.
 
-    This is intended for use with categorical data. See MapField for a
+    This is intended for use with categorical data. See MapColumn for a
     more general mapping type.
     """
 
     def __init__(
         self,
         index_type: pa.DataType,
-        value_type: Union[pa.DataType, pa.Field, Field],
+        value_type: Union[pa.DataType, pa.Field, Column],
         ordered: bool = False,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         """
         Parameters
         ----------
         index_type : IntegerDataType
             The type of the dictionary indices. Must be an integer type.
 
-        value_type : Union[pa.DataType, pa.Field, Field]
+        value_type : Union[pa.DataType, pa.Field, Column]
             The type of the values in the dictionary.
 
         ordered : bool
             Whether the dictionary is ordered.
 
         nullable : bool
             Whether the dictionary can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
-        if isinstance(index_type, Field):
+        if isinstance(index_type, Column):
             index_type = index_type.dtype
-        if isinstance(value_type, Field):
+        if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.dictionary(index_type, value_type, ordered=ordered),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
 
     def __get__(self, obj: "Table", objtype: type) -> pa.DictionaryArray:
         return obj.table[self.name].combine_chunks()
 
 
-class StructField(Field):
-    """A field for storing structured data.
+class StructColumn(Column):
+    """A column for storing structured data.
 
-    In general, prefer to define Tables and use their as_field method
-    instead of using StructField.
+    In general, prefer to define Tables and use their as_column method
+    instead of using StructColumn.
 
     """
 
     def __init__(
         self,
         fields: list[pa.Field],
         nullable: bool = True,
@@ -771,26 +772,26 @@
         fields : List[pa.Field]
             The fields in the struct.
 
         nullable : bool
             Whether the struct can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
         super().__init__(pa.struct(fields), nullable=nullable, metadata=metadata, validator=validator)
 
 
-class RunEndEncodedField(Field):
-    """A field for storing run-end encoded data.
+class RunEndEncodedColumn(Column):
+    """A column for storing run-end encoded data.
 
-    This is a special field type that is used to efficiently store
+    This is a special column type that is used to efficiently store
     highly ordered data. Internally, the data is stored as two
     buffers:
 
     - An array of values, with all consecutive runs of the same value
       reduced to a single element
     - An array of run lengths, with the length of each run
 
@@ -817,18 +818,18 @@
         value_type : pa.DataType
             The type of the values in the run-end encoded data.
 
         nullable : bool
             Whether the data can contain null values.
 
         metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the field.
+            A dictionary of metadata to attach to the column.
 
         validator: Optional[validators.Validator]
-            A validator to run against the field's values.
+            A validator to run against the column's values.
         """
         super().__init__(
             pa.run_end_encoded(run_end_type, value_type),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
```

### Comparing `quivr-0.3.4/quivr/indexing.py` & `quivr-0.4.0/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/quivr/matrix.py` & `quivr-0.4.0/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/quivr/schemagraph.py` & `quivr-0.4.0/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/quivr/tables.py` & `quivr-0.4.0/quivr/tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import sys
 import warnings
 from io import IOBase
-import sys
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
 from typing import Any, ClassVar, Optional, Union
@@ -15,50 +15,50 @@
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
 from .attributes import Attribute
+from .columns import Column, MetadataDict, SubTableColumn
 from .errors import TableFragmentedError, ValidationError
-from .fields import Field, MetadataDict, SubTableField
 from .schemagraph import _walk_schema
 
 
 class Table:
     schema: ClassVar[pa.Schema]
     table: pa.Table
 
     def __init_subclass__(cls, **kwargs):
         fields = []
-        field_validators = {}
+        column_validators = {}
         subtables = {}
         attributes = {}
-        for name, field in cls.__dict__.items():
-            if isinstance(field, Field):
-                fields.append(field.pyarrow_field())
-                if field.validator is not None:
-                    field_validators[name] = field.validator
-                if isinstance(field, SubTableField):
-                    subtables[name] = field
-            elif isinstance(field, Attribute):
-                attributes[name] = field
+        for name, obj in cls.__dict__.items():
+            if isinstance(obj, Column):
+                fields.append(obj.pyarrow_field())
+                if obj.validator is not None:
+                    column_validators[name] = obj.validator
+                if isinstance(obj, SubTableColumn):
+                    subtables[name] = obj
+            elif isinstance(obj, Attribute):
+                attributes[name] = obj
 
         # Generate a pyarrow schema
         schema = pa.schema(fields)
         cls.schema = schema
 
         # Keep track of subtables
         cls._quivr_subtables = subtables
 
         # Add attributes
         cls._quivr_attributes = attributes
 
         # Add validators
-        cls._field_validators = field_validators
+        cls._column_validators = column_validators
 
         # If the subclass has an __init__ override, it must have a
         # with_table override as well.
         if "__init__" in cls.__dict__ and "with_table" not in cls.__dict__:
             raise TypeError(
                 f"{cls.__name__} has an __init__ override, but does not have a with_table "
                 + "override. You must implement both or neither."
@@ -133,24 +133,26 @@
         else:
             raise TypeError(f"Unsupported type: {type(data)}")
         if validate:
             instance.validate()
         return instance
 
     @classmethod
-    def as_field(cls, nullable: bool = True, metadata: Optional[MetadataDict] = None) -> SubTableField[Self]:
-        return SubTableField(cls, nullable=nullable, metadata=metadata)
+    def as_column(
+        cls, nullable: bool = True, metadata: Optional[MetadataDict] = None
+    ) -> SubTableColumn[Self]:
+        return SubTableColumn(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
     def from_kwargs(cls, **kwargs) -> Self:
         """Create a Table instance from keyword arguments.
 
-        Each keyword argument corresponds to a field in the Table.
+        Each keyword argument corresponds to a column in the Table.
 
-        The keys should correspond to the field names, and the values
+        The keys should correspond to the column names, and the values
         can be a list, numpy array, pyarrow array, or Table instance.
         """
         arrays = []
         size = None
 
         # We don't know the size of the table until we've found a
         # field in the schema which corresponds to a kwarg with data.
@@ -243,33 +245,33 @@
 
         Returns:
             A Table object.
 
         Examples:
             >>> import quivr
             >>> class Inner(quivr.Table):
-            ...     a = quivr.StringField()
+            ...     a = quivr.StringColumn()
             ...
             >>> class Outer(quivr.TableBase):
-            ...     z = quivr.StringField()
-            ...     i = Inner.as_field()
+            ...     z = quivr.StringColumn()
+            ...     i = Inner.as_column()
             ...
             >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(rows, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_lists(cls, lists: list[list], **kwargs) -> Self:
         """Create a Table object from a list of lists.
 
-        Each inner list corresponds to a field in the Table. They
-        should be specified in the same order as the fields in the
+        Each inner list corresponds to a column in the Table. They
+        should be specified in the same order as the columns in the
         class.
 
         Args:
             lists: A list of lists. Each inner list corresponds to a column in the table.
             **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
 
 
@@ -286,15 +288,15 @@
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
-        definitions as fields. For that use case, either load an
+        definitions as columns. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
@@ -449,16 +451,16 @@
         """
         table = self.table.sort_by(by)
         return self.__class__(table)
 
     def chunk_counts(self) -> dict[str, int]:
         """Returns the number of discrete memory chunks that make up
         each of the Table's underlying arrays. The keys of the
-        resulting dictionary are the field names, and the values are
-        the number of chunks for that field's data.
+        resulting dictionary are the column names, and the values are
+        the number of chunks for that column's data.
 
         """
         result = {}
         for i, field in enumerate(self.schema):
             result[field.name] = self.table.column(i).num_chunks
         return result
 
@@ -498,17 +500,17 @@
 
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         return table.to_pandas()
 
-    def column(self, field_name: str) -> pa.ChunkedArray:
+    def column(self, column_name: str) -> pa.ChunkedArray:
         """Returns the column with the given name as a raw pyarrow ChunkedArray."""
-        return self.table.column(field_name)
+        return self.table.column(column_name)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
     def __len__(self):
         return len(self.table)
 
@@ -588,15 +590,15 @@
         """Read a table from a Feather file."""
         return cls(table=pyarrow.feather.read_table(path), **kwargs)
 
     def to_csv(self, path: str, attribute_columns: bool = True):
         """Write the table to a CSV file. Any nested structure is flattened.
 
         if attribute_columns is True (the default), then any Attributes defined
-        for the table (or its subtable fields) are stored in the CSV as columns;
+        for the table (or its subtable columns) are stored in the CSV as columns;
         they will have the same value repeated for every row. If it is False,
         then Attribute data will  not be stored in the CSV, so it cannot be read back out.
         """
         table = self.flattened_table()
         if attribute_columns:
             for name, val in self._string_attributes().items():
                 table = table.append_column(
@@ -630,20 +632,20 @@
         metadata = table.schema.metadata or {}
         metadata.update(attribute_meta)
         table = table.replace_schema_metadata(metadata)
         return cls(table, **kwargs)
 
     def is_valid(self) -> bool:
         """Validate the table against the schema."""
-        for name, validator in self._field_validators.items():
+        for name, validator in self._column_validators.items():
             validator.valid(self.table.column(name))
 
     def validate(self):
         """Validate the table against the schema, raising an exception if invalid."""
-        for name, validator in self._field_validators.items():
+        for name, validator in self._column_validators.items():
             try:
                 validator.validate(self.table.column(name))
             except ValidationError as e:
                 raise ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
 
     @classmethod
     def empty(cls, **kwargs) -> Self:
@@ -687,31 +689,31 @@
             else:
                 descriptor = cls._quivr_attributes.get(k)
                 if descriptor is None:
                     warnings.warn(f"unexpected missing descriptor with name={k}")
                 result[k.encode("utf8")] = descriptor.to_bytes(descriptor.from_string(v))
         return result
 
-    def _metadata_for_field(self, field_name: str) -> dict[bytes, bytes]:
-        """Return a dictionary of metadata associated with a subtable field."""
+    def _metadata_for_column(self, column_name: str) -> dict[bytes, bytes]:
+        """Return a dictionary of metadata associated with a subtable column."""
         result = {}
         if self.table.schema.metadata is None:
             return result
-        field_name_bytes = (field_name + ".").encode("utf8")
+        column_name_bytes = (column_name + ".").encode("utf8")
         for key, value in self.table.schema.metadata.items():
-            if key.startswith(field_name_bytes):
-                result[key[len(field_name_bytes) :]] = value
+            if key.startswith(column_name_bytes):
+                result[key[len(column_name_bytes) :]] = value
         return result
 
     @classmethod
     def _attribute_metadata_keys(cls) -> set[str]:
         """Return a set of all subtable attribute names."""
         result = {attr.name for attr in cls._quivr_attributes.values()}
-        for field in cls._quivr_subtables.values():
-            attr_fields = field.table_type._quivr_attributes
+        for column in cls._quivr_subtables.values():
+            attr_fields = column.table_type._quivr_attributes
             for attr in attr_fields.values():
-                result.add(f"{field.name}.{attr.name}")
+                result.add(f"{column.name}.{attr.name}")
 
-            children = field.table_type._attribute_metadata_keys()
+            children = column.table_type._attribute_metadata_keys()
             for key in children:
-                result.add(f"{field.name}.{key}")
+                result.add(f"{column.name}.{key}")
         return result
```

### Comparing `quivr-0.3.4/quivr/validators.py` & `quivr-0.4.0/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/LICENSE` & `quivr-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/README.md` & `quivr-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: quivr
+Version: 0.4.0
+Summary: Container library for working with tabular Arrow data
+Project-URL: Source, https://github.com/spenczar/quivr
+Author-email: Spencer Nelson <spencer@spencerwnelson.com>
+License-File: LICENSE
+Requires-Python: >=3.9
+Requires-Dist: mmh3
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyarrow
+Requires-Dist: typing-extensions>=4.0.0
+Description-Content-Type: text/markdown
+
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
 enforce types and expectations. They are backed by the
 high-performance Arrow memory model, making them well-suited for
@@ -41,29 +56,29 @@
 
 Check out this repo, and `pip install` it.
 
 ## Usage
 
 Your main entrypoint to Quivr is through defining classes which
 represent your tables. You write a subclass of quivr.Table, annotating
-it with Fields that describe the data you're working with, and quivr
+it with Columns that describe the data you're working with, and quivr
 will handle the rest.
 
 ```python
-from quivr import Table, Float64Field
+from quivr import Table, Float64Column
 import pyarrow as pa
 
 
 class Coordinates(Table):
-	x = Float64Field()
-	y = Float64Field()
-	z = Float64Field()
-	vx = Float64Field()
-	vy = Float64Field()
-	vz = Float64Field()
+	x = Float64Column()
+	y = Float64Column()
+	z = Float64Column()
+	vx = Float64Column()
+	vy = Float64Column()
+	vz = Float64Column()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
 coords = Coordinates.from_data(
@@ -84,27 +99,27 @@
 # Access any of the columns as a numpy array with zero copy:
 xs = coords.x.to_numpy()
 
 # Present the table as a pandas DataFrame, with zero copy if possible:
 df = coords.to_dataframe()
 ```
 
-### Embedded definitions and nullable fields
+### Embedded definitions and nullable columns
 
-You can embed one table's definition within another, and you can make fields nullable:
+You can embed one table's definition within another, and you can make columns nullable:
 
 ```python
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
 
-# You can construct embedded fields from Arrow StructArrays, which you can get from
+# You can construct embedded columns from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
 orbits = AsteroidOrbit.from_data(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
@@ -147,52 +162,52 @@
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
-You can also use this to add "meta-fields" which are combinations of other fields. For example:
+You can also use this to add "meta-columns" which are combinations of other columns. For example:
 
 ```python
 class CoordinateCovariance(Table):
-	matrix_values = ListField(pa.float64(), 36)
+	matrix_values = ListColumn(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
-	covariance = CoordinateCovariance.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
+	covariance = CoordinateCovariance.as_column()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
 
 ### Adding instance attributes
 
-You can also add more attributes (that is, non-Field ones) to your
+You can also add more attributes (that is, non-Column ones) to your
 class and its instances, but doing so requires a bit more attention.
 
 You can override `__init__` to add instance-level attributes. However,
 if you do this, there are a few rules:
 
  1. Your `__init__` method must have an attribute called `table`, with
     type `pyarrow.Table`, and you must pass this to Table's `__init__`
@@ -203,16 +218,16 @@
 
 For example:
 
 ```python
 from typing import Self
 
 class AsteroidOrbit(Table):
-    designation = StringField()
-	mass = Float64Field(nullable=True)
+    designation = StringColumn()
+	mass = Float64Column(nullable=True)
 	
 	def __init__(self, table: pa.Table, mu: float):
 	    super().__init__(table)
 		self.mu = mu
 		
 	def with_table(self, table: pa.Table) -> Self:
         return AsteroidOrbit(table, self.mu)
@@ -232,25 +247,25 @@
 
 You can validate that the data inside a Table matches constraints you
 define. Only a small number of validators are currently implemented,
 mostly for numeric checks, but as use cases emerge, more will be
 added.
 
 To add data validation, use the `validator=` keyword inside
-fields. For example:
+columns. For example:
 
 ```python
-from quivr import Table, Int64Field, Float64Field, StringField
+from quivr import Table, Int64Column, Float64Column, StringColumn
 from quivr.validators import gt, ge, le, and_, is_in
 
 class Observation(Table):
-    id = Int64Field(validator=gt(0))
-    ra = Float64Field(validator=and_(ge(0), le(360))
-    dataset_id = StringField(validator=is_in(["ztf", "nsc", "skymapper"])))
-    unvalidated = Int64Field()
+    id = Int64Column(validator=gt(0))
+    ra = Float64Column(validator=and_(ge(0), le(360))
+    dataset_id = StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
+    unvalidated = Int64Column()
 ```
 
 This `Observation` table has validators that
 - the `id` column's values are greater than 0
 - the `ra` column's values are between 0 and 360, inclusive
 - the `dataset_id` column only has strings in the set `{"ztf", "nsc", "skymapper"}`
```

### Comparing `quivr-0.3.4/pyproject.toml` & `quivr-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.3.4/PKG-INFO` & `quivr-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: quivr
-Version: 0.3.4
-Summary: Container library for working with tabular Arrow data
-Project-URL: Source, https://github.com/spenczar/quivr
-Author-email: Spencer Nelson <spencer@spencerwnelson.com>
-License-File: LICENSE
-Requires-Python: >=3.9
-Requires-Dist: mmh3
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: pyarrow
-Requires-Dist: typing-extensions>=4.0.0
-Description-Content-Type: text/markdown
-
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
 enforce types and expectations. They are backed by the
 high-performance Arrow memory model, making them well-suited for
@@ -56,29 +41,29 @@
 
 Check out this repo, and `pip install` it.
 
 ## Usage
 
 Your main entrypoint to Quivr is through defining classes which
 represent your tables. You write a subclass of quivr.Table, annotating
-it with Fields that describe the data you're working with, and quivr
+it with Columns that describe the data you're working with, and quivr
 will handle the rest.
 
 ```python
-from quivr import Table, Float64Field
+from quivr import Table, Float64Column
 import pyarrow as pa
 
 
 class Coordinates(Table):
-	x = Float64Field()
-	y = Float64Field()
-	z = Float64Field()
-	vx = Float64Field()
-	vy = Float64Field()
-	vz = Float64Field()
+	x = Float64Column()
+	y = Float64Column()
+	z = Float64Column()
+	vx = Float64Column()
+	vy = Float64Column()
+	vz = Float64Column()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
 coords = Coordinates.from_data(
@@ -99,27 +84,27 @@
 # Access any of the columns as a numpy array with zero copy:
 xs = coords.x.to_numpy()
 
 # Present the table as a pandas DataFrame, with zero copy if possible:
 df = coords.to_dataframe()
 ```
 
-### Embedded definitions and nullable fields
+### Embedded definitions and nullable columns
 
-You can embed one table's definition within another, and you can make fields nullable:
+You can embed one table's definition within another, and you can make columns nullable:
 
 ```python
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
 
-# You can construct embedded fields from Arrow StructArrays, which you can get from
+# You can construct embedded columns from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
 orbits = AsteroidOrbit.from_data(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
@@ -162,52 +147,52 @@
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
-You can also use this to add "meta-fields" which are combinations of other fields. For example:
+You can also use this to add "meta-columns" which are combinations of other columns. For example:
 
 ```python
 class CoordinateCovariance(Table):
-	matrix_values = ListField(pa.float64(), 36)
+	matrix_values = ListColumn(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
 class AsteroidOrbit(Table):
-	designation = StringField()
-	mass = Float64Field(nullable=True)
-	radius = Float64Field(nullable=True)
-	coords = Coordinates.as_field()
-	covariance = CoordinateCovariance.as_field()
+	designation = StringColumn()
+	mass = Float64Column(nullable=True)
+	radius = Float64Column(nullable=True)
+	coords = Coordinates.as_column()
+	covariance = CoordinateCovariance.as_column()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
 ```
 
 ### Adding instance attributes
 
-You can also add more attributes (that is, non-Field ones) to your
+You can also add more attributes (that is, non-Column ones) to your
 class and its instances, but doing so requires a bit more attention.
 
 You can override `__init__` to add instance-level attributes. However,
 if you do this, there are a few rules:
 
  1. Your `__init__` method must have an attribute called `table`, with
     type `pyarrow.Table`, and you must pass this to Table's `__init__`
@@ -218,16 +203,16 @@
 
 For example:
 
 ```python
 from typing import Self
 
 class AsteroidOrbit(Table):
-    designation = StringField()
-	mass = Float64Field(nullable=True)
+    designation = StringColumn()
+	mass = Float64Column(nullable=True)
 	
 	def __init__(self, table: pa.Table, mu: float):
 	    super().__init__(table)
 		self.mu = mu
 		
 	def with_table(self, table: pa.Table) -> Self:
         return AsteroidOrbit(table, self.mu)
@@ -247,25 +232,25 @@
 
 You can validate that the data inside a Table matches constraints you
 define. Only a small number of validators are currently implemented,
 mostly for numeric checks, but as use cases emerge, more will be
 added.
 
 To add data validation, use the `validator=` keyword inside
-fields. For example:
+columns. For example:
 
 ```python
-from quivr import Table, Int64Field, Float64Field, StringField
+from quivr import Table, Int64Column, Float64Column, StringColumn
 from quivr.validators import gt, ge, le, and_, is_in
 
 class Observation(Table):
-    id = Int64Field(validator=gt(0))
-    ra = Float64Field(validator=and_(ge(0), le(360))
-    dataset_id = StringField(validator=is_in(["ztf", "nsc", "skymapper"])))
-    unvalidated = Int64Field()
+    id = Int64Column(validator=gt(0))
+    ra = Float64Column(validator=and_(ge(0), le(360))
+    dataset_id = StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
+    unvalidated = Int64Column()
 ```
 
 This `Observation` table has validators that
 - the `id` column's values are greater than 0
 - the `ra` column's values are between 0 and 360, inclusive
 - the `dataset_id` column only has strings in the set `{"ztf", "nsc", "skymapper"}`
```

