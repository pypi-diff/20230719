# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.937.tar", last modified: Tue Jul 18 00:17:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.938.tar", last modified: Wed Jul 19 00:21:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.937.tar` & `tencentcloud-sdk-python-batch-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)    31537 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   299742 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    31661 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   299742 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:21:36.000000 tencentcloud-sdk-python-batch-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-batch-3.0.937/setup.py` & `tencentcloud-sdk-python-batch-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/batch_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             model = models.AttachInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateComputeEnv(self, request):
         """用于创建计算环境
 
         :param request: Request instance for CreateComputeEnv.
         :type request: :class:`tencentcloud.batch.v20170312.models.CreateComputeEnvRequest`
@@ -71,15 +71,15 @@
             model = models.CreateComputeEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCpmComputeEnv(self, request):
         """创建黑石计算环境
 
         :param request: Request instance for CreateCpmComputeEnv.
         :type request: :class:`tencentcloud.batch.v20170312.models.CreateCpmComputeEnvRequest`
@@ -94,15 +94,15 @@
             model = models.CreateCpmComputeEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTaskTemplate(self, request):
         """用于创建任务模板
 
         :param request: Request instance for CreateTaskTemplate.
         :type request: :class:`tencentcloud.batch.v20170312.models.CreateTaskTemplateRequest`
@@ -117,15 +117,15 @@
             model = models.CreateTaskTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteComputeEnv(self, request):
         """用于删除计算环境
 
         :param request: Request instance for DeleteComputeEnv.
         :type request: :class:`tencentcloud.batch.v20170312.models.DeleteComputeEnvRequest`
@@ -140,15 +140,15 @@
             model = models.DeleteComputeEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteJob(self, request):
         """用于删除作业记录。
         删除作业的效果相当于删除作业相关的所有信息。删除成功后，作业相关的所有信息都无法查询。
         待删除的作业必须处于完结状态，且其内部包含的所有任务实例也必须处于完结状态，否则会禁止操作。完结状态，是指处于 SUCCEED 或 FAILED 状态。
 
@@ -165,15 +165,15 @@
             model = models.DeleteJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTaskTemplates(self, request):
         """用于删除任务模板信息
 
         :param request: Request instance for DeleteTaskTemplates.
         :type request: :class:`tencentcloud.batch.v20170312.models.DeleteTaskTemplatesRequest`
@@ -188,15 +188,15 @@
             model = models.DeleteTaskTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableCvmInstanceTypes(self, request):
         """查看可用的CVM机型配置信息
 
         :param request: Request instance for DescribeAvailableCvmInstanceTypes.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeAvailableCvmInstanceTypesRequest`
@@ -211,15 +211,15 @@
             model = models.DescribeAvailableCvmInstanceTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComputeEnv(self, request):
         """用于查询计算环境的详细信息
 
         :param request: Request instance for DescribeComputeEnv.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeComputeEnvRequest`
@@ -234,15 +234,15 @@
             model = models.DescribeComputeEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComputeEnvActivities(self, request):
         """用于查询计算环境的活动信息
 
         :param request: Request instance for DescribeComputeEnvActivities.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeComputeEnvActivitiesRequest`
@@ -257,15 +257,15 @@
             model = models.DescribeComputeEnvActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComputeEnvCreateInfo(self, request):
         """查看计算环境的创建信息。
 
         :param request: Request instance for DescribeComputeEnvCreateInfo.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeComputeEnvCreateInfoRequest`
@@ -280,15 +280,15 @@
             model = models.DescribeComputeEnvCreateInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComputeEnvCreateInfos(self, request):
         """用于查看计算环境创建信息列表，包括名称、描述、类型、环境参数、通知及期望节点数等。
 
         :param request: Request instance for DescribeComputeEnvCreateInfos.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeComputeEnvCreateInfosRequest`
@@ -303,15 +303,15 @@
             model = models.DescribeComputeEnvCreateInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComputeEnvs(self, request):
         """用于查看计算环境列表
 
         :param request: Request instance for DescribeComputeEnvs.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeComputeEnvsRequest`
@@ -326,15 +326,15 @@
             model = models.DescribeComputeEnvsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCpmOsInfo(self, request):
         """创建黑石计算环境时，查询批量计算环境支持的黑石操作系统信息
 
         :param request: Request instance for DescribeCpmOsInfo.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeCpmOsInfoRequest`
@@ -349,15 +349,15 @@
             model = models.DescribeCpmOsInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCvmZoneInstanceConfigInfos(self, request):
         """获取批量计算可用区机型配置信息
 
         :param request: Request instance for DescribeCvmZoneInstanceConfigInfos.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeCvmZoneInstanceConfigInfosRequest`
@@ -372,15 +372,15 @@
             model = models.DescribeCvmZoneInstanceConfigInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceCategories(self, request):
         """目前对CVM现有实例族分类，每一类包含若干实例族。该接口用于查询实例分类信息。
 
         :param request: Request instance for DescribeInstanceCategories.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeInstanceCategoriesRequest`
