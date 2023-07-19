# Comparing `tmp/tableschema-sql-1.3.2.tar.gz` & `tmp/tableschema-sql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableschema-sql-1.3.2.tar", last modified: Thu Sep 23 17:06:30 2021, max compression
+gzip compressed data, was "tableschema-sql-2.0.0.tar", last modified: Wed Jul 19 13:14:48 2023, max compression
```

## Comparing `tableschema-sql-1.3.2.tar` & `tableschema-sql-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 17:06:30.531079 tableschema-sql-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2021-09-23 17:06:30.531079 tableschema-sql-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-09-23 17:06:30.531079 tableschema-sql-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 17:06:30.531079 tableschema-sql-1.3.2/tableschema_sql/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/tableschema_sql/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/tableschema_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11284 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/tableschema_sql/mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    10230 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/tableschema_sql/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2021-09-23 17:06:27.000000 tableschema-sql-1.3.2/tableschema_sql/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 17:06:30.531079 tableschema-sql-1.3.2/tableschema_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-23 17:06:30.000000 tableschema-sql-1.3.2/tableschema_sql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:48.759036 tableschema-sql-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 13:14:48.759036 tableschema-sql-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 13:14:48.759036 tableschema-sql-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:48.759036 tableschema-sql-2.0.0/tableschema_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/tableschema_sql/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/tableschema_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/tableschema_sql/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/tableschema_sql/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-19 13:14:41.000000 tableschema-sql-2.0.0/tableschema_sql/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:48.759036 tableschema-sql-2.0.0/tableschema_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 13:14:48.000000 tableschema-sql-2.0.0/tableschema_sql.egg-info/top_level.txt
```

### Comparing `tableschema-sql-1.3.2/LICENSE.md` & `tableschema-sql-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tableschema-sql-1.3.2/Makefile` & `tableschema-sql-2.0.0/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 
 templates:
 	sed -i -E "s/@(\w*)/@$(LEAD)/" .github/issue_template.md
 	sed -i -E "s/@(\w*)/@$(LEAD)/" .github/pull_request_template.md
 
 test:
 	pylama $(PACKAGE)
-	py.test -vvv --cov tableschema_sql --cov-report term-missing || echo 'TESTING FAILED'
+	py.test -vvv --cov tableschema_sql --cov-report term-missing
 
 version:
 	@echo $(VERSION)
```

### Comparing `tableschema-sql-1.3.2/PKG-INFO` & `tableschema-sql-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableschema-sql
-Version: 1.3.2
+Version: 2.0.0
 Summary: Generate SQL tables, load and extract data, based on JSON Table Schema descriptors.
 Home-page: https://github.com/frictionlessdata/tableschema-sql-py
 Author: Open Knowledge Foundation
 Author-email: info@okfn.org
 License: MIT
 Keywords: frictionless data
 Platform: UNKNOWN
