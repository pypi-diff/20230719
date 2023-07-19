# Comparing `tmp/tencentcloud-sdk-python-acp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-acp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-acp-3.0.937.tar", last modified: Tue Jul 18 00:15:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-acp-3.0.938.tar", last modified: Wed Jul 19 00:20:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-acp-3.0.937.tar` & `tencentcloud-sdk-python-acp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/
--rw-r--r--   0 root         (0) root         (0)     8376 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/acp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/__init__.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53725 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:15:43.000000 tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/
+-rw-r--r--   0 root         (0) root         (0)     8408 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/acp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53725 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:20:01.000000 tencentcloud-sdk-python-acp-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:02.000000 tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-acp-3.0.937/setup.py` & `tencentcloud-sdk-python-acp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/acp_client.py` & `tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/acp_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateAppScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAppScanTaskRepeat(self, request):
         """App应用合规隐私诊断重试任务
 
         :param request: Request instance for CreateAppScanTaskRepeat.
         :type request: :class:`tencentcloud.acp.v20220105.models.CreateAppScanTaskRepeatRequest`
@@ -65,15 +65,15 @@
             model = models.CreateAppScanTaskRepeatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChannelTaskReportUrl(self, request):
         """获取子渠道的App合规诊断任务报告url
 
         :param request: Request instance for DescribeChannelTaskReportUrl.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeChannelTaskReportUrlRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeChannelTaskReportUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileTicket(self, request):
         """获取应用合规文件上传凭证，用于上传诊断文件
 
         :param request: Request instance for DescribeFileTicket.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeFileTicketRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeFileTicketResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceUsageInfo(self, request):
         """查询应用合规平台用户资源的使用情况
 
         :param request: Request instance for DescribeResourceUsageInfo.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeResourceUsageInfoRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeResourceUsageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanTaskList(self, request):
         """获取App隐私合规诊断任务列表
 
         :param request: Request instance for DescribeScanTaskList.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeScanTaskListRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeScanTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanTaskReportUrl(self, request):
         """获取App合规诊断任务报告url
 
         :param request: Request instance for DescribeScanTaskReportUrl.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeScanTaskReportUrlRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeScanTaskReportUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanTaskStatus(self, request):
         """查询App隐私合规诊断任务状态
 
         :param request: Request instance for DescribeScanTaskStatus.
         :type request: :class:`tencentcloud.acp.v20220105.models.DescribeScanTaskStatusRequest`
@@ -203,8 +203,8 @@
             model = models.DescribeScanTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/errorcodes.py` & `tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-acp-3.0.937/tencentcloud/acp/v20220105/models.py` & `tencentcloud-sdk-python-acp-3.0.938/tencentcloud/acp/v20220105/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-acp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-acp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-acp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-acp-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-acp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Acp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-acp-3.0.937/README.rst` & `tencentcloud-sdk-python-acp-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-acp-3.0.937/tencentcloud_sdk_python_acp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-acp-3.0.938/tencentcloud_sdk_python_acp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-acp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Acp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

