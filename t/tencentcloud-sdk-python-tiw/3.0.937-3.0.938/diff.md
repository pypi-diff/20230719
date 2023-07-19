# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.937.tar", last modified: Tue Jul 18 00:33:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.938.tar", last modified: Wed Jul 19 00:51:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.937.tar` & `tencentcloud-sdk-python-tiw-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60247 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)   280360 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:33:22.000000 tencentcloud-sdk-python-tiw-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60499 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)   280360 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:51:00.000000 tencentcloud-sdk-python-tiw-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.938/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/setup.py` & `tencentcloud-sdk-python-tiw-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyTiwTrialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplication(self, request):
         """创建白板应用
 
         :param request: Request instance for CreateApplication.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateApplicationRequest`
@@ -65,15 +65,15 @@
             model = models.CreateApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOfflineRecord(self, request):
         """创建课后录制任务
 
         :param request: Request instance for CreateOfflineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateOfflineRecordRequest`
@@ -88,15 +88,15 @@
             model = models.CreateOfflineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePPTCheckTask(self, request):
         """检测PPT文件，识别PPT中包含的动态转码任务（Transcode）不支持的元素
 
         :param request: Request instance for CreatePPTCheckTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreatePPTCheckTaskRequest`
@@ -111,15 +111,15 @@
             model = models.CreatePPTCheckTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSnapshotTask(self, request):
         """创建白板板书生成任务, 在任务结束后，如果提供了回调地址，将通过回调地址通知板书生成结果
 
         :param request: Request instance for CreateSnapshotTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateSnapshotTaskRequest`
@@ -134,15 +134,15 @@
             model = models.CreateSnapshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTranscode(self, request):
         """创建一个文档转码任务
 
         :param request: Request instance for CreateTranscode.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateTranscodeRequest`
@@ -157,15 +157,15 @@
             model = models.CreateTranscodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVideoGenerationTask(self, request):
         """创建视频生成任务
 
         :param request: Request instance for CreateVideoGenerationTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateVideoGenerationTaskRequest`
@@ -180,15 +180,15 @@
             model = models.CreateVideoGenerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAPIService(self, request):
         """通过服务角色调用其他云产品API接口获取信息
 
         :param request: Request instance for DescribeAPIService.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeAPIServiceRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeAPIServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationInfos(self, request):
         """查询白板应用详情
 
         :param request: Request instance for DescribeApplicationInfos.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeApplicationInfosRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeApplicationInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationUsage(self, request):
         """查询互动白板各个子产品用量
 
         :param request: Request instance for DescribeApplicationUsage.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeApplicationUsageRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeApplicationUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBoardSDKLog(self, request):
         """查询客户端白板日志
 
         :param request: Request instance for DescribeBoardSDKLog.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeBoardSDKLogRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeBoardSDKLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIMApplications(self, request):
         """查询可用于创建白板应用的IM应用列表
 
         :param request: Request instance for DescribeIMApplications.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeIMApplicationsRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeIMApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineRecord(self, request):
         """查询课后录制任务的进度与录制结果等相关信息
 
         :param request: Request instance for DescribeOfflineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeOfflineRecordRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeOfflineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineRecordCallback(self, request):
         """查询课后录制回调地址
 
         :param request: Request instance for DescribeOfflineRecordCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeOfflineRecordCallbackRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeOfflineRecordCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOnlineRecord(self, request):
         """查询录制任务状态与结果
 
         :param request: Request instance for DescribeOnlineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeOnlineRecordRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeOnlineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOnlineRecordCallback(self, request):
         """查询实时录制回调地址
 
         :param request: Request instance for DescribeOnlineRecordCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeOnlineRecordCallbackRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeOnlineRecordCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePPTCheck(self, request):
         """查询PPT检测任务的执行进度或结果
 
         :param request: Request instance for DescribePPTCheck.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckRequest`
@@ -410,15 +410,15 @@
             model = models.DescribePPTCheckResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePPTCheckCallback(self, request):
         """查询PPT检测任务回调地址
 
         :param request: Request instance for DescribePPTCheckCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckCallbackRequest`
