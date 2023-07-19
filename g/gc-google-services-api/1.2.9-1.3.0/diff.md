# Comparing `tmp/gc_google_services_api-1.2.9.tar.gz` & `tmp/gc_google_services_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc_google_services_api-1.2.9.tar", max compression
+gzip compressed data, was "gc_google_services_api-1.3.0.tar", max compression
```

## Comparing `gc_google_services_api-1.2.9.tar` & `gc_google_services_api-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/LICENSE
--rw-r--r--   0        0        0     4789 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/README.md
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/__init__.py
--rw-r--r--   0        0        0      796 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/__init__.py
--rw-r--r--   0        0        0     2168 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/test_auth.py
--rw-r--r--   0        0        0     2106 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/__init__.py
--rw-r--r--   0        0        0      988 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/test_bigquery.py
--rw-r--r--   0        0        0     4192 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/__init__.py
--rw-r--r--   0        0        0     7927 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/test_calendar.py
--rw-r--r--   0        0        0     1711 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/__init__.py
--rw-r--r--   0        0        0     2827 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/test_gmail.py
--rw-r--r--   0        0        0     2085 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/__init__.py
--rw-r--r--   0        0        0     3635 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/test_gsheet.py
--rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/__init__.py
--rw-r--r--   0        0        0     3281 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/drive.py
--rw-r--r--   0        0        0     3506 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/workspace.py
--rw-r--r--   0        0        0      656 2023-06-29 08:51:32.352630 gc_google_services_api-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4789 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/__init__.py
+-rw-r--r--   0        0        0      796 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/auth/__tests__/__init__.py
+-rw-r--r--   0        0        0     2192 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/auth/__tests__/test_auth.py
+-rw-r--r--   0        0        0     2770 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/bigquery/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/bigquery/__tests__/__init__.py
+-rw-r--r--   0        0        0      988 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0     4192 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/calendar_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/calendar_api/__tests__/__init__.py
+-rw-r--r--   0        0        0     7927 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py
+-rw-r--r--   0        0        0     1711 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gmail/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gmail/__tests__/__init__.py
+-rw-r--r--   0        0        0     2827 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gmail/__tests__/test_gmail.py
+-rw-r--r--   0        0        0     2085 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gsheet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gsheet/__tests__/__init__.py
+-rw-r--r--   0        0        0     3635 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/permissions/__init__.py
+-rw-r--r--   0        0        0     3281 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/permissions/drive.py
+-rw-r--r--   0        0        0     3506 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/gc_google_services_api/permissions/workspace.py
+-rw-r--r--   0        0        0      656 2023-07-19 09:27:01.573099 gc_google_services_api-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 gc_google_services_api-1.3.0/PKG-INFO
```

### Comparing `gc_google_services_api-1.2.9/LICENSE` & `gc_google_services_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/README.md` & `gc_google_services_api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/auth/__init__.py` & `gc_google_services_api-1.3.0/gc_google_services_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/test_auth.py` & `gc_google_services_api-1.3.0/gc_google_services_api/auth/__tests__/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
         service_account.Credentials = from_service_account_info_mock
 
         return service_account
 
     def _create_service_account_with_subject_mock(self, service_account):
         with_subject_mock = Mock()
-        with_subject_mock.with_subject.return_value = "CREDENTIALS_WITH_SUBJECT"  # noqa: E501
+        with_subject_mock.with_subject.return_value = (
+            "CREDENTIALS_WITH_SUBJECT"  # noqa: E501
+        )
         from_service_account_info_mock = Mock()
         from_service_account_info_mock.from_service_account_info.return_value = (  # noqa: E501
             with_subject_mock
         )
 
         service_account.Credentials = from_service_account_info_mock
```

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__init__.py` & `gc_google_services_api-1.3.0/gc_google_services_api/bigquery/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,35 @@
         retry = Retry()
         retry(query_job.result)
 
     def execute_query(self, query="", error_value=[]):
         query_job = self.client.query(query)
 
         try:
-            # Waitig for the query to finish before return
             self.wait_for_job(query_job)
 
             return query_job.result()
         except Exception as e:
             logging.error(f"[ERROR - execute_query]: {e}")
             return error_value
+
+    def load_massive_data(self, rows_to_insert, table_name):
+        job_config = bigquery.LoadJobConfig()
+        job_config.write_disposition = bigquery.WriteDisposition.WRITE_APPEND
+
+        table_ref = self.client.dataset(self.dataset_id).table(table_name)
+
+        load_job = self.client.load_table_from_json(
+            json_rows=rows_to_insert,
+            destination=table_ref,
+            job_config=job_config,
+        )
+
+        load_job.result()
+        is_process_complete = load_job.state == "DONE"
+
+        if is_process_complete:
+            logging.info("Load batch data successfully.")
+        else:
+            logging.error("Error loading data:", load_job.errors)
+
+        return is_process_complete
```

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/test_bigquery.py` & `gc_google_services_api-1.3.0/gc_google_services_api/bigquery/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__init__.py` & `gc_google_services_api-1.3.0/gc_google_services_api/calendar_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/test_calendar.py` & `gc_google_services_api-1.3.0/gc_google_services_api/calendar_api/__tests__/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/gmail/__init__.py` & `gc_google_services_api-1.3.0/gc_google_services_api/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/test_gmail.py` & `gc_google_services_api-1.3.0/gc_google_services_api/gmail/__tests__/test_gmail.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__init__.py` & `gc_google_services_api-1.3.0/gc_google_services_api/gsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/test_gsheet.py` & `gc_google_services_api-1.3.0/gc_google_services_api/gsheet/__tests__/test_gsheet.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/permissions/drive.py` & `gc_google_services_api-1.3.0/gc_google_services_api/permissions/drive.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/gc_google_services_api/permissions/workspace.py` & `gc_google_services_api-1.3.0/gc_google_services_api/permissions/workspace.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.9/pyproject.toml` & `gc_google_services_api-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gc-google-services-api"
-version = "1.2.9"
+version = "1.3.0"
 description = ""
 authors = ["Jonathan Rodríguez Alejos <jrodriguez.5716@gmail.com>"]
 readme = "README.md"
 packages = [{include = "gc_google_services_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `gc_google_services_api-1.2.9/PKG-INFO` & `gc_google_services_api-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gc-google-services-api
-Version: 1.2.9
+Version: 1.3.0
 Summary: 
 Author: Jonathan Rodríguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

