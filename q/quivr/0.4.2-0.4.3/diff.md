# Comparing `tmp/quivr-0.4.2.tar.gz` & `tmp/quivr-0.4.3.tar.gz`

## Comparing `quivr-0.4.2.tar` & `quivr-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/__version__.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/attributes.py
--rw-r--r--   0        0        0    27573 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/columns.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/errors.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/indexing.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/py.typed
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/schemagraph.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/streaming.py
--rw-r--r--   0        0        0    27707 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/tables.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 quivr-0.4.2/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.2/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.2/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 quivr-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/__version__.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/attributes.py
+-rw-r--r--   0        0        0    34132 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/columns.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/concat.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/defragment.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/errors.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/indexing.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/schemagraph.py
+-rw-r--r--   0        0        0    31283 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/tables.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.3/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.3/README.md
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 quivr-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.3/PKG-INFO
```

### Comparing `quivr-0.4.2/quivr/__init__.py` & `quivr-0.4.3/quivr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     TimestampColumn,
     UInt8Column,
     UInt16Column,
     UInt32Column,
     UInt64Column,
 )
 from .concat import concatenate
+from .defragment import defragment
 from .errors import InvariantViolatedError, TableFragmentedError, ValidationError
 from .indexing import StringIndex
 from .matrix import MatrixArray, MatrixExtensionType
 from .tables import Table
 from .validators import and_, eq, ge, gt, is_in, le, lt
 
 __all__ = [
@@ -91,8 +92,9 @@
     "ge",
     "eq",
     "and_",
     "is_in",
     "StringAttribute",
     "IntAttribute",
     "FloatAttribute",
+    "defragment",
 ]
```

### Comparing `quivr-0.4.2/quivr/attributes.py` & `quivr-0.4.3/quivr/attributes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,125 @@
 import struct
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Generic, Optional, TypeVar
 
 if TYPE_CHECKING:
-    from .table import Table
+    from .tables import Table
 
+T = TypeVar("T")
 
-class Attribute:
+
+class Attribute(Generic[T]):
     """
     An Attribute is an accessor for scalar data in a table.
 
     It works through the descriptor protocol.
 
     All attributes must be serializable into bytes.
 
     Attributes are stored as metadata on the underlying Arrow table's schema.
     """
 
-    def __init__(self, default: Any = None):
+    _type: type[T]
+
+    def __init__(
+        self,
+        default: Optional[T] = None,
+    ):
         self.default = default
         self.name = "__ERR_UNSET_NAME"
 
-    def __get__(self, instance: "Table", owner):
+    def __get__(self, instance: "Table", owner: type) -> T:
         if instance is None:
             return self
-        if instance.table.schema.metadata is None:
-            return self.default
         name = self.name.encode("utf8")
-        if name not in instance.table.schema.metadata:
-            return self.default
+        if instance.table.schema.metadata is None or name not in instance.table.schema.metadata:
+            if self.default is not None:
+                return self.default
+            raise AttributeError(f"Attribute {self.name} is not set and has no default")
         raw = instance.table.schema.metadata[name]
         return self.from_bytes(raw)
 
-    def __set__(self, instance, value):
+    def __set__(self, instance: "Table", value: T) -> None:
         metadata = instance.table.schema.metadata
         if metadata is None:
             metadata = {}
         metadata[self.name.encode("utf8")] = self.to_bytes(value)
         instance.table = instance.table.replace_schema_metadata(metadata)
 
-    def __set_name__(self, owner: type, name: str):
+    def __set_name__(self, owner: type, name: str) -> None:
         self.name = name
 
-    def to_bytes(self, value) -> bytes:
+    def to_bytes(self, value: T) -> bytes:
         """
         Convert the value to bytes.
         """
         raise NotImplementedError
 
-    def from_bytes(self, raw: bytes):
+    def from_bytes(self, raw: bytes) -> T:
         """
         Convert the bytes to a value.
         """
         raise NotImplementedError
 
-    def to_string(self, value) -> str:
+    def to_string(self, value: T) -> str:
         """
         Convert the value to a string. Used for CSV writing.
         """
         raise NotImplementedError
 
-    def from_string(self, raw: str):
+    def from_string(self, raw: str) -> T:
         """
         Convert a string to a value. Used for CSV reading.
         """
         raise NotImplementedError
 
 
-class StringAttribute(Attribute):
+class StringAttribute(Attribute[str]):
+    _type = str
+
     def __init__(self, default: Optional[str] = None):
         super().__init__(default=default)
 
-    def to_bytes(self, value) -> bytes:
+    def to_bytes(self, value: str) -> bytes:
         return value.encode("utf8")
 
-    def from_bytes(self, raw: bytes):
+    def from_bytes(self, raw: bytes) -> str:
         return raw.decode("utf8")
 
-    def to_string(self, value) -> str:
+    def to_string(self, value: str) -> str:
         return value
 
-    def from_string(self, raw: str):
+    def from_string(self, raw: str) -> str:
         return raw
 
 
-class IntAttribute(Attribute):
+class IntAttribute(Attribute[int]):
+    _type = int
+
     def __init__(self, default: Optional[int] = None, nbytes: int = 8, signed: bool = True):
         self.nbytes = nbytes
         self.signed = signed
         super().__init__(default=default)
 
     def to_bytes(self, value: int) -> bytes:
         return value.to_bytes(length=self.nbytes, byteorder="little", signed=self.signed)
 
     def from_bytes(self, raw: bytes) -> int:
         return int.from_bytes(raw, byteorder="little", signed=self.signed)
 
