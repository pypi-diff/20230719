# Comparing `tmp/tencentcloud-sdk-python-csxg-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-csxg-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csxg-3.0.937.tar", last modified: Tue Jul 18 00:21:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csxg-3.0.938.tar", last modified: Wed Jul 19 00:25:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csxg-3.0.937.tar` & `tencentcloud-sdk-python-csxg-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5377 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/csxg_client.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:21:28.000000 tencentcloud-sdk-python-csxg-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/csxg_client.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:25:33.000000 tencentcloud-sdk-python-csxg-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csxg-3.0.938/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csxg
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Csxg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/setup.py` & `tencentcloud-sdk-python-csxg-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/csxg_client.py` & `tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/csxg_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.Create5GInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Delete5GInstance(self, request):
         """删除5G入云服务
 
         :param request: Request instance for Delete5GInstance.
         :type request: :class:`tencentcloud.csxg.v20230303.models.Delete5GInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.Delete5GInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Describe5GAPNs(self, request):
         """查询APN信息
 
         :param request: Request instance for Describe5GAPNs.
         :type request: :class:`tencentcloud.csxg.v20230303.models.Describe5GAPNsRequest`
@@ -88,15 +88,15 @@
             model = models.Describe5GAPNsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Describe5GInstances(self, request):
         """查询5G入云服务
 
         :param request: Request instance for Describe5GInstances.
         :type request: :class:`tencentcloud.csxg.v20230303.models.Describe5GInstancesRequest`
@@ -111,15 +111,15 @@
             model = models.Describe5GInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Modify5GInstanceAttribute(self, request):
         """修改5G入云服务
 
         :param request: Request instance for Modify5GInstanceAttribute.
         :type request: :class:`tencentcloud.csxg.v20230303.models.Modify5GInstanceAttributeRequest`
@@ -134,8 +134,8 @@
             model = models.Modify5GInstanceAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/errorcodes.py` & `tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/csxg/v20230303/models.py` & `tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/csxg/v20230303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csxg-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-csxg-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csxg
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Csxg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.937/README.rst` & `tencentcloud-sdk-python-csxg-3.0.938/README.rst`

 * *Files identical despite different names*

