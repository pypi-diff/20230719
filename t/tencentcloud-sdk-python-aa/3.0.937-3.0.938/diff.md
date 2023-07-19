# Comparing `tmp/tencentcloud-sdk-python-aa-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-aa-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aa-3.0.937.tar", last modified: Tue Jul 18 00:15:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aa-3.0.938.tar", last modified: Wed Jul 19 00:19:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aa-3.0.937.tar` & `tencentcloud-sdk-python-aa-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/aa_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2430 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17163 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:15:30.000000 tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/aa_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17163 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:19:51.000000 tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-aa-3.0.937/setup.py` & `tencentcloud-sdk-python-aa-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/aa_client.py` & `tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/aa_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,8 +42,8 @@
             model = models.QueryActivityAntiRushResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/errorcodes.py` & `tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aa-3.0.937/tencentcloud/aa/v20200224/models.py` & `tencentcloud-sdk-python-aa-3.0.938/tencentcloud/aa/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aa-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aa-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aa-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-aa-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aa
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aa-3.0.937/README.rst` & `tencentcloud-sdk-python-aa-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aa-3.0.937/tencentcloud_sdk_python_aa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aa-3.0.938/tencentcloud_sdk_python_aa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aa
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

