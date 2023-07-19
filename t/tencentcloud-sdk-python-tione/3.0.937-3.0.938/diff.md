# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.937.tar", last modified: Tue Jul 18 00:33:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.938.tar", last modified: Wed Jul 19 00:50:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.937.tar` & `tencentcloud-sdk-python-tione-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12673 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   531149 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144266 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:33:15.000000 tencentcloud-sdk-python-tione-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51244 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12673 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   531149 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22102 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144266 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:50:55.000000 tencentcloud-sdk-python-tione-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tione-3.0.937/setup.py` & `tencentcloud-sdk-python-tione-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/tione_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateBatchModelAccTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBatchTask(self, request):
         """创建跑批任务
 
         :param request: Request instance for CreateBatchTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateBatchTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CreateBatchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDataset(self, request):
         """创建数据集
 
         :param request: Request instance for CreateDataset.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateDatasetRequest`
@@ -88,15 +88,15 @@
             model = models.CreateDatasetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateModelService(self, request):
         """用于创建、发布一个新的模型服务
 
         :param request: Request instance for CreateModelService.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateModelServiceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateModelServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOptimizedModel(self, request):
         """保存优化模型
 
         :param request: Request instance for CreateOptimizedModel.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateOptimizedModelRequest`
@@ -134,15 +134,15 @@
             model = models.CreateOptimizedModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrainingModel(self, request):
         """导入模型
 
         :param request: Request instance for CreateTrainingModel.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateTrainingModelRequest`
@@ -157,15 +157,15 @@
             model = models.CreateTrainingModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrainingTask(self, request):
         """创建模型训练任务
 
         :param request: Request instance for CreateTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateTrainingTaskRequest`
@@ -180,15 +180,15 @@
             model = models.CreateTrainingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBatchTask(self, request):
         """删除跑批任务
 
         :param request: Request instance for DeleteBatchTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteBatchTaskRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteBatchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDataset(self, request):
         """删除数据集
 
         :param request: Request instance for DeleteDataset.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteDatasetRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteDatasetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModelAccelerateTask(self, request):
         """删除模型加速任务
 
         :param request: Request instance for DeleteModelAccelerateTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteModelAccelerateTaskRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteModelAccelerateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModelService(self, request):
         """根据服务id删除模型服务
 
         :param request: Request instance for DeleteModelService.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteModelServiceRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteModelServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModelServiceGroup(self, request):
         """根据服务组id删除服务组下所有模型服务
 
         :param request: Request instance for DeleteModelServiceGroup.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteModelServiceGroupRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteModelServiceGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrainingModel(self, request):
         """删除模型
 
         :param request: Request instance for DeleteTrainingModel.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteTrainingModelRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteTrainingModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrainingModelVersion(self, request):
         """删除模型版本
 
         :param request: Request instance for DeleteTrainingModelVersion.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteTrainingModelVersionRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteTrainingModelVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrainingTask(self, request):
         """删除训练任务
 
         :param request: Request instance for DeleteTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteTrainingTaskRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteTrainingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAPIConfigs(self, request):
         """列举API
 
         :param request: Request instance for DescribeAPIConfigs.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeAPIConfigsRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeAPIConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchTask(self, request):
         """查询跑批任务
 
         :param request: Request instance for DescribeBatchTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBatchTaskRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeBatchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchTaskInstances(self, request):
         """查询跑批实例列表
 
         :param request: Request instance for DescribeBatchTaskInstances.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBatchTaskInstancesRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeBatchTaskInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchTasks(self, request):
         """批量预测任务列表信息
 
         :param request: Request instance for DescribeBatchTasks.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBatchTasksRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeBatchTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillingResourceGroups(self, request):
         """查询资源组详情
 
         :param request: Request instance for DescribeBillingResourceGroups.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBillingResourceGroupsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeBillingResourceGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillingSpecs(self, request):
         """本接口(DescribeBillingSpecs)用于查询计费项列表
 
         :param request: Request instance for DescribeBillingSpecs.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBillingSpecsRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeBillingSpecsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBillingSpecsPrice(self, request):
         """本接口(DescribeBillingSpecsPrice)用于查询计费项价格。
 
         :param request: Request instance for DescribeBillingSpecsPrice.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeBillingSpecsPriceRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeBillingSpecsPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatasetDetailStructured(self, request):
         """查询结构化数据集详情
 
         :param request: Request instance for DescribeDatasetDetailStructured.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeDatasetDetailStructuredRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeDatasetDetailStructuredResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatasetDetailUnstructured(self, request):
         """查询非结构化数据集详情
 
         :param request: Request instance for DescribeDatasetDetailUnstructured.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeDatasetDetailUnstructuredRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeDatasetDetailUnstructuredResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatasets(self, request):
         """查询数据集列表
 
         :param request: Request instance for DescribeDatasets.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeDatasetsRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeDatasetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInferTemplates(self, request):
         """查询推理镜像模板
 
         :param request: Request instance for DescribeInferTemplates.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeInferTemplatesRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeInferTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLatestTrainingMetrics(self, request):
         """查询最近上报的训练自定义指标
 
         :param request: Request instance for DescribeLatestTrainingMetrics.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeLatestTrainingMetricsRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeLatestTrainingMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogs(self, request):
         """获取训练、推理、Notebook服务的日志
 
         :param request: Request instance for DescribeLogs.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeLogsRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelAccEngineVersions(self, request):
         """查询模型加速引擎版本列表
 
         :param request: Request instance for DescribeModelAccEngineVersions.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelAccEngineVersionsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeModelAccEngineVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelAccelerateTask(self, request):
         """查询模型优化任务详情
 
         :param request: Request instance for DescribeModelAccelerateTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelAccelerateTaskRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeModelAccelerateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelAccelerateTasks(self, request):
         """查询模型加速任务列表
 
         :param request: Request instance for DescribeModelAccelerateTasks.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelAccelerateTasksRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeModelAccelerateTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelService(self, request):
         """查询单个服务
 
         :param request: Request instance for DescribeModelService.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeModelServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServiceCallInfo(self, request):
         """展示服务的调用信息
 
         :param request: Request instance for DescribeModelServiceCallInfo.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceCallInfoRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeModelServiceCallInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServiceGroup(self, request):
         """查询单个服务组
 
         :param request: Request instance for DescribeModelServiceGroup.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceGroupRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeModelServiceGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServiceGroups(self, request):
         """列举在线推理服务组
 
         :param request: Request instance for DescribeModelServiceGroups.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceGroupsRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeModelServiceGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServiceHistory(self, request):
         """展示服务的历史版本
 
         :param request: Request instance for DescribeModelServiceHistory.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceHistoryRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeModelServiceHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServiceHotUpdated(self, request):
         """用于查询模型服务能否开启热更新
 
         :param request: Request instance for DescribeModelServiceHotUpdated.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServiceHotUpdatedRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeModelServiceHotUpdatedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelServices(self, request):
         """查询多个服务
 
         :param request: Request instance for DescribeModelServices.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeModelServicesRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeModelServicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingFrameworks(self, request):
         """训练框架列表
 
         :param request: Request instance for DescribeTrainingFrameworks.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingFrameworksRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeTrainingFrameworksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingMetrics(self, request):
         """查询训练自定义指标
 
         :param request: Request instance for DescribeTrainingMetrics.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingMetricsRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeTrainingMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingModelVersion(self, request):
         """查询模型版本
 
         :param request: Request instance for DescribeTrainingModelVersion.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingModelVersionRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeTrainingModelVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingModelVersions(self, request):
         """模型版本列表
 
         :param request: Request instance for DescribeTrainingModelVersions.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingModelVersionsRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeTrainingModelVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingModels(self, request):
         """模型列表
 
         :param request: Request instance for DescribeTrainingModels.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingModelsRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeTrainingModelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingTask(self, request):
         """训练任务详情
 
         :param request: Request instance for DescribeTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingTaskRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeTrainingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingTaskPods(self, request):
         """训练任务pod列表
 
         :param request: Request instance for DescribeTrainingTaskPods.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingTaskPodsRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeTrainingTaskPodsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingTasks(self, request):
         """训练任务列表
 
         :param request: Request instance for DescribeTrainingTasks.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingTasksRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeTrainingTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModelService(self, request):
         """用于更新模型服务
 
         :param request: Request instance for ModifyModelService.
         :type request: :class:`tencentcloud.tione.v20211111.models.ModifyModelServiceRequest`
@@ -1100,15 +1100,15 @@
             model = models.ModifyModelServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModelServicePartialConfig(self, request):
         """增量更新在线推理服务的部分配置，不更新的配置项不需要传入
 
         :param request: Request instance for ModifyModelServicePartialConfig.
         :type request: :class:`tencentcloud.tione.v20211111.models.ModifyModelServicePartialConfigRequest`
@@ -1123,15 +1123,15 @@
             model = models.ModifyModelServicePartialConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceGroupWeights(self, request):
         """更新推理服务组流量分配
 
         :param request: Request instance for ModifyServiceGroupWeights.
         :type request: :class:`tencentcloud.tione.v20211111.models.ModifyServiceGroupWeightsRequest`
@@ -1146,15 +1146,15 @@
             model = models.ModifyServiceGroupWeightsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PushTrainingMetrics(self, request):
         """上报训练自定义指标
 
         :param request: Request instance for PushTrainingMetrics.
         :type request: :class:`tencentcloud.tione.v20211111.models.PushTrainingMetricsRequest`
@@ -1169,15 +1169,15 @@
             model = models.PushTrainingMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartModelAccelerateTask(self, request):
         """重启模型加速任务
 
         :param request: Request instance for RestartModelAccelerateTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.RestartModelAccelerateTaskRequest`
