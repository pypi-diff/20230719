# Comparing `tmp/tencentcloud-sdk-python-cr-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cr-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.937.tar", last modified: Tue Jul 18 00:21:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cr-3.0.938.tar", last modified: Wed Jul 19 00:25:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cr-3.0.937.tar` & `tencentcloud-sdk-python-cr-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26019 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/cr_client.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   136120 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:21:19.000000 tencentcloud-sdk-python-cr-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26131 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/cr_client.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   136120 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:25:25.000000 tencentcloud-sdk-python-cr-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cr-3.0.937/setup.py` & `tencentcloud-sdk-python-cr-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/cr_client.py` & `tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/cr_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyBlackListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyBlackListData(self, request):
         """提交机器人黑名单申请
 
         :param request: Request instance for ApplyBlackListData.
         :type request: :class:`tencentcloud.cr.v20180321.models.ApplyBlackListDataRequest`
@@ -65,15 +65,15 @@
             model = models.ApplyBlackListDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyCreditAudit(self, request):
         """提交信审外呼申请，返回当次请求日期。
 
         :param request: Request instance for ApplyCreditAudit.
         :type request: :class:`tencentcloud.cr.v20180321.models.ApplyCreditAuditRequest`
@@ -88,15 +88,15 @@
             model = models.ApplyCreditAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeBotCallStatus(self, request):
         """更新机器人任务作业状态
 
         :param request: Request instance for ChangeBotCallStatus.
         :type request: :class:`tencentcloud.cr.v20180321.models.ChangeBotCallStatusRequest`
@@ -111,15 +111,15 @@
             model = models.ChangeBotCallStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeBotTaskStatus(self, request):
         """更新机器人任务状态
 
         :param request: Request instance for ChangeBotTaskStatus.
         :type request: :class:`tencentcloud.cr.v20180321.models.ChangeBotTaskStatusRequest`
@@ -134,15 +134,15 @@
             model = models.ChangeBotTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBotTask(self, request):
         """创建机器人任务
 
         :param request: Request instance for CreateBotTask.
         :type request: :class:`tencentcloud.cr.v20180321.models.CreateBotTaskRequest`
@@ -157,15 +157,15 @@
             model = models.CreateBotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBotFlow(self, request):
         """查询机器人对话流
 
         :param request: Request instance for DescribeBotFlow.
         :type request: :class:`tencentcloud.cr.v20180321.models.DescribeBotFlowRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeBotFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCreditResult(self, request):
         """根据信审任务ID和请求日期，获取相关信审结果。
 
         :param request: Request instance for DescribeCreditResult.
         :type request: :class:`tencentcloud.cr.v20180321.models.DescribeCreditResultRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeCreditResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileModel(self, request):
         """查询机器人文件模板
 
         :param request: Request instance for DescribeFileModel.
         :type request: :class:`tencentcloud.cr.v20180321.models.DescribeFileModelRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeFileModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecords(self, request):
         """用于获取指定案件的录音地址，次日早上8:00后可查询前日录音。
 
         :param request: Request instance for DescribeRecords.
         :type request: :class:`tencentcloud.cr.v20180321.models.DescribeRecordsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStatus(self, request):
         """根据上传文件接口的输出参数DataResId，获取相关上传结果。
 
         :param request: Request instance for DescribeTaskStatus.
         :type request: :class:`tencentcloud.cr.v20180321.models.DescribeTaskStatusRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadBotRecord(self, request):
         """下载任务录音与文本，第二天12点后可使用此接口获取对应的录音与文本
 
         :param request: Request instance for DownloadBotRecord.
         :type request: :class:`tencentcloud.cr.v20180321.models.DownloadBotRecordRequest`
@@ -295,15 +295,15 @@
             model = models.DownloadBotRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadDialogueText(self, request):
         """用于获取指定案件的对话文本内容，次日早上8:00后可查询前日对话文本内容。
 
         :param request: Request instance for DownloadDialogueText.
         :type request: :class:`tencentcloud.cr.v20180321.models.DownloadDialogueTextRequest`
