# Comparing `tmp/psyqlepg-0.0.1.tar.gz` & `tmp/psyqlepg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyqlepg-0.0.1.tar", last modified: Sat Jun 24 16:14:25 2023, max compression
+gzip compressed data, was "psyqlepg-0.0.2.tar", last modified: Wed Jul 19 09:24:10 2023, max compression
```

## Comparing `psyqlepg-0.0.1.tar` & `psyqlepg-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-24 16:14:25.565484 psyqlepg-0.0.1/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1515 2023-06-24 15:55:25.000000 psyqlepg-0.0.1/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      515 2023-06-24 16:14:25.565484 psyqlepg-0.0.1/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      502 2023-06-24 15:58:41.000000 psyqlepg-0.0.1/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-24 16:14:25.565484 psyqlepg-0.0.1/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-24 16:14:25.564484 psyqlepg-0.0.1/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-24 16:14:25.564484 psyqlepg-0.0.1/src/psyqlepg/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2812 2023-06-24 16:03:48.000000 psyqlepg-0.0.1/src/psyqlepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-24 16:14:25.565484 psyqlepg-0.0.1/src/psyqlepg.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      515 2023-06-24 16:14:25.000000 psyqlepg-0.0.1/src/psyqlepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      191 2023-06-24 16:14:25.000000 psyqlepg-0.0.1/src/psyqlepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-24 16:14:25.000000 psyqlepg-0.0.1/src/psyqlepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        9 2023-06-24 16:14:25.000000 psyqlepg-0.0.1/src/psyqlepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.113987 psyqlepg-0.0.2/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.2/LICENSE
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      565 2023-07-19 09:24:10.112987 psyqlepg-0.0.2/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       49 2023-07-19 09:20:45.000000 psyqlepg-0.0.2/README.md
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-19 09:21:34.000000 psyqlepg-0.0.2/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-19 09:24:10.113987 psyqlepg-0.0.2/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.107987 psyqlepg-0.0.2/src/
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.111987 psyqlepg-0.0.2/src/psyqlepg/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4177 2023-07-19 09:22:09.000000 psyqlepg-0.0.2/src/psyqlepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.112987 psyqlepg-0.0.2/src/psyqlepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      565 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/top_level.txt
```

### Comparing `psyqlepg-0.0.1/LICENSE` & `psyqlepg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psyqlepg-0.0.1/src/psyqlepg/__init__.py` & `psyqlepg-0.0.2/src/psyqlepg/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from psycopg import sql
+import re
 
 
 def selectone(conn, table, primary_key, identifier):
     query = sql.SQL('''
         select *
         from {table}
         where {primary_key} = %s
@@ -63,14 +64,33 @@
             table=sql.Identifier(table),
             params=sql.SQL(', ').join(params),
             primary_key=sql.Identifier(primary_key))
 
     return conn.execute(query, [*values, identifier])
 
 
+def load_queries(filename):
+    with open(filename) as file:
+        name = None
+        queries = {}
+
+        for line in file:
+            p = re.compile('-- *#([a-z][a-z0-9_]*)', re.IGNORECASE)
+
+            if (m := p.search(line)):
+                name = m.group(1)
+            elif name is not None:
+                if name not in queries:
+                    queries[name] = line
+                else:
+                    queries[name] += line
+
+        return queries
+
+
 class Where:
     def __init__(self, name=None, value=None):
         self.params = []
         self.args = []
         if (name):
             self.append(name, value)
 
@@ -92,14 +112,42 @@
 
 
     def as_string(self, context):
         return self.clause().as_string(context)
 
 
 class Table:
+    queries = None
+
     @classmethod
-    def get(cls, conn, identifier, key = None):
+    def get(cls, conn, identifier, key=None):
         return selectone(conn, cls.table, key or cls.primary_key, identifier)
 
     @classmethod
-    def fetch(cls, conn, where):
+    def find(cls, conn, where):
         return selectall(conn, cls.table, where)
+
+    @classmethod
+    def insert(cls, conn, **kwargs):
+        return insert(conn, cls.table, cls.primary_key, **kwargs)
+
+    @classmethod
+    def update(cls, conn, identifier, key=None, **kwargs):
+        return update(conn, cls.table, key or cls.primary_key, identifier, **kwargs)
+
+    @classmethod
+    def query(cls, query_name):
+        if cls.queries is None:
+            cls.queries = load_queries(cls.queryfile)
+        return cls.queries[query_name]
+
+    @classmethod
+    def queryone(cls, conn, query_name, params=None, **kwargs):
+        query = cls.query(query_name)
+        cur = conn.execute(query, params, **kwargs)
+        return cur.fetchone()
+
+    @classmethod
+    def queryall(cls, conn, query_name, params=None, **kwargs):
+        query = cls.query(query_name)
+        cur = conn.execute(query, params, **kwargs)
+        return cur.fetchall()
```

