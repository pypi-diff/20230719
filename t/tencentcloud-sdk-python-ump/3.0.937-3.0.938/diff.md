# Comparing `tmp/tencentcloud-sdk-python-ump-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ump-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ump-3.0.937.tar", last modified: Tue Jul 18 00:34:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ump-3.0.938.tar", last modified: Wed Jul 19 00:53:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ump-3.0.937.tar` & `tencentcloud-sdk-python-ump-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/
--rw-r--r--   0 root         (0) root         (0)    16023 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/ump_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89302 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:39.000000 tencentcloud-sdk-python-ump-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/
+-rw-r--r--   0 root         (0) root         (0)    16091 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/ump_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89302 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:22.000000 tencentcloud-sdk-python-ump-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ump-3.0.937/setup.py` & `tencentcloud-sdk-python-ump-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ump-3.0.937/tencentcloud_sdk_python_ump.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ump-3.0.938/tencentcloud_sdk_python_ump.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ump
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ump SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/ump_client.py` & `tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/ump_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.CreateCameraAlertsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCameraState(self, request):
         """上报当前场内所有相机的当前状态
 
         :param request: Request instance for CreateCameraState.
         :type request: :class:`tencentcloud.ump.v20200918.models.CreateCameraStateRequest`
@@ -66,15 +66,15 @@
             model = models.CreateCameraStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCapture(self, request):
         """场内抓拍上报接口
 
         :param request: Request instance for CreateCapture.
         :type request: :class:`tencentcloud.ump.v20200918.models.CreateCaptureRequest`
@@ -89,15 +89,15 @@
             model = models.CreateCaptureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultiBizAlert(self, request):
         """集团广场的多经点位告警
 
         :param request: Request instance for CreateMultiBizAlert.
         :type request: :class:`tencentcloud.ump.v20200918.models.CreateMultiBizAlertRequest`
@@ -112,15 +112,15 @@
             model = models.CreateMultiBizAlertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProgramState(self, request):
         """上报所有进程监控信息
 
         :param request: Request instance for CreateProgramState.
         :type request: :class:`tencentcloud.ump.v20200918.models.CreateProgramStateRequest`
@@ -135,15 +135,15 @@
             model = models.CreateProgramStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServerState(self, request):
         """上报所有服务器硬件监控信息
 
         :param request: Request instance for CreateServerState.
         :type request: :class:`tencentcloud.ump.v20200918.models.CreateServerStateRequest`
@@ -158,15 +158,15 @@
             model = models.CreateServerStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMultiBizAlert(self, request):
         """集团广场的多经点位消警
 
         :param request: Request instance for DeleteMultiBizAlert.
         :type request: :class:`tencentcloud.ump.v20200918.models.DeleteMultiBizAlertRequest`
@@ -181,15 +181,15 @@
             model = models.DeleteMultiBizAlertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTask(self, request):
         """删除集团广场对应的任务
 
         :param request: Request instance for DeleteTask.
         :type request: :class:`tencentcloud.ump.v20200918.models.DeleteTaskRequest`
@@ -204,15 +204,15 @@
             model = models.DeleteTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCameras(self, request):
         """获取集团广场对应的摄像头列表
 
         :param request: Request instance for DescribeCameras.
         :type request: :class:`tencentcloud.ump.v20200918.models.DescribeCamerasRequest`
@@ -227,15 +227,15 @@
             model = models.DescribeCamerasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfig(self, request):
         """获取摄像头配置信息
         mac不为空返回指定相机配置
         mac为空返回对应GroupCode和MallId全量配置
 
@@ -252,15 +252,15 @@
             model = models.DescribeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImage(self, request):
         """实时获取底图接口
 
         :param request: Request instance for DescribeImage.
         :type request: :class:`tencentcloud.ump.v20200918.models.DescribeImageRequest`
@@ -275,15 +275,15 @@
             model = models.DescribeImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMultiBizBaseImage(self, request):
         """获取多经点位底图
 
         :param request: Request instance for DescribeMultiBizBaseImage.
         :type request: :class:`tencentcloud.ump.v20200918.models.DescribeMultiBizBaseImageRequest`
@@ -298,15 +298,15 @@
             model = models.DescribeMultiBizBaseImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """查询集团广场对应的任务列表
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.ump.v20200918.models.DescribeTasksRequest`
@@ -321,15 +321,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """获取集团广场的点位列表
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.ump.v20200918.models.DescribeZonesRequest`
@@ -344,15 +344,15 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMultiBizConfig(self, request):
         """集团广场的多经点位配置更新
 
         :param request: Request instance for ModifyMultiBizConfig.
         :type request: :class:`tencentcloud.ump.v20200918.models.ModifyMultiBizConfigRequest`
@@ -367,15 +367,15 @@
             model = models.ModifyMultiBizConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportServiceRegister(self, request):
         """上报服务注册自身的服务地址作为回调地址, 用于信息回传。
 
         :param request: Request instance for ReportServiceRegister.
         :type request: :class:`tencentcloud.ump.v20200918.models.ReportServiceRegisterRequest`
@@ -390,15 +390,15 @@
             model = models.ReportServiceRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchImage(self, request):
         """以图搜图
 
         :param request: Request instance for SearchImage.
         :type request: :class:`tencentcloud.ump.v20200918.models.SearchImageRequest`
@@ -413,8 +413,8 @@
             model = models.SearchImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/errorcodes.py` & `tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ump-3.0.937/tencentcloud/ump/v20200918/models.py` & `tencentcloud-sdk-python-ump-3.0.938/tencentcloud/ump/v20200918/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ump-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ump-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ump-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ump-3.0.938/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ump
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ump SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ump-3.0.937/README.rst` & `tencentcloud-sdk-python-ump-3.0.938/README.rst`

 * *Files identical despite different names*

