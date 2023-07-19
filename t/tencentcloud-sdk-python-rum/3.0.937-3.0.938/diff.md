# Comparing `tmp/tencentcloud-sdk-python-rum-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-rum-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.937.tar", last modified: Tue Jul 18 00:29:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.938.tar", last modified: Wed Jul 19 00:44:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rum-3.0.937.tar` & `tencentcloud-sdk-python-rum-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59777 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/rum_client.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   294640 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:27.000000 tencentcloud-sdk-python-rum-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60037 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/rum_client.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   294640 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:42.000000 tencentcloud-sdk-python-rum-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-rum-3.0.937/setup.py` & `tencentcloud-sdk-python-rum-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rum-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/rum_client.py` & `tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/rum_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             model = models.CreateLogExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOfflineLogConfig(self, request):
         """创建离线日志监听，对应用户的离线日志将上报
 
         :param request: Request instance for CreateOfflineLogConfig.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateOfflineLogConfigRequest`
@@ -69,15 +69,15 @@
             model = models.CreateOfflineLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """创建 RUM 应用（归属于某个团队）
 
         :param request: Request instance for CreateProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateProjectRequest`
@@ -92,15 +92,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReleaseFile(self, request):
         """创建对应项目的文件记录
 
         :param request: Request instance for CreateReleaseFile.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateReleaseFileRequest`
@@ -115,15 +115,15 @@
             model = models.CreateReleaseFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStarProject(self, request):
         """个人用户添加星标项目
 
         :param request: Request instance for CreateStarProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateStarProjectRequest`
@@ -138,15 +138,15 @@
             model = models.CreateStarProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTawInstance(self, request):
         """创建 RUM 业务系统
 
         :param request: Request instance for CreateTawInstance.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateTawInstanceRequest`
@@ -161,15 +161,15 @@
             model = models.CreateTawInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWhitelist(self, request):
         """创建白名单
 
         :param request: Request instance for CreateWhitelist.
         :type request: :class:`tencentcloud.rum.v20210622.models.CreateWhitelistRequest`
@@ -184,15 +184,15 @@
             model = models.CreateWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstance(self, request):
         """删除实例，谨慎操作，不可恢复
 
         :param request: Request instance for DeleteInstance.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteInstanceRequest`
@@ -207,15 +207,15 @@
             model = models.DeleteInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLogExport(self, request):
         """接口请求域名： rum.tencentcloudapi.com 。
 
         本接口用于删除日志下载任务
 
@@ -234,15 +234,15 @@
             model = models.DeleteLogExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOfflineLogConfig(self, request):
         """删除 rum 离线日志监听 - 对应用户的离线日志将不会上报
 
         :param request: Request instance for DeleteOfflineLogConfig.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteOfflineLogConfigRequest`
@@ -257,15 +257,15 @@
             model = models.DeleteOfflineLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOfflineLogRecord(self, request):
         """删除对应的离线日志记录
 
         :param request: Request instance for DeleteOfflineLogRecord.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteOfflineLogRecordRequest`
@@ -280,15 +280,15 @@
             model = models.DeleteOfflineLogRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProject(self, request):
         """删除给定的 rum 的项目
 
         :param request: Request instance for DeleteProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteProjectRequest`
@@ -303,15 +303,15 @@
             model = models.DeleteProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReleaseFile(self, request):
         """将对应 sourcemap 文件删除
 
         :param request: Request instance for DeleteReleaseFile.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteReleaseFileRequest`
@@ -326,15 +326,15 @@
             model = models.DeleteReleaseFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStarProject(self, request):
         """删除用户名下的星标项目
 
         :param request: Request instance for DeleteStarProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteStarProjectRequest`
@@ -349,15 +349,15 @@
             model = models.DeleteStarProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWhitelist(self, request):
         """删除白名单
 
         :param request: Request instance for DeleteWhitelist.
         :type request: :class:`tencentcloud.rum.v20210622.models.DeleteWhitelistRequest`
@@ -372,15 +372,15 @@
             model = models.DeleteWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppDimensionMetrics(self, request):
         """用于查询 app 监控多维分析数据
 
         :param request: Request instance for DescribeAppDimensionMetrics.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppDimensionMetricsRequest`
@@ -395,15 +395,15 @@
             model = models.DescribeAppDimensionMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppMetricsData(self, request):
         """获取 app 监控指标数据
 
         :param request: Request instance for DescribeAppMetricsData.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppMetricsDataRequest`
