# Comparing `tmp/tencentcloud-sdk-python-pts-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-pts-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.937.tar", last modified: Tue Jul 18 00:28:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.938.tar", last modified: Wed Jul 19 00:44:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-pts-3.0.937.tar` & `tencentcloud-sdk-python-pts-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39209 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/pts_client.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   309894 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:57.000000 tencentcloud-sdk-python-pts-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:56.000000 tencentcloud-sdk-python-pts-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39385 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/pts_client.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   309894 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:16.000000 tencentcloud-sdk-python-pts-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-pts-3.0.937/setup.py` & `tencentcloud-sdk-python-pts-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-pts-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/pts_client.py` & `tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/pts_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AbortCronJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AbortJob(self, request):
         """停止任务
 
         :param request: Request instance for AbortJob.
         :type request: :class:`tencentcloud.pts.v20210728.models.AbortJobRequest`
@@ -65,15 +65,15 @@
             model = models.AbortJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AdjustJobSpeed(self, request):
         """调整任务的目标RPS
 
         :param request: Request instance for AdjustJobSpeed.
         :type request: :class:`tencentcloud.pts.v20210728.models.AdjustJobSpeedRequest`
@@ -88,15 +88,15 @@
             model = models.AdjustJobSpeedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyScenario(self, request):
         """复制场景
 
         :param request: Request instance for CopyScenario.
         :type request: :class:`tencentcloud.pts.v20210728.models.CopyScenarioRequest`
@@ -111,15 +111,15 @@
             model = models.CopyScenarioResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlertChannel(self, request):
         """创建告警通知接收组
 
         :param request: Request instance for CreateAlertChannel.
         :type request: :class:`tencentcloud.pts.v20210728.models.CreateAlertChannelRequest`
@@ -134,15 +134,15 @@
             model = models.CreateAlertChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCronJob(self, request):
         """创建定时任务
 
         :param request: Request instance for CreateCronJob.
         :type request: :class:`tencentcloud.pts.v20210728.models.CreateCronJobRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCronJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFile(self, request):
         """创建文件
 
         :param request: Request instance for CreateFile.
         :type request: :class:`tencentcloud.pts.v20210728.models.CreateFileRequest`
@@ -180,15 +180,15 @@
             model = models.CreateFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """创建项目
 
         :param request: Request instance for CreateProject.
         :type request: :class:`tencentcloud.pts.v20210728.models.CreateProjectRequest`
@@ -203,15 +203,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScenario(self, request):
         """创建场景
 
         :param request: Request instance for CreateScenario.
         :type request: :class:`tencentcloud.pts.v20210728.models.CreateScenarioRequest`