@@ -395,15 +395,15 @@
             model = models.DescribeInstanceCategoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJob(self, request):
         """用于查看一个作业的详细信息，包括内部任务（Task）和依赖（Dependence）信息。
 
         :param request: Request instance for DescribeJob.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeJobRequest`
@@ -418,15 +418,15 @@
             model = models.DescribeJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobSubmitInfo(self, request):
         """用于查询指定作业的提交信息，其返回内容包括 JobId 和 SubmitJob 接口中作为输入参数的作业提交信息
 
         :param request: Request instance for DescribeJobSubmitInfo.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeJobSubmitInfoRequest`
@@ -441,15 +441,15 @@
             model = models.DescribeJobSubmitInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobs(self, request):
         """用于查询若干个作业的概览信息
 
         :param request: Request instance for DescribeJobs.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeJobsRequest`
@@ -464,15 +464,15 @@
             model = models.DescribeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTask(self, request):
         """用于查询指定任务的详细信息，包括任务内部的任务实例信息。
 
         :param request: Request instance for DescribeTask.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeTaskRequest`
@@ -487,15 +487,15 @@
             model = models.DescribeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskLogs(self, request):
         """用于获取任务多个实例标准输出和标准错误日志。
 
         :param request: Request instance for DescribeTaskLogs.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeTaskLogsRequest`
@@ -510,15 +510,15 @@
             model = models.DescribeTaskLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskTemplates(self, request):
         """用于查询任务模板信息
 
         :param request: Request instance for DescribeTaskTemplates.
         :type request: :class:`tencentcloud.batch.v20170312.models.DescribeTaskTemplatesRequest`
@@ -533,15 +533,15 @@
             model = models.DescribeTaskTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachInstances(self, request):
         """将添加到计算环境中的实例从计算环境中移出。若是由批量计算自动创建的计算节点实例则不允许移出。
 
         :param request: Request instance for DetachInstances.
         :type request: :class:`tencentcloud.batch.v20170312.models.DetachInstancesRequest`
@@ -556,15 +556,15 @@
             model = models.DetachInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyComputeEnv(self, request):
         """用于修改计算环境属性
 
         :param request: Request instance for ModifyComputeEnv.
         :type request: :class:`tencentcloud.batch.v20170312.models.ModifyComputeEnvRequest`
@@ -579,15 +579,15 @@
             model = models.ModifyComputeEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTaskTemplate(self, request):
         """用于修改任务模板
 
         :param request: Request instance for ModifyTaskTemplate.
         :type request: :class:`tencentcloud.batch.v20170312.models.ModifyTaskTemplateRequest`
@@ -602,15 +602,15 @@
             model = models.ModifyTaskTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryJobs(self, request):
         """用于重试作业中失败的任务实例。
         当且仅当作业处于“FAILED”状态，支持重试操作。重试操作成功后，作业会按照“DAG”中指定的任务依赖关系，依次重试各个任务中失败的任务实例。任务实例的历史信息将被重置，如同首次运行一样，参与后续的调度和执行。
 
         :param request: Request instance for RetryJobs.
@@ -626,15 +626,15 @@
             model = models.RetryJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitJob(self, request):
         """用于提交一个作业
 
         :param request: Request instance for SubmitJob.
         :type request: :class:`tencentcloud.batch.v20170312.models.SubmitJobRequest`
@@ -649,15 +649,15 @@
             model = models.SubmitJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateComputeNode(self, request):
         """用于销毁计算节点。
         对于状态为CREATED、CREATION_FAILED、RUNNING和ABNORMAL的节点，允许销毁处理。
 
         :param request: Request instance for TerminateComputeNode.
@@ -673,15 +673,15 @@
             model = models.TerminateComputeNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateComputeNodes(self, request):
         """用于批量销毁计算节点，不允许重复销毁同一个节点。
 
         :param request: Request instance for TerminateComputeNodes.
         :type request: :class:`tencentcloud.batch.v20170312.models.TerminateComputeNodesRequest`
@@ -696,15 +696,15 @@
             model = models.TerminateComputeNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateJob(self, request):
         """用于终止作业。
         当作业处于“SUBMITTED”状态时，禁止终止操作；当作业处于“SUCCEED”状态时，终止操作不会生效。
         终止作业是一个异步过程。整个终止过程的耗时和任务总数成正比。终止的效果相当于所含的所有任务实例进行TerminateTaskInstance操作。具体效果和用法可参考TerminateTaskInstance。
 
@@ -721,15 +721,15 @@
             model = models.TerminateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateTaskInstance(self, request):
         """用于终止任务实例。
         对于状态已经为“SUCCEED”和“FAILED”的任务实例，不做处理。
         对于状态为“SUBMITTED”、“PENDING”、“RUNNABLE”的任务实例，状态将置为“FAILED”状态。
         对于状态为“STARTING”、“RUNNING”、“FAILED_INTERRUPTED”的任务实例，分区两种情况：如果未显示指定计算环境，会先销毁CVM服务器，然后将状态置为“FAILED”，具有一定耗时；如果指定了计算环境EnvId，任务实例状态置为“FAILED”，并重启执行该任务的CVM服务器，具有一定的耗时。
@@ -748,8 +748,8 @@
             model = models.TerminateTaskInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.938/tencentcloud/batch/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.938/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.937/README.rst` & `tencentcloud-sdk-python-batch-3.0.938/README.rst`

 * *Files identical despite different names*

