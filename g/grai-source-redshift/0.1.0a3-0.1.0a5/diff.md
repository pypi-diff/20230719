# Comparing `tmp/grai_source_redshift-0.1.0a3.tar.gz` & `tmp/grai_source_redshift-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.1.0a3.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.1.0a5.tar", max compression
```

## Comparing `grai_source_redshift-0.1.0a3.tar` & `grai_source_redshift-0.1.0a5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.696812 grai_source_redshift-0.1.0a3/README.md
--rw-r--r--   0        0        0     1152 2023-07-12 11:29:01.662558 grai_source_redshift-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-12 11:29:06.491842 grai_source_redshift-0.1.0a3/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     9040 2023-07-12 10:52:48.739993 grai_source_redshift-0.1.0a3/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1058 2023-07-12 11:08:33.029031 grai_source_redshift-0.1.0a3/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     8092 2023-06-06 17:35:16.820909 grai_source_redshift-0.1.0a3/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     5080 2023-06-06 17:35:16.821232 grai_source_redshift-0.1.0a3/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.821468 grai_source_redshift-0.1.0a3/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 grai_source_redshift-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-19 11:07:12.940719 grai_source_redshift-0.1.0a5/README.md
+-rw-r--r--   0        0        0     1152 2023-07-19 02:54:03.303504 grai_source_redshift-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-07-19 02:54:01.540015 grai_source_redshift-0.1.0a5/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     9040 2023-07-19 02:52:45.264799 grai_source_redshift-0.1.0a5/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1058 2023-07-19 02:49:22.249877 grai_source_redshift-0.1.0a5/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     8585 2023-07-19 02:49:27.269993 grai_source_redshift-0.1.0a5/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     5482 2023-07-19 02:49:27.270274 grai_source_redshift-0.1.0a5/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.268442 grai_source_redshift-0.1.0a5/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 grai_source_redshift-0.1.0a5/PKG-INFO
```

### Comparing `grai_source_redshift-0.1.0a3/pyproject.toml` & `grai_source_redshift-0.1.0a5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai_source_redshift"
-version = "0.1.0-alpha3"
+version = "0.1.0-alpha5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 grai-client = {version = "^0.3.0a21", allow-prereleases = true}
-grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
+grai-schemas = {version = "^0.2.0a7", allow-prereleases = true}
 multimethod = "^1.8"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 botocore = "^1.29.153"
 redshift-connector = "^2.0.911"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
@@ -36,8 +36,8 @@
     [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry_bumpversion.file."src/grai_source_bigquery/__init__.py"]
+[tool.poetry_bumpversion.file."src/grai_source_redshift/__init__.py"]
```

### Comparing `grai_source_redshift-0.1.0a3/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.1.0a5/src/grai_source_redshift/adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, List, Literal, Sequence, TypeVar
+from typing import Any, Dict, List, Literal, Sequence, TypeVar, Union
+
 from warnings import warn
 
 from grai_schemas import config as base_config
 from grai_schemas.generics import DefaultValue
 from grai_schemas.v1 import SourcedEdgeV1, SourcedNodeV1, SourceV1
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnMetadata,
@@ -22,14 +23,15 @@
 from grai_source_redshift.models import (
     ID,
     UNIQUE_COLUMN_CONSTRAINTS,
     Column,
     ColumnConstraint,
     ColumnID,
     Edge,
+    LateBindingViewColumn,
     Table,
     TableID,
 )
 from grai_source_redshift.package_definitions import config
 
 T = TypeVar("T")
 X = TypeVar("X")
@@ -87,14 +89,40 @@
         "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
+def build_grai_metadata_from_column(current: LateBindingViewColumn, version: Literal["v1"] = "v1") -> ColumnMetadata:
+    """
+
+    Args:
+        current (Column):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+
+    data = {
+        "version": version,
+        "node_type": NodeMetadataTypeLabels.column.value,
+        "node_attributes": {
+            "data_type": current.data_type,
+        },
+        "tags": [config.metadata_id],
+    }
+
+    return ColumnMetadata(**data)
+
+
+@build_grai_metadata.register
 def build_grai_metadata_from_node(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     """
 
     Args:
         current (Table):
         version (Literal["v1"], optional):  (Default value = "v1")
 
