# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.937.tar", last modified: Tue Jul 18 00:22:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.938.tar", last modified: Wed Jul 19 00:37:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.937.tar` & `tencentcloud-sdk-python-dbbrain-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    53256 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   325476 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   183920 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:22:09.000000 tencentcloud-sdk-python-dbbrain-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    53472 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   325476 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27767 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   183920 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:37:24.000000 tencentcloud-sdk-python-dbbrain-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddUserContactResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelKillTask(self, request):
         """终止中断会话任务。
 
         :param request: Request instance for CancelKillTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CancelKillTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CancelKillTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseAuditService(self, request):
         """不用审计日志时，关闭数据库审计
 
         :param request: Request instance for CloseAuditService.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CloseAuditServiceRequest`
@@ -88,15 +88,15 @@
             model = models.CloseAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAuditLogFile(self, request):
         """用于创建云数据库实例的审计日志文件，最多下载600w审计日志。
 
         :param request: Request instance for CreateAuditLogFile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateAuditLogFileRequest`
@@ -111,15 +111,15 @@
             model = models.CreateAuditLogFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBDiagReportTask(self, request):
         """创建健康报告，并可以选择是否发送邮件。
 
         :param request: Request instance for CreateDBDiagReportTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateDBDiagReportTaskRequest`
@@ -134,15 +134,15 @@
             model = models.CreateDBDiagReportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBDiagReportUrl(self, request):
         """创建健康报告的浏览地址。
 
         :param request: Request instance for CreateDBDiagReportUrl.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateDBDiagReportUrlRequest`
@@ -157,15 +157,15 @@
             model = models.CreateDBDiagReportUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKillTask(self, request):
         """创建中断会话的任务。
 
         :param request: Request instance for CreateKillTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateKillTaskRequest`
@@ -180,15 +180,15 @@
             model = models.CreateKillTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMailProfile(self, request):
         """创建邮件配置。其中入参ProfileType表示所创建配置的类型，ProfileType 取值包括：dbScan_mail_configuration（数据库巡检邮件配置）、scheduler_mail_configuration（定期生成健康报告的邮件发送配置）。Region统一选择广州，和实例所属地域无关。
 
         :param request: Request instance for CreateMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateMailProfileRequest`
@@ -203,15 +203,15 @@
             model = models.CreateMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxySessionKillTask(self, request):
         """创建中止所有代理节点连接会话的异步任务。当前仅支持 Redis。得到的返回值为异步任务 id，可以作为参数传入接口 DescribeProxySessionKillTasks 查询kill会话任务执行状态。
 
         :param request: Request instance for CreateProxySessionKillTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateProxySessionKillTaskRequest`
@@ -226,15 +226,15 @@
             model = models.CreateProxySessionKillTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRedisBigKeyAnalysisTask(self, request):
         """即时创建redis实例大key分析任务，限制正在运行的即时分析任务数量默认为5。
 
         :param request: Request instance for CreateRedisBigKeyAnalysisTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateRedisBigKeyAnalysisTaskRequest`
@@ -249,15 +249,15 @@
             model = models.CreateRedisBigKeyAnalysisTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSchedulerMailProfile(self, request):
         """该接口用于创建定期生成健康报告并邮件发送的配置，将健康报告的定期生成时间作为参数传入（周一至周日），用于设置健康报告的定期生成时间，同时保存相应的定期邮件发送的配置。
 
         :param request: Request instance for CreateSchedulerMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateSchedulerMailProfileRequest`
@@ -272,15 +272,15 @@
             model = models.CreateSchedulerMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityAuditLogExportTask(self, request):
         """创建安全审计日志导出任务。
 
         :param request: Request instance for CreateSecurityAuditLogExportTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateSecurityAuditLogExportTaskRequest`
@@ -295,15 +295,15 @@
             model = models.CreateSecurityAuditLogExportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSqlFilter(self, request):
         """创建实例SQL限流任务。
 
         :param request: Request instance for CreateSqlFilter.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateSqlFilterRequest`