@@ -418,15 +418,15 @@
             model = models.DescribeAppMetricsDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppSingleCaseDetailList(self, request):
         """查询 app 监控个例样本详情列表
 
         :param request: Request instance for DescribeAppSingleCaseDetailList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseDetailListRequest`
@@ -441,15 +441,15 @@
             model = models.DescribeAppSingleCaseDetailListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAppSingleCaseList(self, request):
         """查询 app 监控个例聚合列表
 
         :param request: Request instance for DescribeAppSingleCaseList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseListRequest`
@@ -464,15 +464,15 @@
             model = models.DescribeAppSingleCaseListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeData(self, request):
         """转发monitor查询
 
         :param request: Request instance for DescribeData.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataRequest`
@@ -487,15 +487,15 @@
             model = models.DescribeDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataCustomUrl(self, request):
         """获取DescribeDataCustomUrl信息
 
         :param request: Request instance for DescribeDataCustomUrl.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataCustomUrlRequest`
@@ -510,15 +510,15 @@
             model = models.DescribeDataCustomUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataEventUrl(self, request):
         """获取DescribeDataEventUrl信息
 
         :param request: Request instance for DescribeDataEventUrl.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataEventUrlRequest`
@@ -533,15 +533,15 @@
             model = models.DescribeDataEventUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataFetchProject(self, request):
         """获取DescribeDataFetchProject信息。已下线，请使用DescribeDataFetchUrl
 
         :param request: Request instance for DescribeDataFetchProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataFetchProjectRequest`
@@ -556,15 +556,15 @@
             model = models.DescribeDataFetchProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataFetchUrl(self, request):
         """获取DescribeDataFetchUrl信息
 
         :param request: Request instance for DescribeDataFetchUrl.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataFetchUrlRequest`
@@ -579,15 +579,15 @@
             model = models.DescribeDataFetchUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataFetchUrlInfo(self, request):
         """获取DescribeDataFetchUrlInfo信息
 
         :param request: Request instance for DescribeDataFetchUrlInfo.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataFetchUrlInfoRequest`
@@ -602,15 +602,15 @@
             model = models.DescribeDataFetchUrlInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataLogUrlInfo(self, request):
         """获取loginfo信息
 
         :param request: Request instance for DescribeDataLogUrlInfo.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataLogUrlInfoRequest`
@@ -625,15 +625,15 @@
             model = models.DescribeDataLogUrlInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataLogUrlStatistics(self, request):
         """获取LogUrlStatistics信息
 
         :param request: Request instance for DescribeDataLogUrlStatistics.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataLogUrlStatisticsRequest`
@@ -648,15 +648,15 @@
             model = models.DescribeDataLogUrlStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataPerformancePage(self, request):
         """获取PerformancePage信息
 
         :param request: Request instance for DescribeDataPerformancePage.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataPerformancePageRequest`
@@ -671,15 +671,15 @@
             model = models.DescribeDataPerformancePageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataPerformanceProject(self, request):
         """获取PerformanceProject信息
 
         :param request: Request instance for DescribeDataPerformanceProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataPerformanceProjectRequest`
@@ -694,15 +694,15 @@
             model = models.DescribeDataPerformanceProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataPvUrlInfo(self, request):
         """获取PvUrlInfo信息
 
         :param request: Request instance for DescribeDataPvUrlInfo.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataPvUrlInfoRequest`
@@ -717,15 +717,15 @@
             model = models.DescribeDataPvUrlInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataPvUrlStatistics(self, request):
         """获取DescribeDataPvUrlStatistics信息
 
         :param request: Request instance for DescribeDataPvUrlStatistics.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataPvUrlStatisticsRequest`
@@ -740,15 +740,15 @@
             model = models.DescribeDataPvUrlStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataReportCount(self, request):
         """获取项目上报量
 
         :param request: Request instance for DescribeDataReportCount.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataReportCountRequest`
