# Comparing `tmp/tencentcloud-sdk-python-api-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-api-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-api-3.0.937.tar", last modified: Tue Jul 18 00:16:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-api-3.0.938.tar", last modified: Wed Jul 19 00:21:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-api-3.0.937.tar` & `tencentcloud-sdk-python-api-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/__init__.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/api_client.py
--rw-r--r--   0 root         (0) root         (0)    17428 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:52.000000 tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    17428 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:01.000000 tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-api-3.0.937/setup.py` & `tencentcloud-sdk-python-api-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-api-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-api-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/errorcodes.py` & `tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/api_client.py` & `tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """本接口(DescribeRegions)用于查询各个产品支持地域信息。
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.api.v20201106.models.DescribeRegionsRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """本接口(DescribeZones)用于查询产品可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.api.v20201106.models.DescribeZonesRequest`
@@ -88,8 +88,8 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-api-3.0.937/tencentcloud/api/v20201106/models.py` & `tencentcloud-sdk-python-api-3.0.938/tencentcloud/api/v20201106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-api-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-api-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-api
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Api SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-api-3.0.937/README.rst` & `tencentcloud-sdk-python-api-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-api-3.0.937/tencentcloud_sdk_python_api.egg-info/PKG-INFO` & `tencentcloud-sdk-python-api-3.0.938/tencentcloud_sdk_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-api
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Api SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