@@ -163,15 +191,15 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_app_metadata.register
-def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
+def build_metadata_from_column(current: Union[Column, LateBindingViewColumn], version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Column):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -239,21 +267,17 @@
 
     Returns:
 
     Raises:
 
     """
     integration_meta = build_app_metadata(obj, version)
-    base_metadata = build_grai_metadata(obj, version)
-    integration_meta["grai"] = base_metadata
+    integration_meta["grai"] = build_grai_metadata(obj, version)
 
-    return {
-        base_config.metadata_id: base_metadata,
-        config.metadata_id: integration_meta,
-    }
+    return integration_meta
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any):
     """
 
     Args:
@@ -265,15 +289,15 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_column_to_client(current: Column, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
+def adapt_column_to_client(current: Union[Column, Table, LateBindingViewColumn], source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Column):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -287,35 +311,15 @@
         "display_name": current.name,
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
-@adapt_to_client.register
-def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
-    """
-
-    Args:
-        current (Table):
-        version (Literal["v1"], optional):  (Default value = "v1")
-
-    Returns:
 
-    Raises:
-
-    """
-    spec_dict = {
-        "name": current.full_name,
-        "namespace": current.namespace,
-        "display_name": current.name,
-        "data_source": source,
-        "metadata": build_metadata(current, version),
-    }
-    return SourcedNodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: ID, node2: ID) -> str:
     """
 
     Args:
         node1 (ID):
```

### Comparing `grai_source_redshift-0.1.0a3/src/grai_source_redshift/base.py` & `grai_source_redshift-0.1.0a5/src/grai_source_redshift/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.1.0a3/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.1.0a5/src/grai_source_redshift/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from redshift_connector.core import Connection
 
 from grai_source_redshift.models import (
     Column,
     ColumnID,
     Edge,
     EdgeQuery,
+    LateBindingViewColumn,
     RedshiftNode,
     Table,
 )
 
 
 class RedshiftConfig(BaseSettings):
     """ """
@@ -166,15 +167,28 @@
                    data_type,
                    character_maximum_length,
                    numeric_precision
             FROM information_schema.columns
             WHERE table_schema NOT IN ('pg_catalog', 'information_schema', 'pg_internal')
             ORDER BY ordinal_position;
         """
-        return [Column(**result, namespace=self.namespace) for result in self.query_runner(query)]
+        columns = [Column(**result, namespace=self.namespace) for result in self.query_runner(query)]
+
+        late_binding_query = """
+            select *
+            from pg_get_late_binding_view_cols()
+            cols(column_schema name, table_name name, column_name name, data_type varchar, col_num int);
+        """
+
+        late_binding_views = [
+            LateBindingViewColumn(**result, namespace=self.namespace)
+            for result in self.query_runner(late_binding_query)
+        ]
+        columns.extend(late_binding_views)
+        return columns
 
     def get_table_columns(self, table: Table):
         """
 
         Args:
             table (Table):
```

### Comparing `grai_source_redshift-0.1.0a3/src/grai_source_redshift/models.py` & `grai_source_redshift-0.1.0a5/src/grai_source_redshift/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,31 @@
         """
         if full_name is not None:
             return full_name
         result = f"{values['column_schema']}.{values['table']}.{values['name']}"
         return result
 
 
+class LateBindingViewColumn(RedshiftNode):
+    name: str = Field(alias="column_name")
+    table: str = Field(alias="table_name")
+    column_schema: str = Field(alias="schema")
+    namespace: str
+    data_type: str
+
+    class Config:
+        """ """
+
+        allow_population_by_field_name = True
+
+    @property
+    def full_name(self):
+        return f"{self.column_schema}.{self.table}.{self.name}"
+
+
 class Constraint(str, Enum):
     """ """
 
     foreign_key = "FOREIGN KEY"
     primary_key = "PRIMARY KEY"
     belongs_to = "bt"
```

### Comparing `grai_source_redshift-0.1.0a3/PKG-INFO` & `grai_source_redshift-0.1.0a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.1.0a3
+Version: 0.1.0a5
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: botocore (>=1.29.153,<2.0.0)
 Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
-Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
+Requires-Dist: grai-schemas (>=0.2.0a7,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: redshift-connector (>=2.0.911,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift
 Description-Content-Type: text/markdown
```

