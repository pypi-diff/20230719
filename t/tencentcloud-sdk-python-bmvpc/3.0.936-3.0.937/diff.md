# Comparing `tmp/tencentcloud-sdk-python-bmvpc-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-bmvpc-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bmvpc-3.0.936.tar", last modified: Mon Jul 17 00:18:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bmvpc-3.0.937.tar", last modified: Tue Jul 18 00:18:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bmvpc-3.0.936.tar` & `tencentcloud-sdk-python-bmvpc-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58712 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/bmvpc_client.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   250943 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:18:36.000000 tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58712 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/bmvpc_client.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   250943 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:18:16.000000 tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/setup.py` & `tencentcloud-sdk-python-bmvpc-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/bmvpc_client.py` & `tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/bmvpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/errorcodes.py` & `tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/bmvpc/v20180625/models.py` & `tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/bmvpc/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.936'
+__version__ = '3.0.937'
```

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-bmvpc-3.0.937/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmvpc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Bmvpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/README.rst` & `tencentcloud-sdk-python-bmvpc-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmvpc-3.0.936/tencentcloud_sdk_python_bmvpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bmvpc-3.0.937/tencentcloud_sdk_python_bmvpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmvpc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Bmvpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

