# Comparing `tmp/tencentcloud-sdk-python-asw-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-asw-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asw-3.0.937.tar", last modified: Tue Jul 18 00:17:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asw-3.0.938.tar", last modified: Wed Jul 19 00:21:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asw-3.0.937.tar` & `tencentcloud-sdk-python-asw-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/
--rw-r--r--   0 root         (0) root         (0)     9098 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/asw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/__init__.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    44296 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:17.000000 tencentcloud-sdk-python-asw-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:16.000000 tencentcloud-sdk-python-asw-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/
+-rw-r--r--   0 root         (0) root         (0)     9134 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/asw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    44296 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:21:21.000000 tencentcloud-sdk-python-asw-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-asw-3.0.937/setup.py` & `tencentcloud-sdk-python-asw-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/asw_client.py` & `tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/asw_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateFlowServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExecution(self, request):
         """查询执行详细信息
 
         :param request: Request instance for DescribeExecution.
         :type request: :class:`tencentcloud.asw.v20200722.models.DescribeExecutionRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeExecutionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExecutionHistory(self, request):
         """一次执行会有很多步骤，经过很多节点，这个接口描述某一次执行的事件的历史
 
         :param request: Request instance for DescribeExecutionHistory.
         :type request: :class:`tencentcloud.asw.v20200722.models.DescribeExecutionHistoryRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeExecutionHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExecutions(self, request):
         """对状态机的执行历史进行描述.
 
         :param request: Request instance for DescribeExecutions.
         :type request: :class:`tencentcloud.asw.v20200722.models.DescribeExecutionsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeExecutionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowServiceDetail(self, request):
         """查询该用户指定状态机下的详情数据。
 
         :param request: Request instance for DescribeFlowServiceDetail.
         :type request: :class:`tencentcloud.asw.v20200722.models.DescribeFlowServiceDetailRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeFlowServiceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowServices(self, request):
         """查询指定用户下所有状态机，以列表形式返回
 
         :param request: Request instance for DescribeFlowServices.
         :type request: :class:`tencentcloud.asw.v20200722.models.DescribeFlowServicesRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeFlowServicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFlowService(self, request):
         """该接口用于修改状态机
 
         :param request: Request instance for ModifyFlowService.
         :type request: :class:`tencentcloud.asw.v20200722.models.ModifyFlowServiceRequest`
@@ -180,15 +180,15 @@
             model = models.ModifyFlowServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartExecution(self, request):
         """为指定的状态机启动一次执行
 
         :param request: Request instance for StartExecution.
         :type request: :class:`tencentcloud.asw.v20200722.models.StartExecutionRequest`
@@ -203,15 +203,15 @@
             model = models.StartExecutionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopExecution(self, request):
         """终止某个状态机
 
         :param request: Request instance for StopExecution.
         :type request: :class:`tencentcloud.asw.v20200722.models.StopExecutionRequest`
@@ -226,8 +226,8 @@
             model = models.StopExecutionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/errorcodes.py` & `tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asw-3.0.937/tencentcloud/asw/v20200722/models.py` & `tencentcloud-sdk-python-asw-3.0.938/tencentcloud/asw/v20200722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asw-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asw-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asw-3.0.937/tencentcloud_sdk_python_asw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asw-3.0.938/tencentcloud_sdk_python_asw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asw
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Asw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asw-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-asw-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asw
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Asw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asw-3.0.937/README.rst` & `tencentcloud-sdk-python-asw-3.0.938/README.rst`

 * *Files identical despite different names*

