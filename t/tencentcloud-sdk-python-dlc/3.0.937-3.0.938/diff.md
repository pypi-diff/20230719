# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.937.tar", last modified: Tue Jul 18 00:22:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.938.tar", last modified: Wed Jul 19 00:37:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.937.tar` & `tencentcloud-sdk-python-dlc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82345 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   562386 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82705 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   562386 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:37:46.000000 tencentcloud-sdk-python-dlc-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/setup.py` & `tencentcloud-sdk-python-dlc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.938/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddDMSPartitionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddUsersToWorkGroup(self, request):
         """添加用户到工作组
 
         :param request: Request instance for AddUsersToWorkGroup.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AddUsersToWorkGroupRequest`
@@ -65,15 +65,15 @@
             model = models.AddUsersToWorkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AlterDMSDatabase(self, request):
         """DMS元数据更新库
 
         :param request: Request instance for AlterDMSDatabase.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AlterDMSDatabaseRequest`
@@ -88,15 +88,15 @@
             model = models.AlterDMSDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AlterDMSPartition(self, request):
         """DMS元数据更新分区
 
         :param request: Request instance for AlterDMSPartition.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AlterDMSPartitionRequest`
@@ -111,15 +111,15 @@
             model = models.AlterDMSPartitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AlterDMSTable(self, request):
         """DMS元数据更新表
 
         :param request: Request instance for AlterDMSTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AlterDMSTableRequest`
@@ -134,15 +134,15 @@
             model = models.AlterDMSTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachUserPolicy(self, request):
         """绑定鉴权策略到用户
 
         :param request: Request instance for AttachUserPolicy.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AttachUserPolicyRequest`
@@ -157,15 +157,15 @@
             model = models.AttachUserPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachWorkGroupPolicy(self, request):
         """绑定鉴权策略到工作组
 
         :param request: Request instance for AttachWorkGroupPolicy.
         :type request: :class:`tencentcloud.dlc.v20210125.models.AttachWorkGroupPolicyRequest`
@@ -180,15 +180,15 @@
             model = models.AttachWorkGroupPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindWorkGroupsToUser(self, request):
         """绑定工作组到用户
 
         :param request: Request instance for BindWorkGroupsToUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.BindWorkGroupsToUserRequest`
@@ -203,15 +203,15 @@
             model = models.BindWorkGroupsToUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelNotebookSessionStatement(self, request):
         """本接口（CancelNotebookSessionStatement）用于取消session中执行的任务
 
         :param request: Request instance for CancelNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementRequest`
@@ -226,15 +226,15 @@
             model = models.CancelNotebookSessionStatementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelNotebookSessionStatementBatch(self, request):
         """本接口（CancelNotebookSessionStatementBatch）用于批量取消Session 中执行的任务
 
         :param request: Request instance for CancelNotebookSessionStatementBatch.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementBatchRequest`
@@ -249,15 +249,15 @@
             model = models.CancelNotebookSessionStatementBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelSparkSessionBatchSQL(self, request):
         """本接口（CancelSparkSessionBatchSQL）用于取消Spark SQL批任务。
 
         :param request: Request instance for CancelSparkSessionBatchSQL.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelSparkSessionBatchSQLRequest`
@@ -272,15 +272,15 @@
             model = models.CancelSparkSessionBatchSQLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelTask(self, request):
         """本接口（CancelTask），用于取消任务
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTaskRequest`
@@ -295,15 +295,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckLockMetaData(self, request):
         """元数据锁检查
 
         :param request: Request instance for CheckLockMetaData.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CheckLockMetaDataRequest`
@@ -318,15 +318,15 @@
             model = models.CheckLockMetaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDMSDatabase(self, request):
         """DMS元数据创建库
 
         :param request: Request instance for CreateDMSDatabase.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateDMSDatabaseRequest`