@@ -433,15 +433,15 @@
             model = models.DescribePPTCheckCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePostpaidUsage(self, request):
         """查询用户后付费用量
 
         :param request: Request instance for DescribePostpaidUsage.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePostpaidUsageRequest`
@@ -456,15 +456,15 @@
             model = models.DescribePostpaidUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQualityMetrics(self, request):
         """查询互动白板质量数据
 
         :param request: Request instance for DescribeQualityMetrics.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeQualityMetricsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeQualityMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordSearch(self, request):
         """根据房间号搜索实时录制任务
 
         :param request: Request instance for DescribeRecordSearch.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeRecordSearchRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeRecordSearchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoomList(self, request):
         """查询白板房间列表
 
         :param request: Request instance for DescribeRoomList.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeRoomListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeRoomListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRunningTasks(self, request):
         """根据指定的任务类型，获取当前正在执行中的任务列表。只能查询最近3天内创建的任务。
 
         :param request: Request instance for DescribeRunningTasks.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeRunningTasksRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeRunningTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotTask(self, request):
         """获取指定白板板书生成任务信息
 
         :param request: Request instance for DescribeSnapshotTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeSnapshotTaskRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeSnapshotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTIWDailyUsage(self, request):
         """查询互动白板天维度计费用量。
         1. 单次查询统计区间最多不能超过31天。
         2. 由于统计延迟等原因，暂时不支持查询当天数据，建议在次日上午7点以后再来查询前一天的用量，例如在10月27日上午7点后，再来查询到10月26日整天的用量
 
@@ -596,15 +596,15 @@
             model = models.DescribeTIWDailyUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTIWRoomDailyUsage(self, request):
         """查询互动白板房间维度每天计费用量。
         1. 单次查询统计区间最多不能超过31天。
         2. 由于统计延迟等原因，暂时不支持查询当天数据，建议在次日上午7点以后再来查询前一天的用量，例如在10月27日上午7点后，再来查询到10月26日整天的用量
 
@@ -621,15 +621,15 @@
             model = models.DescribeTIWRoomDailyUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscode(self, request):
         """查询文档转码任务的执行进度与转码结果
 
         :param request: Request instance for DescribeTranscode.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeRequest`
@@ -644,15 +644,15 @@
             model = models.DescribeTranscodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscodeCallback(self, request):
         """查询文档转码回调地址
 
         :param request: Request instance for DescribeTranscodeCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeCallbackRequest`
@@ -667,15 +667,15 @@
             model = models.DescribeTranscodeCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscodeSearch(self, request):
         """按文档名称搜索转码任务
 
         :param request: Request instance for DescribeTranscodeSearch.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeTranscodeSearchRequest`
@@ -690,15 +690,15 @@
             model = models.DescribeTranscodeSearchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsageSummary(self, request):
         """查询指定时间段内子产品的用量汇总
 
         :param request: Request instance for DescribeUsageSummary.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeUsageSummaryRequest`
@@ -713,15 +713,15 @@
             model = models.DescribeUsageSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserList(self, request):
         """查询白板用户列表
 
         :param request: Request instance for DescribeUserList.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeUserListRequest`
@@ -736,15 +736,15 @@
             model = models.DescribeUserListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserResources(self, request):
         """查询客户资源列表
 
         :param request: Request instance for DescribeUserResources.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeUserResourcesRequest`
@@ -759,15 +759,15 @@
             model = models.DescribeUserResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserStatus(self, request):
         """查询互动白板用户详情，包括是否开通了互动白板，当前互动白板服务有效期等信息
 
         :param request: Request instance for DescribeUserStatus.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeUserStatusRequest`
@@ -782,15 +782,15 @@
             model = models.DescribeUserStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVideoGenerationTask(self, request):
         """查询录制视频生成任务状态与结果
 
         :param request: Request instance for DescribeVideoGenerationTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeVideoGenerationTaskRequest`
@@ -805,15 +805,15 @@
             model = models.DescribeVideoGenerationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVideoGenerationTaskCallback(self, request):
         """查询录制视频生成回调地址
 
         :param request: Request instance for DescribeVideoGenerationTaskCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeVideoGenerationTaskCallbackRequest`
