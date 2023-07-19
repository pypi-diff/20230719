# Comparing `tmp/vango-1.1.0.tar.gz` & `tmp/vango-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vango-1.1.0.tar", last modified: Tue Jul 18 01:43:44 2023, max compression
+gzip compressed data, was "dist/vango-1.1.1.tar", last modified: Wed Jul 19 03:02:36 2023, max compression
```

## Comparing `vango-1.1.0.tar` & `vango-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-18 01:43:44.000000 vango-1.1.0/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-18 01:43:44.000000 vango-1.1.0/PKG-INFO
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-18 01:43:44.000000 vango-1.1.0/vango.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-18 01:43:44.000000 vango-1.1.0/vango.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      198 2023-07-18 01:43:44.000000 vango-1.1.0/vango.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)       11 2023-07-18 01:43:44.000000 vango-1.1.0/vango.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-18 01:43:44.000000 vango-1.1.0/vango.egg-info/dependency_links.txt
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-18 01:43:44.000000 vango-1.1.0/vango/
--rw-r--r--   0 jan        (501) staff       (20)     2192 2023-07-18 01:41:31.000000 vango-1.1.0/vango/openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.1.0/vango/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)      523 2023-07-18 01:41:31.000000 vango-1.1.0/setup.py
--rw-r--r--   0 jan        (501) staff       (20)       59 2023-07-18 01:43:44.000000 vango-1.1.0/setup.cfg
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-18 01:43:44.000000 vango-1.1.0/VGPY/
--rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.1.0/VGPY/vango_openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.1.0/VGPY/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-19 03:02:36.000000 vango-1.1.1/PKG-INFO
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      198 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)       11 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-19 03:02:36.000000 vango-1.1.1/vango.egg-info/dependency_links.txt
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/vango/
+-rw-r--r--   0 jan        (501) staff       (20)     2337 2023-07-19 03:02:28.000000 vango-1.1.1/vango/openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.1.1/vango/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)      523 2023-07-19 03:02:28.000000 vango-1.1.1/setup.py
+-rw-r--r--   0 jan        (501) staff       (20)       59 2023-07-19 03:02:36.000000 vango-1.1.1/setup.cfg
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-19 03:02:36.000000 vango-1.1.1/VGPY/
+-rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.1.1/VGPY/vango_openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.1.1/VGPY/__init__.py
```

### Comparing `vango-1.1.0/vango/openapi.py` & `vango-1.1.1/vango/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,31 @@
 # 上传文件
 # task_id 任务ID 必填
 # file_path 本地文件路径 必填
 # options 额外参数 非必填
 def upload_task_file(task_id, file_path, options):
     data = {"task_id": task_id, "options": options}
 
-    with open(file_path, "rb") as upload_file:
-        files = {"file": upload_file}
+    try:
+        with open(file_path, "rb") as upload_file:
+            files = {"file": upload_file}
+
+            sign, userName, timestamp = _get_sign()
+            headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
+                       "VG-Request-Time": str(timestamp), "VG-Request-App": "openapi"}
+            url = 'http://internal.vango_openapi.data-ad.37ops.com/openapi/task/file_upload'
+
+            response = requests.post(url=url, files=files, data=data, headers=headers)
+            if response.status_code == 200:
+                return json.loads(response.text)
+            return response.json()
+
+    except Exception as e:
+            return '文件上传错误：{e}'
 
-        sign, userName, timestamp = _get_sign()
-        headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
-                   "VG-Request-Time": str(timestamp)}
-        url = 'http://dev.vango_tapd_1166744_openapi.data-ad.37ops.com/openapi/task/file_upload'
-
-        response = requests.post(url=url, files=files, data=data, headers=headers)
-        if response.status_code == 200:
-            return json.loads(response.text)
-        return response.json()
 
 
 def _get_sign():
     user = _get_user_info()
     userName = ''
     password = ''
     if user[0]:
```

### Comparing `vango-1.1.0/setup.py` & `vango-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='vango',
-    version='1.1.0',
+    version='1.1.1',
     description='van go open api',
     author='JanVee',
     author_email='814107539@qq.com',
     packages=find_packages(),
     install_requires=[],
     keywords = ("vango", "VGPY"),
     long_description = "An feature extraction algorithm, van_go open api",
```

### Comparing `vango-1.1.0/VGPY/vango_openapi.py` & `vango-1.1.1/VGPY/vango_openapi.py`

 * *Files identical despite different names*

