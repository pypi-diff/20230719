# Comparing `tmp/tencentcloud-sdk-python-mmps-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mmps-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mmps-3.0.937.tar", last modified: Tue Jul 18 00:27:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mmps-3.0.938.tar", last modified: Wed Jul 19 00:42:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mmps-3.0.937.tar` & `tencentcloud-sdk-python-mmps-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15467 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/mmps_client.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    83019 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:27:19.000000 tencentcloud-sdk-python-mmps-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15527 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/mmps_client.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    83019 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:42:42.000000 tencentcloud-sdk-python-mmps-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/setup.py` & `tencentcloud-sdk-python-mmps-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/tencentcloud_sdk_python_mmps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mmps-3.0.938/tencentcloud_sdk_python_mmps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mmps
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mmps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/mmps_client.py` & `tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/mmps_client.py`

 * *Files 7% similar despite different names*

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
         """小程序隐私合规诊断重试任务
 
         :param request: Request instance for CreateAppScanTaskRepeat.
         :type request: :class:`tencentcloud.mmps.v20200710.models.CreateAppScanTaskRepeatRequest`
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
 
 
     def CreateFlySecMiniAppProfessionalScanTask(self, request):
         """创建小程序安全深度诊断任务
 
         :param request: Request instance for CreateFlySecMiniAppProfessionalScanTask.
         :type request: :class:`tencentcloud.mmps.v20200710.models.CreateFlySecMiniAppProfessionalScanTaskRequest`
@@ -88,15 +88,15 @@
             model = models.CreateFlySecMiniAppProfessionalScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlySecMiniAppScanTask(self, request):
         """创建小程序翼扬安全的基础或深度诊断任务
 
         :param request: Request instance for CreateFlySecMiniAppScanTask.
         :type request: :class:`tencentcloud.mmps.v20200710.models.CreateFlySecMiniAppScanTaskRequest`
@@ -111,15 +111,15 @@
             model = models.CreateFlySecMiniAppScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlySecMiniAppScanTaskRepeat(self, request):
         """重新提交基础诊断任务
 
         :param request: Request instance for CreateFlySecMiniAppScanTaskRepeat.
         :type request: :class:`tencentcloud.mmps.v20200710.models.CreateFlySecMiniAppScanTaskRepeatRequest`
@@ -134,15 +134,15 @@
             model = models.CreateFlySecMiniAppScanTaskRepeatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicDiagnosisResourceUsageInfo(self, request):
         """查询翼扬安全基础诊断资源使用情况
 
         :param request: Request instance for DescribeBasicDiagnosisResourceUsageInfo.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeBasicDiagnosisResourceUsageInfoRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeBasicDiagnosisResourceUsageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlySecMiniAppReportUrl(self, request):
         """获取翼扬诊断任务报告链接地址
 
         :param request: Request instance for DescribeFlySecMiniAppReportUrl.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeFlySecMiniAppReportUrlRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeFlySecMiniAppReportUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlySecMiniAppScanReportList(self, request):
         """查询指定小程序版本的翼扬诊断安全得分
 
         :param request: Request instance for DescribeFlySecMiniAppScanReportList.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeFlySecMiniAppScanReportListRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeFlySecMiniAppScanReportListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlySecMiniAppScanTaskList(self, request):
         """获取翼扬安全诊断任务列表
 
         :param request: Request instance for DescribeFlySecMiniAppScanTaskList.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeFlySecMiniAppScanTaskListRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeFlySecMiniAppScanTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlySecMiniAppScanTaskParam(self, request):
         """获取用户提交的基础诊断任务参数信息
 
         :param request: Request instance for DescribeFlySecMiniAppScanTaskParam.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeFlySecMiniAppScanTaskParamRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeFlySecMiniAppScanTaskParamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlySecMiniAppScanTaskStatus(self, request):
         """查询翼扬安全诊断任务状态
 
         :param request: Request instance for DescribeFlySecMiniAppScanTaskStatus.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeFlySecMiniAppScanTaskStatusRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeFlySecMiniAppScanTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceUsageInfo(self, request):
         """查询翼扬安全资源使用情况
 
         :param request: Request instance for DescribeResourceUsageInfo.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeResourceUsageInfoRequest`
@@ -295,15 +295,15 @@
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
         """获取小程序隐私合规诊断任务列表
 
         :param request: Request instance for DescribeScanTaskList.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeScanTaskListRequest`
@@ -318,15 +318,15 @@
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
         """获取小程序合规诊断任务报告url
 
         :param request: Request instance for DescribeScanTaskReportUrl.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeScanTaskReportUrlRequest`
@@ -341,15 +341,15 @@
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
         """查询小程序隐私合规诊断任务状态
 
         :param request: Request instance for DescribeScanTaskStatus.
         :type request: :class:`tencentcloud.mmps.v20200710.models.DescribeScanTaskStatusRequest`
@@ -364,8 +364,8 @@
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

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/errorcodes.py` & `tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/mmps/v20200710/models.py` & `tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/mmps/v20200710/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mmps-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mmps-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mmps
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mmps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mmps-3.0.937/README.rst` & `tencentcloud-sdk-python-mmps-3.0.938/README.rst`

 * *Files identical despite different names*

