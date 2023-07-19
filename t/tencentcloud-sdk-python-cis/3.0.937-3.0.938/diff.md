# Comparing `tmp/tencentcloud-sdk-python-cis-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cis-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cis-3.0.937.tar", last modified: Tue Jul 18 00:20:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cis-3.0.938.tar", last modified: Wed Jul 19 00:24:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cis-3.0.937.tar` & `tencentcloud-sdk-python-cis-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7698 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/cis_client.py
--rw-r--r--   0 root         (0) root         (0)    38589 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:20:18.000000 tencentcloud-sdk-python-cis-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7726 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/cis_client.py
+-rw-r--r--   0 root         (0) root         (0)    38589 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:24:24.000000 tencentcloud-sdk-python-cis-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cis-3.0.937/setup.py` & `tencentcloud-sdk-python-cis-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cis-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/errorcodes.py` & `tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/cis_client.py` & `tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/cis_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateContainerInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteContainerInstance(self, request):
         """此接口（DeleteContainerInstance）用于删除容器实例
 
         :param request: Request instance for DeleteContainerInstance.
         :type request: :class:`tencentcloud.cis.v20180408.models.DeleteContainerInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteContainerInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerInstance(self, request):
         """此接口（DescribeContainerInstance）用于获取容器实例详情
 
         :param request: Request instance for DescribeContainerInstance.
         :type request: :class:`tencentcloud.cis.v20180408.models.DescribeContainerInstanceRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeContainerInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerInstanceEvents(self, request):
         """此接口（DescribeContainerInstanceEvents）用于查询容器实例事件列表
 
         :param request: Request instance for DescribeContainerInstanceEvents.
         :type request: :class:`tencentcloud.cis.v20180408.models.DescribeContainerInstanceEventsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeContainerInstanceEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerInstances(self, request):
         """此接口（DescribeContainerInstances）查询容器实例列表
 
         :param request: Request instance for DescribeContainerInstances.
         :type request: :class:`tencentcloud.cis.v20180408.models.DescribeContainerInstancesRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeContainerInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerLog(self, request):
         """此接口（DescribeContainerLog）用于获取容器日志信息
 
         :param request: Request instance for DescribeContainerLog.
         :type request: :class:`tencentcloud.cis.v20180408.models.DescribeContainerLogRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeContainerLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateCis(self, request):
         """此接口（InquiryPriceCreateCis）用于查询容器实例价格
 
         :param request: Request instance for InquiryPriceCreateCis.
         :type request: :class:`tencentcloud.cis.v20180408.models.InquiryPriceCreateCisRequest`
@@ -180,8 +180,8 @@
             model = models.InquiryPriceCreateCisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cis-3.0.937/tencentcloud/cis/v20180408/models.py` & `tencentcloud-sdk-python-cis-3.0.938/tencentcloud/cis/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cis-3.0.937/tencentcloud_sdk_python_cis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cis-3.0.938/tencentcloud_sdk_python_cis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cis-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cis-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cis-3.0.937/README.rst` & `tencentcloud-sdk-python-cis-3.0.938/README.rst`

 * *Files identical despite different names*

