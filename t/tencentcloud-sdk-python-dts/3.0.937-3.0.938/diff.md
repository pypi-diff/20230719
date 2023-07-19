# Comparing `tmp/tencentcloud-sdk-python-dts-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dts-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.937.tar", last modified: Tue Jul 18 00:23:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.938.tar", last modified: Wed Jul 19 00:38:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dts-3.0.937.tar` & `tencentcloud-sdk-python-dts-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/
--rw-r--r--   0 root         (0) root         (0)    47170 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/dts_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   327362 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/
--rw-r--r--   0 root         (0) root         (0)    24761 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/dts_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   124284 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:04.000000 tencentcloud-sdk-python-dts-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/
+-rw-r--r--   0 root         (0) root         (0)    47354 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   327362 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/
+-rw-r--r--   0 root         (0) root         (0)    24853 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   124284 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:16.000000 tencentcloud-sdk-python-dts-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dts-3.0.937/setup.py` & `tencentcloud-sdk-python-dts-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/dts_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.CompleteMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfigureSyncJob(self, request):
         """配置一个同步任务
 
         :param request: Request instance for ConfigureSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ConfigureSyncJobRequest`
@@ -67,15 +67,15 @@
             model = models.ConfigureSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ContinueMigrateJob(self, request):
         """恢复一个暂停中的迁移任务。
 
         :param request: Request instance for ContinueMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ContinueMigrateJobRequest`
@@ -90,15 +90,15 @@
             model = models.ContinueMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ContinueSyncJob(self, request):
         """恢复处于已暂停状态的数据同步任务。
 
         :param request: Request instance for ContinueSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ContinueSyncJobRequest`
@@ -113,15 +113,15 @@
             model = models.ContinueSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCheckSyncJob(self, request):
         """校验同步任务，检查必要参数和周边配置。
 
         :param request: Request instance for CreateCheckSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateCheckSyncJobRequest`
@@ -136,15 +136,15 @@
             model = models.CreateCheckSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCompareTask(self, request):
         """本接口用于创建数据对比任务，创建成功后会返回数据对比任务 ID，形如：dts-8yv4w2i1-cmp-37skmii9，创建成功后可通过StartCompare启动一致性校验任务
 
         :param request: Request instance for CreateCompareTask.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateCompareTaskRequest`
@@ -159,15 +159,15 @@
             model = models.CreateCompareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigrateCheckJob(self, request):
         """校验迁移任务，
         在开始迁移前, 必须调用本接口创建校验迁移任务, 且校验成功后才能开始迁移. 校验的结果可以通过DescribeMigrationCheckJob查看，
         校验成功后,迁移任务若有修改, 则必须重新校验并通过后, 才能开始迁移
 
@@ -184,15 +184,15 @@
             model = models.CreateMigrateCheckJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigrationService(self, request):
         """购买迁移任务。购买成功后会返回随机生成的迁移任务id列表，也可以通过查询迁移任务任务列表接口`DescribeMigrationJobs`看到购买成功的实例Id。注意，一旦购买成功后源及目标数据库类型，源及目标实例地域不可修改。
 
         :param request: Request instance for CreateMigrationService.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateMigrationServiceRequest`
@@ -207,15 +207,15 @@
             model = models.CreateMigrationServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateModifyCheckSyncJob(self, request):
         """在修改同步任务的配置后、通过该接口校验当前任务是否支持修改对象操作
 
         :param request: Request instance for CreateModifyCheckSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateModifyCheckSyncJobRequest`
@@ -230,15 +230,15 @@
             model = models.CreateModifyCheckSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSyncJob(self, request):
         """创建一个同步任务
 
         :param request: Request instance for CreateSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateSyncJobRequest`
@@ -253,15 +253,15 @@
             model = models.CreateSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCompareTask(self, request):
         """删除一致性校验任务。当一致性校验任务状态为success、failed、canceled 时可以执行此操作。
 
         :param request: Request instance for DeleteCompareTask.
         :type request: :class:`tencentcloud.dts.v20211206.models.DeleteCompareTaskRequest`
@@ -276,15 +276,15 @@
             model = models.DeleteCompareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCheckSyncJobResult(self, request):
         """查询同步校验任务结果，检查必要参数和周边配置
 
         :param request: Request instance for DescribeCheckSyncJobResult.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeCheckSyncJobResultRequest`
