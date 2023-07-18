# Comparing `tmp/ton-http-api-2.0.8.tar.gz` & `tmp/ton-http-api-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ton-http-api-2.0.8.tar", last modified: Fri Jun 24 21:02:24 2022, max compression
+gzip compressed data, was "ton-http-api-2.0.9.tar", last modified: Sat Jun 25 21:17:00 2022, max compression
```

## Comparing `ton-http-api-2.0.8.tar` & `ton-http-api-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 21:02:24.066121 ton-http-api-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     8541 2022-06-24 21:02:24.066121 ton-http-api-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 21:02:24.066121 ton-http-api-2.0.8/pyTON/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    27883 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    20269 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4300 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7507 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/pyTON/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 21:02:24.066121 ton-http-api-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-06-24 21:02:15.000000 ton-http-api-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 21:02:24.066121 ton-http-api-2.0.8/ton_http_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8541 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 21:02:24.000000 ton-http-api-2.0.8/ton_http_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 21:17:00.190468 ton-http-api-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8541 2022-06-25 21:17:00.190468 ton-http-api-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 21:17:00.186468 ton-http-api-2.0.9/pyTON/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27883 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20269 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4300 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7507 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/pyTON/worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-25 21:17:00.190468 ton-http-api-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-06-25 21:16:50.000000 ton-http-api-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 21:17:00.190468 ton-http-api-2.0.9/ton_http_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8541 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 21:17:00.000000 ton-http-api-2.0.9/ton_http_api.egg-info/zip-safe
```

### Comparing `ton-http-api-2.0.8/PKG-INFO` & `ton-http-api-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ton-http-api
-Version: 2.0.8
+Version: 2.0.9
 Summary: HTTP API for TON (The Open Network)
 Home-page: https://github.com/toncenter/ton-http-api
 Author: K-Dimentional Tree
 Author-email: kdimentionaltree@gmail.com
 License: UNKNOWN
 Description: ![splash_http_api](https://user-images.githubusercontent.com/1449561/154847286-989a6c51-1615-45e1-b40f-aec7c13014fa.png)
```

### Comparing `ton-http-api-2.0.8/README.md` & `ton-http-api-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/cache.py` & `ton-http-api-2.0.9/pyTON/cache.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/cli.py` & `ton-http-api-2.0.9/pyTON/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     logs_args.add_argument('--logs-level', type=str, choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'], default='ERROR', help='Logging level')
     logs_args.add_argument('--logs-jsonify', default=False, action='store_true', help='Print logs in JSON format')
 
     args = parser.parse_args()
     setup_environment(args)
 
     from pyTON.main import app
-    uvicorn.run(app, host=args.host, port=args.port)
+    uvicorn.run(app, host=args.host, port=args.port, log_level=args.logs_level.lower())
```

### Comparing `ton-http-api-2.0.8/pyTON/main.py` & `ton-http-api-2.0.9/pyTON/main.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/manager.py` & `ton-http-api-2.0.9/pyTON/manager.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/models.py` & `ton-http-api-2.0.9/pyTON/models.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/settings.py` & `ton-http-api-2.0.9/pyTON/settings.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/pyTON/worker.py` & `ton-http-api-2.0.9/pyTON/worker.py`

 * *Files identical despite different names*

### Comparing `ton-http-api-2.0.8/setup.py` & `ton-http-api-2.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'loguru>=0.6.0',
         'fastapi>=0.78.0',
         'pydantic>=1.9.1',
         'requests>=2.28.0',
         'ring>=0.9.1',
         'uvicorn>=0.17.6',
         'gunicorn>=20.1.0',
-        'pytonlib==0.0.17',
+        'pytonlib==0.0.20',
         'inject>=4.3.1'
     ],
     package_data={},
     zip_safe=True,
     python_requires='>=3.7',
     classifiers=[
          "Development Status :: 3 - Alpha",
```

### Comparing `ton-http-api-2.0.8/ton_http_api.egg-info/PKG-INFO` & `ton-http-api-2.0.9/ton_http_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ton-http-api
-Version: 2.0.8
+Version: 2.0.9
 Summary: HTTP API for TON (The Open Network)
 Home-page: https://github.com/toncenter/ton-http-api
 Author: K-Dimentional Tree
 Author-email: kdimentionaltree@gmail.com
 License: UNKNOWN
 Description: ![splash_http_api](https://user-images.githubusercontent.com/1449561/154847286-989a6c51-1615-45e1-b40f-aec7c13014fa.png)
```

