# Comparing `tmp/easy_crud_repo_service-0.1.2.tar.gz` & `tmp/easy_crud_repo_service-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_crud_repo_service-0.1.2.tar", max compression
+gzip compressed data, was "easy_crud_repo_service-0.1.3.tar", max compression
```

## Comparing `easy_crud_repo_service-0.1.2.tar` & `easy_crud_repo_service-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.2/easy_crud_repo_service/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 19:59:22.482391 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/__init__.py
--rw-r--r--   0        0        0      183 2023-04-23 20:02:18.331784 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/player.py
--rw-r--r--   0        0        0      146 2023-04-23 20:02:18.341597 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/team.py
--rw-r--r--   0        0        0        0 2023-04-23 20:00:48.714154 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 20:36:23.143148 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/__init__.py
--rw-r--r--   0        0        0     3974 2023-05-03 04:14:11.478426 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/builders.py
--rw-r--r--   0        0        0     1121 2023-05-03 04:14:11.503306 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/get_connection_pool.py
--rw-r--r--   0        0        0     5605 2023-05-03 04:20:43.332850 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/crud_repo.py
--rw-r--r--   0        0        0      582 2023-05-03 04:56:01.714891 easy_crud_repo_service-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9657 2023-05-03 04:07:14.199155 easy_crud_repo_service-0.1.2/README.md
--rw-r--r--   0        0        0     9862 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.3/easy_crud_repo_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:59:22.482391 easy_crud_repo_service-0.1.3/easy_crud_repo_service/model/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-19 15:56:52.181084 easy_crud_repo_service-0.1.3/easy_crud_repo_service/model/car.py
+-rw-r--r--   0        0        0      141 2023-07-19 15:56:40.506857 easy_crud_repo_service-0.1.3/easy_crud_repo_service/model/order.py
+-rw-r--r--   0        0        0      183 2023-07-19 15:56:40.511887 easy_crud_repo_service-0.1.3/easy_crud_repo_service/model/player.py
+-rw-r--r--   0        0        0      146 2023-07-19 15:56:40.517858 easy_crud_repo_service-0.1.3/easy_crud_repo_service/model/team.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:00:48.714154 easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:36:23.143148 easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/connections/__init__.py
+-rw-r--r--   0        0        0     3974 2023-05-03 04:14:11.478426 easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/connections/builders.py
+-rw-r--r--   0        0        0     1121 2023-05-03 04:14:11.503306 easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/connections/get_connection_pool.py
+-rw-r--r--   0        0        0     5626 2023-07-19 15:51:11.979283 easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/crud_repo.py
+-rw-r--r--   0        0        0      582 2023-07-19 16:01:38.508754 easy_crud_repo_service-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9657 2023-05-03 04:07:14.199155 easy_crud_repo_service-0.1.3/README.md
+-rw-r--r--   0        0        0     9862 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.3/PKG-INFO
```

### Comparing `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/builders.py` & `easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/connections/builders.py`

 * *Files identical despite different names*

### Comparing `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/get_connection_pool.py` & `easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/connections/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/crud_repo.py` & `easy_crud_repo_service-0.1.3/easy_crud_repo_service/repo/crud_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         try:
             if connection_object.is_connected():
                 cursor_object = connection_object.cursor()
                 yield cursor_object
                 connection_object.commit()
         except Error as e:
             connection_object.rollback()
+            raise e
         finally:
             if connection_object.is_connected():
                 cursor_object.close()
                 connection_object.close()
 
     def _table_name(self) -> str:
         """ Creates table name using inflection.tableize() that will change expression for lowercase plural"""
```

### Comparing `easy_crud_repo_service-0.1.2/pyproject.toml` & `easy_crud_repo_service-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy-crud-repo-service"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Smolke <d.smolczynski1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "easy_crud_repo_service"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `easy_crud_repo_service-0.1.2/README.md` & `easy_crud_repo_service-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `easy_crud_repo_service-0.1.2/PKG-INFO` & `easy_crud_repo_service-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-crud-repo-service
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbm-database-service (>=0.2.5,<0.3.0)
```