@@ -1192,15 +1192,15 @@
             model = models.RestartModelAccelerateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartTrainingTask(self, request):
         """启动模型训练任务
 
         :param request: Request instance for StartTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StartTrainingTaskRequest`
@@ -1215,15 +1215,15 @@
             model = models.StartTrainingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopBatchTask(self, request):
         """停止跑批任务
 
         :param request: Request instance for StopBatchTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StopBatchTaskRequest`
@@ -1238,15 +1238,15 @@
             model = models.StopBatchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopModelAccelerateTask(self, request):
         """停止模型加速任务
 
         :param request: Request instance for StopModelAccelerateTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StopModelAccelerateTaskRequest`
@@ -1261,15 +1261,15 @@
             model = models.StopModelAccelerateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopTrainingTask(self, request):
         """停止模型训练任务
 
         :param request: Request instance for StopTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StopTrainingTaskRequest`
@@ -1284,8 +1284,8 @@
             model = models.StopTrainingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/tione_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCodeRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotebookInstance(self, request):
         """创建Notebook实例
 
         :param request: Request instance for CreateNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.CreateNotebookInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.CreateNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNotebookLifecycleScript(self, request):
         """创建Notebook生命周期脚本
 
         :param request: Request instance for CreateNotebookLifecycleScript.
         :type request: :class:`tencentcloud.tione.v20191022.models.CreateNotebookLifecycleScriptRequest`
@@ -88,15 +88,15 @@
             model = models.CreateNotebookLifecycleScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePresignedNotebookInstanceUrl(self, request):
         """创建Notebook授权Url
 
         :param request: Request instance for CreatePresignedNotebookInstanceUrl.
         :type request: :class:`tencentcloud.tione.v20191022.models.CreatePresignedNotebookInstanceUrlRequest`