@@ -299,15 +299,15 @@
             model = models.DescribeCheckSyncJobResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompareReport(self, request):
         """查询一致性校验任务详情
 
         :param request: Request instance for DescribeCompareReport.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeCompareReportRequest`
@@ -322,15 +322,15 @@
             model = models.DescribeCompareReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompareTasks(self, request):
         """查询一致性校验任务列表，调用该接口后可通过接口`DescribeCompareTasks` 查询一致性校验任务列表来获得启动后的状态。
 
         :param request: Request instance for DescribeCompareTasks.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeCompareTasksRequest`
@@ -345,15 +345,15 @@
             model = models.DescribeCompareTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrateDBInstances(self, request):
         """本接口用于查询支持迁移的云数据库实例
 
         :param request: Request instance for DescribeMigrateDBInstances.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeMigrateDBInstancesRequest`
@@ -368,15 +368,15 @@
             model = models.DescribeMigrateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationCheckJob(self, request):
         """本接口用于创建校验后,获取校验的结果. 能查询到当前校验的状态和进度.
         若通过校验, 则可调用'StartMigrateJob' 开始迁移.
         若未通过校验, 则能查询到校验失败的原因. 请按照报错, 通过'ModifyMigrationJob'修改迁移配置或是调整源/目标实例的相关参数.
 
@@ -393,15 +393,15 @@
             model = models.DescribeMigrationCheckJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationDetail(self, request):
         """查询某个迁移任务详情
 
         :param request: Request instance for DescribeMigrationDetail.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeMigrationDetailRequest`
@@ -416,15 +416,15 @@
             model = models.DescribeMigrationDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationJobs(self, request):
         """查询数据迁移任务列表
 
         :param request: Request instance for DescribeMigrationJobs.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeMigrationJobsRequest`
@@ -439,15 +439,15 @@
             model = models.DescribeMigrationJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModifyCheckSyncJobResult(self, request):
         """在创建修改对象的校验任务后、通过该接口查看校验任务的结果
 
         :param request: Request instance for DescribeModifyCheckSyncJobResult.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeModifyCheckSyncJobResultRequest`
@@ -462,15 +462,15 @@
             model = models.DescribeModifyCheckSyncJobResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSyncJobs(self, request):
         """查询同步任务信息
 
         :param request: Request instance for DescribeSyncJobs.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeSyncJobsRequest`
@@ -485,15 +485,15 @@
             model = models.DescribeSyncJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyMigrateJob(self, request):
         """下线数据迁移任务。计费任务必须先调用隔离(IsolateMigrateJob)接口，且只有是**已隔离**状态下，才能调用此接口销毁任务。对于不计费任务，调用隔离(IsolateMigrateJob)接口删除任务操作。
 
         :param request: Request instance for DestroyMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.DestroyMigrateJobRequest`
@@ -508,15 +508,15 @@
             model = models.DestroyMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroySyncJob(self, request):
         """下线同步任务，任务在已隔离状态下可以通过此操作进行任务下线，即彻底删除任务。下线操作后可通过查询同步任务信息接口DescribeSyncJobs获取任务列表查看状态，此操作成功后无法看到此任务表示下线成功。
 
         :param request: Request instance for DestroySyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.DestroySyncJobRequest`
@@ -531,15 +531,15 @@
             model = models.DestroySyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateMigrateJob(self, request):
         """隔离退还数据迁移服务。调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。对于计费任务，在任务隔离后可进行解除隔离(RecoverMigrationJob)操作或直接进行下线销毁(DestroyMigrateJob)操作。对于不计费任务，调用此接口会直接销毁任务，无法进行恢复操作。
 
         :param request: Request instance for IsolateMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.IsolateMigrateJobRequest`
@@ -554,15 +554,15 @@
             model = models.IsolateMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateSyncJob(self, request):
         """隔离同步任务，隔离后可通过查询同步任务信息接口DescribeSyncJobs获取隔离后状态。在任务隔离后可进行解除隔离(RecoverSyncJob)操作或直接进行下线操作。对于不计费任务，调用此接口后会直接删除任务，无法进行恢复操作。
 
         :param request: Request instance for IsolateSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.IsolateSyncJobRequest`