```

### Comparing `tableschema-sql-1.3.2/README.md` & `tableschema-sql-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tableschema-sql-1.3.2/setup.py` & `tableschema-sql-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 
 
 # Prepare
 PACKAGE = 'tableschema_sql'
 NAME = PACKAGE.replace('_', '-')
 INSTALL_REQUIRES = [
     'six>=1.9',
-    'sqlalchemy>=1.0',
+    'sqlalchemy>=2.0,<3',
     'pybloom_live>=2.2',
     'tabulator>=1.1',
     'tableschema>=1.0',
+    'cryptography'
 ]
 TESTS_REQUIRE = [
     'coverage',
     'mock',
     'pylama',
     'pytest',
     'pytest-cov',
```

### Comparing `tableschema-sql-1.3.2/tableschema_sql/mapper.py` & `tableschema-sql-2.0.0/tableschema_sql/mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,19 @@
                     checks.append(Check('"%s" <= %s' % (field.name, value)))
                 elif name == 'pattern':
                     if self.__dialect in ['postgresql']:
                         checks.append(Check('"%s" ~ \'%s\'' % (field.name, value)))
                     else:
                         checks.append(Check('"%s" REGEXP \'%s\'' % (field.name, value)))
                 elif name == 'enum':
-                    column_type = sa.Enum(*value, name='%s_%s_enum' % (table_name, field.name))
+                    if self.__dialect in ['sqlite']:
+                        checks.append(Check(sa.text('"%s" in (:values)' % field.name)
+                                              .bindparams(sa.bindparam(key="values", value=value, expanding=True))))
+                    else:
+                        column_type = sa.Enum(*value, name='%s_%s_enum' % (table_name, field.name))
             column = sa.Column(*([field.name, column_type] + checks),
                 nullable=nullable, comment=comment, unique=unique)
             columns.append(column)
             column_mapping[field.name] = column
 
         # Primary key
         pk = descriptor.get('primaryKey', None)
```

### Comparing `tableschema-sql-1.3.2/tableschema_sql/storage.py` & `tableschema-sql-2.0.0/tableschema_sql/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,44 +46,45 @@
     """
 
     # Public
 
     def __init__(self, engine, dbschema=None, prefix='', reflect_only=None, autoincrement=None):
 
         # Set attributes
-        self.__connection = engine.connect()
+        self.__engine = engine
         self.__dbschema = dbschema
         self.__prefix = prefix
         self.__descriptors = {}
         self.__fallbacks = {}
         self.__autoincrement = autoincrement
         self.__only = reflect_only or (lambda _: True)
         self.__dialect = engine.dialect.name
 
         # Added regex support to sqlite
         if self.__dialect == 'sqlite':
             def regexp(expr, item):
                 reg = re.compile(expr)
                 return reg.search(item) is not None
             # It will fail silently if this function already exists
-            self.__connection.connection.create_function('REGEXP', 2, regexp)
+            with self.__engine.connect() as __connection:
+                __connection.connection.create_function('REGEXP', 2, regexp)
 
         # Create mapper
         self.__mapper = Mapper(prefix=prefix, dialect=self.__dialect)
 
         # Create metadata and reflect
-        self.__metadata = MetaData(bind=self.__connection, schema=self.__dbschema)
+        self.__metadata = MetaData(schema=self.__dbschema)
         self.__reflect()
 
     def __repr__(self):
 
         # Template and format
         template = 'Storage <{engine}/{dbschema}>'
         text = template.format(
-            engine=self.__connection.engine,
+            engine=self.__engine,
             dbschema=self.__dbschema)
 
         return text
 
     @property
     def buckets(self):
         buckets = []
@@ -136,15 +137,15 @@
             Table(table_name, self.__metadata, *(columns + constraints + indexes),
                   comment=table_comment)
             self.__descriptors[bucket] = descriptor
             self.__fallbacks[bucket] = fallbacks
 
         # Create tables, update metadata
         try:
-            self.__metadata.create_all()
+            self.__metadata.create_all(bind=self.__engine)
         except sqlalchemy.exc.ProgrammingError as exception:
             if 'there is no unique constraint matching given keys' in str(exception):
                 message = 'Foreign keys can only reference primary key or unique fields\n%s'
                 six.raise_from(
                     tableschema.exceptions.ValidationError(message % str(exception)),
                     None)
 
@@ -173,15 +174,15 @@
                 del self.__descriptors[bucket]
 
             # Add table to tables
             table = self.__get_table(bucket)
             tables.append(table)
 
         # Drop tables, update metadata
-        self.__metadata.drop_all(tables=tables)
+        self.__metadata.drop_all(tables=tables, bind=self.__engine)
         self.__metadata.clear()
         self.__reflect()
 
     def describe(self, bucket, descriptor=None):
 
         # Set descriptor
         if descriptor is not None:
@@ -201,20 +202,19 @@
     def iter(self, bucket):
 
         # Get table and fallbacks
         table = self.__get_table(bucket)
         schema = tableschema.Schema(self.describe(bucket))
         autoincrement = self.__get_autoincrement_for_bucket(bucket)
 
-        # Open and close transaction
-        with self.__connection.begin():
-            # Streaming could be not working for some backends:
-            # http://docs.sqlalchemy.org/en/latest/core/connections.html
-            select = table.select().execution_options(stream_results=True)
-            result = select.execute()
+        # Streaming could be not working for some backends:
+        # http://docs.sqlalchemy.org/en/latest/core/connections.html
+        select = table.select().execution_options(stream_results=True)
+        with self.__engine.connect() as connection:
+            result = connection.execute(select)
             for row in result:
                 row = self.__mapper.restore_row(
                     row, schema=schema, autoincrement=autoincrement)
                 yield row
 
     def read(self, bucket):
         rows = list(self.iter(bucket))
@@ -248,37 +248,36 @@
         table = self.__get_table(bucket)
         schema = tableschema.Schema(self.describe(bucket))
         fallbacks = self.__fallbacks.get(bucket, [])
 
         # Write rows to table
         convert_row = partial(self.__mapper.convert_row, schema=schema, fallbacks=fallbacks)
         autoincrement = self.__get_autoincrement_for_bucket(bucket)
-        writer = Writer(table, schema,
+        writer = Writer(self.__engine, table, schema,
             # Only PostgreSQL supports "returning" so we don't use autoincrement for all
             autoincrement=autoincrement if self.__dialect in ['postgresql'] else None,
             update_keys=update_keys,
             convert_row=convert_row,
             buffer_size=buffer_size,
             use_bloom_filter=use_bloom_filter)
-        with self.__connection.begin():
-            gen = writer.write(rows, keyed=keyed)
-            if as_generator:
-                return gen
-            collections.deque(gen, maxlen=0)
+        gen = writer.write(rows, keyed=keyed)
+        if as_generator:
+            return gen
+        collections.deque(gen, maxlen=0)
 
     # Private
 
     def __get_table(self, bucket):
         table_name = self.__mapper.convert_bucket(bucket)
         if self.__dbschema:
             table_name = '.'.join((self.__dbschema, table_name))
         return self.__metadata.tables[table_name]
 
     def __reflect(self):
         def only(name, _):
             return self.__only(name) and self.__mapper.restore_bucket(name) is not None
-        self.__metadata.reflect(only=only)
+        self.__metadata.reflect(only=only, bind=self.__engine)
 
     def __get_autoincrement_for_bucket(self, bucket):
         if isinstance(self.__autoincrement, dict):
             return self.__autoincrement.get(bucket)
         return self.__autoincrement
```

### Comparing `tableschema-sql-1.3.2/tableschema_sql/writer.py` & `tableschema-sql-2.0.0/tableschema_sql/writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,107 @@
 # -*- coding: utf-8 -*-
 from __future__ import division
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import pybloom_live
-from sqlalchemy import select
 from collections import namedtuple
 WrittenRow = namedtuple('WrittenRow', ['row', 'updated', 'updated_id'])
 
 
 # Module API
 
 class Writer(object):
 
     # Public
 
-    def __init__(self, table, schema, update_keys,
+    def __init__(self, engine, table, schema, update_keys,
                  autoincrement, convert_row, buffer_size,
                  use_bloom_filter):
         """Writer to insert/update rows into table
         """
+        self.__engine = engine
         self.__table = table
         self.__schema = schema
         self.__update_keys = update_keys
         self.__autoincrement = autoincrement
         self.__convert_row = convert_row
         self.__buffer = []
         self.__buffer_size = buffer_size
         self.__use_bloom_filter = use_bloom_filter
         if update_keys is not None and use_bloom_filter:
-            self.__prepare_bloom()
+            with self.__engine.connect() as connection:
+                self.__prepare_bloom(connection)
 
     def write(self, rows, keyed=False):
         """Write rows/keyed_rows to table
         """
-        for row in rows:
-            keyed_row = row
-            if not keyed:
-                keyed_row = dict(zip(self.__schema.field_names, row))
-            keyed_row = self.__convert_row(keyed_row)
-            if self.__check_existing(keyed_row):
-                for wr in self.__insert():
-                    yield wr
-                ret = self.__update(keyed_row)
-                if ret is not None:
-                    yield WrittenRow(keyed_row, True, ret if self.__autoincrement else None)
-                    continue
-            self.__buffer.append(keyed_row)
-            if len(self.__buffer) > self.__buffer_size:
-                for wr in self.__insert():
-                    yield wr
-        for wr in self.__insert():
-            yield wr
+        with self.__engine.connect() as connection:
+            for row in rows:
+                keyed_row = row
+                if not keyed:
+                    keyed_row = dict(zip(self.__schema.field_names, row))
+                keyed_row = self.__convert_row(keyed_row)
+                if self.__check_existing(keyed_row):
+                    for wr in self.__insert(connection):
+                        yield wr
+                    ret = self.__update(connection, keyed_row)
+                    if ret is not None:
+                        yield WrittenRow(keyed_row, True, ret if self.__autoincrement else None)
+                        continue
+                self.__buffer.append(keyed_row)
+                if len(self.__buffer) > self.__buffer_size:
+                    for wr in self.__insert(connection):
+                        yield wr
+            for wr in self.__insert(connection):
+                yield wr
+            connection.commit()
 
     # Private
 
-    def __prepare_bloom(self):
+    def __prepare_bloom(self, connection):
         """Prepare bloom for existing checks
         """
         self.__bloom = pybloom_live.ScalableBloomFilter()
         columns = [getattr(self.__table.c, key) for key in self.__update_keys]
-        keys = select(columns).execution_options(stream_results=True).execute()
+        keys = connection.execute(self.__table.select().with_only_columns(*columns).execution_options(stream_results=True))
         for key in keys:
             self.__bloom.add(tuple(key))
 
-    def __insert(self):
+    def __insert(self, connection):
         """Insert rows to table
         """
         if len(self.__buffer) > 0:
             # Insert data
             statement = self.__table.insert()
             if self.__autoincrement:
                 statement = statement.returning(
                     getattr(self.__table.c, self.__autoincrement))
                 statement = statement.values(self.__buffer)
-                res = statement.execute()
+                res = connection.execute(statement)
                 for id, in res:
                     row = self.__buffer.pop(0)
                     yield WrittenRow(row, False, id)
             else:
-                statement.execute(self.__buffer)
+                connection.execute(statement, self.__buffer)
                 for row in self.__buffer:
                     yield WrittenRow(row, False, None)
             # Clean memory
             self.__buffer = []
 
-    def __update(self, row):
+    def __update(self, connection, row):
         """Update rows in table
         """
         expr = self.__table.update().values(row)
         for key in self.__update_keys:
             expr = expr.where(getattr(self.__table.c, key) == row[key])
         if self.__autoincrement:
             expr = expr.returning(getattr(self.__table.c, self.__autoincrement))
-        res = expr.execute()
+        res = connection.execute(expr)
         if res.rowcount > 0:
             if self.__autoincrement:
                 first = next(iter(res))
                 last_row_id = first[0]
                 return last_row_id
             return 0
         return None
```

### Comparing `tableschema-sql-1.3.2/tableschema_sql.egg-info/PKG-INFO` & `tableschema-sql-2.0.0/tableschema_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableschema-sql
-Version: 1.3.2
+Version: 2.0.0
 Summary: Generate SQL tables, load and extract data, based on JSON Table Schema descriptors.
 Home-page: https://github.com/frictionlessdata/tableschema-sql-py
 Author: Open Knowledge Foundation
 Author-email: info@okfn.org
 License: MIT
 Keywords: frictionless data
 Platform: UNKNOWN
```

