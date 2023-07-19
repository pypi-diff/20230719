# Comparing `tmp/tencentcloud-sdk-python-region-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-region-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-region-3.0.937.tar", last modified: Tue Jul 18 00:29:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-region-3.0.938.tar", last modified: Wed Jul 19 00:44:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-region-3.0.937.tar` & `tencentcloud-sdk-python-region-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3744 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/region_client.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18296 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:29:13.000000 tencentcloud-sdk-python-region-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/region_client.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18296 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:44:29.000000 tencentcloud-sdk-python-region-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-region-3.0.937/setup.py` & `tencentcloud-sdk-python-region-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-region-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/region_client.py` & `tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/region_client.py`

 * *Files 5% similar despite different names*

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
         :type request: :class:`tencentcloud.region.v20220627.models.DescribeRegionsRequest`
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
         :type request: :class:`tencentcloud.region.v20220627.models.DescribeZonesRequest`
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

### Comparing `tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/errorcodes.py` & `tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.937/tencentcloud/region/v20220627/models.py` & `tencentcloud-sdk-python-region-3.0.938/tencentcloud/region/v20220627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.937/tencentcloud_sdk_python_region.egg-info/PKG-INFO` & `tencentcloud-sdk-python-region-3.0.938/tencentcloud_sdk_python_region.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-region
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Region SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-region-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-region-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-region
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Region SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-region-3.0.937/README.rst` & `tencentcloud-sdk-python-region-3.0.938/README.rst`

 * *Files identical despite different names*

