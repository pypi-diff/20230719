# Comparing `tmp/tencentcloud-dlc-provider-0.0.2.tar.gz` & `tmp/tencentcloud-dlc-provider-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencentcloud-dlc-provider-0.0.2.tar", last modified: Tue May 30 08:35:03 2023, max compression
+gzip compressed data, was "tencentcloud-dlc-provider-0.0.3.tar", last modified: Wed Jul 19 04:29:33 2023, max compression
```

## Comparing `tencentcloud-dlc-provider-0.0.2.tar` & `tencentcloud-dlc-provider-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.157075 tencentcloud-dlc-provider-0.0.2/
--rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 08:35:03.156746 tencentcloud-dlc-provider-0.0.2/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-30 08:35:03.157175 tencentcloud-dlc-provider-0.0.2/setup.cfg
--rw-r--r--   0 huangzheng   (501) staff       (20)      401 2023-05-30 08:34:32.000000 tencentcloud-dlc-provider-0.0.2/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.151569 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/
--rw-r--r--   0 huangzheng   (501) staff       (20)      362 2023-05-29 11:55:16.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.154976 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7840 2023-05-30 02:28:26.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/dlc_hook.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.156029 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2746 2023-05-30 08:03:13.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/dlc_operator.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.154257 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      530 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       95 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       26 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/top_level.txt
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-07-19 04:29:33.547627 tencentcloud-dlc-provider-0.0.3/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-07-19 04:29:33.547126 tencentcloud-dlc-provider-0.0.3/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-07-19 04:29:33.547788 tencentcloud-dlc-provider-0.0.3/setup.cfg
+-rw-r--r--   0 huangzheng   (501) staff       (20)      401 2023-07-19 04:29:17.000000 tencentcloud-dlc-provider-0.0.3/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-07-19 04:29:33.539188 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      362 2023-05-29 11:55:16.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-07-19 04:29:33.544247 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7841 2023-07-19 04:24:04.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/hooks/dlc_hook.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-07-19 04:29:33.545895 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2746 2023-05-30 08:03:13.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/operators/dlc_operator.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-07-19 04:29:33.542851 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      530 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       95 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       26 2023-07-19 04:29:33.000000 tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/top_level.txt
```

### Comparing `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/dlc_hook.py` & `tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/hooks/dlc_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         describe_data_engine_req.Filters = [describe_data_engine_req_filter]
         LOG.info(f"describe_data_engine_req: [{vars(describe_data_engine_req)}]")
         describe_data_engine_rsp = client.DescribeDataEngines(describe_data_engine_req)
         if len(describe_data_engine_rsp.DataEngines) == 0:
             LOG.error(f"DataEngine: [{engine}] is not exist! ")
             return set()
         task_type = "SQLTask"
-        if describe_data_engine_rsp.DataEngines[0].EngineType.lower().find("spark") > 0:
+        if describe_data_engine_rsp.DataEngines[0].EngineType.lower().find("spark") >= 0:
             task_type = "SparkSQLTask"
 
         request = models.CreateTasksRequest()
         request.Tasks = models.TasksInfo()
         request.DatabaseName = ""
         request.DataEngineName = engine
         request.Tasks.SQL = base64.b64encode(sql.encode('utf8')).decode('utf8')
```

### Comparing `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/dlc_operator.py` & `tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider/operators/dlc_operator.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/SOURCES.txt` & `tencentcloud-dlc-provider-0.0.3/tencentcloud_dlc_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

