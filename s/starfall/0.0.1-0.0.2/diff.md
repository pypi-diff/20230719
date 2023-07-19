# Comparing `tmp/starfall-0.0.1.tar.gz` & `tmp/starfall-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfall-0.0.1.tar", last modified: Wed Jul 19 09:18:53 2023, max compression
+gzip compressed data, was "starfall-0.0.2.tar", last modified: Wed Jul 19 10:08:27 2023, max compression
```

## Comparing `starfall-0.0.1.tar` & `starfall-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 09:18:53.642910 starfall-0.0.1/
--rw-r--r--   0 alex       (501) staff       (20)     1060 2023-07-18 09:52:27.000000 starfall-0.0.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     2090 2023-07-19 09:18:53.642785 starfall-0.0.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      127 2023-07-18 10:21:28.000000 starfall-0.0.1/README.md
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-19 09:18:53.642951 starfall-0.0.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1842 2023-07-19 08:54:32.000000 starfall-0.0.1/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 09:18:53.641730 starfall-0.0.1/starfall/
--rw-r--r--   0 alex       (501) staff       (20)      139 2023-07-19 03:13:28.000000 starfall-0.0.1/starfall/__init__.py
--rw-rw-r--   0 alex       (501) staff       (20)     9164 2023-07-19 03:14:37.000000 starfall-0.0.1/starfall/executor.py
--rw-rw-r--   0 alex       (501) staff       (20)     7705 2023-07-19 03:10:38.000000 starfall-0.0.1/starfall/helper.py
--rw-rw-r--   0 alex       (501) staff       (20)     5957 2023-07-19 03:26:39.000000 starfall-0.0.1/starfall/main.py
--rw-r--r--   0 alex       (501) staff       (20)      286 2023-07-19 03:13:14.000000 starfall-0.0.1/starfall/start.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 09:18:53.642584 starfall-0.0.1/starfall.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     2090 2023-07-19 09:18:53.000000 starfall-0.0.1/starfall.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      312 2023-07-19 09:18:53.000000 starfall-0.0.1/starfall.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-19 09:18:53.000000 starfall-0.0.1/starfall.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-19 09:17:40.000000 starfall-0.0.1/starfall.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       33 2023-07-19 09:18:53.000000 starfall-0.0.1/starfall.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-07-19 09:18:53.000000 starfall-0.0.1/starfall.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 10:08:27.701397 starfall-0.0.2/
+-rw-r--r--   0 alex       (501) staff       (20)     1060 2023-07-18 09:52:27.000000 starfall-0.0.2/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     2086 2023-07-19 10:08:27.701279 starfall-0.0.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      124 2023-07-19 09:25:47.000000 starfall-0.0.2/README.md
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-19 10:08:27.701447 starfall-0.0.2/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1842 2023-07-19 08:54:32.000000 starfall-0.0.2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 10:08:27.700351 starfall-0.0.2/starfall/
+-rw-r--r--   0 alex       (501) staff       (20)      162 2023-07-19 09:43:07.000000 starfall-0.0.2/starfall/__init__.py
+-rw-rw-r--   0 alex       (501) staff       (20)     9162 2023-07-19 10:06:26.000000 starfall-0.0.2/starfall/executor.py
+-rw-rw-r--   0 alex       (501) staff       (20)     6399 2023-07-19 10:01:44.000000 starfall-0.0.2/starfall/helper.py
+-rw-rw-r--   0 alex       (501) staff       (20)     7290 2023-07-19 10:07:10.000000 starfall-0.0.2/starfall/main.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-19 10:08:27.701084 starfall-0.0.2/starfall.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     2086 2023-07-19 10:08:27.000000 starfall-0.0.2/starfall.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      294 2023-07-19 10:08:27.000000 starfall-0.0.2/starfall.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-19 10:08:27.000000 starfall-0.0.2/starfall.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-19 10:08:21.000000 starfall-0.0.2/starfall.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       33 2023-07-19 10:08:27.000000 starfall-0.0.2/starfall.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        9 2023-07-19 10:08:27.000000 starfall-0.0.2/starfall.egg-info/top_level.txt
```

### Comparing `starfall-0.0.1/LICENSE` & `starfall-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starfall-0.0.1/PKG-INFO` & `starfall-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfall
-Version: 0.0.1
+Version: 0.0.2
 Summary: An executor of Cron Job
 Home-page: https://github.com/parselife/starfall/tree/master/
 Author: Alex
 Author-email: yxfacw@163.com
 License: MIT License
         
         Copyright (c) 2023 Alex
@@ -23,15 +23,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Keywords: Cron Job Executor
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -42,8 +42,8 @@
 
 <!--
  * @Author: Alex
  * @LastEditors: Alex yxfacw@163.com
  * @Date: 2023-07-18 18:19:20
  * @Description:  
 -->
-## py-executor
+## Starfall
```

### Comparing `starfall-0.0.1/setup.py` & `starfall-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `starfall-0.0.1/starfall/executor.py` & `starfall-0.0.2/starfall/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging
 import queue
 import requests
 import json
 import multiprocessing
 from concurrent.futures import ThreadPoolExecutor
 from helper import SUCCESS_RESP, TriggerParam, response_err, create_logger, clear_logger
-from helper import job_admin_uri, job_admin_access_token
+from main import job_admin_uri, job_admin_access_token
 from ast import literal_eval
 logger = logging.getLogger('main.Executor')
 
 # key: job_id value: JobThread
 job_threads = dict()
 
 """
```