-    def to_string(self, value) -> str:
+    def to_string(self, value: int) -> str:
         return str(value)
 
-    def from_string(self, raw: str):
+    def from_string(self, raw: str) -> int:
         return int(raw)
 
 
-class FloatAttribute(Attribute):
+class FloatAttribute(Attribute[float]):
+    _type = float
+
     def __init__(self, default: Optional[float] = None, nbytes: int = 8):
         if nbytes == 8:
             self._struct_fmt = "<d"
         elif nbytes == 4:
             self._struct_fmt = "<f"
         elif nbytes == 2:
             self._struct_fmt = "<e"
@@ -114,14 +127,14 @@
             raise ValueError("nbytes must be 2, 4 or 8")
         super().__init__(default=default)
 
     def to_bytes(self, value: float) -> bytes:
         return struct.pack(self._struct_fmt, value)
 
     def from_bytes(self, raw: bytes) -> float:
-        return struct.unpack(self._struct_fmt, raw)[0]
+        return float(struct.unpack(self._struct_fmt, raw)[0])
 
-    def to_string(self, value) -> str:
+    def to_string(self, value: float) -> str:
         return "{:.17g}".format(value)
 
-    def from_string(self, raw: str):
+    def from_string(self, raw: str) -> float:
         return float(raw)
```

### Comparing `quivr-0.4.2/quivr/columns.py` & `quivr-0.4.3/quivr/columns.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+from __future__ import annotations
+
 import sys
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
-from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Union
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Self
+else:
+    from typing import Self
+
+from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Union, overload
 
 import pyarrow as pa
 
 from . import validators
 
 if TYPE_CHECKING:
     from .tables import Table
@@ -30,27 +38,35 @@
         validator: Optional[validators.Validator] = None,
     ):
         self.dtype = dtype
         self.nullable = nullable
         self.metadata = metadata
         self.validator = validator
 
-    def __get__(self, obj: "Table", objtype: type):
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
+    def __get__(self, obj: Table, objtype: type) -> pa.Array:
+        ...
+
+    def __get__(self, obj: Union[Table, None], objtype: type) -> Union[Self, pa.Array]:
         if obj is None:
             return self
         return obj.table.column(self.name)
 
-    def __set__(self, obj: "Table", value):
+    def __set__(self, obj: Table, value: pa.Array) -> None:
         idx = obj.table.schema.get_field_index(self.name)
         obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value])
 
-    def __set_name__(self, owner: type, name: str):
+    def __set_name__(self, owner: type, name: str) -> None:
         self.name = name
 
-    def pyarrow_field(self):
+    def pyarrow_field(self) -> pa.Field:
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
 
 
 T = TypeVar("T", bound="Table")
 
 
 class SubTableColumn(Column, Generic[T]):
@@ -60,23 +76,31 @@
 
     def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
-    def __get__(self, obj: "Table", objtype: type) -> T:
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
+    def __get__(self, obj: Table, objtype: type) -> T:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, T]:
         if obj is None:
             return self
         array = obj.table.column(self.name)
 
         metadata = self.metadata
         if metadata is None:
             metadata = {}
-        metadata.update(obj._metadata_for_column(self.name))
+        metadata.update(obj._metadata_for_column(self.name))  # type: ignore
 
         schema = self.schema.with_metadata(metadata)
 
         subtable = pa.Table.from_arrays(array.flatten(), schema=schema)
         return self.table_type(subtable)
 
 