@@ -341,15 +341,15 @@
             model = models.CreateDMSDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDMSTable(self, request):
         """DMS元数据创建表
 
         :param request: Request instance for CreateDMSTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateDMSTableRequest`
@@ -364,15 +364,15 @@
             model = models.CreateDMSTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDataEngine(self, request):
         """为用户创建数据引擎
 
         :param request: Request instance for CreateDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateDataEngineRequest`
@@ -387,15 +387,15 @@
             model = models.CreateDataEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDatabase(self, request):
         """本接口（CreateDatabase）用于生成建库SQL语句。
 
         :param request: Request instance for CreateDatabase.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateDatabaseRequest`
@@ -410,15 +410,15 @@
             model = models.CreateDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateExportTask(self, request):
         """该接口（CreateExportTask）用于创建导出任务
 
         :param request: Request instance for CreateExportTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateExportTaskRequest`
@@ -433,15 +433,15 @@
             model = models.CreateExportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImportTask(self, request):
         """该接口（CreateImportTask）用于创建导入任务
 
         :param request: Request instance for CreateImportTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateImportTaskRequest`
@@ -456,15 +456,15 @@
             model = models.CreateImportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInternalTable(self, request):
         """创建托管存储内表（该接口已废弃）
 
         :param request: Request instance for CreateInternalTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateInternalTableRequest`
@@ -479,15 +479,15 @@
             model = models.CreateInternalTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotebookSession(self, request):
         """本接口（CreateNotebookSession）用于创建交互式session（notebook）
 
         :param request: Request instance for CreateNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionRequest`
@@ -502,15 +502,15 @@
             model = models.CreateNotebookSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotebookSessionStatement(self, request):
         """本接口（CreateNotebookSessionStatement）用于在session中执行代码片段
 
         :param request: Request instance for CreateNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementRequest`
@@ -525,15 +525,15 @@
             model = models.CreateNotebookSessionStatementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotebookSessionStatementSupportBatchSQL(self, request):
         """本接口（CreateNotebookSessionStatementSupportBatchSQL）用于创建交互式session并执行SQL任务
 
         :param request: Request instance for CreateNotebookSessionStatementSupportBatchSQL.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementSupportBatchSQLRequest`
@@ -548,15 +548,15 @@
             model = models.CreateNotebookSessionStatementSupportBatchSQLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResultDownload(self, request):
         """创建查询结果下载任务
 
         :param request: Request instance for CreateResultDownload.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateResultDownloadRequest`
@@ -571,15 +571,15 @@
             model = models.CreateResultDownloadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScript(self, request):
         """该接口（CreateScript）用于创建sql脚本。
 
         :param request: Request instance for CreateScript.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateScriptRequest`
@@ -594,15 +594,15 @@
             model = models.CreateScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSparkApp(self, request):
         """创建spark作业
 
         :param request: Request instance for CreateSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppRequest`
@@ -617,15 +617,15 @@
             model = models.CreateSparkAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSparkAppTask(self, request):
         """启动Spark作业
 
         :param request: Request instance for CreateSparkAppTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppTaskRequest`
@@ -640,15 +640,15 @@
             model = models.CreateSparkAppTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSparkSessionBatchSQL(self, request):
         """本接口（CreateSparkSessionBatchSQL）用于向Spark作业引擎提交Spark SQL批任务。
 
         :param request: Request instance for CreateSparkSessionBatchSQL.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkSessionBatchSQLRequest`
@@ -663,15 +663,15 @@
             model = models.CreateSparkSessionBatchSQLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStoreLocation(self, request):
         """该接口（CreateStoreLocation）新增或覆盖计算结果存储位置。
 
         :param request: Request instance for CreateStoreLocation.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateStoreLocationRequest`
@@ -686,15 +686,15 @@
             model = models.CreateStoreLocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTable(self, request):
         """本接口（CreateTable）用于生成建表SQL。
 
         :param request: Request instance for CreateTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTableRequest`
@@ -709,15 +709,15 @@
             model = models.CreateTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTask(self, request):
         """本接口（CreateTask）用于创建并执行SQL任务。（推荐使用CreateTasks接口）
 
         :param request: Request instance for CreateTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTaskRequest`
@@ -732,15 +732,15 @@
             model = models.CreateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTasks(self, request):
         """本接口（CreateTasks），用于批量创建并执行SQL任务
 
         :param request: Request instance for CreateTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTasksRequest`
