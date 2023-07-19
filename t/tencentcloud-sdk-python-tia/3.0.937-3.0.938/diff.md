# Comparing `tmp/tencentcloud-sdk-python-tia-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tia-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.937.tar", last modified: Tue Jul 18 00:32:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.938.tar", last modified: Wed Jul 19 00:50:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tia-3.0.937.tar` & `tencentcloud-sdk-python-tia-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/
--rw-r--r--   0 root         (0) root         (0)    10642 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/tia_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49879 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:45.000000 tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/
+-rw-r--r--   0 root         (0) root         (0)    10682 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/tia_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49879 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:26.000000 tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tia-3.0.937/setup.py` & `tencentcloud-sdk-python-tia-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/tia_client.py` & `tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/tia_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateModel(self, request):
         """部署模型，用以对外提供服务。有两种部署模式：`无服务器模式` 和 `集群模式`。`无服务器模式` 下，模型文件被部署到无服务器云函数，即 [SCF](https://cloud.tencent.com/product/scf)，用户可以在其控制台上进一步操作。`集群模式` 下，模型文件被部署到 TI-A 的计算集群中。
 
         :param request: Request instance for CreateModel.
         :type request: :class:`tencentcloud.tia.v20180226.models.CreateModelRequest`
@@ -65,15 +65,15 @@
             model = models.CreateModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteJob(self, request):
         """删除训练任务
 
         :param request: Request instance for DeleteJob.
         :type request: :class:`tencentcloud.tia.v20180226.models.DeleteJobRequest`
@@ -88,15 +88,15 @@
             model = models.DeleteJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModel(self, request):
         """删除指定的部署模型。模型有两种部署模式：`无服务器模式` 和 `集群模式`。`无服务器模式` 下，模型文件被部署到无服务器云函数，即 [SCF](https://cloud.tencent.com/product/scf)，用户可以在其控制台上进一步操作。`集群模式` 下，模型文件被部署到 TI-A 的计算集群中。
 
         :param request: Request instance for DeleteModel.
         :type request: :class:`tencentcloud.tia.v20180226.models.DeleteModelRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJob(self, request):
         """获取训练任务详情
 
         :param request: Request instance for DescribeJob.
         :type request: :class:`tencentcloud.tia.v20180226.models.DescribeJobRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModel(self, request):
         """描述已经部署的某个模型。而模型部署有两种模式：`无服务器模式` 和 `集群模式`。`无服务器模式` 下，模型文件被部署到无服务器云函数，即 [SCF](https://cloud.tencent.com/product/scf)，用户可以在其控制台上进一步操作。`集群模式` 下，模型文件被部署到 TI-A 的计算集群中。
 
         :param request: Request instance for DescribeModel.
         :type request: :class:`tencentcloud.tia.v20180226.models.DescribeModelRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InstallAgent(self, request):
         """安装agent
 
         :param request: Request instance for InstallAgent.
         :type request: :class:`tencentcloud.tia.v20180226.models.InstallAgentRequest`
@@ -180,15 +180,15 @@
             model = models.InstallAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListJobs(self, request):
         """列举训练任务
 
         :param request: Request instance for ListJobs.
         :type request: :class:`tencentcloud.tia.v20180226.models.ListJobsRequest`
@@ -203,15 +203,15 @@
             model = models.ListJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListModels(self, request):
         """用以列举已经部署的模型。而部署有两种模式：`无服务器模式` 和 `集群模式`。`无服务器模式` 下，模型文件被部署到无服务器云函数，即 [SCF](https://cloud.tencent.com/product/scf)，用户可以在其控制台上进一步操作。`集群模式` 下，模型文件被部署到 TI-A 的计算集群中。不同部署模式下的模型分开列出。
 
         :param request: Request instance for ListModels.
         :type request: :class:`tencentcloud.tia.v20180226.models.ListModelsRequest`
@@ -226,15 +226,15 @@
             model = models.ListModelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryLogs(self, request):
         """查询 TI-A 训练任务的日志
 
         :param request: Request instance for QueryLogs.
         :type request: :class:`tencentcloud.tia.v20180226.models.QueryLogsRequest`
@@ -249,8 +249,8 @@
             model = models.QueryLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/errorcodes.py` & `tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.937/tencentcloud/tia/v20180226/models.py` & `tencentcloud-sdk-python-tia-3.0.938/tencentcloud/tia/v20180226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tia-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tia-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.937/README.rst` & `tencentcloud-sdk-python-tia-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.937/tencentcloud_sdk_python_tia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.938/tencentcloud_sdk_python_tia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

