# Comparing `tmp/capsulecorp-0.1.6.tar.gz` & `tmp/capsulecorp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.6.tar", last modified: Mon Jul 17 16:04:33 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.7.tar", last modified: Wed Jul 19 14:17:51 2023, max compression
```

## Comparing `capsulecorp-0.1.6.tar` & `capsulecorp-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.573022 capsulecorp-0.1.6/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.6/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 16:04:33.572540 capsulecorp-0.1.6/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.6/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.562995 capsulecorp-0.1.6/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.6/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.6/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.571665 capsulecorp-0.1.6/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.6/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     8833 2023-07-17 16:00:44.000000 capsulecorp-0.1.6/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.6/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.6/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.6/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-17 16:00:59.000000 capsulecorp-0.1.6/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-17 16:04:33.567905 capsulecorp-0.1.6/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-17 16:04:32.000000 capsulecorp-0.1.6/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-17 16:04:32.000000 capsulecorp-0.1.6/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-17 16:04:33.000000 capsulecorp-0.1.6/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.6/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-17 16:04:33.573186 capsulecorp-0.1.6/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.6/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.727478 capsulecorp-0.1.7/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.7/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-19 14:17:51.726590 capsulecorp-0.1.7/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.7/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.705343 capsulecorp-0.1.7/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.7/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.7/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.724106 capsulecorp-0.1.7/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.7/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     8822 2023-07-18 18:00:19.000000 capsulecorp-0.1.7/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.7/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    11719 2023-07-19 13:41:59.000000 capsulecorp-0.1.7/capsulecorp/utilities/s3_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.7/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     5206 2023-07-19 13:43:55.000000 capsulecorp-0.1.7/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-18 16:47:33.000000 capsulecorp-0.1.7/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.712840 capsulecorp-0.1.7/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-19 14:17:50.000000 capsulecorp-0.1.7/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      496 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-19 14:17:50.000000 capsulecorp-0.1.7/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.7/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-19 14:17:51.727766 capsulecorp-0.1.7/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.7/setup.py
```

### Comparing `capsulecorp-0.1.6/LICENSE` & `capsulecorp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.6/capsulecorp/query_driver.py` & `capsulecorp-0.1.7/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.6/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.7/capsulecorp/utilities/databricks_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             token (str): DataBricks API token
             job_id (int): respective job id
 
         Returns:
             request response
     """
     return requests.post(
-        os.path.join(databricks_host, 'api/2.0/jobs/run-now'),
+        os.path.join(host, 'api/2.0/jobs/run-now'),
         headers={"Authorization": f"Bearer {token}"},
         json={"job_id": job_id, **kwargs})
 
 
 def get_run_status(host, token, run_id):
     """
         Get DataBricks run status information given a run id.
```

### Comparing `capsulecorp-0.1.6/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.7/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.6/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.7/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.6/setup.py` & `capsulecorp-0.1.7/setup.py`

 * *Files identical despite different names*

