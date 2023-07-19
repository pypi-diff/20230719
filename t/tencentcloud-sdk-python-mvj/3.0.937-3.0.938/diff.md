# Comparing `tmp/tencentcloud-sdk-python-mvj-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mvj-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mvj-3.0.937.tar", last modified: Tue Jul 18 00:28:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mvj-3.0.938.tar", last modified: Wed Jul 19 00:43:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mvj-3.0.937.tar` & `tencentcloud-sdk-python-mvj-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/
--rw-r--r--   0 root         (0) root         (0)     2099 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/mvj_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:03.000000 tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/mvj_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:23.000000 tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/setup.py` & `tencentcloud-sdk-python-mvj-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/mvj_client.py` & `tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/mvj_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,8 +44,8 @@
             model = models.MarketingValueJudgementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/errorcodes.py` & `tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/tencentcloud/mvj/v20190926/models.py` & `tencentcloud-sdk-python-mvj-3.0.938/tencentcloud/mvj/v20190926/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mvj-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mvj
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mvj SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/README.rst` & `tencentcloud-sdk-python-mvj-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mvj-3.0.937/tencentcloud_sdk_python_mvj.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mvj-3.0.938/tencentcloud_sdk_python_mvj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mvj
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mvj SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