@@ -318,15 +318,15 @@
             model = models.CreateSqlFilterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAuditLogFile(self, request):
         """用于删除云数据库实例的审计日志文件。
 
         :param request: Request instance for DeleteAuditLogFile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteAuditLogFileRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteAuditLogFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDBDiagReportTasks(self, request):
         """根据任务id删除健康报告生成任务
 
         :param request: Request instance for DeleteDBDiagReportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteDBDiagReportTasksRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteDBDiagReportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityAuditLogExportTasks(self, request):
         """删除安全审计日志导出任务。
 
         :param request: Request instance for DeleteSecurityAuditLogExportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteSecurityAuditLogExportTasksRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteSecurityAuditLogExportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSqlFilters(self, request):
         """删除实例SQL限流任务。
 
         :param request: Request instance for DeleteSqlFilters.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteSqlFiltersRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteSqlFiltersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllUserContact(self, request):
         """获取邮件发送中联系人的相关信息。
 
         :param request: Request instance for DescribeAllUserContact.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAllUserContactRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeAllUserContactResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllUserGroup(self, request):
         """获取邮件发送联系组的相关信息。
 
         :param request: Request instance for DescribeAllUserGroup.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAllUserGroupRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeAllUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditInstanceList(self, request):
         """查询实例列表
 
         :param request: Request instance for DescribeAuditInstanceList.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAuditInstanceListRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeAuditInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditLogFiles(self, request):
         """用于创建云数据库实例的审计日志文件
 
         :param request: Request instance for DescribeAuditLogFiles.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAuditLogFilesRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeAuditLogFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagEvent(self, request):
         """获取实例异常诊断事件的详情信息。
 
         :param request: Request instance for DescribeDBDiagEvent.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBDiagEventRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeDBDiagEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagEvents(self, request):
         """获取指定时间段内的诊断事件列表，支持依据风险等级、实例ID等条件过滤。
 
         :param request: Request instance for DescribeDBDiagEvents.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBDiagEventsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeDBDiagEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagHistory(self, request):
         """获取实例诊断事件的列表。
 
         :param request: Request instance for DescribeDBDiagHistory.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBDiagHistoryRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeDBDiagHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagReportTasks(self, request):
         """查询健康报告生成任务列表。
 
         :param request: Request instance for DescribeDBDiagReportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBDiagReportTasksRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeDBDiagReportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSpaceStatus(self, request):
         """获取指定时间段内的实例空间使用概览，包括磁盘增长量(MB)、磁盘剩余(MB)、磁盘总量(MB)及预计可用天数。
 
         :param request: Request instance for DescribeDBSpaceStatus.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBSpaceStatusRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeDBSpaceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiagDBInstances(self, request):
         """获取实例信息列表。Region统一选择广州。
 
         :param request: Request instance for DescribeDiagDBInstances.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDiagDBInstancesRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeDiagDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHealthScore(self, request):
         """根据实例ID获取指定时间段（30分钟）的健康得分，以及异常扣分项。
 
         :param request: Request instance for DescribeHealthScore.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeHealthScoreRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeHealthScoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMailProfile(self, request):
         """获取发送邮件的配置， 包括数据库巡检的邮件配置以及定期生成健康报告的邮件发送配置。
 
         :param request: Request instance for DescribeMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeMailProfileRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMySqlProcessList(self, request):
         """查询关系型数据库的实时线程列表。
 
         :param request: Request instance for DescribeMySqlProcessList.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeMySqlProcessListRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeMySqlProcessListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNoPrimaryKeyTables(self, request):
         """查询实例无主键表。
 
         :param request: Request instance for DescribeNoPrimaryKeyTables.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeNoPrimaryKeyTablesRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeNoPrimaryKeyTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyProcessStatistics(self, request):
         """获取当前实例下的单个proxy的会话统计详情信息， 返回数据为单个 proxy 的会话统计信息。【注意】该接口仅限部分环境调用。
 
         :param request: Request instance for DescribeProxyProcessStatistics.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeProxyProcessStatisticsRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeProxyProcessStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxySessionKillTasks(self, request):
         """用于查询 redis 执行 kill 会话任务后代理节点的执行结果，入参异步任务 ID 从接口 CreateProxySessionKillTask 调用成功后取得。当前 product 只支持：redis。
 
         :param request: Request instance for DescribeProxySessionKillTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeProxySessionKillTasksRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeProxySessionKillTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRedisTopBigKeys(self, request):
         """查询redis实例大key列表。
 
         :param request: Request instance for DescribeRedisTopBigKeys.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeRedisTopBigKeysRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeRedisTopBigKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRedisTopKeyPrefixList(self, request):
         """查询redis实例top key前缀列表。
 
         :param request: Request instance for DescribeRedisTopKeyPrefixList.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeRedisTopKeyPrefixListRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeRedisTopKeyPrefixListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityAuditLogDownloadUrls(self, request):
         """查询安全审计日志导出文件下载链接。目前日志文件下载仅提供腾讯云内网地址，请通过广州地域的腾讯云服务器进行下载。
 
         :param request: Request instance for DescribeSecurityAuditLogDownloadUrls.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSecurityAuditLogDownloadUrlsRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeSecurityAuditLogDownloadUrlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityAuditLogExportTasks(self, request):
         """查询安全审计日志导出任务列表。
 
         :param request: Request instance for DescribeSecurityAuditLogExportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSecurityAuditLogExportTasksRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeSecurityAuditLogExportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogTimeSeriesStats(self, request):
         """获取慢日志统计柱状图。
 
         :param request: Request instance for DescribeSlowLogTimeSeriesStats.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogTimeSeriesStatsRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeSlowLogTimeSeriesStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogTopSqls(self, request):
         """按照Sql模板+schema的聚合方式，统计排序指定时间段内的top慢sql。
 
         :param request: Request instance for DescribeSlowLogTopSqls.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogTopSqlsRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeSlowLogTopSqlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogUserHostStats(self, request):
         """获取慢日志来源地址统计分布图。
 
         :param request: Request instance for DescribeSlowLogUserHostStats.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogUserHostStatsRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeSlowLogUserHostStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogs(self, request):
         """获取指定时间内某个sql模板的慢日志明细
 
         :param request: Request instance for DescribeSlowLogs.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeSlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSqlFilters(self, request):
         """查询实例SQL限流任务列表。
 
         :param request: Request instance for DescribeSqlFilters.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSqlFiltersRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeSqlFiltersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSqlTemplate(self, request):
         """查询SQL模板。
 
         :param request: Request instance for DescribeSqlTemplate.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSqlTemplateRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeSqlTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceSchemaTimeSeries(self, request):
         """获取实例占用空间最大的前几个库在指定时间段内的每日由DBbrain定时采集的空间数据，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceSchemaTimeSeries.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeTopSpaceSchemaTimeSeriesRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeTopSpaceSchemaTimeSeriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceSchemas(self, request):
         """获取实例Top库的实时空间统计信息，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceSchemas.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeTopSpaceSchemasRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeTopSpaceSchemasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceTableTimeSeries(self, request):
         """获取实例占用空间最大的前几张表在指定时间段内的每日由DBbrain定时采集的空间数据，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceTableTimeSeries.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeTopSpaceTableTimeSeriesRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeTopSpaceTableTimeSeriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceTables(self, request):
         """获取实例Top表的实时空间统计信息，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceTables.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeTopSpaceTablesRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeTopSpaceTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserSqlAdvice(self, request):
         """获取SQL优化建议。【产品用户回馈，此接口限免开放，后续将并入dbbrain专业版】
 
         :param request: Request instance for DescribeUserSqlAdvice.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeUserSqlAdviceRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeUserSqlAdviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KillMySqlThreads(self, request):
         """根据会话ID中断当前会话，该接口分为两次提交：第一次为预提交阶段，Stage为"Prepare"，得到的返回值包含SqlExecId；第二次为确认提交， Stage为"Commit"， 将SqlExecId的值作为参数传入，最终终止会话进程。
 
         :param request: Request instance for KillMySqlThreads.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.KillMySqlThreadsRequest`
@@ -1146,15 +1146,15 @@
             model = models.KillMySqlThreadsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAuditService(self, request):
         """修改审计配置相关信息，如高频存储时长等
 
         :param request: Request instance for ModifyAuditService.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.ModifyAuditServiceRequest`