@@ -89,15 +113,23 @@
         self,
         nullable: bool = True,
         validator: Optional[validators.Validator] = None,
         metadata: Optional[MetadataDict] = None,
     ):
         super().__init__(pa.int8(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Int8Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int8Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int16Column(Column):
     """
@@ -108,105 +140,161 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int16(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Int16Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int16Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int32(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Int32Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int64(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Int64Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt8Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint8(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt8Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt8Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt16Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint16(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt16Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt16Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt32Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint32(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt32Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt64Column(Column):
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint64(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.UInt64Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float16Column(Column):
     """
@@ -217,15 +305,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.HalfFloatArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.HalfFloatArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float32Column(Column):
     """
@@ -236,15 +332,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float32(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.FloatArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.FloatArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float64Column(Column):
     """
@@ -255,15 +359,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float64(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.lib.DoubleArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.DoubleArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class StringColumn(Column):
     """A column for storing strings.
@@ -278,15 +390,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.string(), nullable=nullable, metadata=metadata, validator=validator)
 
-    def __get__(self, obj: "Table", objtype: type) -> pa.StringArray:
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
+    def __get__(self, obj: Table, objtype: type) -> pa.StringArray:
+        ...
+
+    def __get__(self, obj: Optional[Table], objtype: type) -> Union[pa.StringArray, Self]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeBinaryColumn(Column):
     """
@@ -298,15 +418,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeBinaryArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeBinaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeStringColumn(Column):
     """
@@ -318,15 +446,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.large_string(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeStringArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeStringArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date32Column(Column):
     """A column for storing dates.
@@ -340,15 +476,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Date32Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Date32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date64Column(Column):
     """A column for storing dates.
@@ -362,15 +506,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Date64Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Date64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class TimestampColumn(Column):
     """A column for storing timestamps.
@@ -395,15 +547,23 @@
         tz: Optional[str] = None,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.TimestampArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.TimestampArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time32Column(Column):
     """
@@ -421,15 +581,23 @@
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Time32Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Time32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time64Column(Column):
     """
@@ -447,15 +615,23 @@
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Time64Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Time64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class DurationColumn(Column):
     """
@@ -473,15 +649,23 @@
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.DurationArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.DurationArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class MonthDayNanoIntervalColumn(Column):
     """A column for storing calendar intervals (an elapsed number of months,
@@ -501,15 +685,23 @@
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(
             pa.month_day_nano_interval(), nullable=nullable, metadata=metadata, validator=validator
         )
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.MonthDayNanoIntervalArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.MonthDayNanoIntervalArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class BinaryColumn(Column):
     """A column for storing opaque binary data.
@@ -528,15 +720,23 @@
         length: int = -1,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.binary(length), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.BinaryArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.BinaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal128Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
@@ -561,15 +761,23 @@
     """
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal128(precision, scale), nullable=nullable, metadata=metadata)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal128Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Decimal128Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal256Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
@@ -583,15 +791,23 @@
     """
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal256(precision, scale), nullable=nullable, metadata=metadata)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.Decimal256Array:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Decimal256Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class NullColumn(Column):
     """A column for storing null values.
@@ -605,15 +821,23 @@
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.null(), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.NullArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.NullArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 # Complex types follow
 
@@ -658,15 +882,23 @@
         """
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.list_(value_type, list_size), nullable=nullable, metadata=metadata, validator=validator
         )
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.ListArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.ListArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeListColumn(Column):
     """A column for storing large lists of values.
@@ -702,15 +934,23 @@
         validator: Optional[validators.Validator]
             A validator to run against the column's values.
         """
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.LargeListArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeListArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class MapColumn(Column):
     """A column for storing maps of key-value pairs.
@@ -749,15 +989,23 @@
             key_type = key_type.dtype
         if isinstance(item_type, Column):
             item_type = item_type.dtype
         super().__init__(
             pa.map_(key_type, item_type), nullable=nullable, metadata=metadata, validator=validator
         )
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.MapArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.MapArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class DictionaryColumn(Column):
     """A column for storing dictionary-encoded values.
@@ -803,15 +1051,23 @@
         super().__init__(
             pa.dictionary(index_type, value_type, ordered=ordered),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
 
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
     def __get__(self, obj: "Table", objtype: type) -> pa.DictionaryArray:
+        ...
+
+    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.DictionaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class StructColumn(Column):
     """A column for storing structured data.
```

### Comparing `quivr-0.4.2/quivr/concat.py` & `quivr-0.4.3/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.2/quivr/indexing.py` & `quivr-0.4.3/quivr/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
 
     def __init__(self, table: T, column: str, size: int = 1000):
         self.table = table
         self.column = column
         self.idx = self._build_index(size)
 
-    def _build_index(self, size: int):
+    def _build_index(self, size: int) -> pa.Array:
         index_array = [None for _ in range(size)]
         data = self.table.table.column(self.column)
         assert data.type == pa.string()
 
         for i, value in enumerate(data.to_numpy()):
             slot = mmh3.hash(value) % size
             if index_array[slot] is None:
```

### Comparing `quivr-0.4.2/quivr/matrix.py` & `quivr-0.4.3/quivr/matrix.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+from typing import Any
+
+import numpy.typing as npt
 import pyarrow as pa
 
 
-class MatrixExtensionType(pa.PyExtensionType):
+class MatrixExtensionType(pa.PyExtensionType):  # type: ignore
     """This is a custom type for embedding multi-dimensional arrays
     into Table schemas.
 
     """
 
     def __init__(self, shape: tuple[int, int], element_dtype: pa.DataType):
         self.shape = shape
         self.element_dtype = element_dtype
         self.dtype = element_dtype
         for dim in reversed(self.shape):
             self.dtype = pa.list_(self.dtype)
         pa.PyExtensionType.__init__(self, self.dtype)
 
-    def __reduce__(self):
+    def __reduce__(self) -> tuple[type, tuple[tuple[int, int], pa.DataType]]:
         return (
             MatrixExtensionType,
             (self.shape, self.element_dtype),
         )
 
-    def __arrow_ext_class__(self):
+    def __arrow_ext_class__(self) -> type:
         return MatrixArray
 
 
-class MatrixArray(pa.ExtensionArray):
-    def to_numpy(self):
+class MatrixArray(pa.ExtensionArray):  # type: ignore
+    def to_numpy(self) -> npt.NDArray[Any]:
         storage = self.storage
         row_size = 1
         for dim in reversed(self.type.shape):
             storage = storage.flatten()
             row_size *= dim
         np_array = storage.to_numpy()
 
         n_row = len(storage) // row_size
-        return np_array.reshape((n_row, *self.type.shape))
+        reshaped: npt.NDArray[Any] = np_array.reshape((n_row, *self.type.shape))
+        return reshaped
```

### Comparing `quivr-0.4.2/quivr/schemagraph.py` & `quivr-0.4.3/quivr/schemagraph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Callable, NoReturn, Optional
+from typing import Callable, Optional
 
 import pyarrow as pa
 
 
 def _walk_schema(
     field: pa.Field,
-    visitor: Callable[[pa.Field, list[pa.Field]], NoReturn],
-    ancestors: Optional[list] = None,
-):
+    visitor: Callable[[pa.Field, list[pa.Field]], None],
+    ancestors: Optional[list[pa.Field]] = None,
+) -> None:
     # Visit every struct field embedded within a field in depth-first fashion.
     #
     # Runs visitor(struct_field, [ancestors...]) on each struct field.
     if ancestors is None:
         ancestors = [field]
     else:
         ancestors += [field]
```

### Comparing `quivr-0.4.2/quivr/tables.py` & `quivr-0.4.3/quivr/tables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import os
 import sys
-import warnings
 from io import IOBase
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
-from typing import Any, ClassVar, Optional, Union
+from typing import Any, ClassVar, Iterator, Optional, Type, TypeAlias, Union
 
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
 from .attributes import Attribute
 from .columns import Column, MetadataDict, SubTableColumn
 from .errors import TableFragmentedError, ValidationError
 from .schemagraph import _walk_schema
+from .validators import Validator
+
+AttributeValueType: TypeAlias = Union[int, float, str]
+DataSourceType: TypeAlias = Union[pa.Array, list[Any], "Table", pd.Series, npt.NDArray[Any]]
 
 
 class Table:
     schema: ClassVar[pa.Schema]
     table: pa.Table
 
-    def __init_subclass__(cls, **kwargs):
+    _quivr_subtables: ClassVar[dict[str, SubTableColumn[Any]]]
+    _quivr_attributes: ClassVar[dict[str, Attribute[Any]]]
+    _column_validators: ClassVar[dict[str, Validator]]
+
+    def __init_subclass__(cls: Type["Table"], **kwargs: Any):
         fields = []
         column_validators = {}
         subtables = {}
         attributes = {}
         for name, obj in cls.__dict__.items():
             if isinstance(obj, Column):
                 fields.append(obj.pyarrow_field())
@@ -62,24 +70,29 @@
             raise TypeError(
                 f"{cls.__name__} has an __init__ override, but does not have a with_table "
                 + "override. You must implement both or neither."
             )
 
         super().__init_subclass__(**kwargs)
 
-    def __init__(self, table: pa.Table, **kwargs):
+    def __init__(self, table: pa.Table, **kwargs: AttributeValueType):
         self.table = table
         for name, value in kwargs.items():
             if name in self._quivr_attributes:
                 setattr(self, name, value)
             else:
                 raise AttributeError(f"{self.__class__.__name__} has no attribute {name}")
 
     @classmethod
-    def from_data(cls, data: Optional[Any] = None, validate: bool = True, **kwargs) -> Self:
+    def from_data(
+        cls,
+        data: Union[pa.Table, dict[str, Any], list[Any], pd.DataFrame, None] = None,
+        validate: bool = True,
+        **kwargs: Union[AttributeValueType, DataSourceType],
+    ) -> Self:
         """
         Create an instance of the Table and populate it with data.
 
         This is a convenience method which tries to infer the right
         underlying constructors to use based on the type of data. It
         can also accept keyword-style arguments to pass data in. If
         you know the data's structure well in advance, the more
@@ -111,61 +124,77 @@
             >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
             MyTable(size=2)
 
 
         """
         if data is None:
             instance = cls.from_kwargs(**kwargs)
-        elif isinstance(data, pa.Table):
-            instance = cls(table=data, **kwargs)
-        elif isinstance(data, dict):
-            instance = cls.from_pydict(data, **kwargs)
-        elif isinstance(data, list):
-            if len(data) == 0:
-                instance = cls.from_rows(data, **kwargs)
-            elif isinstance(data[0], dict):
-                instance = cls.from_rows(data, **kwargs)
-            elif isinstance(data[0], list):
-                instance = cls.from_lists(data, **kwargs)
-            else:
-                raise TypeError(f"Unsupported type: {type(data[0])}")
-        elif isinstance(data, pd.DataFrame):
-            instance = cls.from_dataframe(data, **kwargs)
         else:
-            raise TypeError(f"Unsupported type: {type(data)}")
+            attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
+            if isinstance(data, pa.Table):
+                instance = cls(table=data, **attrib_kwargs)
+            elif isinstance(data, dict):
+                instance = cls.from_pydict(data, **attrib_kwargs)
+            elif isinstance(data, list):
+                if len(data) == 0:
+                    instance = cls.from_rows(data, **attrib_kwargs)
+                elif isinstance(data[0], dict):
+                    instance = cls.from_rows(data, **attrib_kwargs)
+                elif isinstance(data[0], list):
+                    instance = cls.from_lists(data, **attrib_kwargs)
+                else:
+                    raise TypeError(f"Unsupported type: {type(data[0])}")
+            elif isinstance(data, pd.DataFrame):
+                instance = cls.from_dataframe(data, **attrib_kwargs)
+            else:
+                raise TypeError(f"Unsupported type: {type(data)}")
+
         if validate:
             instance.validate()
         return instance
 
     @classmethod
+    def _attribute_kwargs_from_kwargs(
+        cls, kwargs: dict[str, Union[AttributeValueType, DataSourceType]]
+    ) -> dict[str, AttributeValueType]:
+        attrib_kwargs: dict[str, AttributeValueType] = {}
+        for k, v in kwargs.items():
+            if k not in cls._quivr_attributes:
+                raise TypeError(f"Unexpected keyword argument: {k}")
+            if not isinstance(v, cls._quivr_attributes[k]._type):
+                raise TypeError(f"Expected {cls._quivr_attributes[k]._type}, got {type(v)} for {k}")
+            attrib_kwargs[k] = v
+        return attrib_kwargs
+
+    @classmethod
     def as_column(
         cls, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ) -> SubTableColumn[Self]:
         return SubTableColumn(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
-    def from_kwargs(cls, **kwargs) -> Self:
+    def from_kwargs(cls, **kwargs: Union[DataSourceType, AttributeValueType]) -> Self:
         """Create a Table instance from keyword arguments.
 
         Each keyword argument corresponds to a column in the Table.
 
         The keys should correspond to the column names, and the values
         can be a list, numpy array, pyarrow array, or Table instance.
         """
-        arrays = []
+        arrays: list[Union[None, pa.Array]] = []
         size = None
 
         # We don't know the size of the table until we've found a
         # field in the schema which corresponds to a kwarg with data.
         # Therefore, we need to keep track of which columns are empty
         # *before* we've discovered the size of the table so we can
         # populate them with nulls later.
         empty_columns = []
 
-        metadata = {}
+        metadata: dict[bytes, bytes] = {}
         for i, field in enumerate(cls.schema):
             column_name = field.name
             value = kwargs.pop(column_name, None)
 
             if value is None:
                 if not field.nullable:
                     raise ValueError(f"Missing non-nullable column {column_name}")
@@ -175,15 +204,15 @@
                     else:
                         # We'll have to wait until we get to a non-None column
                         # to figure out the size.
                         empty_columns.append(i)
                         arrays.append(None)
                     continue
             if size is None:
-                size = len(value)
+                size = len(value)  # type: ignore
             elif len(value) != size:
                 raise ValueError(
                     f"Column {column_name} has wrong length {len(value)} (first column has length {size})"
                 )
 
             if isinstance(value, Table):
                 field_meta = value.table.schema.metadata
@@ -204,19 +233,23 @@
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
             arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
-        return cls.from_arrays(arrays, metadata=metadata, **kwargs)
+        attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
+        return cls.from_arrays(arrays, metadata=metadata, **attrib_kwargs)
 
     @classmethod
     def from_arrays(
-        cls, arrays: list[pa.array], metadata: Optional[dict[bytes, bytes]] = None, **kwargs
+        cls,
+        arrays: list[pa.array],
+        metadata: Optional[dict[bytes, bytes]] = None,
+        **kwargs: AttributeValueType,
     ) -> Self:
         """Create a Table object from a list of arrays.
 
         Args:
             arrays: A list of pyarrow.Array objects.
             metadata: An optional dictionary of metadata to attach to the Table.
             **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
@@ -228,20 +261,22 @@
         if metadata is None:
             metadata = {}
         schema = cls.schema.with_metadata(metadata)
         table = pa.Table.from_arrays(arrays, schema=schema)
         return cls(table=table, **kwargs)
 
     @classmethod
-    def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]], **kwargs) -> Self:
+    def from_pydict(
+        cls, d: dict[str, Union[pa.array, list[Any], npt.NDArray[Any]]], **kwargs: AttributeValueType
+    ) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
-    def from_rows(cls, rows: list[dict], **kwargs) -> Self:
+    def from_rows(cls, rows: list[dict[str, Any]], **kwargs: AttributeValueType) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
         Args:
             rows: A list of values. Each value corresponds to a row in the table.
             **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
 
@@ -261,15 +296,15 @@
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(rows, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
-    def from_lists(cls, lists: list[list], **kwargs) -> Self:
+    def from_lists(cls, lists: list[list[Any]], **kwargs: AttributeValueType) -> Self:
         """Create a Table object from a list of lists.
 
         Each inner list corresponds to a column in the Table. They
         should be specified in the same order as the columns in the
         class.
 
         Args:
@@ -281,15 +316,15 @@
             A TableBase object.
 
         """
         table = pa.Table.from_arrays(list(map(pa.array, lists)), schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
-    def from_dataframe(cls, df: pd.DataFrame, **kwargs):
+    def from_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
         This function cannot load "flattened" dataframes. This only
@@ -298,15 +333,15 @@
         unflattened DataFrame, or use from_flat_dataframe.
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
-    def _unflatten_table(cls, table: pa.Table):
+    def _unflatten_table(cls, table: pa.Table) -> pa.Table:
         """Unflatten a Table.
 
         This is used when loading a flattened CSV into a nested
         Table. It takes a Table with a flat schema, and returns a
         Table with a nested schema.
 
         """
@@ -315,15 +350,15 @@
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         # Walk the schema, and build a StructArray for each embedded
         # type.
 
-        def struct_array_for(field: pa.Field, ancestors: list[pa.Field]):
+        def struct_array_for(field: pa.Field, ancestors: list[pa.Field]) -> pa.StructArray:
             prefix = ".".join([f.name for f in ancestors if f.name] + [field.name])
 
             child_arrays = []
             for subfield in field.type:
                 if pa.types.is_struct(subfield.type):
                     child_arrays.append(struct_array_for(subfield, ancestors + [field]))
                 else:
@@ -337,15 +372,15 @@
                 child_arrays.append(struct_array_for(field, []))
             else:
                 child_arrays.append(table.column(field.name).combine_chunks())
 
         return pa.Table.from_arrays(child_arrays, schema=cls.schema)
 
     @classmethod
-    def from_flat_dataframe(cls, df: pd.DataFrame, **kwargs):
+    def from_flat_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
         """Load a flattened DataFrame into the Table.
 
         known bug: Doesn't correctly interpret fixed-length lists.
         """
         struct_fields = []
         for field in cls.schema:
             if pa.types.is_struct(field.type):
@@ -367,15 +402,15 @@
         #   ]))
         #
         # Then the struct array for the inner struct will be stored in
         # the dictionary at the key "foo.bar".
 
         struct_arrays: dict[str, pa.StructArray] = {}
 
-        def visitor(field: pa.Field, ancestors: list[pa.Field]):
+        def visitor(field: pa.Field, ancestors: list[pa.Field]) -> None:
             # Modify the dataframe in place, trimming out the columns we
             # have already processed in depth-first order.
             nonlocal df
             if len(ancestors) == 0:
                 # Root - gets special behavior.
                 df_key = ""
             else:
@@ -500,67 +535,65 @@
         "foo" column, and the values will of the column will be
         dictionaries representing the struct values.
 
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
-        return table.to_pandas()
+        df: pd.DataFrame = table.to_pandas()
+        return df
 
     def column(self, column_name: str) -> pa.ChunkedArray:
         """Returns the column with the given name as a raw pyarrow ChunkedArray."""
         return self.table.column(column_name)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.table)
 
     def with_table(self, table: pa.Table) -> Self:
         return self.__class__(table)
 
-    def __getitem__(self, idx):
-        # TODO: This comes out a little funky. You get chunked arrays
-        # instead of arrays. Is there a way to flatten them safely?
-
+    def __getitem__(self, idx: Union[int, slice]) -> Self:
         if isinstance(idx, int):
             table = self.table[idx : idx + 1]
         else:
             table = self.table[idx]
         return self.with_table(table)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Self]:
         for i in range(len(self)):
             yield self[i : i + 1]
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Table):
-            return self.table.equals(other.table)
+            return bool(self.table.equals(other.table, check_metadata=True))
         if isinstance(other, pa.Table):
-            return self.table.equals(other)
+            return bool(self.table.equals(other, check_metadata=True))
         return False
 
     def take(self, row_indices: Union[list[int], pa.IntegerArray]) -> Self:
         """Return a new Table with only the rows at the given indices."""
         return self.__class__(self.table.take(row_indices))
 
-    def to_parquet(self, path: str, **kwargs):
+    def to_parquet(self, path: str, **kwargs: Any) -> None:
         """Write the table to a Parquet file."""
         pyarrow.parquet.write_table(self.table, path, **kwargs)
 
     @classmethod
     def from_parquet(
         cls,
         path: str,
         memory_map: bool = False,
         pq_buffer_size: int = 0,
         filters: Optional[pc.Expression] = None,
-        **kwargs,
-    ):
+        **kwargs: AttributeValueType,
+    ) -> Self:
         """Read a table from a Parquet file.
 
         Arguments:
             path: The path to the Parquet file.
             memory_map: If True, memory-map the file, otherwise read it into memory.
             pq_buffer_size: If positive, perform read buffering when
                 deserializing individual column chunks. Otherwise, IO
@@ -579,24 +612,24 @@
             columns=[field.name for field in cls.schema],
             memory_map=memory_map,
             buffer_size=pq_buffer_size,
             filters=filters,
         )
         return cls(table=table, **kwargs)
 
-    def to_feather(self, path: str, **kwargs):
+    def to_feather(self, path: str, **kwargs: Any) -> None:
         """Write the table to a Feather file."""
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
-    def from_feather(cls, path: str, **kwargs):
+    def from_feather(cls, path: str, **kwargs: AttributeValueType) -> Self:
         """Read a table from a Feather file."""
         return cls(table=pyarrow.feather.read_table(path), **kwargs)
 
-    def to_csv(self, path: str, attribute_columns: bool = True):
+    def to_csv(self, path: str, attribute_columns: bool = True) -> None:
         """Write the table to a CSV file. Any nested structure is flattened.
 
         if attribute_columns is True (the default), then any Attributes defined
         for the table (or its subtable columns) are stored in the CSV as columns;
         they will have the same value repeated for every row. If it is False,
         then Attribute data will  not be stored in the CSV, so it cannot be read back out.
         """
@@ -606,15 +639,17 @@
                 table = table.append_column(
                     name,
                     pa.repeat(val, len(table)),
                 )
         pyarrow.csv.write_csv(table, path)
 
     @classmethod
-    def from_csv(cls, input_file: Union[str, os.PathLike, IOBase], **kwargs):
+    def from_csv(
+        cls, input_file: Union[str, os.PathLike, IOBase], **kwargs: AttributeValueType  # type: ignore
+    ) -> Self:
         """Read a table from a CSV file."""
         flat_table = pyarrow.csv.read_csv(input_file)
 
         # Gather any attributes from the CSV. We do this by looking for specially named
         # columns, and grabbing the value from their first row.
         attributes = {}
         attr_names = cls._attribute_metadata_keys()
@@ -635,28 +670,30 @@
         metadata.update(attribute_meta)
         table = table.replace_schema_metadata(metadata)
         return cls(table, **kwargs)
 
     def is_valid(self) -> bool:
         """Validate the table against the schema."""
         for name, validator in self._column_validators.items():
-            validator.valid(self.table.column(name))
+            if not validator.valid(self.table.column(name)):
+                return False
+        return True
 
-    def validate(self):
+    def validate(self) -> None:
         """Validate the table against the schema, raising an exception if invalid."""
         for name, validator in self._column_validators.items():
             try:
                 validator.validate(self.table.column(name))
             except ValidationError as e:
                 raise ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
 
     @classmethod
-    def empty(cls, **kwargs) -> Self:
+    def empty(cls, **kwargs: AttributeValueType) -> Self:
         """Create an empty instance of the table."""
-        data = [[] for _ in range(len(cls.schema))]
+        data = [[] for _ in range(len(cls.schema))]  # type: ignore
         empty_table = pa.table(data, schema=cls.schema)
         return cls(table=empty_table, **kwargs)
 
     def attributes(self) -> dict[str, Any]:
         """Return a dictionary of the table's attributes."""
         return {name: getattr(self, name) for name in self._quivr_attributes}
 
@@ -687,21 +724,21 @@
                 subtable_item = cls._quivr_subtables[subtable_name].table_type._unpack_string_metadata(
                     {subtable_key: v}
                 )
                 result[k.encode("utf8")] = next(iter(subtable_item.values()))
             else:
                 descriptor = cls._quivr_attributes.get(k)
                 if descriptor is None:
-                    warnings.warn(f"unexpected missing descriptor with name={k}")
+                    raise AttributeError(f"unexpected missing descriptor with name={k}")
                 result[k.encode("utf8")] = descriptor.to_bytes(descriptor.from_string(v))
         return result
 
     def _metadata_for_column(self, column_name: str) -> dict[bytes, bytes]:
         """Return a dictionary of metadata associated with a subtable column."""
-        result = {}
+        result: dict[bytes, bytes] = {}
         if self.table.schema.metadata is None:
             return result
         column_name_bytes = (column_name + ".").encode("utf8")
         for key, value in self.table.schema.metadata.items():
             if key.startswith(column_name_bytes):
                 result[key[len(column_name_bytes) :]] = value
         return result
@@ -715,7 +752,46 @@
             for attr in attr_fields.values():
                 result.add(f"{column.name}.{attr.name}")
 
             children = column.table_type._attribute_metadata_keys()
             for key in children:
                 result.add(f"{column.name}.{key}")
         return result
+
+    def apply_mask(self, mask: pa.BooleanArray | np.ndarray | list[bool]) -> Self:
+        """Return a new table with rows filtered to match a boolean mask.
+
+        The mask must have the same length as the table. At each index, if the mask's
+        value is True, the row will be included in the new table; if False, it will be
+        excluded.
+
+        If the mask is a pyarrow BooleanArray, it must not have any null values.
+        """
+        if len(mask) != len(self):
+            raise ValueError("mask must be the same length as the table")
+        if isinstance(mask, pa.BooleanArray):
+            if mask.null_count > 0:
+                raise ValueError("mask must not contain null values")
+        return self.__class__(self.table.filter(mask))
+
+    def where(self, expr: pc.Expression) -> Self:
+        """Return a new table with rows filtered to match an expression.
+
+        The expression must be a pyarrow Expression that evaluates to a boolean array.
+
+        Examples
+        --------
+        >>> from quivr import Table, Int64Column
+        >>> import pyarrow.compute as pc
+        >>> class MyTable(Table):
+        ...     x = Int64Column()
+        ...     y = Int64Column()
+        ...
+        >>> t = MyTable.from_data(x=[1, 2, 3], y=[4, 5, 6])
+        >>> filtered = t.where(pc.field("x") > 1)
+        >>> print(filtered.x.to_pylist())
+        [2, 3]
+        >>> print(filtered.y.to_pylist())
+        [5, 6]
+
+        """
+        return self.__class__(self.table.filter(expr))
```

### Comparing `quivr-0.4.2/quivr/validators.py` & `quivr-0.4.3/quivr/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,27 @@
         self.args = args
         self.label = label
 
     def _check_arity(self, func: pc.Function, args: list[Any]) -> None:
         if not func.arity == (len(args) + 1):
             raise ValueError("Invalid number of arguments")
 
-    def evaluate(self, array) -> pyarrow.Array:
+    def evaluate(self, array: pyarrow.Array) -> pyarrow.Array:
         return self.func.call([array, *self.args])
 
-    def valid(self, array) -> bool:
+    def valid(self, array: pyarrow.Array) -> bool:
         if self.func.kind == "scalar_aggregate":
-            return self.evaluate(array).as_py()
+            return self.evaluate(array).as_py()  # type: ignore
         else:
-            return pc.all(self.evaluate(array)).as_py()
+            results = self.evaluate(array)
+            if results.null_count == len(results):
+                return True
+            return pc.all(self.evaluate(array)).as_py()  # type: ignore
 
-    def validate(self, array) -> None:
+    def validate(self, array: pyarrow.Array) -> None:
         if not self.valid(array):
             if self.func.kind == "scalar_aggregate":
                 raise ValidationError(f"array did not pass validator '{self.label}'")
             indices, failures = self.failures(array)
             if len(failures) == 1:
                 index = indices[0].as_py()
                 value = failures[0].as_py()
@@ -44,15 +47,15 @@
                 value = failures[0].as_py()
                 msg = (
                     f"validator '{self.label}' failed on {n_failed} values, "
                     + f"first failure: val={value}, index={index}"
                 )
                 raise ValidationError(msg, failures)
 
-    def failures(self, array) -> (pyarrow.Array, pyarrow.Array):
+    def failures(self, array: pyarrow.Array) -> tuple[pyarrow.Array, pyarrow.Array]:
         """
         Returns a tuple of two arrays, the first containing the indices of the invalid values,
         and the second containing the invalid values themselves.
 
         If the validator is a scalar aggregate function, raises a TypeError.
         """
         if self.func.kind == "scalar_aggregate":
@@ -74,91 +77,91 @@
         func = pc.get_function("is_in")
         super().__init__(func, args, label)
 
     def _check_arity(self, func: pc.Function, args: list[Any]) -> None:
         if not len(args) == 1:
             raise ValueError("Invalid number of arguments")
 
-    def evaluate(self, array) -> pyarrow.Array:
+    def evaluate(self, array: pyarrow.Array) -> pyarrow.Array:
         return self.func.call([array], self.args[0])
 
 
 class AndValidator(Validator):
-    def __init__(self, validators, label: str):
+    def __init__(self, validators: list[Validator], label: str):
         self.validators = validators
         func = pc.get_function("and")
         super().__init__(func, validators, label)
 
     def _check_arity(self, func: pc.Function, args: list[Any]) -> None:
         if not len(args) > 1:
             raise ValueError("Invalid number of arguments passed to and_")
 
-    def evaluate(self, array) -> pyarrow.Array:
+    def evaluate(self, array: pyarrow.Array) -> pyarrow.Array:
         return pc.and_(*[v.evaluate(array) for v in self.validators])
 
 
-def eq(val) -> Validator:
+def eq(val: Any) -> Validator:
     """
     Validator that all data in a column is equal to a given value.
     """
     func = pc.get_function("equal")
     label = f"eq({val})"
     return Validator(func, [val], label)
 
 
-def lt(val) -> Validator:
+def lt(val: Any) -> Validator:
     """
     Validator that all data in a column is less than a given value.
     """
     func = pc.get_function("less")
     label = f"lt({val})"
     return Validator(func, [val], label)
 
 
-def le(val) -> Validator:
+def le(val: Any) -> Validator:
     """
     Validator that all data in a column is less than or equal to a given value.
     """
     func = pc.get_function("less_equal")
     label = f"le({val})"
     return Validator(func, [val], label)
 
 
-def gt(val) -> Validator:
+def gt(val: Any) -> Validator:
     """
     Validator that all data in a column is greater than a given value.
     """
     func = pc.get_function("greater")
     label = f"gt({val})"
     return Validator(func, [val], label)
 
 
-def ge(val) -> Validator:
+def ge(val: Any) -> Validator:
     """
     Validator that all data in a column is greater than or equal to a given value.
     """
     func = pc.get_function("greater_equal")
     label = f"ge({val})"
     return Validator(func, [val], label)
 
 
-def is_in(val, fail_on_null: bool = False) -> IsInValidator:
+def is_in(val: Any, fail_on_null: bool = False) -> IsInValidator:
     """Validator that all data in a column is in a given set.
 
     If fail_on_null is true, then nulls always trigger an
     error. Otherwise, they are matched to the value set, just like
     regular values.
 
     """
     label = f"is_in({val})"
     if not isinstance(val, pyarrow.Array):
         val = pyarrow.array(val)
     val = pc.SetLookupOptions(value_set=val, skip_nulls=fail_on_null)
     return IsInValidator([val], label)
 
 
-def and_(*validators) -> Validator:
+def and_(*validators: Validator) -> Validator:
     """
     Validator that all data in a column passes all of the given validators.
     """
     label = "and({})".format(", ".join([v.label for v in validators]))
-    return AndValidator(validators, label)
+    return AndValidator(list(validators), label)
```

### Comparing `quivr-0.4.2/LICENSE` & `quivr-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.4.2/README.md` & `quivr-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.4.2/pyproject.toml` & `quivr-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,36 +28,23 @@
 ]
 
 [tool.hatch.version]
 path = "quivr/__version__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
+  "black",
   "isort",
   "mypy",
   "pandas-stubs",
   "pytest",
   "pytest-benchmark",
   "ruff",
 ]
 
-[tool.hatch.envs.py310]
-python = "3.10"
-dependencies = [
-  "pytest",
-  "pytest-benchmark",
-]
-
-[tool.hatch.envs.py39]
-python = "3.9"
-dependencies = [
-  "pytest",
-  "pytest-benchmark",
-]
-
 [tool.hatch.envs.default.scripts]
 check = [
   "lint",
   "typecheck",
   "test",
 ]
 fix = [
@@ -69,15 +56,15 @@
   "isort --check-only ./quivr ./test"
 ]
 format = [
   "black ./quivr ./test",
   "isort ./quivr ./test"
 ]
 typecheck = [
-  "mypy ./quivr",
+  "mypy --strict ./quivr ./examples ./test/typing_tests",
 ]
 test = [
   "pytest --benchmark-disable ./test",
 ]
 benchmark = [
   "pytest --benchmark-only ./test"
 ]
```

### Comparing `quivr-0.4.2/PKG-INFO` & `quivr-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.4.2
+Version: 0.4.3
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