@@ -577,15 +577,15 @@
             model = models.IsolateSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCompareTask(self, request):
         """修改一致性校验任务，在任务创建后启动之前，可修改一致性校验参数
 
         :param request: Request instance for ModifyCompareTask.
         :type request: :class:`tencentcloud.dts.v20211206.models.ModifyCompareTaskRequest`
@@ -600,15 +600,15 @@
             model = models.ModifyCompareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCompareTaskName(self, request):
         """修改一致性校验任务名称
 
         :param request: Request instance for ModifyCompareTaskName.
         :type request: :class:`tencentcloud.dts.v20211206.models.ModifyCompareTaskNameRequest`
@@ -623,15 +623,15 @@
             model = models.ModifyCompareTaskNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrateJobSpec(self, request):
         """调整实例规格，此接口只支持按量计费任务的调整。调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。
 
         :param request: Request instance for ModifyMigrateJobSpec.
         :type request: :class:`tencentcloud.dts.v20211206.models.ModifyMigrateJobSpecRequest`
@@ -646,15 +646,15 @@
             model = models.ModifyMigrateJobSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrateName(self, request):
         """修改迁移任务名
 
         :param request: Request instance for ModifyMigrateName.
         :type request: :class:`tencentcloud.dts.v20211206.models.ModifyMigrateNameRequest`
@@ -669,15 +669,15 @@
             model = models.ModifyMigrateNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrationJob(self, request):
         """配置迁移服务，配置成功后可通过`CreateMigrationCheckJob` 创建迁移校验任务接口发起校验任务，只有校验通过才能启动迁移任务。
 
         :param request: Request instance for ModifyMigrationJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ModifyMigrationJobRequest`
@@ -692,15 +692,15 @@
             model = models.ModifyMigrationJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySyncJobConfig(self, request):
         """该接口支持在同步任务启动后修改任务的配置
         修改同步配置的完整流程：修改同步任务配置->创建修改同步任务配置的校验任务->查询修改配置的校验任务的结果->启动修改配置任务
 
         :param request: Request instance for ModifySyncJobConfig.
@@ -716,15 +716,15 @@
             model = models.ModifySyncJobConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PauseMigrateJob(self, request):
         """暂停一个迁移任务。
 
         :param request: Request instance for PauseMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.PauseMigrateJobRequest`
@@ -739,15 +739,15 @@
             model = models.PauseMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PauseSyncJob(self, request):
         """暂停处于同步中的数据同步任务。
 
         :param request: Request instance for PauseSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.PauseSyncJobRequest`
@@ -762,15 +762,15 @@
             model = models.PauseSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverMigrateJob(self, request):
         """解除隔离数据迁移任务，用户手动发起隔离后的手动解隔离，只有任务状态为已隔离(手动操作)状态下才能触发此操作。调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。
 
         :param request: Request instance for RecoverMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.RecoverMigrateJobRequest`
@@ -785,15 +785,15 @@
             model = models.RecoverMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverSyncJob(self, request):
         """解除隔离同步任务，任务在已隔离状态下可调用该接口解除隔离状态任务，同时可通过查询同步任务信息接口DescribeSyncJobs，获取操作后状态。
 
         :param request: Request instance for RecoverSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.RecoverSyncJobRequest`
@@ -808,15 +808,15 @@
             model = models.RecoverSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResizeSyncJob(self, request):
         """调整同步任务规格，此接口只支持按量计费任务的调整，调用此接口后不会立即生效，后台调整时间大概为3~5分钟。调用此接口后可通过查询同步任务信息接口DescribeSyncJobs，获取变配后的状态。
 
         :param request: Request instance for ResizeSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ResizeSyncJobRequest`
@@ -831,15 +831,15 @@
             model = models.ResizeSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeMigrateJob(self, request):
         """重试数据迁移任务，针对异常情况可进行重试，对于redis在失败时也可重试。注意：此操作跳过校验阶段，直接重新发起任务，相当于从StartMigrationJob开始执行。调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。
 
         :param request: Request instance for ResumeMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ResumeMigrateJobRequest`