@@ -1169,15 +1169,15 @@
             model = models.ModifyAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDiagDBInstanceConf(self, request):
         """修改实例巡检开关。
 
         :param request: Request instance for ModifyDiagDBInstanceConf.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.ModifyDiagDBInstanceConfRequest`
@@ -1192,15 +1192,15 @@
             model = models.ModifyDiagDBInstanceConfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySqlFilters(self, request):
         """更改实例限流任务状态，目前仅用于终止限流。
 
         :param request: Request instance for ModifySqlFilters.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.ModifySqlFiltersRequest`
@@ -1215,15 +1215,15 @@
             model = models.ModifySqlFiltersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenAuditService(self, request):
         """开启数据库审计服务
 
         :param request: Request instance for OpenAuditService.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.OpenAuditServiceRequest`
@@ -1238,15 +1238,15 @@
             model = models.OpenAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyUserAccount(self, request):
         """验证用户数据库账号权限，获取会话token。
 
         :param request: Request instance for VerifyUserAccount.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.VerifyUserAccountRequest`
@@ -1261,8 +1261,8 @@
             model = models.VerifyUserAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20210527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddUserContactResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBDiagReportTask(self, request):
         """创建健康报告，并可以选择是否发送邮件。
 
         :param request: Request instance for CreateDBDiagReportTask.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.CreateDBDiagReportTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CreateDBDiagReportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBDiagReportUrl(self, request):
         """创建健康报告的浏览地址。
 
         :param request: Request instance for CreateDBDiagReportUrl.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.CreateDBDiagReportUrlRequest`
@@ -88,15 +88,15 @@
             model = models.CreateDBDiagReportUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMailProfile(self, request):
         """创建邮件配置。其中入参ProfileType表示所创建配置的类型，ProfileType 取值包括：dbScan_mail_configuration（数据库巡检邮件配置）、scheduler_mail_configuration（定期生成健康报告的邮件发送配置）。Region统一选择广州，和实例所属地域无关。
 
         :param request: Request instance for CreateMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.CreateMailProfileRequest`
@@ -111,15 +111,15 @@
             model = models.CreateMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSchedulerMailProfile(self, request):
         """该接口用于创建定期生成健康报告并邮件发送的配置，将健康报告的定期生成时间作为参数传入（周一至周日），用于设置健康报告的定期生成时间，同时保存相应的定期邮件发送的配置。
 
         :param request: Request instance for CreateSchedulerMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.CreateSchedulerMailProfileRequest`