@@ -755,15 +755,15 @@
             model = models.CreateTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTasksInOrder(self, request):
         """按顺序创建任务（已经废弃，后期不再维护，请使用接口CreateTasks）
 
         :param request: Request instance for CreateTasksInOrder.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTasksInOrderRequest`
@@ -778,15 +778,15 @@
             model = models.CreateTasksInOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """创建用户
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateUserRequest`
@@ -801,15 +801,15 @@
             model = models.CreateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkGroup(self, request):
         """创建工作组
 
         :param request: Request instance for CreateWorkGroup.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateWorkGroupRequest`
@@ -824,15 +824,15 @@
             model = models.CreateWorkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNotebookSession(self, request):
         """本接口（DeleteNotebookSession）用于删除交互式session（notebook）
 
         :param request: Request instance for DeleteNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteNotebookSessionRequest`
@@ -847,15 +847,15 @@
             model = models.DeleteNotebookSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScript(self, request):
         """该接口（DeleteScript）用于删除sql脚本。
 
         :param request: Request instance for DeleteScript.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteScriptRequest`
@@ -870,15 +870,15 @@
             model = models.DeleteScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSparkApp(self, request):
         """删除spark作业
 
         :param request: Request instance for DeleteSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteSparkAppRequest`
@@ -893,15 +893,15 @@
             model = models.DeleteSparkAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUser(self, request):
         """删除用户
 
         :param request: Request instance for DeleteUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteUserRequest`
@@ -916,15 +916,15 @@
             model = models.DeleteUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsersFromWorkGroup(self, request):
         """从工作组中删除用户
 
         :param request: Request instance for DeleteUsersFromWorkGroup.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteUsersFromWorkGroupRequest`
@@ -939,15 +939,15 @@
             model = models.DeleteUsersFromWorkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWorkGroup(self, request):
         """删除工作组
 
         :param request: Request instance for DeleteWorkGroup.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteWorkGroupRequest`
