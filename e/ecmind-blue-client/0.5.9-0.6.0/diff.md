# Comparing `tmp/ecmind_blue_client-0.5.9.tar.gz` & `tmp/ecmind_blue_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecmind_blue_client-0.5.9.tar", last modified: Fri Mar 24 06:13:34 2023, max compression
+gzip compressed data, was "ecmind_blue_client-0.6.0.tar", last modified: Wed Jul 19 10:24:14 2023, max compression
```

## Comparing `ecmind_blue_client-0.5.9.tar` & `ecmind_blue_client-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-03-24 06:13:34.318791 ecmind_blue_client-0.5.9/
--rw-r--r--   0 rk        (1000) rk        (1000)     1069 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/LICENSE
--rw-r--r--   0 rk        (1000) rk        (1000)     2138 2023-03-24 06:13:34.318791 ecmind_blue_client-0.5.9/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)     1443 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/README.md
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-03-24 06:13:34.315457 ecmind_blue_client-0.5.9/ecmind_blue_client/
--rw-r--r--   0 rk        (1000) rk        (1000)      421 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/__init__.py
--rw-r--r--   0 rk        (1000) rk        (1000)      303 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/blue_exception.py
--rw-r--r--   0 rk        (1000) rk        (1000)    25250 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/client.py
--rw-r--r--   0 rk        (1000) rk        (1000)     3471 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/com_client.py
--rw-r--r--   0 rk        (1000) rk        (1000)    21895 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/const.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1006 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/dms_result.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2280 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/job.py
--rw-r--r--   0 rk        (1000) rk        (1000)     7352 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/options.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1890 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/param.py
--rw-r--r--   0 rk        (1000) rk        (1000)     3953 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/query_condition_field.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2234 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/query_condition_group.py
--rw-r--r--   0 rk        (1000) rk        (1000)     1958 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/query_result_field.py
--rw-r--r--   0 rk        (1000) rk        (1000)      998 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/result.py
--rw-r--r--   0 rk        (1000) rk        (1000)     2758 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/result_file.py
--rw-r--r--   0 rk        (1000) rk        (1000)     4696 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/soap_client.py
--rw-r--r--   0 rk        (1000) rk        (1000)     5910 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client.py
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-03-24 06:13:34.318791 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/
--rw-r--r--   0 rk        (1000) rk        (1000)        0 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/__init__.py
--rw-r--r--   0 rk        (1000) rk        (1000)      322 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/call_job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)      263 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/file_footer.py
--rw-r--r--   0 rk        (1000) rk        (1000)      688 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/file_header.py
--rw-r--r--   0 rk        (1000) rk        (1000)    17936 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_caller.py
--rw-r--r--   0 rk        (1000) rk        (1000)      616 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_header.py
--rw-r--r--   0 rk        (1000) rk        (1000)      254 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_parameter_data.py
--rw-r--r--   0 rk        (1000) rk        (1000)      207 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_parameter_description.py
--rw-r--r--   0 rk        (1000) rk        (1000)      552 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)      177 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/response_job_error_data.py
--rw-r--r--   0 rk        (1000) rk        (1000)      301 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/response_job_error_description.py
--rw-r--r--   0 rk        (1000) rk        (1000)      427 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/response_job_errors.py
--rw-r--r--   0 rk        (1000) rk        (1000)      373 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/response_job_parameters.py
--rw-r--r--   0 rk        (1000) rk        (1000)     5121 2023-03-24 06:07:27.000000 ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_pool_client.py
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-03-24 06:13:34.315457 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/
--rw-r--r--   0 rk        (1000) rk        (1000)     2138 2023-03-24 06:13:34.000000 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)     1574 2023-03-24 06:13:34.000000 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/SOURCES.txt
--rw-r--r--   0 rk        (1000) rk        (1000)        1 2023-03-24 06:13:34.000000 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/dependency_links.txt
--rw-r--r--   0 rk        (1000) rk        (1000)      314 2023-03-24 06:13:34.000000 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/requires.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       19 2023-03-24 06:13:34.000000 ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/top_level.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       38 2023-03-24 06:13:34.318791 ecmind_blue_client-0.5.9/setup.cfg
--rw-r--r--   0 rk        (1000) rk        (1000)     1370 2023-03-24 06:11:12.000000 ecmind_blue_client-0.5.9/setup.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-07-19 10:24:14.623458 ecmind_blue_client-0.6.0/
+-rw-r--r--   0 rk        (1000) rk        (1000)     1069 2020-10-31 20:41:55.000000 ecmind_blue_client-0.6.0/LICENSE
+-rw-r--r--   0 rk        (1000) rk        (1000)     2138 2023-07-19 10:24:14.620125 ecmind_blue_client-0.6.0/PKG-INFO
+-rw-r--r--   0 rk        (1000) rk        (1000)     1443 2021-04-09 09:47:25.000000 ecmind_blue_client-0.6.0/README.md
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-07-19 10:24:14.620125 ecmind_blue_client-0.6.0/ecmind_blue_client/
+-rw-r--r--   0 rk        (1000) rk        (1000)      421 2022-08-23 12:31:26.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/__init__.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      303 2022-08-23 08:56:05.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/blue_exception.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    25250 2023-06-22 08:52:34.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     3471 2022-08-23 09:09:55.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/com_client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    21895 2023-06-22 08:52:34.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/const.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1006 2022-08-23 12:30:43.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/dms_result.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2280 2022-08-23 09:25:30.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/job.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     7352 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/options.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1890 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/param.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     3953 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/query_condition_field.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2234 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/query_condition_group.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     1958 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/query_result_field.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      998 2022-08-23 12:34:27.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/result.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     2758 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/result_file.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     4696 2022-08-23 09:14:46.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/soap_client.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     5910 2022-08-23 08:57:47.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-07-19 10:24:14.620125 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/
+-rw-r--r--   0 rk        (1000) rk        (1000)        0 2020-11-03 20:07:55.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/__init__.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      322 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/call_job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      263 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/file_footer.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      688 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/file_header.py
+-rw-r--r--   0 rk        (1000) rk        (1000)    17844 2023-07-19 10:20:01.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_caller.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      616 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_header.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      254 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_parameter_data.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      207 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_parameter_description.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      552 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      177 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/response_job_error_data.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      301 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/response_job_error_description.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      427 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/response_job_errors.py
+-rw-r--r--   0 rk        (1000) rk        (1000)      373 2022-07-13 09:00:02.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/response_job_parameters.py
+-rw-r--r--   0 rk        (1000) rk        (1000)     5121 2023-06-22 08:52:34.000000 ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_pool_client.py
+drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-07-19 10:24:14.620125 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/
+-rw-r--r--   0 rk        (1000) rk        (1000)     2138 2023-07-19 10:24:14.000000 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/PKG-INFO
+-rw-r--r--   0 rk        (1000) rk        (1000)     1574 2023-07-19 10:24:14.000000 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/SOURCES.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)        1 2023-07-19 10:24:14.000000 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/dependency_links.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)      314 2023-07-19 10:24:14.000000 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/requires.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)       19 2023-07-19 10:24:14.000000 ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/top_level.txt
+-rw-r--r--   0 rk        (1000) rk        (1000)       38 2023-07-19 10:24:14.623458 ecmind_blue_client-0.6.0/setup.cfg
+-rw-r--r--   0 rk        (1000) rk        (1000)     1370 2023-07-19 10:23:20.000000 ecmind_blue_client-0.6.0/setup.py
```

### Comparing `ecmind_blue_client-0.5.9/LICENSE` & `ecmind_blue_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/PKG-INFO` & `ecmind_blue_client-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmind_blue_client
-Version: 0.5.9
+Version: 0.6.0
 Summary: A client wrapper for blue
 Home-page: https://gitlab.ecmind.ch/open/ecmind_blue_client
 Author: Ulrich Wohlfeil, Roland Koller
 Author-email: info@ecmind.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecmind_blue_client-0.5.9/README.md` & `ecmind_blue_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/client.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/com_client.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/com_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/const.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/const.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/dms_result.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/dms_result.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/job.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/job.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/options.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/options.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/param.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/param.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/query_condition_field.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/query_condition_field.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/query_condition_group.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/query_condition_group.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/query_result_field.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/query_result_field.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/result.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/result.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/result_file.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/result_file.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/soap_client.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/soap_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/file_header.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/file_header.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_caller.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_caller.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,16 +306,15 @@
         )
 
     def parse_response_body(self, body_raw):
         result = {}
 
         # Read Mode
         mode = unpack("s", body_raw[0:1])[0]  # Always R