@@ -828,15 +828,15 @@
             model = models.DescribeVideoGenerationTaskCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWarningCallback(self, request):
         """查询告警回调地址。此功能需要申请白名单使用。
 
         :param request: Request instance for DescribeWarningCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWarningCallbackRequest`
@@ -851,15 +851,15 @@
             model = models.DescribeWarningCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteboardApplicationConfig(self, request):
         """查询白板应用任务相关的配置，包括存储桶、回调等
 
         :param request: Request instance for DescribeWhiteboardApplicationConfig.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardApplicationConfigRequest`
@@ -874,15 +874,15 @@
             model = models.DescribeWhiteboardApplicationConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteboardBucketConfig(self, request):
         """查询文档转码，实时录制存储桶的配置
 
         :param request: Request instance for DescribeWhiteboardBucketConfig.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardBucketConfigRequest`
@@ -897,15 +897,15 @@
             model = models.DescribeWhiteboardBucketConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteboardPush(self, request):
         """查询推流任务状态与结果
 
         :param request: Request instance for DescribeWhiteboardPush.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardPushRequest`
@@ -920,15 +920,15 @@
             model = models.DescribeWhiteboardPushResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteboardPushCallback(self, request):
         """查询白板推流回调地址
 
         :param request: Request instance for DescribeWhiteboardPushCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardPushCallbackRequest`
@@ -943,15 +943,15 @@
             model = models.DescribeWhiteboardPushCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhiteboardPushSearch(self, request):
         """根据房间号搜索白板推流任务
 
         :param request: Request instance for DescribeWhiteboardPushSearch.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardPushSearchRequest`
@@ -966,15 +966,15 @@
             model = models.DescribeWhiteboardPushSearchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplication(self, request):
         """修改白板应用
 
         :param request: Request instance for ModifyApplication.
         :type request: :class:`tencentcloud.tiw.v20190919.models.ModifyApplicationRequest`
@@ -989,15 +989,15 @@
             model = models.ModifyApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAutoRenewFlag(self, request):
         """设置白板月功能费自动续费
 
         :param request: Request instance for ModifyAutoRenewFlag.
         :type request: :class:`tencentcloud.tiw.v20190919.models.ModifyAutoRenewFlagRequest`
@@ -1012,15 +1012,15 @@
             model = models.ModifyAutoRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWhiteboardApplicationConfig(self, request):
         """修改白板应用任务相关的配置，包括存储桶、回调等
 
         :param request: Request instance for ModifyWhiteboardApplicationConfig.
         :type request: :class:`tencentcloud.tiw.v20190919.models.ModifyWhiteboardApplicationConfigRequest`
@@ -1035,15 +1035,15 @@
             model = models.ModifyWhiteboardApplicationConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWhiteboardBucketConfig(self, request):
         """设置文档转码，实时录制存储桶的配置
 
         :param request: Request instance for ModifyWhiteboardBucketConfig.
         :type request: :class:`tencentcloud.tiw.v20190919.models.ModifyWhiteboardBucketConfigRequest`
@@ -1058,15 +1058,15 @@
             model = models.ModifyWhiteboardBucketConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PauseOnlineRecord(self, request):
         """暂停实时录制
 
         :param request: Request instance for PauseOnlineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.PauseOnlineRecordRequest`
@@ -1081,15 +1081,15 @@
             model = models.PauseOnlineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeOnlineRecord(self, request):
         """恢复实时录制
 
         :param request: Request instance for ResumeOnlineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.ResumeOnlineRecordRequest`
@@ -1104,15 +1104,15 @@
             model = models.ResumeOnlineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetOfflineRecordCallback(self, request):
         """设置课后录制回调地址
 
         :param request: Request instance for SetOfflineRecordCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetOfflineRecordCallbackRequest`
