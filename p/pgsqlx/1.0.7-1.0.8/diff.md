# Comparing `tmp/pgsqlx-1.0.7.tar.gz` & `tmp/pgsqlx-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.7.tar", last modified: Wed Jul 19 06:33:47 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.8.tar", last modified: Wed Jul 19 06:54:59 2023, max compression
```

## Comparing `pgsqlx-1.0.7.tar` & `pgsqlx-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx/
--rw-rw-rw-   0        0        0      239 2023-07-19 06:33:03.000000 pgsqlx-1.0.7/pgsqlx/config_holder.py
--rw-rw-rw-   0        0        0      561 2023-07-19 05:39:26.000000 pgsqlx-1.0.7/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19514 2023-07-19 06:33:03.000000 pgsqlx-1.0.7/pgsqlx/db.py
--rw-rw-rw-   0        0        0     7471 2023-07-19 06:33:02.000000 pgsqlx-1.0.7/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.7/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    38370 2023-07-19 06:33:03.000000 pgsqlx-1.0.7/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-07-19 06:32:34.000000 pgsqlx-1.0.7/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     6386 2023-07-19 06:33:03.000000 pgsqlx-1.0.7/pgsqlx/sql_holder.py
--rw-rw-rw-   0        0        0     5113 2023-07-19 06:33:02.000000 pgsqlx-1.0.7/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6511 2023-07-19 06:33:02.000000 pgsqlx-1.0.7/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.7/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4268 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      402 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4268 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-19 06:33:47.000000 pgsqlx-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-19 06:33:44.000000 pgsqlx-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx/
+-rw-rw-rw-   0        0        0      239 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/config_holder.py
+-rw-rw-rw-   0        0        0      561 2023-07-19 05:39:26.000000 pgsqlx-1.0.8/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0    19514 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     7471 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.8/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0    38451 2023-07-19 06:53:41.000000 pgsqlx-1.0.8/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-07-19 06:32:34.000000 pgsqlx-1.0.8/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0     6386 2023-07-19 06:33:03.000000 pgsqlx-1.0.8/pgsqlx/sql_holder.py
+-rw-rw-rw-   0        0        0     5113 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6511 2023-07-19 06:33:02.000000 pgsqlx-1.0.8/pgsqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.8/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4268 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      402 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4268 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:54:59.000000 pgsqlx-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-07-19 06:54:56.000000 pgsqlx-1.0.8/setup.py
```

### Comparing `pgsqlx-1.0.7/pgsqlx/constant.py` & `pgsqlx-1.0.8/pgsqlx/constant.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/db.py` & `pgsqlx-1.0.8/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/dbx.py` & `pgsqlx-1.0.8/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/log_support.py` & `pgsqlx-1.0.8/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/orm.py` & `pgsqlx-1.0.8/pgsqlx/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -854,14 +854,16 @@
         return "{} in({})".format(k[:-4], ','.join(['?' for _ in v])), v
     if k.endswith("__in"):
         return "{} in({})".format(k[:-4], '?'), v
     if k.endswith("__not_in") and isinstance(v, Sequence) and not isinstance(v, str):
         return "{} not in({})".format(k[:-8], ','.join(['?' for _ in v])), v
     if k.endswith("__not_in"):
         return "{} not in({})".format(k[:-8], '?'), v
+    if k.endswith("__like"):
+        return "{} like ?".format(k[:-6], '?'), v
     if k.endswith("__startswith"):
         return "{} like ?".format(k[:-12]), '{}%'.format(v)
     if k.endswith("__endswith"):
         return "{} like ?".format(k[:-10]), '%{}'.format(v)
     if k.endswith("__contains"):
         return "{} like ?".format(k[:-10]), '%{}%'.format(v)
     if k.endswith("__range") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
```

### Comparing `pgsqlx-1.0.7/pgsqlx/snowflake.py` & `pgsqlx-1.0.8/pgsqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/sql_holder.py` & `pgsqlx-1.0.8/pgsqlx/sql_holder.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/sql_mapper.py` & `pgsqlx-1.0.8/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx/support.py` & `pgsqlx-1.0.8/pgsqlx/support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.8/pgsqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.7
+Version: 1.0.8
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.7/PKG-INFO` & `pgsqlx-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.7
+Version: 1.0.8
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.7/README.rst` & `pgsqlx-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.7/setup.py` & `pgsqlx-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.7',
+    version='1.0.8',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

