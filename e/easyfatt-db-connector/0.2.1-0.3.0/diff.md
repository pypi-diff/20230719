# Comparing `tmp/easyfatt_db_connector-0.2.1.tar.gz` & `tmp/easyfatt_db_connector-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfatt_db_connector-0.2.1.tar", max compression
+gzip compressed data, was "easyfatt_db_connector-0.3.0.tar", max compression
```

## Comparing `easyfatt_db_connector-0.2.1.tar` & `easyfatt_db_connector-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.2.1/LICENSE
--rw-r--r--   0        0        0      676 2023-06-27 16:02:56.358075 easyfatt_db_connector-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2205 2023-06-26 18:42:58.676372 easyfatt_db_connector-0.2.1/README.md
--rw-r--r--   0        0        0       68 2023-05-05 17:04:51.361083 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/__init__.py
--rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/constants.py
--rw-r--r--   0        0        0       52 2023-05-05 17:04:51.377081 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/__init__.py
--rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/__init__.py
--rw-r--r--   0        0        0     6880 2023-06-27 15:57:18.413422 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_base.py
--rw-r--r--   0        0        0     3054 2023-06-27 16:02:10.307915 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_fdb.py
--rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
--rw-r--r--   0        0        0      294 2023-05-05 17:04:51.438081 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/exceptions.py
--rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/__init__.py
--rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/factory.py
--rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/__init__.py
--rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/models.py
--rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/__init__.py
--rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/decorators.py
--rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/downloader.py
--rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.3.0/LICENSE
+-rw-r--r--   0        0        0      858 2023-07-19 11:09:34.997601 easyfatt_db_connector-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7472 2023-07-19 11:09:14.187602 easyfatt_db_connector-0.3.0/README.md
+-rw-r--r--   0        0        0      159 2023-07-14 08:17:32.167009 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/constants.py
+-rw-r--r--   0        0        0       52 2023-07-11 18:37:02.948252 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/__init__.py
+-rw-r--r--   0        0        0     6880 2023-06-27 15:57:18.413422 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_base.py
+-rw-r--r--   0        0        0     4320 2023-06-28 23:13:06.501806 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_fdb.py
+-rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
+-rw-r--r--   0        0        0      674 2023-07-18 15:14:49.864785 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/exceptions.py
+-rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/factory.py
+-rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/__init__.py
+-rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/decorators.py
+-rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/downloader.py
+-rw-r--r--   0        0        0     1388 2023-07-18 15:39:01.437958 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-17 14:07:01.710189 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/__init__.py
+-rw-r--r--   0        0        0      982 2023-07-17 14:08:21.793688 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/fields.py
+-rw-r--r--   0        0        0    12307 2023-07-19 10:55:41.045602 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/mapper.py
+-rw-r--r--   0        0        0     2302 2023-07-19 09:25:29.675103 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/README.md
+-rw-r--r--   0        0        0     3852 2023-07-19 10:29:25.313603 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/company.py
+-rw-r--r--   0        0        0    32696 2023-07-19 10:26:28.461603 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/document.py
+-rw-r--r--   0        0        0     5855 2023-07-19 10:37:16.667602 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/product.py
+-rw-r--r--   0        0        0     2926 2023-07-15 12:18:32.404214 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/README.md
+-rw-r--r--   0        0        0     2908 2023-07-14 10:02:05.284009 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/root.py
+-rw-r--r--   0        0        0     1449 2023-07-19 10:37:40.096102 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/vat_code.py
+-rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.3.0/PKG-INFO
```

### Comparing `easyfatt_db_connector-0.2.1/LICENSE` & `easyfatt_db_connector-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.1/pyproject.toml` & `easyfatt_db_connector-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "easyfatt-db-connector"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Luca Salvarani <lucasalvarani99@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "easyfatt_db_connector", from = "./src/"}]
+repository = "https://github.com/LukeSavefrogs/easyfatt-db-connector/"
+homepage = "https://github.com/LukeSavefrogs/easyfatt-db-connector/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 requests = "^2.30.0"
 fdb = "^2.0.2"
 sqlalchemy-firebird = "^2.0.0"
 sqlalchemy = "^2.0.12"
+lxml = "^4.9.3"
+lxml-stubs = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 poethepoet = "^0.20.0"
 
 [build-system]