@@ -962,15 +962,15 @@
             model = models.DeleteWorkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDMSDatabase(self, request):
         """DMS元数据获取库
 
         :param request: Request instance for DescribeDMSDatabase.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDMSDatabaseRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDMSDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDMSPartitions(self, request):
         """DMS元数据获取分区
 
         :param request: Request instance for DescribeDMSPartitions.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDMSPartitionsRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDMSPartitionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDMSTable(self, request):
         """DMS元数据获取表
 
         :param request: Request instance for DescribeDMSTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDMSTableRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeDMSTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDMSTables(self, request):
         """DMS元数据获取表列表
 
         :param request: Request instance for DescribeDMSTables.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDMSTablesRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeDMSTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataEngines(self, request):
         """本接口（DescribeDataEngines）用于查询DataEngines信息列表
 
         :param request: Request instance for DescribeDataEngines.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginesRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeDataEnginesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabases(self, request):
         """本接口（DescribeDatabases）用于查询数据库列表。
 
         :param request: Request instance for DescribeDatabases.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDatabasesRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEngineUsageInfo(self, request):
         """本接口根据引擎ID查询数据引擎资源使用情况
 
         :param request: Request instance for DescribeEngineUsageInfo.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeEngineUsageInfoRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeEngineUsageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeForbiddenTablePro(self, request):
         """本接口（DescribeForbiddenTablePro）用于查询被禁用的表属性列表（新）
 
         :param request: Request instance for DescribeForbiddenTablePro.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTableProRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeForbiddenTableProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLakeFsDirSummary(self, request):
         """查询托管存储指定目录的Summary
 
         :param request: Request instance for DescribeLakeFsDirSummary.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsDirSummaryRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeLakeFsDirSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLakeFsInfo(self, request):
         """查询用户的托管存储信息
 
         :param request: Request instance for DescribeLakeFsInfo.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeLakeFsInfoRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeLakeFsInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSession(self, request):
         """本接口（DescribeNotebookSession）用于查询交互式 session详情信息
 
         :param request: Request instance for DescribeNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeNotebookSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSessionLog(self, request):
         """本接口（DescribeNotebookSessionLog）用于查询交互式 session日志
 
         :param request: Request instance for DescribeNotebookSessionLog.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionLogRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeNotebookSessionLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSessionStatement(self, request):
         """本接口（DescribeNotebookSessionStatement）用于查询session 中执行任务的详情
 
         :param request: Request instance for DescribeNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeNotebookSessionStatementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSessionStatementSqlResult(self, request):
         """本接口（DescribeNotebookSessionStatementSqlResult）用于获取statement运行结果。
 
         :param request: Request instance for DescribeNotebookSessionStatementSqlResult.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementSqlResultRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeNotebookSessionStatementSqlResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSessionStatements(self, request):
         """本接口（DescribeNotebookSessionStatements）用于查询Session中执行的任务列表
 
         :param request: Request instance for DescribeNotebookSessionStatements.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementsRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeNotebookSessionStatementsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSessions(self, request):
         """本接口（DescribeNotebookSessions）用于查询交互式 session列表
 
         :param request: Request instance for DescribeNotebookSessions.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionsRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeNotebookSessionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResultDownload(self, request):
         """查询结果下载任务
 
         :param request: Request instance for DescribeResultDownload.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeResultDownloadRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeResultDownloadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScripts(self, request):
         """该接口（DescribeScripts）用于查询SQL脚本列表
 
         :param request: Request instance for DescribeScripts.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeScriptsRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeScriptsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSparkAppJob(self, request):
         """查询spark作业信息
 
         :param request: Request instance for DescribeSparkAppJob.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeSparkAppJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSparkAppJobs(self, request):
         """查询spark作业列表
 
         :param request: Request instance for DescribeSparkAppJobs.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobsRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeSparkAppJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSparkAppTasks(self, request):
         """查询Spark作业的运行任务列表
 
         :param request: Request instance for DescribeSparkAppTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppTasksRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeSparkAppTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSparkSessionBatchSqlLog(self, request):
         """本接口（DescribeSparkSessionBatchSqlLog）用于获取SparkSQL批任务日志
 
         :param request: Request instance for DescribeSparkSessionBatchSqlLog.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlLogRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeSparkSessionBatchSqlLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStoreLocation(self, request):
         """查询计算结果存储位置。
 
         :param request: Request instance for DescribeStoreLocation.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeStoreLocationRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeStoreLocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTable(self, request):
         """本接口（DescribeTable），用于查询单个表的详细信息。
 
         :param request: Request instance for DescribeTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeTableRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTables(self, request):
         """本接口（DescribeTables）用于查询数据表列表。
 
         :param request: Request instance for DescribeTables.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeTablesRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskResult(self, request):
         """查询任务结果
 
         :param request: Request instance for DescribeTaskResult.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeTaskResultRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """该接口（DescribleTasks）用于查询任务列表
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeTasksRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsers(self, request):
         """获取用户列表信息
 
         :param request: Request instance for DescribeUsers.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeUsersRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeViews(self, request):
         """本接口（DescribeViews）用于查询数据视图列表。
 
         :param request: Request instance for DescribeViews.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeViewsRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribeViewsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkGroups(self, request):
         """获取工作组列表
 
         :param request: Request instance for DescribeWorkGroups.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeWorkGroupsRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeWorkGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachUserPolicy(self, request):
         """解绑用户鉴权策略
 
         :param request: Request instance for DetachUserPolicy.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DetachUserPolicyRequest`
@@ -1675,15 +1675,15 @@
             model = models.DetachUserPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachWorkGroupPolicy(self, request):
         """解绑工作组鉴权策略
 
         :param request: Request instance for DetachWorkGroupPolicy.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DetachWorkGroupPolicyRequest`
@@ -1698,15 +1698,15 @@
             model = models.DetachWorkGroupPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DropDMSDatabase(self, request):
         """DMS元数据删除库
 
         :param request: Request instance for DropDMSDatabase.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DropDMSDatabaseRequest`