@@ -134,15 +134,15 @@
             model = models.CreateSchedulerMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityAuditLogExportTask(self, request):
         """创建安全审计日志导出任务。
 
         :param request: Request instance for CreateSecurityAuditLogExportTask.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.CreateSecurityAuditLogExportTaskRequest`
@@ -157,15 +157,15 @@
             model = models.CreateSecurityAuditLogExportTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityAuditLogExportTasks(self, request):
         """删除安全审计日志导出任务。
 
         :param request: Request instance for DeleteSecurityAuditLogExportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DeleteSecurityAuditLogExportTasksRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteSecurityAuditLogExportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllUserContact(self, request):
         """获取邮件发送中联系人的相关信息。
 
         :param request: Request instance for DescribeAllUserContact.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeAllUserContactRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeAllUserContactResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllUserGroup(self, request):
         """获取邮件发送联系组的相关信息。
 
         :param request: Request instance for DescribeAllUserGroup.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeAllUserGroupRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeAllUserGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagEvent(self, request):
         """获取实例异常诊断事件的详情信息。
 
         :param request: Request instance for DescribeDBDiagEvent.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeDBDiagEventRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeDBDiagEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagHistory(self, request):
         """获取实例诊断事件的列表。
 
         :param request: Request instance for DescribeDBDiagHistory.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeDBDiagHistoryRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeDBDiagHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBDiagReportTasks(self, request):
         """查询健康报告生成任务列表。
 
         :param request: Request instance for DescribeDBDiagReportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeDBDiagReportTasksRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeDBDiagReportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSpaceStatus(self, request):
         """获取指定时间段内的实例空间使用概览，包括磁盘增长量(MB)、磁盘剩余(MB)、磁盘总量(MB)及预计可用天数。
 
         :param request: Request instance for DescribeDBSpaceStatus.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeDBSpaceStatusRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeDBSpaceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiagDBInstances(self, request):
         """获取实例信息列表。Region统一选择广州。
 
         :param request: Request instance for DescribeDiagDBInstances.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeDiagDBInstancesRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeDiagDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHealthScore(self, request):
         """根据实例ID获取指定时间段（30分钟）的健康得分，以及异常扣分项。
 
         :param request: Request instance for DescribeHealthScore.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeHealthScoreRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeHealthScoreResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMailProfile(self, request):
         """获取发送邮件的配置， 包括数据库巡检的邮件配置以及定期生成健康报告的邮件发送配置。Region统一选择广州。
 
         :param request: Request instance for DescribeMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeMailProfileRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeMailProfileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityAuditLogDownloadUrls(self, request):
         """查询安全审计日志导出文件下载链接。目前日志文件下载仅提供腾讯云内网地址，请通过广州地域的腾讯云服务器进行下载。
 
         :param request: Request instance for DescribeSecurityAuditLogDownloadUrls.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeSecurityAuditLogDownloadUrlsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeSecurityAuditLogDownloadUrlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityAuditLogExportTasks(self, request):
         """查询安全审计日志导出任务列表。
 
         :param request: Request instance for DescribeSecurityAuditLogExportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeSecurityAuditLogExportTasksRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeSecurityAuditLogExportTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogTimeSeriesStats(self, request):
         """获取慢日志统计柱状图。
 
         :param request: Request instance for DescribeSlowLogTimeSeriesStats.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeSlowLogTimeSeriesStatsRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeSlowLogTimeSeriesStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogTopSqls(self, request):
         """按照Sql模板+schema的聚合方式，统计排序指定时间段内的top慢sql。
 
         :param request: Request instance for DescribeSlowLogTopSqls.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeSlowLogTopSqlsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeSlowLogTopSqlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogUserHostStats(self, request):
         """获取慢日志来源地址统计分布图。
 
         :param request: Request instance for DescribeSlowLogUserHostStats.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeSlowLogUserHostStatsRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeSlowLogUserHostStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceSchemaTimeSeries(self, request):
         """获取实例占用空间最大的前几个库在指定时间段内的每日由DBbrain定时采集的空间数据，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceSchemaTimeSeries.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeTopSpaceSchemaTimeSeriesRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeTopSpaceSchemaTimeSeriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceSchemas(self, request):
         """获取实例Top库的实时空间统计信息，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceSchemas.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeTopSpaceSchemasRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeTopSpaceSchemasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceTableTimeSeries(self, request):
         """获取实例占用空间最大的前几张表在指定时间段内的每日由DBbrain定时采集的空间数据，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceTableTimeSeries.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeTopSpaceTableTimeSeriesRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeTopSpaceTableTimeSeriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopSpaceTables(self, request):
         """获取实例Top表的实时空间统计信息，默认返回按大小排序。
 
         :param request: Request instance for DescribeTopSpaceTables.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeTopSpaceTablesRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeTopSpaceTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserSqlAdvice(self, request):
         """获取SQL优化建议。
 
         :param request: Request instance for DescribeUserSqlAdvice.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.DescribeUserSqlAdviceRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeUserSqlAdviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDiagDBInstanceConf(self, request):
         """修改实例巡检开关。
 
         :param request: Request instance for ModifyDiagDBInstanceConf.
         :type request: :class:`tencentcloud.dbbrain.v20191016.models.ModifyDiagDBInstanceConfRequest`
@@ -640,8 +640,8 @@
             model = models.ModifyDiagDBInstanceConfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.938/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.938/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.937/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.938/README.rst`

 * *Files identical despite different names*