@@ -226,15 +226,15 @@
             model = models.CreateScenarioResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlertChannel(self, request):
         """删除告警通知接收组
 
         :param request: Request instance for DeleteAlertChannel.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteAlertChannelRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteAlertChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCronJobs(self, request):
         """删除定时任务
 
         :param request: Request instance for DeleteCronJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteCronJobsRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteCronJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFiles(self, request):
         """删除文件
 
         :param request: Request instance for DeleteFiles.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteFilesRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteJobs(self, request):
         """删除任务
 
         :param request: Request instance for DeleteJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteJobsRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProjects(self, request):
         """删除项目
 
         :param request: Request instance for DeleteProjects.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteProjectsRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScenarios(self, request):
         """删除场景
 
         :param request: Request instance for DeleteScenarios.
         :type request: :class:`tencentcloud.pts.v20210728.models.DeleteScenariosRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteScenariosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlertChannels(self, request):
         """查询告警通知接收组
 
         :param request: Request instance for DescribeAlertChannels.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeAlertChannelsRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeAlertChannelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlertRecords(self, request):
         """返回告警历史项的列表
 
         :param request: Request instance for DescribeAlertRecords.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeAlertRecordsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeAlertRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableMetrics(self, request):
         """查询系统支持的指标
 
         :param request: Request instance for DescribeAvailableMetrics.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeAvailableMetricsRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeAvailableMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCheckSummary(self, request):
         """查询检查点汇总信息
 
         :param request: Request instance for DescribeCheckSummary.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeCheckSummaryRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeCheckSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCronJobs(self, request):
         """列出定时任务，非必填数组为空就默认全选
 
         :param request: Request instance for DescribeCronJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeCronJobsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeCronJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeErrorSummary(self, request):
         """查询错误详情汇总信息
 
         :param request: Request instance for DescribeErrorSummary.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeErrorSummaryRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeErrorSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFiles(self, request):
         """查询文件列表
 
         :param request: Request instance for DescribeFiles.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeFilesRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobs(self, request):
         """查询任务列表
 
         :param request: Request instance for DescribeJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeJobsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLabelValues(self, request):
         """查询标签内容
 
         :param request: Request instance for DescribeLabelValues.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeLabelValuesRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeLabelValuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMetricLabelWithValues(self, request):
         """查询指标所有的label及values值
 
         :param request: Request instance for DescribeMetricLabelWithValues.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeMetricLabelWithValuesRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeMetricLabelWithValuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNormalLogs(self, request):
         """压测过程日志包括引擎输出日志及用户输出日志
 
         :param request: Request instance for DescribeNormalLogs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeNormalLogsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeNormalLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """查询项目列表
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeProjectsRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """查询地域列表
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeRegionsRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRequestSummary(self, request):
         """查询请求汇总信息
 
         :param request: Request instance for DescribeRequestSummary.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeRequestSummaryRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeRequestSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleBatchQuery(self, request):
         """批量查询指标，返回固定时间点指标内容
 
         :param request: Request instance for DescribeSampleBatchQuery.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeSampleBatchQueryRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeSampleBatchQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleLogs(self, request):
         """查询采样日志
 
         :param request: Request instance for DescribeSampleLogs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeSampleLogsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeSampleLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleMatrixBatchQuery(self, request):
         """批量查询指标矩阵
 
         :param request: Request instance for DescribeSampleMatrixBatchQuery.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeSampleMatrixBatchQueryRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeSampleMatrixBatchQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleMatrixQuery(self, request):
         """查询指标矩阵
 
         :param request: Request instance for DescribeSampleMatrixQuery.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeSampleMatrixQueryRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeSampleMatrixQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleQuery(self, request):
         """查询指标，返回固定时间点指标内容
 
         :param request: Request instance for DescribeSampleQuery.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeSampleQueryRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeSampleQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScenarioWithJobs(self, request):
         """查询场景配置并附带已经执行的任务内容
 
         :param request: Request instance for DescribeScenarioWithJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeScenarioWithJobsRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeScenarioWithJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScenarios(self, request):
         """查询场景列表
 
         :param request: Request instance for DescribeScenarios.
         :type request: :class:`tencentcloud.pts.v20210728.models.DescribeScenariosRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeScenariosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateTmpKey(self, request):
         """生成临时COS凭证
 
         :param request: Request instance for GenerateTmpKey.
         :type request: :class:`tencentcloud.pts.v20210728.models.GenerateTmpKeyRequest`
@@ -870,15 +870,15 @@
             model = models.GenerateTmpKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartCronJobs(self, request):
         """重启状态为已中止的定时任务
 
         :param request: Request instance for RestartCronJobs.
         :type request: :class:`tencentcloud.pts.v20210728.models.RestartCronJobsRequest`
@@ -893,15 +893,15 @@
             model = models.RestartCronJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartJob(self, request):
         """创建并启动任务
 
         :param request: Request instance for StartJob.
         :type request: :class:`tencentcloud.pts.v20210728.models.StartJobRequest`
@@ -916,15 +916,15 @@
             model = models.StartJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCronJob(self, request):
         """更新定时任务
 
         :param request: Request instance for UpdateCronJob.
         :type request: :class:`tencentcloud.pts.v20210728.models.UpdateCronJobRequest`
@@ -939,15 +939,15 @@
             model = models.UpdateCronJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFileScenarioRelation(self, request):
         """更新关联文件场景
 
         :param request: Request instance for UpdateFileScenarioRelation.
         :type request: :class:`tencentcloud.pts.v20210728.models.UpdateFileScenarioRelationRequest`
@@ -962,15 +962,15 @@
             model = models.UpdateFileScenarioRelationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateJob(self, request):
         """更新任务
 
         :param request: Request instance for UpdateJob.
         :type request: :class:`tencentcloud.pts.v20210728.models.UpdateJobRequest`
@@ -985,15 +985,15 @@
             model = models.UpdateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProject(self, request):
         """更新项目
 
         :param request: Request instance for UpdateProject.
         :type request: :class:`tencentcloud.pts.v20210728.models.UpdateProjectRequest`
@@ -1008,15 +1008,15 @@
             model = models.UpdateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScenario(self, request):
         """更新场景
 
         :param request: Request instance for UpdateScenario.
         :type request: :class:`tencentcloud.pts.v20210728.models.UpdateScenarioRequest`
@@ -1031,8 +1031,8 @@
             model = models.UpdateScenarioResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/errorcodes.py` & `tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.937/tencentcloud/pts/v20210728/models.py` & `tencentcloud-sdk-python-pts-3.0.938/tencentcloud/pts/v20210728/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.937/tencentcloud_sdk_python_pts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.938/tencentcloud_sdk_python_pts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.937/README.rst` & `tencentcloud-sdk-python-pts-3.0.938/README.rst`

 * *Files identical despite different names*