@@ -854,15 +854,15 @@
             model = models.ResumeMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeSyncJob(self, request):
         """重试同步任务，部分可恢复报错情况下，可通过该接口重试同步任务，可通过查询同步任务信息接口DescribeSyncJobs，获取操作后状态。
 
         :param request: Request instance for ResumeSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.ResumeSyncJobRequest`
@@ -877,15 +877,15 @@
             model = models.ResumeSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SkipCheckItem(self, request):
         """本接口用于校验检查项不通过后，可进行跳过此校验项操作，后端将不再校验该项。任何校验步骤都是不应该跳过的，通过校验是能正确执行的前置条件。支持跳过的产品及链路的校验项可 [参考文档](https://cloud.tencent.com/document/product/571/61639)。
 
         :param request: Request instance for SkipCheckItem.
         :type request: :class:`tencentcloud.dts.v20211206.models.SkipCheckItemRequest`
@@ -900,15 +900,15 @@
             model = models.SkipCheckItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SkipSyncCheckItem(self, request):
         """本接口用于校验检查项不通过后，可进行跳过此校验项操作，后端将不再校验该项。任何校验步骤都是不应该跳过的，通过校验是能正确执行的前置条件。支持跳过的产品及链路的校验项可 [参考文档](https://cloud.tencent.com/document/product/571/61639)。
 
         :param request: Request instance for SkipSyncCheckItem.
         :type request: :class:`tencentcloud.dts.v20211206.models.SkipSyncCheckItemRequest`
@@ -923,15 +923,15 @@
             model = models.SkipSyncCheckItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartCompare(self, request):
         """启动一致性校验任务，启动之前需要先通过接口`CreateCompareTask` 创建一致性校验任务，启动后可通过接口`DescribeCompareTasks` 查询一致性校验任务列表来获得启动后的状态
 
         :param request: Request instance for StartCompare.
         :type request: :class:`tencentcloud.dts.v20211206.models.StartCompareRequest`
@@ -946,15 +946,15 @@
             model = models.StartCompareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMigrateJob(self, request):
         """本接口（StartMigrationJob）用于启动迁移任务。调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。
 
         :param request: Request instance for StartMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.StartMigrateJobRequest`
@@ -969,15 +969,15 @@
             model = models.StartMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartModifySyncJob(self, request):
         """在查询修改对象的校验任务的结果中的status为success后、通过该接口开始修改配置流程
 
         :param request: Request instance for StartModifySyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.StartModifySyncJobRequest`
@@ -992,15 +992,15 @@
             model = models.StartModifySyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartSyncJob(self, request):
         """启动同步任务
 
         :param request: Request instance for StartSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.StartSyncJobRequest`
@@ -1015,15 +1015,15 @@
             model = models.StartSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopCompare(self, request):
         """终止一致性校验任务
 
         :param request: Request instance for StopCompare.
         :type request: :class:`tencentcloud.dts.v20211206.models.StopCompareRequest`
@@ -1038,15 +1038,15 @@
             model = models.StopCompareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMigrateJob(self, request):
         """本接口（StopMigrateJob）用于终止数据迁移任务。
         调用此接口后可通过查询迁移服务列表接口`DescribeMigrationJobs`来查询当前任务状态。
 
         :param request: Request instance for StopMigrateJob.
@@ -1062,15 +1062,15 @@
             model = models.StopMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopSyncJob(self, request):
         """结束同步任务，操作后可通过查询同步任务信息接口DescribeSyncJobs，获取操作后的状态。
 
         :param request: Request instance for StopSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.StopSyncJobRequest`
@@ -1085,8 +1085,8 @@
             model = models.StopSyncJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20211206/models.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20211206/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/dts_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ActivateSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompleteMigrateJob(self, request):
         """本接口（CompleteMigrateJob）用于完成数据迁移任务。
         选择采用增量迁移方式的任务, 需要在迁移进度进入准备完成阶段后, 调用本接口, 停止迁移增量数据。
         通过DescribeMigrateJobs接口查询到任务的状态为准备完成（status=8）时，此时可以调用本接口完成迁移任务。
 
@@ -67,15 +67,15 @@
             model = models.CompleteMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigrateCheckJob(self, request):
         """创建校验迁移任务
         在开始迁移前, 必须调用本接口创建校验, 且校验成功后才能开始迁移. 校验的结果可以通过DescribeMigrateCheckJob查看.
         校验成功后,迁移任务若有修改, 则必须重新创建校验并通过后, 才能开始迁移.
 
@@ -94,15 +94,15 @@
             model = models.CreateMigrateCheckJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigrateJob(self, request):
         """本接口（CreateMigrateJob）用于创建数据迁移任务。
 
         如果是金融区链路, 请使用域名: dts.ap-shenzhen-fsi.tencentcloudapi.com
 
@@ -119,15 +119,15 @@
             model = models.CreateMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubscribe(self, request):
         """本接口(CreateSubscribe)用于创建一个数据订阅实例。
 
         :param request: Request instance for CreateSubscribe.
         :type request: :class:`tencentcloud.dts.v20180330.models.CreateSubscribeRequest`
@@ -142,15 +142,15 @@
             model = models.CreateSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMigrateJob(self, request):
         """本接口（DeleteMigrationJob）用于删除数据迁移任务。当通过DescribeMigrateJobs接口查询到任务的状态为：检验中（status=3）、运行中（status=7）、准备完成（status=8）、撤销中（status=11）或者完成中（status=12）时，不允许删除任务。
 
         :param request: Request instance for DeleteMigrateJob.
         :type request: :class:`tencentcloud.dts.v20180330.models.DeleteMigrateJobRequest`
@@ -165,15 +165,15 @@
             model = models.DeleteMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAsyncRequestInfo(self, request):
         """本接口（DescribeAsyncRequestInfo）用于查询任务执行结果
 
         :param request: Request instance for DescribeAsyncRequestInfo.
         :type request: :class:`tencentcloud.dts.v20180330.models.DescribeAsyncRequestInfoRequest`
@@ -188,15 +188,15 @@
             model = models.DescribeAsyncRequestInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrateCheckJob(self, request):
         """本接口用于创建校验后,获取校验的结果. 能查询到当前校验的状态和进度.
         若通过校验, 则可调用'StartMigrateJob' 开始迁移.
         若未通过校验, 则能查询到校验失败的原因. 请按照报错, 通过'ModifyMigrateJob'修改迁移配置或是调整源/目标实例的相关参数.
 
@@ -213,15 +213,15 @@
             model = models.DescribeMigrateCheckJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrateJobs(self, request):
         """查询数据迁移任务.
         如果是金融区链路, 请使用域名: https://dts.ap-shenzhen-fsi.tencentcloudapi.com
 
         :param request: Request instance for DescribeMigrateJobs.
@@ -237,15 +237,15 @@
             model = models.DescribeMigrateJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegionConf(self, request):
         """本接口（DescribeRegionConf）用于查询可售卖订阅实例的地域
 
         :param request: Request instance for DescribeRegionConf.
         :type request: :class:`tencentcloud.dts.v20180330.models.DescribeRegionConfRequest`
@@ -260,15 +260,15 @@
             model = models.DescribeRegionConfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubscribeConf(self, request):
         """本接口（DescribeSubscribeConf）用于查询订阅实例配置
 
         :param request: Request instance for DescribeSubscribeConf.
         :type request: :class:`tencentcloud.dts.v20180330.models.DescribeSubscribeConfRequest`
@@ -283,15 +283,15 @@
             model = models.DescribeSubscribeConfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubscribes(self, request):
         """本接口(DescribeSubscribes)获取数据订阅实例信息列表，默认分页，每次返回20条
 
         :param request: Request instance for DescribeSubscribes.
         :type request: :class:`tencentcloud.dts.v20180330.models.DescribeSubscribesRequest`
@@ -306,15 +306,15 @@
             model = models.DescribeSubscribesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateSubscribe(self, request):
         """本接口（IsolateSubscribe）用于隔离小时计费的订阅实例。调用后，订阅实例将不能使用，同时停止计费。
 
         :param request: Request instance for IsolateSubscribe.
         :type request: :class:`tencentcloud.dts.v20180330.models.IsolateSubscribeRequest`
@@ -329,15 +329,15 @@
             model = models.IsolateSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigrateJob(self, request):
         """本接口（ModifyMigrateJob）用于修改数据迁移任务。
         当迁移任务处于下述状态时，允许调用本接口修改迁移任务：迁移创建中（status=1）、 校验成功(status=4)、校验失败(status=5)、迁移失败(status=10)。但源实例、目标实例类型和目标实例地域不允许修改。
 
         如果是金融区链路, 请使用域名: dts.ap-shenzhen-fsi.tencentcloudapi.com
@@ -355,15 +355,15 @@
             model = models.ModifyMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscribeAutoRenewFlag(self, request):
         """修改订阅实例自动续费标识
 
         :param request: Request instance for ModifySubscribeAutoRenewFlag.
         :type request: :class:`tencentcloud.dts.v20180330.models.ModifySubscribeAutoRenewFlagRequest`
@@ -378,15 +378,15 @@
             model = models.ModifySubscribeAutoRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscribeConsumeTime(self, request):
         """本接口(ModifySubscribeConsumeTime)用于修改数据订阅通道的消费时间点
 
         :param request: Request instance for ModifySubscribeConsumeTime.
         :type request: :class:`tencentcloud.dts.v20180330.models.ModifySubscribeConsumeTimeRequest`
@@ -401,15 +401,15 @@
             model = models.ModifySubscribeConsumeTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscribeName(self, request):
         """本接口(ModifySubscribeName)用于修改数据订阅实例的名称
 
         :param request: Request instance for ModifySubscribeName.
         :type request: :class:`tencentcloud.dts.v20180330.models.ModifySubscribeNameRequest`
@@ -424,15 +424,15 @@
             model = models.ModifySubscribeNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscribeObjects(self, request):
         """本接口(ModifySubscribeObjects)用于修改数据订阅通道的订阅规则
 
         :param request: Request instance for ModifySubscribeObjects.
         :type request: :class:`tencentcloud.dts.v20180330.models.ModifySubscribeObjectsRequest`
@@ -447,15 +447,15 @@
             model = models.ModifySubscribeObjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubscribeVipVport(self, request):
         """本接口(ModifySubscribeVipVport)用于修改数据订阅实例的IP和端口号
 
         :param request: Request instance for ModifySubscribeVipVport.
         :type request: :class:`tencentcloud.dts.v20180330.models.ModifySubscribeVipVportRequest`
@@ -470,15 +470,15 @@
             model = models.ModifySubscribeVipVportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OfflineIsolatedSubscribe(self, request):
         """本接口（OfflineIsolatedSubscribe）用于下线已隔离的数据订阅实例
 
         :param request: Request instance for OfflineIsolatedSubscribe.
         :type request: :class:`tencentcloud.dts.v20180330.models.OfflineIsolatedSubscribeRequest`
@@ -493,15 +493,15 @@
             model = models.OfflineIsolatedSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetSubscribe(self, request):
         """本接口(ResetSubscribe)用于重置数据订阅实例，已经激活的数据订阅实例，重置后可以使用ActivateSubscribe接口绑定其他的数据库实例
 
         :param request: Request instance for ResetSubscribe.
         :type request: :class:`tencentcloud.dts.v20180330.models.ResetSubscribeRequest`
@@ -516,15 +516,15 @@
             model = models.ResetSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMigrateJob(self, request):
         """本接口（StartMigrationJob）用于启动迁移任务。非定时迁移任务会在调用后立即开始迁移，定时任务则会开始倒计时。
         调用此接口前，请务必先使用CreateMigrateCheckJob校验数据迁移任务，并通过DescribeMigrateJobs接口查询到任务状态为校验通过（status=4）时，才能启动数据迁移任务。
 
         :param request: Request instance for StartMigrateJob.
@@ -540,15 +540,15 @@
             model = models.StartMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMigrateJob(self, request):
         """本接口（StopMigrateJob）用于撤销数据迁移任务。
         在迁移过程中允许调用该接口撤销迁移, 撤销迁移的任务会失败。通过DescribeMigrateJobs接口查询到任务状态为运行中（status=7）或准备完成（status=8）时，才能撤销数据迁移任务。
 
         :param request: Request instance for StopMigrateJob.
@@ -564,8 +564,8 @@
             model = models.StopMigrateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud/dts/v20180330/models.py` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud/dts/v20180330/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.937/tencentcloud_sdk_python_dts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.938/tencentcloud_sdk_python_dts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.937/README.rst` & `tencentcloud-sdk-python-dts-3.0.938/README.rst`

 * *Files identical despite different names*