@@ -111,15 +111,15 @@
             model = models.CreatePresignedNotebookInstanceUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrainingJob(self, request):
         """创建训练任务
 
         :param request: Request instance for CreateTrainingJob.
         :type request: :class:`tencentcloud.tione.v20191022.models.CreateTrainingJobRequest`
@@ -134,15 +134,15 @@
             model = models.CreateTrainingJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCodeRepository(self, request):
         """删除存储库
 
         :param request: Request instance for DeleteCodeRepository.
         :type request: :class:`tencentcloud.tione.v20191022.models.DeleteCodeRepositoryRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteCodeRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNotebookInstance(self, request):
         """删除notebook实例
 
         :param request: Request instance for DeleteNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.DeleteNotebookInstanceRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNotebookLifecycleScript(self, request):
         """删除Notebook生命周期脚本
 
         :param request: Request instance for DeleteNotebookLifecycleScript.
         :type request: :class:`tencentcloud.tione.v20191022.models.DeleteNotebookLifecycleScriptRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteNotebookLifecycleScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodeRepositories(self, request):
         """查询存储库列表
 
         :param request: Request instance for DescribeCodeRepositories.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeCodeRepositoriesRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeCodeRepositoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCodeRepository(self, request):
         """查询存储库详情
 
         :param request: Request instance for DescribeCodeRepository.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeCodeRepositoryRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeCodeRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookInstance(self, request):
         """查询Notebook实例详情
 
         :param request: Request instance for DescribeNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeNotebookInstanceRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookInstances(self, request):
         """查询Notebook实例列表
 
         :param request: Request instance for DescribeNotebookInstances.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeNotebookInstancesRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeNotebookInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookLifecycleScript(self, request):
         """查看notebook生命周期脚本详情
 
         :param request: Request instance for DescribeNotebookLifecycleScript.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeNotebookLifecycleScriptRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeNotebookLifecycleScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookLifecycleScripts(self, request):
         """查看notebook生命周期脚本列表
 
         :param request: Request instance for DescribeNotebookLifecycleScripts.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeNotebookLifecycleScriptsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeNotebookLifecycleScriptsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNotebookSummary(self, request):
         """查询Notebook概览数据
 
         :param request: Request instance for DescribeNotebookSummary.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeNotebookSummaryRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeNotebookSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingJob(self, request):
         """查询训练任务
 
         :param request: Request instance for DescribeTrainingJob.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeTrainingJobRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeTrainingJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrainingJobs(self, request):
         """查询训练任务列表
 
         :param request: Request instance for DescribeTrainingJobs.
         :type request: :class:`tencentcloud.tione.v20191022.models.DescribeTrainingJobsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeTrainingJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartNotebookInstance(self, request):
         """启动Notebook实例
 
         :param request: Request instance for StartNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.StartNotebookInstanceRequest`
@@ -433,15 +433,15 @@
             model = models.StartNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopNotebookInstance(self, request):
         """停止Notebook实例
 
         :param request: Request instance for StopNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.StopNotebookInstanceRequest`
