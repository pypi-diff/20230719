# Comparing `tmp/tencentcloud-sdk-python-memcached-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-memcached-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-memcached-3.0.937.tar", last modified: Tue Jul 18 00:27:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-memcached-3.0.938.tar", last modified: Wed Jul 19 00:42:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-memcached-3.0.937.tar` & `tencentcloud-sdk-python-memcached-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/memcached_client.py
--rw-r--r--   0 root         (0) root         (0)    16292 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-18 00:27:11.000000 tencentcloud-sdk-python-memcached-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/memcached_client.py
+-rw-r--r--   0 root         (0) root         (0)    16292 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-19 00:42:33.000000 tencentcloud-sdk-python-memcached-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/tencentcloud_sdk_python_memcached.egg-info/PKG-INFO` & `tencentcloud-sdk-python-memcached-3.0.938/tencentcloud_sdk_python_memcached.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-memcached
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Memcached SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/setup.py` & `tencentcloud-sdk-python-memcached-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.937'
+__version__ = '3.0.938'
```

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/errorcodes.py` & `tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/memcached_client.py` & `tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/memcached_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,8 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/tencentcloud/memcached/v20190318/models.py` & `tencentcloud-sdk-python-memcached-3.0.938/tencentcloud/memcached/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-memcached-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-memcached
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Memcached SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-memcached-3.0.937/README.rst` & `tencentcloud-sdk-python-memcached-3.0.938/README.rst`

 * *Files identical despite different names*