@@ -1127,15 +1127,15 @@
             model = models.SetOfflineRecordCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetOnlineRecordCallback(self, request):
         """设置实时录制回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40258
 
         :param request: Request instance for SetOnlineRecordCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetOnlineRecordCallbackRequest`
@@ -1150,15 +1150,15 @@
             model = models.SetOnlineRecordCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetOnlineRecordCallbackKey(self, request):
         """设置实时录制回调鉴权密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetOnlineRecordCallbackKey.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetOnlineRecordCallbackKeyRequest`
@@ -1173,15 +1173,15 @@
             model = models.SetOnlineRecordCallbackKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetPPTCheckCallback(self, request):
         """设置PPT检测任务回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260#c9cbe05f-fe1a-4410-b4dc-40cc301c7b81
 
         :param request: Request instance for SetPPTCheckCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackRequest`
@@ -1196,15 +1196,15 @@
             model = models.SetPPTCheckCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetPPTCheckCallbackKey(self, request):
         """设置PPT检测任务回调密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetPPTCheckCallbackKey.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackKeyRequest`
@@ -1219,15 +1219,15 @@
             model = models.SetPPTCheckCallbackKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTranscodeCallback(self, request):
         """设置文档转码回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260
 
         :param request: Request instance for SetTranscodeCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetTranscodeCallbackRequest`
@@ -1242,15 +1242,15 @@
             model = models.SetTranscodeCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTranscodeCallbackKey(self, request):
         """设置文档转码回调鉴权密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetTranscodeCallbackKey.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetTranscodeCallbackKeyRequest`
@@ -1265,15 +1265,15 @@
             model = models.SetTranscodeCallbackKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetVideoGenerationTaskCallback(self, request):
         """设置录制视频生成回调地址
 
         :param request: Request instance for SetVideoGenerationTaskCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetVideoGenerationTaskCallbackRequest`
@@ -1288,15 +1288,15 @@
             model = models.SetVideoGenerationTaskCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetVideoGenerationTaskCallbackKey(self, request):
         """设置视频生成回调鉴权密钥
 
         :param request: Request instance for SetVideoGenerationTaskCallbackKey.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetVideoGenerationTaskCallbackKeyRequest`
@@ -1311,15 +1311,15 @@
             model = models.SetVideoGenerationTaskCallbackKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetWarningCallback(self, request):
         """设置告警回调地址。此功能需要申请白名单使用。
 
         :param request: Request instance for SetWarningCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetWarningCallbackRequest`
@@ -1334,15 +1334,15 @@
             model = models.SetWarningCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetWhiteboardPushCallback(self, request):
         """设置白板推流回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetWhiteboardPushCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetWhiteboardPushCallbackRequest`
@@ -1357,15 +1357,15 @@
             model = models.SetWhiteboardPushCallbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetWhiteboardPushCallbackKey(self, request):
         """设置白板推流回调鉴权密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetWhiteboardPushCallbackKey.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetWhiteboardPushCallbackKeyRequest`
@@ -1380,15 +1380,15 @@
             model = models.SetWhiteboardPushCallbackKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartOnlineRecord(self, request):
         """发起一个实时录制任务
 
         :param request: Request instance for StartOnlineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.StartOnlineRecordRequest`
@@ -1403,15 +1403,15 @@
             model = models.StartOnlineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartWhiteboardPush(self, request):
         """发起一个白板推流任务
 
         :param request: Request instance for StartWhiteboardPush.
         :type request: :class:`tencentcloud.tiw.v20190919.models.StartWhiteboardPushRequest`
@@ -1426,15 +1426,15 @@
             model = models.StartWhiteboardPushResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopOnlineRecord(self, request):
         """停止实时录制
 
         :param request: Request instance for StopOnlineRecord.
         :type request: :class:`tencentcloud.tiw.v20190919.models.StopOnlineRecordRequest`
@@ -1449,15 +1449,15 @@
             model = models.StopOnlineRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopWhiteboardPush(self, request):
         """停止白板推流任务
 
         :param request: Request instance for StopWhiteboardPush.
         :type request: :class:`tencentcloud.tiw.v20190919.models.StopWhiteboardPushRequest`
@@ -1472,8 +1472,8 @@
             model = models.StopWhiteboardPushResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/tiw/v20190919/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.938/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.937/README.rst` & `tencentcloud-sdk-python-tiw-3.0.938/README.rst`

 * *Files identical despite different names*