-
-        logging.debug("Mode is %s", mode)
+        
         body_raw = body_raw[1:]  # drop bytes
 
         # Read Internal Parameters
         internal_length = unpack(">i", body_raw[0:4])[0]  # read byte length of internal parameters
         body_raw = body_raw[4:]  # drop bytes
 
         internal_raw = body_raw[:internal_length]  # slice internal parameters
@@ -330,15 +329,14 @@
         params_raw = body_raw[:params_length]  # slice parameters
         body_raw = body_raw[params_length:]  # drop bytes
 
         result["parameters"] = self.parse_parameters(params_raw)
 
         # Read Errors
         error_length = unpack(">i", body_raw[0:4])[0]  # read byte length of errors
-        logging.debug("Error length is %s", error_length)
         error_raw = body_raw[4:]  # drop bytes
 
         result["errors"] = self.parse_errors(error_raw)
 
         return result
 
     def parse_parameters(self, params_raw):
```

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_header.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_header.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_client_classes/job_parameters.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_client_classes/job_parameters.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client/tcp_pool_client.py` & `ecmind_blue_client-0.6.0/ecmind_blue_client/tcp_pool_client.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/PKG-INFO` & `ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmind-blue-client
-Version: 0.5.9
+Version: 0.6.0
 Summary: A client wrapper for blue
 Home-page: https://gitlab.ecmind.ch/open/ecmind_blue_client
 Author: Ulrich Wohlfeil, Roland Koller
 Author-email: info@ecmind.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecmind_blue_client-0.5.9/ecmind_blue_client.egg-info/SOURCES.txt` & `ecmind_blue_client-0.6.0/ecmind_blue_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client-0.5.9/setup.py` & `ecmind_blue_client-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ecmind_blue_client",
-    version="0.5.9",
+    version="0.6.0",
     author="Ulrich Wohlfeil, Roland Koller",
     author_email="info@ecmind.ch",
     description="A client wrapper for blue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.ecmind.ch/open/ecmind_blue_client",
     packages=setuptools.find_packages(),
```