@@ -763,15 +763,15 @@
             model = models.DescribeDataReportCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataSetUrlStatistics(self, request):
         """获取DescribeDataSetUrlStatistics信息
 
         :param request: Request instance for DescribeDataSetUrlStatistics.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataSetUrlStatisticsRequest`
@@ -786,15 +786,15 @@
             model = models.DescribeDataSetUrlStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataStaticProject(self, request):
         """获取DescribeDataStaticProject信息
 
         :param request: Request instance for DescribeDataStaticProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataStaticProjectRequest`
@@ -809,15 +809,15 @@
             model = models.DescribeDataStaticProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataStaticResource(self, request):
         """获取DescribeDataStaticResource信息
 
         :param request: Request instance for DescribeDataStaticResource.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataStaticResourceRequest`
@@ -832,15 +832,15 @@
             model = models.DescribeDataStaticResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataStaticUrl(self, request):
         """获取DescribeDataStaticUrl信息
 
         :param request: Request instance for DescribeDataStaticUrl.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataStaticUrlRequest`
@@ -855,15 +855,15 @@
             model = models.DescribeDataStaticUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataWebVitalsPage(self, request):
         """获取DescribeDataWebVitalsPage信息，用户核心活动信息
         页面加载性能之Web Vitals。性能关键点
 
         :param request: Request instance for DescribeDataWebVitalsPage.
@@ -879,15 +879,15 @@
             model = models.DescribeDataWebVitalsPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeError(self, request):
         """获取首页错误信息
 
         :param request: Request instance for DescribeError.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeErrorRequest`
@@ -902,15 +902,15 @@
             model = models.DescribeErrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogExports(self, request):
         """接口请求域名： rum.tencentcloudapi.com 。
 
         本接口用于获取日志下载任务列表
 
@@ -929,15 +929,15 @@
             model = models.DescribeLogExportsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogList(self, request):
         """(已下线，请用DescribeRumLogList)
 
         :param request: Request instance for DescribeLogList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeLogListRequest`
@@ -952,15 +952,15 @@
             model = models.DescribeLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineLogConfigs(self, request):
         """获取设置的离线日志监听配置 - 返回设置的用户唯一标识
 
         :param request: Request instance for DescribeOfflineLogConfigs.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeOfflineLogConfigsRequest`
@@ -975,15 +975,15 @@
             model = models.DescribeOfflineLogConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineLogRecords(self, request):
         """获取所有离线日志记录(最多100条)
 
         :param request: Request instance for DescribeOfflineLogRecords.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeOfflineLogRecordsRequest`
@@ -998,15 +998,15 @@
             model = models.DescribeOfflineLogRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOfflineLogs(self, request):
         """获取对应离线日志
 
         :param request: Request instance for DescribeOfflineLogs.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeOfflineLogsRequest`
@@ -1021,15 +1021,15 @@
             model = models.DescribeOfflineLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectLimits(self, request):
         """获取应用上报抽样信息
 
         :param request: Request instance for DescribeProjectLimits.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeProjectLimitsRequest`
@@ -1044,15 +1044,15 @@
             model = models.DescribeProjectLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """获取项目列表（实例创建的团队下的项目列表）
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeProjectsRequest`
@@ -1067,15 +1067,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePvList(self, request):
         """获取项目下的PV列表
 
         :param request: Request instance for DescribePvList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribePvListRequest`
@@ -1090,15 +1090,15 @@
             model = models.DescribePvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReleaseFileSign(self, request):
         """获取上传文件存储的临时密钥
 
         :param request: Request instance for DescribeReleaseFileSign.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeReleaseFileSignRequest`
@@ -1113,15 +1113,15 @@
             model = models.DescribeReleaseFileSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReleaseFiles(self, request):
         """获取应用对应sourcemap文件列表
 
         :param request: Request instance for DescribeReleaseFiles.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeReleaseFilesRequest`
@@ -1136,15 +1136,15 @@
             model = models.DescribeReleaseFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRumGroupLog(self, request):
         """获取项目下的日志聚合信息
 
         :param request: Request instance for DescribeRumGroupLog.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeRumGroupLogRequest`
@@ -1159,15 +1159,15 @@
             model = models.DescribeRumGroupLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRumLogExport(self, request):
         """获取项目下的日志列表（实例创建的项目下的日志列表）
 
         :param request: Request instance for DescribeRumLogExport.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeRumLogExportRequest`
@@ -1182,15 +1182,15 @@
             model = models.DescribeRumLogExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRumLogExports(self, request):
         """获取项目下的日志导出列表
 
         :param request: Request instance for DescribeRumLogExports.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeRumLogExportsRequest`
