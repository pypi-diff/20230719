# Comparing `tmp/tencentcloud-sdk-python-pds-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-pds-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-pds-3.0.937.tar", last modified: Tue Jul 18 00:28:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-pds-3.0.938.tar", last modified: Wed Jul 19 00:44:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-pds-3.0.937.tar` & `tencentcloud-sdk-python-pds-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8332 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)     2829 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/pds_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:41.000000 tencentcloud-sdk-python-pds-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/pds_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:02.000000 tencentcloud-sdk-python-pds-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-pds-3.0.937/setup.py` & `tencentcloud-sdk-python-pds-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/errorcodes.py` & `tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/models.py` & `tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pds-3.0.937/tencentcloud/pds/v20210701/pds_client.py` & `tencentcloud-sdk-python-pds-3.0.938/tencentcloud/pds/v20210701/pds_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeNewUserAcquisitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStockEstimation(self, request):
         """查询存量判断服务
 
         :param request: Request instance for DescribeStockEstimation.
         :type request: :class:`tencentcloud.pds.v20210701.models.DescribeStockEstimationRequest`
@@ -65,8 +65,8 @@
             model = models.DescribeStockEstimationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-pds-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-pds-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-pds-3.0.937/tencentcloud_sdk_python_pds.egg-info/PKG-INFO` & `tencentcloud-sdk-python-pds-3.0.938/tencentcloud_sdk_python_pds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pds
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Pds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pds-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-pds-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pds
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Pds SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pds-3.0.937/README.rst` & `tencentcloud-sdk-python-pds-3.0.938/README.rst`

 * *Files identical despite different names*

