# Comparing `tmp/tencentcloud-sdk-python-npp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-npp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-npp-3.0.937.tar", last modified: Tue Jul 18 00:28:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-npp-3.0.938.tar", last modified: Wed Jul 19 00:43:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-npp-3.0.937.tar` & `tencentcloud-sdk-python-npp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/
--rw-r--r--   0 root         (0) root         (0)     7942 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/npp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60419 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:13.000000 tencentcloud-sdk-python-npp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     7974 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/npp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60419 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:32.000000 tencentcloud-sdk-python-npp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-npp-3.0.937/setup.py` & `tencentcloud-sdk-python-npp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-npp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-npp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/npp_client.py` & `tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/npp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCallBackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DelVirtualNum(self, request):
         """直拨解绑中间号
 
         :param request: Request instance for DelVirtualNum.
         :type request: :class:`tencentcloud.npp.v20190823.models.DelVirtualNumRequest`
@@ -65,15 +65,15 @@
             model = models.DelVirtualNumResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCallBack(self, request):
         """回拨呼叫取消
 
         :param request: Request instance for DeleteCallBack.
         :type request: :class:`tencentcloud.npp.v20190823.models.DeleteCallBackRequest`
@@ -88,15 +88,15 @@
             model = models.DeleteCallBackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallBackCdr(self, request):
         """回拨话单获取接口
 
         :param request: Request instance for DescribeCallBackCdr.
         :type request: :class:`tencentcloud.npp.v20190823.models.DescribeCallBackCdrRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeCallBackCdrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallBackStatus(self, request):
         """回拨通话状态获取
 
         :param request: Request instance for DescribeCallBackStatus.
         :type request: :class:`tencentcloud.npp.v20190823.models.DescribeCallBackStatusRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeCallBackStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallerDisplayList(self, request):
         """回拨拉取主叫显号号码集合
 
         :param request: Request instance for DescribeCallerDisplayList.
         :type request: :class:`tencentcloud.npp.v20190823.models.DescribeCallerDisplayListRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeCallerDisplayListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Get400Cdr(self, request):
         """直拨话单获取接口
 
         :param request: Request instance for Get400Cdr.
         :type request: :class:`tencentcloud.npp.v20190823.models.Get400CdrRequest`
@@ -180,15 +180,15 @@
             model = models.Get400CdrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetVirtualNum(self, request):
         """直拨获取中间号（App 使用方发起）
 
         :param request: Request instance for GetVirtualNum.
         :type request: :class:`tencentcloud.npp.v20190823.models.GetVirtualNumRequest`
@@ -203,8 +203,8 @@
             model = models.GetVirtualNumResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/errorcodes.py` & `tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-npp-3.0.937/tencentcloud/npp/v20190823/models.py` & `tencentcloud-sdk-python-npp-3.0.938/tencentcloud/npp/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-npp-3.0.937/tencentcloud_sdk_python_npp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-npp-3.0.938/tencentcloud_sdk_python_npp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-npp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Npp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-npp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-npp-3.0.938/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-npp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Npp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-npp-3.0.937/README.rst` & `tencentcloud-sdk-python-npp-3.0.938/README.rst`

 * *Files identical despite different names*