@@ -318,15 +318,15 @@
             model = models.DownloadDialogueTextResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadRecordList(self, request):
         """<p>用于获取录音下载链接清单，次日早上8:00后可查询前日录音清单。</p>
         <p>注意：录音清单中的录音下载链接仅次日20:00之前有效，请及时下载。</p>
 
         :param request: Request instance for DownloadRecordList.
@@ -342,15 +342,15 @@
             model = models.DownloadRecordListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadReport(self, request):
         """用于下载结果报表。当日23:00后，可获取当日到期/逾期提醒结果，次日00:30后，可获取昨日回访结果。
 
         :param request: Request instance for DownloadReport.
         :type request: :class:`tencentcloud.cr.v20180321.models.DownloadReportRequest`
@@ -365,15 +365,15 @@
             model = models.DownloadReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportBotData(self, request):
         """导出机器人数据
 
         :param request: Request instance for ExportBotData.
         :type request: :class:`tencentcloud.cr.v20180321.models.ExportBotDataRequest`
@@ -388,15 +388,15 @@
             model = models.ExportBotDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBlackListData(self, request):
         """查看黑名单数据列表
 
         :param request: Request instance for QueryBlackListData.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryBlackListDataRequest`
@@ -411,15 +411,15 @@
             model = models.QueryBlackListDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBotList(self, request):
         """查询机器人任务状态列表
 
         :param request: Request instance for QueryBotList.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryBotListRequest`
@@ -434,15 +434,15 @@
             model = models.QueryBotListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCallList(self, request):
         """机器人任务查询
 
         :param request: Request instance for QueryCallList.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryCallListRequest`
@@ -457,15 +457,15 @@
             model = models.QueryCallListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryInstantData(self, request):
         """实时数据查询
 
         :param request: Request instance for QueryInstantData.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryInstantDataRequest`
@@ -480,15 +480,15 @@
             model = models.QueryInstantDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryProducts(self, request):
         """查询产品列表
 
         :param request: Request instance for QueryProducts.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryProductsRequest`
@@ -503,15 +503,15 @@
             model = models.QueryProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryRecordList(self, request):
         """查询录音列表
 
         :param request: Request instance for QueryRecordList.
         :type request: :class:`tencentcloud.cr.v20180321.models.QueryRecordListRequest`
@@ -526,15 +526,15 @@
             model = models.QueryRecordListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateBotTask(self, request):
         """更新机器人任务
 
         :param request: Request instance for UpdateBotTask.
         :type request: :class:`tencentcloud.cr.v20180321.models.UpdateBotTaskRequest`
@@ -549,15 +549,15 @@
             model = models.UpdateBotTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadBotData(self, request):
         """上传机器人任务数据
 
         :param request: Request instance for UploadBotData.
         :type request: :class:`tencentcloud.cr.v20180321.models.UploadBotDataRequest`
@@ -572,15 +572,15 @@
             model = models.UploadBotDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadBotFile(self, request):
         """上传机器人文件
 
         :param request: Request instance for UploadBotFile.
         :type request: :class:`tencentcloud.cr.v20180321.models.UploadBotFileRequest`
@@ -595,15 +595,15 @@
             model = models.UploadBotFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadDataFile(self, request):
         """上传文件，接口返回数据任务ID，支持xlsx、xls、csv、zip格式。
 
         :param request: Request instance for UploadDataFile.
         :type request: :class:`tencentcloud.cr.v20180321.models.UploadDataFileRequest`
@@ -619,15 +619,15 @@
             model = models.UploadDataFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadDataJson(self, request):
         """上传Json格式数据，接口返回数据任务ID
 
         :param request: Request instance for UploadDataJson.
         :type request: :class:`tencentcloud.cr.v20180321.models.UploadDataJsonRequest`
@@ -642,15 +642,15 @@
             model = models.UploadDataJsonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFile(self, request):
         """客户通过调用该接口上传需催收文档，格式需为excel格式。接口返回任务ID。
 
         :param request: Request instance for UploadFile.
         :type request: :class:`tencentcloud.cr.v20180321.models.UploadFileRequest`
@@ -665,8 +665,8 @@
             model = models.UploadFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/errorcodes.py` & `tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.937/tencentcloud/cr/v20180321/models.py` & `tencentcloud-sdk-python-cr-3.0.938/tencentcloud/cr/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cr-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cr-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cr-3.0.937/tencentcloud_sdk_python_cr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.938/tencentcloud_sdk_python_cr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cr-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cr-3.0.937/README.rst` & `tencentcloud-sdk-python-cr-3.0.938/README.rst`

 * *Files identical despite different names*