@@ -456,15 +456,15 @@
             model = models.StopNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopTrainingJob(self, request):
         """停止训练任务
 
         :param request: Request instance for StopTrainingJob.
         :type request: :class:`tencentcloud.tione.v20191022.models.StopTrainingJobRequest`
@@ -479,15 +479,15 @@
             model = models.StopTrainingJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCodeRepository(self, request):
         """更新存储库
 
         :param request: Request instance for UpdateCodeRepository.
         :type request: :class:`tencentcloud.tione.v20191022.models.UpdateCodeRepositoryRequest`
@@ -502,15 +502,15 @@
             model = models.UpdateCodeRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateNotebookInstance(self, request):
         """更新Notebook实例
 
         :param request: Request instance for UpdateNotebookInstance.
         :type request: :class:`tencentcloud.tione.v20191022.models.UpdateNotebookInstanceRequest`
@@ -525,15 +525,15 @@
             model = models.UpdateNotebookInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateNotebookLifecycleScript(self, request):
         """更新notebook生命周期脚本
 
         :param request: Request instance for UpdateNotebookLifecycleScript.
         :type request: :class:`tencentcloud.tione.v20191022.models.UpdateNotebookLifecycleScriptRequest`
@@ -548,8 +548,8 @@
             model = models.UpdateNotebookLifecycleScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.937/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.938/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.937/README.rst` & `tencentcloud-sdk-python-tione-3.0.938/README.rst`

 * *Files identical despite different names*