### Comparing `starfall-0.0.1/starfall/helper.py` & `starfall-0.0.2/starfall/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,59 +8,16 @@
 
 import datetime
 from logging import handlers
 import os
 import logging
 import time
 from werkzeug.datastructures import ImmutableDict
-import configparser
-import json
 import logging.config
 
-# region -----------------config----------------------
-
-PROJ_ROOT = os.path.dirname(os.path.abspath(__file__))
-print(f'root path: {PROJ_ROOT}')
-
-# JOB_PATH = os.path.join(ROOT_PATH, 'job')
-# print(f'job 目录： {JOB_PATH}')
-
-# 从环境变量获取日志路径配置
-RUNTIME_LOG_PATH = os.environ.get('LOG_PATH', os.path.join(PROJ_ROOT, 'log'))
-# 自动创建日志目录
-if os.path.exists(RUNTIME_LOG_PATH) == False:
-    os.makedirs(RUNTIME_LOG_PATH)
-
-# 解析日志配置
-log_config = os.path.join(PROJ_ROOT, 'logging.json')
-if os.path.exists(log_config):
-    with open(log_config) as f:
-        log_config_obj = json.load(f)
-    logging.config.dictConfig(log_config_obj)
-
-# 解析配置
-parser = configparser.ConfigParser()
-parser.read(os.path.join(PROJ_ROOT, 'conf.ini'))
-# 端口号
-port = parser.getint('Executor', 'PORT')
-# 注册应用name
-app_name = parser.get('Executor', 'NAME')
-job_admin_uri = parser.get('Executor', 'ADMIN_URI')
-job_admin_access_token = parser.get('Executor', 'ACCESS_TOKEN')
-
-print(f'''
-      -----------------------------
-      port: {port}
-      name: {app_name}
-      admin_uri: {job_admin_uri}
-      access_token: {job_admin_access_token}
-      -----------------------------
-      ''')
-
-# endregion -------------------------------------
 
 # 无内容的成功响应
 SUCCESS_RESP = ImmutableDict({
     "code": 200,
     "msg": None
 })
```

### Comparing `starfall-0.0.1/starfall/main.py` & `starfall-0.0.2/starfall/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,27 +14,77 @@
 import socket
 import time
 from flask import Flask
 from flask import jsonify
 from flask import request
 from flask import make_response
 from helper import LogParam, TriggerParam, response_ok, SUCCESS_RESP, response_err, read_log_line
-from helper import job_admin_uri, job_admin_access_token, app_name, port, PROJ_ROOT
 import executor
+from waitress import serve
+import os
+import configparser
+import json
 
-logger = logging.getLogger('main.Bootstrap')
+logger = None
+
+port = 9002
+app_name = 'starfall'
+job_admin_uri = None
+job_admin_access_token = None
+runtime_log_path = None
 
-if job_admin_uri is None:
-    raise Exception(f'环境变量`ADMIN_URI`不能为空')
-if app_name is None:
-    raise Exception(f'环境变量`APP_NAME`不能为空')
 
 app = Flask(__name__)
 
 
+def init(proj_path: str):
+    # 初始化
+    # 从环境变量获取日志路径配置
+    runtime_log_path = os.environ.get(
+        'LOG_PATH', os.path.join(proj_path, 'log'))
+    # 自动创建日志目录
+    if os.path.exists(runtime_log_path) == False:
+        os.makedirs(runtime_log_path)
+    # 解析日志配置
+    log_config = os.path.join(proj_path, 'logging.json')
+    if os.path.exists(log_config):
+        with open(log_config) as f:
+            log_config_obj = json.load(f)
+        logging.config.dictConfig(log_config_obj)
+
+    logger = logging.getLogger('main.base')
+    # 解析配置
+    parser = configparser.ConfigParser()
+    parser.read(os.path.join(proj_path, 'conf.ini'))
+    # 端口号
+    port = parser.getint('Executor', 'PORT')
+    # 注册应用name
+    app_name = parser.get('Executor', 'NAME')
+    job_admin_uri = parser.get('Executor', 'ADMIN_URI')
+    job_admin_access_token = parser.get('Executor', 'ACCESS_TOKEN')
+
+    print(f'''
+      -----------------------------
+      port: {port}
+      name: {app_name}
+      admin_uri: {job_admin_uri}
+      access_token: {job_admin_access_token}
+      -----------------------------
+      ''')
+
+
+# start serve
+def start_serve():
+    if job_admin_uri is None:
+        raise Exception(f'配置参数`ADMIN_URI`不能为空')
+    if app_name is None:
+        raise Exception(f'配置参数`APP_NAME`不能为空')
+    serve(app, host='0.0.0.0', port=port)
+
+
 def resolve_request_to(class_):
     """转换请求json对象为实体类
     Args:
         class_ (_type_): 实体类
     """
     def wrap(f):
         def decorator(*args):
```

### Comparing `starfall-0.0.1/starfall.egg-info/PKG-INFO` & `starfall-0.0.2/starfall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfall
-Version: 0.0.1
+Version: 0.0.2
 Summary: An executor of Cron Job
 Home-page: https://github.com/parselife/starfall/tree/master/
 Author: Alex
 Author-email: yxfacw@163.com
 License: MIT License
         
         Copyright (c) 2023 Alex
@@ -23,15 +23,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Keywords: Cron Job Executor
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -42,8 +42,8 @@
 
 <!--
  * @Author: Alex
  * @LastEditors: Alex yxfacw@163.com
  * @Date: 2023-07-18 18:19:20
  * @Description:  
 -->
-## py-executor
+## Starfall
```

