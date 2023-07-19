# Comparing `tmp/pypomes_core-0.1.8.tar.gz` & `tmp/pypomes_core-0.1.9.tar.gz`

## Comparing `pypomes_core-0.1.8.tar` & `pypomes_core-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/README.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_core-0.1.9/PKG-INFO
```

### Comparing `pypomes_core-0.1.8/src/pypomes_core/__init__.py` & `pypomes_core-0.1.9/src/pypomes_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,9 +94,9 @@
     validate_format_error, validate_format_errors,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.8"
-__version_info__ = (0, 1, 8)
+__version__ = "0.1.9"
+__version_info__ = (0, 1, 9)
```

### Comparing `pypomes_core-0.1.8/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/email_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/env_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/file_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/http_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/http_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,40 +201,43 @@
     item: dict = __HTTP_STATUS.get(status_code, {"description": "Unknown status code"})
     result = f"HTTP status code {status_code}: {item.get('description')}"
 
     return result
 
 
 def http_json_from_get(errors: list[str], url: str, headers: dict = None,
-                       params: dict = None, logger: logging.Logger = None) -> dict:
+                       params: dict = None, badge: str = None, logger: logging.Logger = None) -> dict:
 
     if logger is not None:
         logger.info(f"Invoking GET: '{url}'")
 
     # initialize return variable
     result: dict | None = None
 
     try:
         response: requests.Response = requests.get(url=url,
                                                    headers=headers,
                                                    params=params)
         if logger is not None:
             logger.info(f"Invoked '{url}', status: '{http_status_name(response.status_code)}'")
         result = response.json()
+        if badge is not None:
+            result["badge"] = badge
     except Exception as e:
         msg: str = f"Error invoking '{url}': '{exc_format(e, sys.exc_info())}'"
         if logger is not None:
             logger.info(msg)
         errors.append(msg)
 
     return result
 
 
-def http_json_from_post(errors: list[str], url: str, headers: dict = None, params: dict = None,
-                        data: dict = None, json: dict = None, logger: logging.Logger = None) -> dict:
+def http_json_from_post(errors: list[str], url: str, headers: dict = None,
+                        params: dict = None, data: dict = None, json: dict = None,
+                        badge: str = None, logger: logging.Logger = None) -> dict:
 
     if logger is not None:
         logger.info(f"Invoking POST: '{url}'")
 
     # initialize return variable
     result: dict | None = None
 
@@ -243,14 +246,16 @@
                                                     headers=headers,
                                                     data=data,
                                                     json=json,
                                                     params=params)
         if logger is not None:
             logger.info(f"Invoked '{url}', status: '{http_status_name(response.status_code)}'")
         result = response.json()
+        if badge is not None:
+            result["badge"] = badge
     except Exception as e:
         msg: str = f"Error invoking '{url}': '{exc_format(e, sys.exc_info())}'"
         if logger is not None:
             logger.info(msg)
         errors.append(msg)
 
     return result
```

### Comparing `pypomes_core-0.1.8/src/pypomes_core/json_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/list_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/str_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.1.9/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/LICENSE` & `pypomes_core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.1.8/pyproject.toml` & `pypomes_core-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.1.8/PKG-INFO` & `pypomes_core-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

