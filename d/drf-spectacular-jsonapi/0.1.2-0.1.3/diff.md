# Comparing `tmp/drf-spectacular-jsonapi-0.1.2.tar.gz` & `tmp/drf-spectacular-jsonapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-spectacular-jsonapi-0.1.2.tar", last modified: Wed Mar 22 11:43:23 2023, max compression
+gzip compressed data, was "drf-spectacular-jsonapi-0.1.3.tar", last modified: Wed Jul 19 13:11:31 2023, max compression
```

## Comparing `drf-spectacular-jsonapi-0.1.2.tar` & `drf-spectacular-jsonapi-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:23.786537 drf-spectacular-jsonapi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-22 11:43:23.782537 drf-spectacular-jsonapi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:23.782537 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:23.782537 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/plumbing.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:23.782537 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-22 11:43:23.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-22 11:43:23.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:43:23.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-22 11:43:23.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-22 11:43:23.000000 drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 11:43:23.786537 drf-spectacular-jsonapi-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2163 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:43:23.782537 drf-spectacular-jsonapi-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-03-22 11:43:12.000000 drf-spectacular-jsonapi-0.1.2/tests/tests_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/plumbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-19 13:11:31.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-19 13:11:31.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:11:31.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 13:11:31.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 13:11:31.000000 drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2163 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.555642 drf-spectacular-jsonapi-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-07-19 13:11:15.000000 drf-spectacular-jsonapi-0.1.3/tests/tests_schema.py
```

### Comparing `drf-spectacular-jsonapi-0.1.2/LICENSE` & `drf-spectacular-jsonapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/PKG-INFO` & `drf-spectacular-jsonapi-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-spectacular-jsonapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: open api 3 schema generator for drf-json-api package based on drf-spectacular package.
 Home-page: https://github.com/jokiefer/drf-spectecular-json-api
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-spectacular-jsonapi-0.1.2/README.rst` & `drf-spectacular-jsonapi-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/converters.py` & `drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/converters.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/openapi.py` & `drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,21 +197,21 @@
         else:
             schema = build_json_api_data_frame(schema)
         return schema
 
     def _get_response_for_code(self, serializer, status_code, media_types=None, direction='response'):
         response = super()._get_response_for_code(
             serializer, status_code, media_types, direction)
-
-        if "application/vnd.api+json" in response["content"] and "Paginated" not in response["content"]["application/vnd.api+json"]["schema"]["$ref"]:
+        content = response.get("content")
+        if content and "application/vnd.api+json" in content and "Paginated" not in content["application/vnd.api+json"]["schema"]["$ref"]:
             response_component = ResolvedComponent(
                 name=self._get_serializer_name(
                     serializer=serializer, direction=direction)+"Response",
                 type=ResolvedComponent.SCHEMA,
                 schema=build_json_api_data_frame(
-                    response["content"]["application/vnd.api+json"]["schema"]),
+                    content["application/vnd.api+json"]["schema"]),
                 object=serializer.child if is_list_serializer(
                     serializer) else serializer
             )
             self.registry.register_on_missing(response_component)
-            response["content"]["application/vnd.api+json"]["schema"] = response_component.ref
+            content["application/vnd.api+json"]["schema"] = response_component.ref
         return response
```

### Comparing `drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi/schemas/pagination.py` & `drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/PKG-INFO` & `drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-spectacular-jsonapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: open api 3 schema generator for drf-json-api package based on drf-spectacular package.
 Home-page: https://github.com/jokiefer/drf-spectecular-json-api
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-spectacular-jsonapi-0.1.2/drf_spectacular_jsonapi.egg-info/SOURCES.txt` & `drf-spectacular-jsonapi-0.1.3/drf_spectacular_jsonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/setup.py` & `drf-spectacular-jsonapi-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-jsonapi-0.1.2/tests/tests_schema.py` & `drf-spectacular-jsonapi-0.1.3/tests/tests_schema.py`

 * *Files identical despite different names*

