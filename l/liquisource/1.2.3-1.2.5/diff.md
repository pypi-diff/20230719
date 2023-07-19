# Comparing `tmp/liquisource-1.2.3.tar.gz` & `tmp/liquisource-1.2.5.tar.gz`

## Comparing `liquisource-1.2.3.tar` & `liquisource-1.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 liquisource-1.2.3/requirements.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/ck_client.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/config.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/es_client.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/mongo_client.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/mysql_client.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.3/liquiclient/redis_client.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.3/.gitignore
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 liquisource-1.2.3/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 liquisource-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 liquisource-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 liquisource-1.2.5/requirements.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/ck_client.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/config.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/es_client.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/mongo_client.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/mysql_client.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 liquisource-1.2.5/liquiclient/redis_client.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 liquisource-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 liquisource-1.2.5/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 liquisource-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 liquisource-1.2.5/PKG-INFO
```

### Comparing `liquisource-1.2.3/liquiclient/config.py` & `liquisource-1.2.5/liquiclient/config.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.3/liquiclient/es_client.py` & `liquisource-1.2.5/liquiclient/es_client.py`

 * *Files identical despite different names*

### Comparing `liquisource-1.2.3/liquiclient/mysql_client.py` & `liquisource-1.2.5/liquiclient/mysql_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,38 +8,35 @@
 
 
 # 获取mysql实例
 def get_mysql_client():
     # 由于默认liquibase是jdbc的，这里解析对应的ip port
     params = parse_jdbc_dsn(get_property("url"))
     client = mysql.connector.connect(**params)
-    client.autocommit = True
 
-    return client.cursor()
+    return client
 
 
 def parse_jdbc_dsn(dsn):
     url_str = dsn.lstrip("jdbc:mysql://")
     # 如果URL没有scheme，为其添加默认的http或https
     if not url_str.startswith(('http://', 'https://')):
         url_str = 'http://' + url_str
 
-    print(url_str)
     # 当成url解析
     url_obj = urlparse(url_str)
     query_params = parse_qs(url_obj.query)
-    print(query_params)
+
     # 获取账号密码
     username = get_property("username")
     password = get_property("password")
 
     config = {
         "host": url_obj.hostname,
         "port": url_obj.port,
         "database": url_obj.path.lstrip("/"),
         "user": username,
         "password": password,
         "charset": query_params['characterEncoding'][0],
     }
-    print(config)
 
     return config
```

### Comparing `liquisource-1.2.3/README.md` & `liquisource-1.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,10 +47,11 @@
 
 ```
 
 ## 发布包
 ```python
 python3 -m pip install --upgrade build
 python3 -m build
+python3 -m pip install --upgrade twine
 python3 -m twine upload  dist/*
 
 ```
```

### Comparing `liquisource-1.2.3/pyproject.toml` & `liquisource-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "liquisource"
-version = "1.2.3"
+version = "1.2.5"
 authors = [
   { name="jiyis", email="425995717@qq.com" },
 ]
 description = "A liquibase datasource client for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `liquisource-1.2.3/PKG-INFO` & `liquisource-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquisource
-Version: 1.2.3
+Version: 1.2.5
 Summary: A liquibase datasource client for python
 Project-URL: Homepage, https://github.com/jiyis/liquisource
 Project-URL: Bug Tracker, https://github.com/jiyis/liquisource/issues
 Author-email: jiyis <425995717@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -67,10 +67,11 @@
 
 ```
 
 ## 发布包
 ```python
 python3 -m pip install --upgrade build
 python3 -m build
+python3 -m pip install --upgrade twine
 python3 -m twine upload  dist/*
 
 ```
```

