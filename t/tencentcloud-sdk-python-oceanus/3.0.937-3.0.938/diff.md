# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.937.tar", last modified: Tue Jul 18 00:28:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.938.tar", last modified: Wed Jul 19 00:43:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.937.tar` & `tencentcloud-sdk-python-oceanus-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9664 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25309 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)   217602 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:28:18.000000 tencentcloud-sdk-python-oceanus-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9664 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25417 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)   217602 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:43:37.000000 tencentcloud-sdk-python-oceanus-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:43:36.000000 tencentcloud-sdk-python-oceanus-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CheckSavepointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyJobs(self, request):
         """单条和批量复制作业
 
         :param request: Request instance for CopyJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CopyJobsRequest`
@@ -65,15 +65,15 @@
             model = models.CopyJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFolder(self, request):
         """作业列表页面新建文件夹请求
 
         :param request: Request instance for CreateFolder.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CreateFolderRequest`
@@ -88,15 +88,15 @@
             model = models.CreateFolderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateJob(self, request):
         """新建作业接口，一个 AppId 最多允许创建1000个作业
 
         :param request: Request instance for CreateJob.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CreateJobRequest`
@@ -111,15 +111,15 @@
             model = models.CreateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateJobConfig(self, request):
         """创建作业配置，一个作业最多有100个配置版本
 
         :param request: Request instance for CreateJobConfig.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CreateJobConfigRequest`
@@ -134,15 +134,15 @@
             model = models.CreateJobConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResource(self, request):
         """创建资源接口
 
         :param request: Request instance for CreateResource.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CreateResourceRequest`
@@ -157,15 +157,15 @@
             model = models.CreateResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResourceConfig(self, request):
         """创建资源配置接口
 
         :param request: Request instance for CreateResourceConfig.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.CreateResourceConfigRequest`
@@ -180,15 +180,15 @@
             model = models.CreateResourceConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteJobs(self, request):
         """批量删除作业接口，批量操作数量上限20
 
         :param request: Request instance for DeleteJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DeleteJobsRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteResourceConfigs(self, request):
         """删除资源版本
 
         :param request: Request instance for DeleteResourceConfigs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DeleteResourceConfigsRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteResourceConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteResources(self, request):
         """删除资源接口
 
         :param request: Request instance for DeleteResources.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DeleteResourcesRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTableConfig(self, request):
         """删除作业表配置
 
         :param request: Request instance for DeleteTableConfig.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DeleteTableConfigRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteTableConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """查询集群
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeClustersRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobConfigs(self, request):
         """查询作业配置列表，一次最多查询100个
 
         :param request: Request instance for DescribeJobConfigs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobConfigsRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeJobConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobSavepoint(self, request):
         """查找Savepoint列表
 
         :param request: Request instance for DescribeJobSavepoint.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobSavepointRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeJobSavepointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobSubmissionLog(self, request):
         """查询作业实例启动日志
 
         :param request: Request instance for DescribeJobSubmissionLog.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobSubmissionLogRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeJobSubmissionLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobs(self, request):
         """查询作业
 
         :param request: Request instance for DescribeJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeJobsRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceConfigs(self, request):
         """描述资源配置接口
 
         :param request: Request instance for DescribeResourceConfigs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeResourceConfigsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeResourceConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceRelatedJobs(self, request):
         """获取资源关联作业信息
 
         :param request: Request instance for DescribeResourceRelatedJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeResourceRelatedJobsRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeResourceRelatedJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResources(self, request):
         """描述资源接口
 
         :param request: Request instance for DescribeResources.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeResourcesRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSystemResources(self, request):
         """描述系统资源接口
 
         :param request: Request instance for DescribeSystemResources.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeSystemResourcesRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeSystemResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTreeJobs(self, request):
         """生成树状作业显示结构
 
         :param request: Request instance for DescribeTreeJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeTreeJobsRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeTreeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTreeResources(self, request):
         """查询树状结构资源列表
 
         :param request: Request instance for DescribeTreeResources.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeTreeResourcesRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeTreeResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkSpaces(self, request):
         """授权工作空间列表
 
         :param request: Request instance for DescribeWorkSpaces.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeWorkSpacesRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeWorkSpacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyJob(self, request):
         """更新作业属性，仅允许以下3种操作，不支持组合操作：
         (1)	更新作业名称
         (2)	更新作业备注
         (3)	更新作业最大并行度
@@ -580,15 +580,15 @@
             model = models.ModifyJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunJobs(self, request):
         """批量启动或者恢复作业，批量操作数量上限20
 
         :param request: Request instance for RunJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.RunJobsRequest`
@@ -603,15 +603,15 @@
             model = models.RunJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopJobs(self, request):
         """批量停止作业，批量操作数量上限为20
 
         :param request: Request instance for StopJobs.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.StopJobsRequest`
@@ -626,15 +626,15 @@
             model = models.StopJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TriggerJobSavepoint(self, request):
         """触发Savepoint
 
         :param request: Request instance for TriggerJobSavepoint.
         :type request: :class:`tencentcloud.oceanus.v20190422.models.TriggerJobSavepointRequest`
@@ -649,8 +649,8 @@
             model = models.TriggerJobSavepointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud/oceanus/v20190422/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.938/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.937/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.938/README.rst`

 * *Files identical despite different names*