@@ -1721,15 +1721,15 @@
             model = models.DropDMSDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DropDMSPartitions(self, request):
         """DMS元数据删除分区
 
         :param request: Request instance for DropDMSPartitions.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DropDMSPartitionsRequest`
@@ -1744,15 +1744,15 @@
             model = models.DropDMSPartitionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DropDMSTable(self, request):
         """DMS元数据删除表
 
         :param request: Request instance for DropDMSTable.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DropDMSTableRequest`
@@ -1767,15 +1767,15 @@
             model = models.DropDMSTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateCreateMangedTableSql(self, request):
         """生成创建托管表语句
 
         :param request: Request instance for GenerateCreateMangedTableSql.
         :type request: :class:`tencentcloud.dlc.v20210125.models.GenerateCreateMangedTableSqlRequest`
@@ -1790,15 +1790,15 @@
             model = models.GenerateCreateMangedTableSqlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTaskJobLogDetail(self, request):
         """本接口（ListTaskJobLogDetail）用于获取spark 作业任务日志详情
 
         :param request: Request instance for ListTaskJobLogDetail.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ListTaskJobLogDetailRequest`
@@ -1813,15 +1813,15 @@
             model = models.ListTaskJobLogDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LockMetaData(self, request):
         """元数据锁
 
         :param request: Request instance for LockMetaData.
         :type request: :class:`tencentcloud.dlc.v20210125.models.LockMetaDataRequest`
@@ -1836,15 +1836,15 @@
             model = models.LockMetaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGovernEventRule(self, request):
         """修改数据治理事件阈值
 
         :param request: Request instance for ModifyGovernEventRule.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyGovernEventRuleRequest`
@@ -1859,15 +1859,15 @@
             model = models.ModifyGovernEventRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySparkApp(self, request):
         """更新spark作业
 
         :param request: Request instance for ModifySparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppRequest`
@@ -1882,15 +1882,15 @@
             model = models.ModifySparkAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySparkAppBatch(self, request):
         """本接口（ModifySparkAppBatch）用于批量修改Spark作业参数配置
 
         :param request: Request instance for ModifySparkAppBatch.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppBatchRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifySparkAppBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUser(self, request):
         """修改用户信息
 
         :param request: Request instance for ModifyUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyUserRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWorkGroup(self, request):
         """修改工作组信息
 
         :param request: Request instance for ModifyWorkGroup.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifyWorkGroupRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyWorkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportHeartbeatMetaData(self, request):
         """上报元数据心跳
 
         :param request: Request instance for ReportHeartbeatMetaData.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ReportHeartbeatMetaDataRequest`
@@ -1974,15 +1974,15 @@
             model = models.ReportHeartbeatMetaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SuspendResumeDataEngine(self, request):
         """本接口用于控制挂起或启动数据引擎
 
         :param request: Request instance for SuspendResumeDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.SuspendResumeDataEngineRequest`
@@ -1997,15 +1997,15 @@
             model = models.SuspendResumeDataEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchDataEngine(self, request):
         """切换主备集群
 
         :param request: Request instance for SwitchDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.SwitchDataEngineRequest`
@@ -2020,15 +2020,15 @@
             model = models.SwitchDataEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindWorkGroupsFromUser(self, request):
         """解绑用户上的用户组
 
         :param request: Request instance for UnbindWorkGroupsFromUser.
         :type request: :class:`tencentcloud.dlc.v20210125.models.UnbindWorkGroupsFromUserRequest`
@@ -2043,15 +2043,15 @@
             model = models.UnbindWorkGroupsFromUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlockMetaData(self, request):
         """元数据解锁
 
         :param request: Request instance for UnlockMetaData.
         :type request: :class:`tencentcloud.dlc.v20210125.models.UnlockMetaDataRequest`
@@ -2066,15 +2066,15 @@
             model = models.UnlockMetaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRowFilter(self, request):
         """此接口用于更新行过滤规则。注意只能更新过滤规则，不能更新规格对象catalog，database和table。
 
         :param request: Request instance for UpdateRowFilter.
         :type request: :class:`tencentcloud.dlc.v20210125.models.UpdateRowFilterRequest`
@@ -2089,8 +2089,8 @@
             model = models.UpdateRowFilterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/dlc/v20210125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.937/README.rst` & `tencentcloud-sdk-python-dlc-3.0.938/README.rst`

 * *Files identical despite different names*