@@ -1205,15 +1205,15 @@
             model = models.DescribeRumLogExportsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRumLogList(self, request):
         """获取项目下的日志列表（实例创建的项目下的日志列表）
 
         :param request: Request instance for DescribeRumLogList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeRumLogListRequest`
@@ -1228,15 +1228,15 @@
             model = models.DescribeRumLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRumStatsLogList(self, request):
         """获取项目下的日志列表，分钟级
 
         :param request: Request instance for DescribeRumStatsLogList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeRumStatsLogListRequest`
@@ -1251,15 +1251,15 @@
             model = models.DescribeRumStatsLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScores(self, request):
         """获取首页分数列表
 
         :param request: Request instance for DescribeScores.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeScoresRequest`
@@ -1274,15 +1274,15 @@
             model = models.DescribeScoresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTawAreas(self, request):
         """查询片区信息
 
         :param request: Request instance for DescribeTawAreas.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeTawAreasRequest`
@@ -1297,15 +1297,15 @@
             model = models.DescribeTawAreasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTawInstances(self, request):
         """查询实例信息
 
         :param request: Request instance for DescribeTawInstances.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeTawInstancesRequest`
@@ -1320,15 +1320,15 @@
             model = models.DescribeTawInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUvList(self, request):
         """获取项目下的UV列表
 
         :param request: Request instance for DescribeUvList.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeUvListRequest`
@@ -1343,15 +1343,15 @@
             model = models.DescribeUvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWhitelists(self, request):
         """获取白名单列表
 
         :param request: Request instance for DescribeWhitelists.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeWhitelistsRequest`
@@ -1366,15 +1366,15 @@
             model = models.DescribeWhitelistsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstance(self, request):
         """修改 RUM 业务系统
 
         :param request: Request instance for ModifyInstance.
         :type request: :class:`tencentcloud.rum.v20210622.models.ModifyInstanceRequest`
@@ -1389,15 +1389,15 @@
             model = models.ModifyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProject(self, request):
         """修改 RUM 应用信息
 
         :param request: Request instance for ModifyProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.ModifyProjectRequest`
@@ -1412,15 +1412,15 @@
             model = models.ModifyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProjectLimit(self, request):
         """新增修改限流
 
         :param request: Request instance for ModifyProjectLimit.
         :type request: :class:`tencentcloud.rum.v20210622.models.ModifyProjectLimitRequest`
@@ -1435,15 +1435,15 @@
             model = models.ModifyProjectLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeInstance(self, request):
         """恢复 RUM 业务系统，恢复后，用户可以正常使用和上报数据
 
         :param request: Request instance for ResumeInstance.
         :type request: :class:`tencentcloud.rum.v20210622.models.ResumeInstanceRequest`
@@ -1458,15 +1458,15 @@
             model = models.ResumeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeProject(self, request):
         """恢复应用使用与上报数据
 
         :param request: Request instance for ResumeProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.ResumeProjectRequest`
@@ -1481,15 +1481,15 @@
             model = models.ResumeProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopInstance(self, request):
         """停止实例
 
         :param request: Request instance for StopInstance.
         :type request: :class:`tencentcloud.rum.v20210622.models.StopInstanceRequest`
@@ -1504,15 +1504,15 @@
             model = models.StopInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopProject(self, request):
         """停止项目使用与上报数据
 
         :param request: Request instance for StopProject.
         :type request: :class:`tencentcloud.rum.v20210622.models.StopProjectRequest`
@@ -1527,8 +1527,8 @@
             model = models.StopProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/errorcodes.py` & `tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.937/tencentcloud/rum/v20210622/models.py` & `tencentcloud-sdk-python-rum-3.0.938/tencentcloud/rum/v20210622/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.937/tencentcloud_sdk_python_rum.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.938/tencentcloud_sdk_python_rum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.937/README.rst` & `tencentcloud-sdk-python-rum-3.0.938/README.rst`

 * *Files identical despite different names*