```

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_base.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_base.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_fdb.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_fdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 import tempfile
 from typing import Any, Generator, Literal, Optional
 from pathlib import Path
 
 import fdb
 
-from easyfatt_db_connector.core.exceptions import FirebirdClientError
+from easyfatt_db_connector.core.exceptions import DatabaseLockedError
 from easyfatt_db_connector.core.connection._base import EasyfattDBGeneric
 
 class TypedFDBConnection(fdb.Connection):
     """ Stub class used only to provide correct type hjinting to child classes,
     since the `fdb.Connection` class does not provide any type hinting for some return values.
     
     DO NOT USE THIS CLASS DIRECTLY: The methods are not implemented and will raise a NotImplementedError.
@@ -20,47 +20,75 @@
         raise NotImplementedError
 
     def cursor(self) -> fdb.Cursor:
         raise NotImplementedError
 
 
 class EasyfattFDB(EasyfattDBGeneric):
+    def _connect(self, database_path: Path) -> TypedFDBConnection:
+        """ Wrapper around `fdb.connect` which handles some edge cases.
+
+        Args:
+            database_path (Path): The path to the database file.
+
+        Raises:
+            FirebirdClientError: If the database is locked.
+        """
+        try:
+            # Use `WIN1252` instead of `UTF8` to fix error "SQLCODE: -204 block size exceeds implementation restriction"
+            # See https://stackoverflow.com/q/40170882/8965861
+            return fdb.connect(
+                database=str(database_path),
+                user=self.db_username,
+                password=self.db_password if self.db_password else None,
+                charset=self.db_charset,
+                fb_library_name=str(self.firebird_path / "fbembed.dll"),
+            )
+        except (fdb.DatabaseError, UnicodeDecodeError) as e:
+            error_message = str(e)
+
+            try:
+                sqlcode = e.args[1]
+            except:
+                sqlcode = None
+            
+            if (
+                ("codec can't decode byte" in error_message) or   # Not sure why, but sometimes this error pops up when the database is locked
+                ("lock manager error" in error_message) or        # Database locked
+                (sqlcode == -902)                                 # Database file used by another process
+            ):
+                raise DatabaseLockedError(
+                    f"The database '{self.archive_path}' is locked. Close Easyfatt and try again."
+                )
+            
+            # Error is not handled, propagate it to the caller
+            raise
+        
     """ Implementation of the `EasyfattDBGeneric` class using the `fdb` library. """
     @contextmanager
     def connect(self) -> Generator[TypedFDBConnection, None, None]:
         """Connect to the database and return a connection object.
 
         Can be used as a context manager.
 
         Yields:
             TypedFDBConnection: The connection object.
         
         Raises:
             FirebirdClientError: If the database is locked.
-        """
-        # if self.is_locked():
-        #     raise FirebirdClientError(
-        #         f"The database '{self.archive_path}' is locked. Close Easyfatt and try again."
-        #     )
-        
+        """     
         handle, path = tempfile.mkstemp(prefix=f"{self.archive_path.stem}-", suffix=".eft.tmp~")
         os.close(handle)
 
         temp_database = Path(path)
         shutil.copy(self.archive_path, temp_database)
 
         connection = None
         try:
-            connection: TypedFDBConnection = fdb.connect(
-                database=str(temp_database),
-                user=self.db_username,
-                password=self.db_password if self.db_password else None,
-                charset=self.db_charset,
-                fb_library_name=str(self.firebird_path / "fbembed.dll"),
-            )
+            connection: TypedFDBConnection = self._connect(temp_database)
             yield connection
 
         except Exception:
             raise
 
         finally:
             if connection is not None:
@@ -70,19 +98,21 @@
 
 
 
 if __name__ == "__main__":
     database_path = Path("~/Documents/Danea Easyfatt/TestArchivio.eft").expanduser()
 
     db = EasyfattFDB(database_path)
-    print(f"- Is database locked: {db.is_locked()}")
+    # print(f"- Is database locked: {db.is_locked()}")
     print(f"- Connection string : '{db.get_connection_string()}'")
 
     with db.connect() as connection:
         # Informazioni generali sul DB
         print(f"Version    : {connection.version}")
         print(f"Created on : {connection.creation_date}")
         print(f"DB Name    : {connection.database_name}")
         print(f"ReadOnly   : {connection.isreadonly()}")
 
         cur = connection.cursor()
-        print(cur.execute("select * from RDB$ROLES").fetchall())
+        print(cur.execute("select * from RDB$ROLES").fetchall())
+    
+    print(f"The end.")
```

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/factory.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/factory.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/models.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/models.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/downloader.py` & `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/downloader.py`

 * *Files identical despite different names*

