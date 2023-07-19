# Comparing `tmp/tencentcloud-sdk-python-iotvideo-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iotvideo-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.937.tar", last modified: Tue Jul 18 00:25:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.938.tar", last modified: Wed Jul 19 00:41:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotvideo-3.0.937.tar` & `tencentcloud-sdk-python-iotvideo-3.0.938.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87013 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   365162 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72251 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   303767 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64459 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229605 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      861 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:58.000000 tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87393 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   365162 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72567 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   303767 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64723 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:41:22.000000 tencentcloud-sdk-python-iotvideo-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:23.000000 tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/setup.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyAIModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchUpdateFirmware(self, request):
         """本接口（BatchUpdateFirmware）用于批量更新设备固件
 
         :param request: Request instance for BatchUpdateFirmware.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.BatchUpdateFirmwareRequest`
@@ -65,15 +65,15 @@
             model = models.BatchUpdateFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindCloudStorageUser(self, request):
         """绑定云存用户
 
         :param request: Request instance for BindCloudStorageUser.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.BindCloudStorageUserRequest`
@@ -88,15 +88,15 @@
             model = models.BindCloudStorageUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallDeviceActionAsync(self, request):
         """异步调用设备行为
 
         :param request: Request instance for CallDeviceActionAsync.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CallDeviceActionAsyncRequest`
@@ -111,15 +111,15 @@
             model = models.CallDeviceActionAsyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallDeviceActionSync(self, request):
         """同步调用设备行为
 
         :param request: Request instance for CallDeviceActionSync.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CallDeviceActionSyncRequest`
@@ -134,15 +134,15 @@
             model = models.CallDeviceActionSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallTRTCDevice(self, request):
         """呼叫TRTC设备
 
         :param request: Request instance for CallTRTCDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CallTRTCDeviceRequest`
@@ -157,15 +157,15 @@
             model = models.CallTRTCDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelAIModelApplication(self, request):
         """取消AI模型申请
 
         :param request: Request instance for CancelAIModelApplication.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CancelAIModelApplicationRequest`
@@ -180,15 +180,15 @@
             model = models.CancelAIModelApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelDeviceFirmwareTask(self, request):
         """本接口用于取消设备升级任务
 
         :param request: Request instance for CancelDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CancelDeviceFirmwareTaskRequest`
@@ -203,15 +203,15 @@
             model = models.CancelDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckForwardAuth(self, request):
         """判断是否开启转发的权限
 
         :param request: Request instance for CheckForwardAuth.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CheckForwardAuthRequest`
@@ -226,15 +226,15 @@
             model = models.CheckForwardAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ControlDeviceData(self, request):
         """根据设备产品ID、设备名称，设置控制设备的属性数据。
 
         :param request: Request instance for ControlDeviceData.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ControlDeviceDataRequest`
@@ -249,15 +249,15 @@
             model = models.ControlDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAIDetection(self, request):
         """发起AI推理请求
 
         :param request: Request instance for CreateAIDetection.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateAIDetectionRequest`
@@ -272,15 +272,15 @@
             model = models.CreateAIDetectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBatch(self, request):
         """创建批次
 
         :param request: Request instance for CreateBatch.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateBatchRequest`
@@ -295,15 +295,15 @@
             model = models.CreateBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCOSCredentials(self, request):
         """创建COS上传密钥
 
         :param request: Request instance for CreateCOSCredentials.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateCOSCredentialsRequest`
@@ -318,15 +318,15 @@
             model = models.CreateCOSCredentialsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudStorage(self, request):
         """开通云存服务
 
         :param request: Request instance for CreateCloudStorage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateCloudStorageRequest`
@@ -341,15 +341,15 @@
             model = models.CreateCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDataForward(self, request):
         """创建数据转发
 
         :param request: Request instance for CreateDataForward.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateDataForwardRequest`
@@ -364,15 +364,15 @@
             model = models.CreateDataForwardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateForwardRule(self, request):
         """创建转发规则
 
         :param request: Request instance for CreateForwardRule.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateForwardRuleRequest`
@@ -387,15 +387,15 @@
             model = models.CreateForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
         """创建产品
 
         :param request: Request instance for CreateProduct.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateProductRequest`
@@ -410,15 +410,15 @@
             model = models.CreateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTaskFileUrl(self, request):
         """本接口（CreateTaskFileUrl）用于获取产品级任务文件上传链接
 
         :param request: Request instance for CreateTaskFileUrl.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.CreateTaskFileUrlRequest`
@@ -433,15 +433,15 @@
             model = models.CreateTaskFileUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDevice(self, request):
         """删除设备
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteDeviceRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFirmware(self, request):
         """本接口（DeleteFirmware）用于删除固件
 
         :param request: Request instance for DeleteFirmware.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteFirmwareRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteForwardRule(self, request):
         """删除转发规则
 
         :param request: Request instance for DeleteForwardRule.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteForwardRuleRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProduct(self, request):
         """删除产品
 
         :param request: Request instance for DeleteProduct.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DeleteProductRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIModelApplications(self, request):
         """用户AI模型申请记录
 
         :param request: Request instance for DescribeAIModelApplications.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeAIModelApplicationsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeAIModelApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIModelChannel(self, request):
         """查看AI推理结果推送配置
 
         :param request: Request instance for DescribeAIModelChannel.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeAIModelChannelRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeAIModelChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIModelUsage(self, request):
         """查看AI模型资源包
 
         :param request: Request instance for DescribeAIModelUsage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeAIModelUsageRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeAIModelUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIModels(self, request):
         """拉取AI模型列表
 
         :param request: Request instance for DescribeAIModels.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeAIModelsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeAIModelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccount(self, request):
         """获取消费版账号信息
 
         :param request: Request instance for DescribeAccount.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeAccountRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBalance(self, request):
         """查询账户余额
 
         :param request: Request instance for DescribeBalance.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeBalanceRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBalanceTransactions(self, request):
         """拉取账户流水
 
         :param request: Request instance for DescribeBalanceTransactions.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeBalanceTransactionsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeBalanceTransactionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatch(self, request):
         """获取批次详情
 
         :param request: Request instance for DescribeBatch.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeBatchRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchs(self, request):
         """获取批次列表
 
         :param request: Request instance for DescribeBatchs.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeBatchsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeBatchsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBonuses(self, request):
         """查看运营活动资源包列表
 
         :param request: Request instance for DescribeBonuses.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeBonusesRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeBonusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCategory(self, request):
         """获取Category详情
 
         :param request: Request instance for DescribeCategory.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCategoryRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeCategoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorage(self, request):
         """获取设备云存服务详情
 
         :param request: Request instance for DescribeCloudStorage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageDate(self, request):
         """获取具有云存的日期
 
         :param request: Request instance for DescribeCloudStorageDate.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageDateRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeCloudStorageDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageEvents(self, request):
         """拉取云存事件列表
 
         :param request: Request instance for DescribeCloudStorageEvents.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageEventsRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeCloudStorageEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStoragePackageConsumeDetails(self, request):
         """获取云存套餐包消耗详细记录
 
         :param request: Request instance for DescribeCloudStoragePackageConsumeDetails.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStoragePackageConsumeDetailsRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeCloudStoragePackageConsumeDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStoragePackageConsumeStats(self, request):
         """获取云存套餐包消耗统计
 
         :param request: Request instance for DescribeCloudStoragePackageConsumeStats.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStoragePackageConsumeStatsRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeCloudStoragePackageConsumeStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageStreamData(self, request):
         """获取设备图片流数据
 
         :param request: Request instance for DescribeCloudStorageStreamData.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageStreamDataRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeCloudStorageStreamDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageThumbnail(self, request):
         """拉取云存事件缩略图
 
         :param request: Request instance for DescribeCloudStorageThumbnail.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageThumbnailRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeCloudStorageThumbnailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageTime(self, request):
         """获取某一天云存时间轴
 
         :param request: Request instance for DescribeCloudStorageTime.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageTimeRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeCloudStorageTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudStorageUsers(self, request):
         """拉取云存用户列表
 
         :param request: Request instance for DescribeCloudStorageUsers.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeCloudStorageUsersRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeCloudStorageUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataForwardList(self, request):
         """获取数据转发列表
 
         :param request: Request instance for DescribeDataForwardList.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDataForwardListRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDataForwardListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
         """查看设备详情
 
         :param request: Request instance for DescribeDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceActionHistory(self, request):
         """为用户提供获取动作历史的能力。
 
         :param request: Request instance for DescribeDeviceActionHistory.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceActionHistoryRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeDeviceActionHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceCommLog(self, request):
         """获取设备在指定时间范围内的通讯日志
 
         :param request: Request instance for DescribeDeviceCommLog.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceCommLogRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeDeviceCommLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceData(self, request):
         """获取设备属性数据
 
         :param request: Request instance for DescribeDeviceData.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceDataRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceDataHistory(self, request):
         """获取设备在指定时间范围内上报的历史数据。
 
         :param request: Request instance for DescribeDeviceDataHistory.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceDataHistoryRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeDeviceDataHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceDataStats(self, request):
         """查询设备数据统计
 
         :param request: Request instance for DescribeDeviceDataStats.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceDataStatsRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeDeviceDataStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceEventHistory(self, request):
         """获取设备的历史事件
 
         :param request: Request instance for DescribeDeviceEventHistory.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceEventHistoryRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeDeviceEventHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceStatusLog(self, request):
         """获取设备上下线日志
 
         :param request: Request instance for DescribeDeviceStatusLog.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDeviceStatusLogRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeDeviceStatusLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
         """获取设备列表
 
         :param request: Request instance for DescribeDevices.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeDevicesRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmware(self, request):
         """本接口（DescribeFirmware）用于查询固件信息
 
         :param request: Request instance for DescribeFirmware.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTask(self, request):
         """此接口查询固件升级任务详情
 
         :param request: Request instance for DescribeFirmwareTask.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareTaskRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTaskDevices(self, request):
         """本接口用于查询固件升级任务的设备列表
 
         :param request: Request instance for DescribeFirmwareTaskDevices.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareTaskDevicesRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeFirmwareTaskDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTaskDistribution(self, request):
         """本接口用于查询固件升级任务状态分布
 
         :param request: Request instance for DescribeFirmwareTaskDistribution.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareTaskDistributionRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeFirmwareTaskDistributionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTaskStatistics(self, request):
         """本接口用于查询固件升级任务统计信息
 
         :param request: Request instance for DescribeFirmwareTaskStatistics.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareTaskStatisticsRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeFirmwareTaskStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTasks(self, request):
         """本接口用于查询固件升级任务列表
 
         :param request: Request instance for DescribeFirmwareTasks.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeFirmwareTasksRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeFirmwareTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeForwardRule(self, request):
         """获取产品转发规则
 
         :param request: Request instance for DescribeForwardRule.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeForwardRuleRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMessageDataStats(self, request):
         """查询设备消息数量统计
 
         :param request: Request instance for DescribeMessageDataStats.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeMessageDataStatsRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeMessageDataStatsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModelDefinition(self, request):
         """查询产品配置的数据模板信息
 
         :param request: Request instance for DescribeModelDefinition.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeModelDefinitionRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackageConsumeTask(self, request):
         """查询套餐消耗记录详情
 
         :param request: Request instance for DescribePackageConsumeTask.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribePackageConsumeTaskRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribePackageConsumeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackageConsumeTasks(self, request):
         """查询套餐消耗记录列表
 
         :param request: Request instance for DescribePackageConsumeTasks.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribePackageConsumeTasksRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribePackageConsumeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProduct(self, request):
         """获取产品详情
 
         :param request: Request instance for DescribeProduct.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeProductRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductDynamicRegister(self, request):
         """获取产品动态注册详情
 
         :param request: Request instance for DescribeProductDynamicRegister.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeProductDynamicRegisterRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProducts(self, request):
         """获取产品列表
 
         :param request: Request instance for DescribeProducts.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeProductsRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushChannel(self, request):
         """查看推送通道
 
         :param request: Request instance for DescribePushChannel.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribePushChannelRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribePushChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSDKLog(self, request):
         """获取设备sdk日志
 
         :param request: Request instance for DescribeSDKLog.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeSDKLogRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeSDKLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUser(self, request):
         """获取video消费版用户信息
 
         :param request: Request instance for DescribeUser.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.DescribeUserRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditFirmware(self, request):
         """本接口用于编辑固件信息
 
         :param request: Request instance for EditFirmware.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.EditFirmwareRequest`
@@ -1629,15 +1629,15 @@
             model = models.EditFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenSingleDeviceSignatureOfPublic(self, request):
         """获取设备的绑定签名
 
         :param request: Request instance for GenSingleDeviceSignatureOfPublic.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.GenSingleDeviceSignatureOfPublicRequest`
@@ -1652,15 +1652,15 @@
             model = models.GenSingleDeviceSignatureOfPublicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateSignedVideoURL(self, request):
         """获取视频防盗链播放URL
 
         :param request: Request instance for GenerateSignedVideoURL.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.GenerateSignedVideoURLRequest`
@@ -1675,15 +1675,15 @@
             model = models.GenerateSignedVideoURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAllFirmwareVersion(self, request):
         """本接口（GetAllFirmwareVersion）用于获取所有的版本列表
 
         :param request: Request instance for GetAllFirmwareVersion.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.GetAllFirmwareVersionRequest`
@@ -1698,15 +1698,15 @@
             model = models.GetAllFirmwareVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFirmwareURL(self, request):
         """本接口（GetFirmwareURL）用于获取固件存储的URL
 
         :param request: Request instance for GetFirmwareURL.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.GetFirmwareURLRequest`
@@ -1721,15 +1721,15 @@
             model = models.GetFirmwareURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportModelDefinition(self, request):
         """导入其它产品的数据模板，覆盖现有数据模板的物模型和产品分类信息
 
         :param request: Request instance for ImportModelDefinition.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ImportModelDefinitionRequest`
@@ -1744,15 +1744,15 @@
             model = models.ImportModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InheritCloudStorageUser(self, request):
         """继承云存用户
 
         :param request: Request instance for InheritCloudStorageUser.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.InheritCloudStorageUserRequest`
@@ -1767,15 +1767,15 @@
             model = models.InheritCloudStorageUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListFirmwares(self, request):
         """本接口（ListFirmwares）用于获取固件列表
 
         :param request: Request instance for ListFirmwares.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ListFirmwaresRequest`
@@ -1790,15 +1790,15 @@
             model = models.ListFirmwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDataForward(self, request):
         """修改数据转发
 
         :param request: Request instance for ModifyDataForward.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyDataForwardRequest`
@@ -1813,15 +1813,15 @@
             model = models.ModifyDataForwardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDataForwardStatus(self, request):
         """设置数据转发状态
 
         :param request: Request instance for ModifyDataForwardStatus.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyDataForwardStatusRequest`
@@ -1836,15 +1836,15 @@
             model = models.ModifyDataForwardStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDevice(self, request):
         """修改设备信息
 
         :param request: Request instance for ModifyDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyDeviceRequest`
@@ -1859,15 +1859,15 @@
             model = models.ModifyDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDeviceLogLevel(self, request):
         """更新设备日志级别
 
         :param request: Request instance for ModifyDeviceLogLevel.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyDeviceLogLevelRequest`
@@ -1882,15 +1882,15 @@
             model = models.ModifyDeviceLogLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyForwardRule(self, request):
         """修改转发规则
 
         :param request: Request instance for ModifyForwardRule.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyForwardRuleRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifyForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyModelDefinition(self, request):
         """提供修改产品的数据模板的能力
 
         :param request: Request instance for ModifyModelDefinition.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyModelDefinitionRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProduct(self, request):
         """修改产品信息
 
         :param request: Request instance for ModifyProduct.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyProductRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProductDynamicRegister(self, request):
         """修改产品动态注册
 
         :param request: Request instance for ModifyProductDynamicRegister.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyProductDynamicRegisterRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPushChannel(self, request):
         """更新推送通道
 
         :param request: Request instance for ModifyPushChannel.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ModifyPushChannelRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyPushChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishMessage(self, request):
         """本接口（PublishMessage）用于使用自定义透传协议进行设备远控
 
         :param request: Request instance for PublishMessage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.PublishMessageRequest`
@@ -2020,15 +2020,15 @@
             model = models.PublishMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportAliveDevice(self, request):
         """上报活跃设备
 
         :param request: Request instance for ReportAliveDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ReportAliveDeviceRequest`
@@ -2043,15 +2043,15 @@
             model = models.ReportAliveDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetCloudStorage(self, request):
         """重置云存服务
 
         :param request: Request instance for ResetCloudStorage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.ResetCloudStorageRequest`
@@ -2066,15 +2066,15 @@
             model = models.ResetCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryDeviceFirmwareTask(self, request):
         """本接口用于重试设备升级任务
 
         :param request: Request instance for RetryDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.RetryDeviceFirmwareTaskRequest`
@@ -2089,15 +2089,15 @@
             model = models.RetryDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetForwardAuth(self, request):
         """设置转发权限
 
         :param request: Request instance for SetForwardAuth.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.SetForwardAuthRequest`
@@ -2112,15 +2112,15 @@
             model = models.SetForwardAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransferCloudStorage(self, request):
         """转移云存服务
 
         :param request: Request instance for TransferCloudStorage.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.TransferCloudStorageRequest`
@@ -2135,15 +2135,15 @@
             model = models.TransferCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAIModelChannel(self, request):
         """更新AI推理结果推送配置
 
         :param request: Request instance for UpdateAIModelChannel.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.UpdateAIModelChannelRequest`
@@ -2158,15 +2158,15 @@
             model = models.UpdateAIModelChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFirmware(self, request):
         """本接口（UploadFirmware）用于上传设备固件信息
 
         :param request: Request instance for UploadFirmware.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.UploadFirmwareRequest`
@@ -2181,15 +2181,15 @@
             model = models.UploadFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WakeUpDevice(self, request):
         """设备唤醒
 
         :param request: Request instance for WakeUpDevice.
         :type request: :class:`tencentcloud.iotvideo.v20211125.models.WakeUpDeviceRequest`
@@ -2204,8 +2204,8 @@
             model = models.WakeUpDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20211125/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20211125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,1831 +13,1560 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.abstract_client import AbstractClient
-from tencentcloud.iotvideo.v20201215 import models
+from tencentcloud.iotvideo.v20191126 import models
 
 
 class IotvideoClient(AbstractClient):
-    _apiVersion = '2020-12-15'
+    _apiVersion = '2019-11-26'
     _endpoint = 'iotvideo.tencentcloudapi.com'
     _service = 'iotvideo'
 
 
-    def ApplyAIModel(self, request):
-        """申请AI模型
+    def ClearDeviceActiveCode(self, request):
+        """清除设备激活码
 
-        :param request: Request instance for ApplyAIModel.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ApplyAIModelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ApplyAIModelResponse`
+        :param request: Request instance for ClearDeviceActiveCode.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ClearDeviceActiveCodeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ClearDeviceActiveCodeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ApplyAIModel", params, headers=headers)
+            body = self.call("ClearDeviceActiveCode", params, headers=headers)
             response = json.loads(body)
-            model = models.ApplyAIModelResponse()
+            model = models.ClearDeviceActiveCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def BatchUpdateFirmware(self, request):
-        """本接口（BatchUpdateFirmware）用于批量更新设备固件
+    def CreateAnonymousAccessToken(self, request):
+        """创建匿名访问Token
 
-        :param request: Request instance for BatchUpdateFirmware.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.BatchUpdateFirmwareRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.BatchUpdateFirmwareResponse`
+        :param request: Request instance for CreateAnonymousAccessToken.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateAnonymousAccessTokenRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateAnonymousAccessTokenResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("BatchUpdateFirmware", params, headers=headers)
+            body = self.call("CreateAnonymousAccessToken", params, headers=headers)
             response = json.loads(body)
-            model = models.BatchUpdateFirmwareResponse()
+            model = models.CreateAnonymousAccessTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def BindCloudStorageUser(self, request):
-        """绑定云存用户
+    def CreateAppUsr(self, request):
+        """本接口（CreateAppUsr）用于接收由厂商云发送过来的注册请求,建立厂商云终端用户与IoT Video终端用户的映射关系。
 
-        :param request: Request instance for BindCloudStorageUser.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.BindCloudStorageUserRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.BindCloudStorageUserResponse`
+        :param request: Request instance for CreateAppUsr.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateAppUsrRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateAppUsrResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("BindCloudStorageUser", params, headers=headers)
+            body = self.call("CreateAppUsr", params, headers=headers)
             response = json.loads(body)
-            model = models.BindCloudStorageUserResponse()
+            model = models.CreateAppUsrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CancelAIModelApplication(self, request):
-        """取消AI模型申请
+    def CreateBinding(self, request):
+        """本接口（CreateBinding）用于终端用户和设备进行绑定，具体的应用场景如下：
+            终端用户与设备具有“强关联”关系。用户与设备绑定之后，用户终端即具备了该设备的访问权限,访问或操作设备时，无需获取设备访问Token。
 
-        :param request: Request instance for CancelAIModelApplication.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CancelAIModelApplicationRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CancelAIModelApplicationResponse`
+        :param request: Request instance for CreateBinding.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateBindingRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateBindingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CancelAIModelApplication", params, headers=headers)
+            body = self.call("CreateBinding", params, headers=headers)
             response = json.loads(body)
-            model = models.CancelAIModelApplicationResponse()
+            model = models.CreateBindingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CancelDeviceFirmwareTask(self, request):
-        """本接口用于取消设备升级任务
+    def CreateDevToken(self, request):
+        """本接口（CreateDevToken）用于以下场景：
+        终端用户与设备没有强绑定关联关系;
+        允许终端用户短时或一次性临时访问设备;
+        当终端用户与设备有强绑定关系时，可以不用调用此接口
 
-        :param request: Request instance for CancelDeviceFirmwareTask.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CancelDeviceFirmwareTaskRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CancelDeviceFirmwareTaskResponse`
+        :param request: Request instance for CreateDevToken.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevTokenRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevTokenResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CancelDeviceFirmwareTask", params, headers=headers)
+            body = self.call("CreateDevToken", params, headers=headers)
             response = json.loads(body)
-            model = models.CancelDeviceFirmwareTaskResponse()
+            model = models.CreateDevTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CheckForwardAuth(self, request):
-        """判断是否开启转发的权限
+    def CreateDevices(self, request):
+        """本接口（CreateDevices）用于批量创建新的物联网视频通信设备。
+        注意：腾讯云不会对设备私钥进行保存，请自行保管好您的设备私钥。
 
-        :param request: Request instance for CheckForwardAuth.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CheckForwardAuthRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CheckForwardAuthResponse`
+        :param request: Request instance for CreateDevices.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevicesRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevicesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CheckForwardAuth", params, headers=headers)
+            body = self.call("CreateDevices", params, headers=headers)
             response = json.loads(body)
-            model = models.CheckForwardAuthResponse()
+            model = models.CreateDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ControlDeviceData(self, request):
-        """根据设备产品ID、设备名称，设置控制设备的属性数据。
+    def CreateGencode(self, request):
+        """本接口（CreateGencode）用于生成设备物模型源代码
 
-        :param request: Request instance for ControlDeviceData.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ControlDeviceDataRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ControlDeviceDataResponse`
+        :param request: Request instance for CreateGencode.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateGencodeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateGencodeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ControlDeviceData", params, headers=headers)
+            body = self.call("CreateGencode", params, headers=headers)
             response = json.loads(body)
-            model = models.ControlDeviceDataResponse()
+            model = models.CreateGencodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateAIDetection(self, request):
-        """发起AI推理请求
+    def CreateIotDataType(self, request):
+        """本接口（CreateIotDataType）用于创建自定义物模型数据类型。
 
-        :param request: Request instance for CreateAIDetection.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateAIDetectionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateAIDetectionResponse`
+        :param request: Request instance for CreateIotDataType.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotDataTypeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotDataTypeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateAIDetection", params, headers=headers)
+            body = self.call("CreateIotDataType", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateAIDetectionResponse()
+            model = models.CreateIotDataTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateBatch(self, request):
-        """创建批次
+    def CreateIotModel(self, request):
+        """本接口（CreateIotModel）用于定义的物模型提交。
+        该接口实现了物模型草稿箱的功能，保存用户最后一次编辑的物模型数据。
 
-        :param request: Request instance for CreateBatch.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateBatchRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateBatchResponse`
+        :param request: Request instance for CreateIotModel.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotModelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotModelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateBatch", params, headers=headers)
+            body = self.call("CreateIotModel", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateBatchResponse()
+            model = models.CreateIotModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateCOSCredentials(self, request):
-        """创建COS上传密钥
-
-        :param request: Request instance for CreateCOSCredentials.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateCOSCredentialsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateCOSCredentialsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateCOSCredentials", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateCOSCredentialsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateCloudStorage(self, request):
-        """开通云存服务
-
-        :param request: Request instance for CreateCloudStorage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateCloudStorageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateCloudStorageResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateCloudStorage", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateCloudStorageResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateDataForward(self, request):
-        """创建数据转发
-
-        :param request: Request instance for CreateDataForward.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateDataForwardRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateDataForwardResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateDataForward", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateDataForwardResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateForwardRule(self, request):
-        """创建转发规则
-
-        :param request: Request instance for CreateForwardRule.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateForwardRuleRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateForwardRuleResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateForwardRule", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateForwardRuleResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
-        """创建产品
+        """本接口（CreateProduct）用于创建一个新的物联网智能视频产品。
 
         :param request: Request instance for CreateProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateProductResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateProduct", params, headers=headers)
             response = json.loads(body)
             model = models.CreateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def CreateTaskFileUrl(self, request):
-        """本接口（CreateTaskFileUrl）用于获取产品级任务文件上传链接
-
-        :param request: Request instance for CreateTaskFileUrl.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateTaskFileUrlRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateTaskFileUrlResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateTaskFileUrl", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateTaskFileUrlResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DeleteDevice(self, request):
-        """删除设备
-
-        :param request: Request instance for DeleteDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteDeviceResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeleteDevice", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeleteDeviceResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DeleteFirmware(self, request):
-        """本接口（DeleteFirmware）用于删除固件
-
-        :param request: Request instance for DeleteFirmware.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteFirmwareRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteFirmwareResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeleteFirmware", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeleteFirmwareResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DeleteForwardRule(self, request):
-        """删除转发规则
-
-        :param request: Request instance for DeleteForwardRule.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteForwardRuleRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteForwardRuleResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeleteForwardRule", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeleteForwardRuleResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteProduct(self, request):
-        """删除产品
+    def CreateStorage(self, request):
+        """该接口已经停止维护，请勿使用
 
-        :param request: Request instance for DeleteProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteProductResponse`
+        :param request: Request instance for CreateStorage.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteProduct", params, headers=headers)
+            body = self.call("CreateStorage", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteProductResponse()
+            model = models.CreateStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeAIModelApplications(self, request):
-        """用户AI模型申请记录
+    def CreateStorageService(self, request):
+        """购买云存服务
 
-        :param request: Request instance for DescribeAIModelApplications.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelApplicationsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelApplicationsResponse`
+        :param request: Request instance for CreateStorageService.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageServiceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageServiceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAIModelApplications", params, headers=headers)
+            body = self.call("CreateStorageService", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAIModelApplicationsResponse()
+            model = models.CreateStorageServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeAIModelChannel(self, request):
-        """查看AI推理结果推送配置
+    def CreateTraceIds(self, request):
+        """本接口（CreateTraceIds）用于将设备加到日志跟踪白名单。
 
-        :param request: Request instance for DescribeAIModelChannel.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelChannelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelChannelResponse`
+        :param request: Request instance for CreateTraceIds.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateTraceIdsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateTraceIdsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAIModelChannel", params, headers=headers)
+            body = self.call("CreateTraceIds", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAIModelChannelResponse()
+            model = models.CreateTraceIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeAIModelUsage(self, request):
-        """查看AI模型资源包
+    def CreateUploadPath(self, request):
+        """本接口（CreateUploadPath）用于获取固件上传路径。
 
-        :param request: Request instance for DescribeAIModelUsage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelUsageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelUsageResponse`
+        :param request: Request instance for CreateUploadPath.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateUploadPathRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateUploadPathResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAIModelUsage", params, headers=headers)
+            body = self.call("CreateUploadPath", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAIModelUsageResponse()
+            model = models.CreateUploadPathResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeAIModels(self, request):
-        """拉取AI模型列表
+    def CreateUsrToken(self, request):
+        """本接口（CreateUsrToken）用于终端用户获取IoT Video平台的accessToken，初始化SDK,连接到IoT Video接入服务器。
 
-        :param request: Request instance for DescribeAIModels.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelsResponse`
+        :param request: Request instance for CreateUsrToken.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateUsrTokenRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateUsrTokenResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAIModels", params, headers=headers)
+            body = self.call("CreateUsrToken", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAIModelsResponse()
+            model = models.CreateUsrTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBalance(self, request):
-        """查询账户余额
+    def DeleteAppUsr(self, request):
+        """本接口（DeleteAppUsr）用于删除终端用户。
 
-        :param request: Request instance for DescribeBalance.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceResponse`
+        :param request: Request instance for DeleteAppUsr.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteAppUsrRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteAppUsrResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBalance", params, headers=headers)
+            body = self.call("DeleteAppUsr", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBalanceResponse()
+            model = models.DeleteAppUsrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBalanceTransactions(self, request):
-        """拉取账户流水
+    def DeleteBinding(self, request):
+        """本接口（DeleteBinding）用于终端用户和设备进行解绑定。
 
-        :param request: Request instance for DescribeBalanceTransactions.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceTransactionsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceTransactionsResponse`
+        :param request: Request instance for DeleteBinding.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteBindingRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteBindingResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBalanceTransactions", params, headers=headers)
+            body = self.call("DeleteBinding", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBalanceTransactionsResponse()
+            model = models.DeleteBindingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBatch(self, request):
-        """获取批次详情
+    def DeleteDevice(self, request):
+        """本接口（DeleteDevice）用于删除设备，可进行批量操作，每次操作最多100台设备。
 
-        :param request: Request instance for DescribeBatch.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchResponse`
+        :param request: Request instance for DeleteDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBatch", params, headers=headers)
+            body = self.call("DeleteDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBatchResponse()
+            model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBatchs(self, request):
-        """获取批次列表
+    def DeleteIotDataType(self, request):
+        """本接口（DeleteIotDataType）用于删除自定义物模型数据类型。
 
-        :param request: Request instance for DescribeBatchs.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchsResponse`
+        :param request: Request instance for DeleteIotDataType.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteIotDataTypeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteIotDataTypeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBatchs", params, headers=headers)
+            body = self.call("DeleteIotDataType", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBatchsResponse()
+            model = models.DeleteIotDataTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCategory(self, request):
-        """获取Category详情
+    def DeleteMessageQueue(self, request):
+        """本接口（DeleteMessageQueue）用于删除物联网智能视频产品的转发消息配置信息。
 
-        :param request: Request instance for DescribeCategory.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCategoryRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCategoryResponse`
+        :param request: Request instance for DeleteMessageQueue.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteMessageQueueRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteMessageQueueResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCategory", params, headers=headers)
+            body = self.call("DeleteMessageQueue", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCategoryResponse()
+            model = models.DeleteMessageQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorage(self, request):
-        """获取设备云存服务详情
+    def DeleteOtaVersion(self, request):
+        """本接口（DeleteOtaVersion）用于删除固件版本信息。
 
-        :param request: Request instance for DescribeCloudStorage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageResponse`
+        :param request: Request instance for DeleteOtaVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteOtaVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteOtaVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorage", params, headers=headers)
+            body = self.call("DeleteOtaVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageResponse()
+            model = models.DeleteOtaVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorageDate(self, request):
-        """获取具有云存的日期
+    def DeleteProduct(self, request):
+        """本接口（DeleteProduct）用于删除一个物联网智能视频产品。
 
-        :param request: Request instance for DescribeCloudStorageDate.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageDateRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageDateResponse`
+        :param request: Request instance for DeleteProduct.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorageDate", params, headers=headers)
+            body = self.call("DeleteProduct", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageDateResponse()
+            model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorageEvents(self, request):
-        """拉取云存事件列表
+    def DeleteTraceIds(self, request):
+        """本接口（DeleteTraceIds）用于将设备从日志跟踪白名单中删除，该接口可批量操作，最多支持同时操作100台设备。
 
-        :param request: Request instance for DescribeCloudStorageEvents.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageEventsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageEventsResponse`
+        :param request: Request instance for DeleteTraceIds.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteTraceIdsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteTraceIdsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorageEvents", params, headers=headers)
+            body = self.call("DeleteTraceIds", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageEventsResponse()
+            model = models.DeleteTraceIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorageThumbnail(self, request):
-        """拉取云存事件缩略图
+    def DeliverStorageService(self, request):
+        """将已购买的云存服务转移到另一设备
 
-        :param request: Request instance for DescribeCloudStorageThumbnail.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageThumbnailRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageThumbnailResponse`
+        :param request: Request instance for DeliverStorageService.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeliverStorageServiceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeliverStorageServiceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorageThumbnail", params, headers=headers)
+            body = self.call("DeliverStorageService", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageThumbnailResponse()
+            model = models.DeliverStorageServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorageTime(self, request):
-        """获取某一天云存时间轴
+    def DescribeAccountBalance(self, request):
+        """客户可通过本接口获取账户余额信息, 默认接口请求频率限制：1次/秒
 
-        :param request: Request instance for DescribeCloudStorageTime.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageTimeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageTimeResponse`
+        :param request: Request instance for DescribeAccountBalance.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeAccountBalanceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeAccountBalanceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorageTime", params, headers=headers)
+            body = self.call("DescribeAccountBalance", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageTimeResponse()
+            model = models.DescribeAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeCloudStorageUsers(self, request):
-        """拉取云存用户列表
+    def DescribeBindDev(self, request):
+        """本接口（DescribeBindDev）用于查询终端用户绑定的设备列表。
 
-        :param request: Request instance for DescribeCloudStorageUsers.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageUsersRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageUsersResponse`
+        :param request: Request instance for DescribeBindDev.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindDevRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindDevResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeCloudStorageUsers", params, headers=headers)
+            body = self.call("DescribeBindDev", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeCloudStorageUsersResponse()
+            model = models.DescribeBindDevResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeDataForwardList(self, request):
-        """获取数据转发列表
+    def DescribeBindUsr(self, request):
+        """本接口（DescribeBindUsr）用于查询设备被分享的所有用户列表。
 
-        :param request: Request instance for DescribeDataForwardList.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDataForwardListRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDataForwardListResponse`
+        :param request: Request instance for DescribeBindUsr.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindUsrRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindUsrResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDataForwardList", params, headers=headers)
+            body = self.call("DescribeBindUsr", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDataForwardListResponse()
+            model = models.DescribeBindUsrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
-        """查看设备详情
+        """本接口（DescribeDevice）获取设备信息。
 
         :param request: Request instance for DescribeDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDevice", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDeviceActionHistory(self, request):
-        """为用户提供获取动作历史的能力。
-
-        :param request: Request instance for DescribeDeviceActionHistory.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceActionHistoryRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceActionHistoryResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDeviceActionHistory", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDeviceActionHistoryResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDeviceCommLog(self, request):
-        """获取设备在指定时间范围内的通讯日志
-
-        :param request: Request instance for DescribeDeviceCommLog.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceCommLogRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceCommLogResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDeviceCommLog", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDeviceCommLogResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDeviceData(self, request):
-        """获取设备属性数据
-
-        :param request: Request instance for DescribeDeviceData.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDeviceData", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDeviceDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeDeviceDataHistory(self, request):
-        """获取设备在指定时间范围内上报的历史数据。
+    def DescribeDeviceModel(self, request):
+        """本接口（DescribeDeviceModel）用于获取设备物模型。
 
-        :param request: Request instance for DescribeDeviceDataHistory.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataHistoryRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataHistoryResponse`
+        :param request: Request instance for DescribeDeviceModel.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceModelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceModelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDeviceDataHistory", params, headers=headers)
+            body = self.call("DescribeDeviceModel", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDeviceDataHistoryResponse()
+            model = models.DescribeDeviceModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDeviceEventHistory(self, request):
-        """获取设备的历史事件
-
-        :param request: Request instance for DescribeDeviceEventHistory.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceEventHistoryRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceEventHistoryResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDeviceEventHistory", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDeviceEventHistoryResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeDeviceStatusLog(self, request):
-        """获取设备上下线日志
-
-        :param request: Request instance for DescribeDeviceStatusLog.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceStatusLogRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceStatusLogResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeDeviceStatusLog", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeDeviceStatusLogResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
-        """获取设备列表
+        """本接口（DescribeDevices）用于获取设备信息列表。
 
         :param request: Request instance for DescribeDevices.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDevicesRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDevicesResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDevicesRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDevicesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDevices", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmware(self, request):
-        """本接口（DescribeFirmware）用于查询固件信息
+    def DescribeIotDataType(self, request):
+        """本接口（DescribeIotDataType）用于查询自定义的物模型数据类型。
 
-        :param request: Request instance for DescribeFirmware.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareResponse`
+        :param request: Request instance for DescribeIotDataType.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotDataTypeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotDataTypeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmware", params, headers=headers)
+            body = self.call("DescribeIotDataType", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareResponse()
+            model = models.DescribeIotDataTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmwareTask(self, request):
-        """此接口查询固件升级任务详情
+    def DescribeIotModel(self, request):
+        """本接口（DescribeIotModel）用于获取物模型定义详情。
 
-        :param request: Request instance for DescribeFirmwareTask.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskResponse`
+        :param request: Request instance for DescribeIotModel.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmwareTask", params, headers=headers)
+            body = self.call("DescribeIotModel", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareTaskResponse()
+            model = models.DescribeIotModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmwareTaskDevices(self, request):
-        """本接口用于查询固件升级任务的设备列表
+    def DescribeIotModels(self, request):
+        """本接口（DescribeIotModels）用于列出物模型历史版本列表。
 
-        :param request: Request instance for DescribeFirmwareTaskDevices.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDevicesRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDevicesResponse`
+        :param request: Request instance for DescribeIotModels.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmwareTaskDevices", params, headers=headers)
+            body = self.call("DescribeIotModels", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareTaskDevicesResponse()
+            model = models.DescribeIotModelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmwareTaskDistribution(self, request):
-        """本接口用于查询固件升级任务状态分布
+    def DescribeLogs(self, request):
+        """本接口（DescribeLogs）用于查询设备日志列表。
+        设备日志最长保留时长为15天,超期自动清除。
 
-        :param request: Request instance for DescribeFirmwareTaskDistribution.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDistributionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDistributionResponse`
+        :param request: Request instance for DescribeLogs.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeLogsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeLogsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmwareTaskDistribution", params, headers=headers)
+            body = self.call("DescribeLogs", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareTaskDistributionResponse()
+            model = models.DescribeLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmwareTaskStatistics(self, request):
-        """本接口用于查询固件升级任务统计信息
+    def DescribeMessageQueue(self, request):
+        """本接口（DescribeMessageQueue）用于查询物联网智能视频产品转发消息配置。
 
-        :param request: Request instance for DescribeFirmwareTaskStatistics.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskStatisticsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskStatisticsResponse`
+        :param request: Request instance for DescribeMessageQueue.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeMessageQueueRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeMessageQueueResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmwareTaskStatistics", params, headers=headers)
+            body = self.call("DescribeMessageQueue", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareTaskStatisticsResponse()
+            model = models.DescribeMessageQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeFirmwareTasks(self, request):
-        """本接口用于查询固件升级任务列表
+    def DescribeModelDataRet(self, request):
+        """本接口（DescribeModelDataRet）用于根据TaskId获取对设备物模型操作最终响应的结果。
 
-        :param request: Request instance for DescribeFirmwareTasks.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTasksRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTasksResponse`
+        :param request: Request instance for DescribeModelDataRet.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeModelDataRetRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeModelDataRetResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeFirmwareTasks", params, headers=headers)
+            body = self.call("DescribeModelDataRet", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeFirmwareTasksResponse()
+            model = models.DescribeModelDataRetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeForwardRule(self, request):
-        """获取产品转发规则
+    def DescribeOsList(self, request):
+        """查看操作系统支持的芯片列表
 
-        :param request: Request instance for DescribeForwardRule.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeForwardRuleRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeForwardRuleResponse`
+        :param request: Request instance for DescribeOsList.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOsListRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOsListResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeForwardRule", params, headers=headers)
+            body = self.call("DescribeOsList", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeForwardRuleResponse()
+            model = models.DescribeOsListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeModelDefinition(self, request):
-        """查询产品配置的数据模板信息
+    def DescribeOtaVersions(self, request):
+        """本接口（DescribeOtaVersions）用于查询固件版本信息列表。
 
-        :param request: Request instance for DescribeModelDefinition.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeModelDefinitionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeModelDefinitionResponse`
+        :param request: Request instance for DescribeOtaVersions.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOtaVersionsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOtaVersionsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeModelDefinition", params, headers=headers)
+            body = self.call("DescribeOtaVersions", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeModelDefinitionResponse()
+            model = models.DescribeOtaVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProduct(self, request):
-        """获取产品详情
+        """本接口（DescribeProduct）用于获取单个产品的详细信息。
 
         :param request: Request instance for DescribeProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeProduct", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeProductDynamicRegister(self, request):
-        """获取产品动态注册详情
+    def DescribeProducts(self, request):
+        """本接口（DescribeProducts）用于列出用户账号下的物联网智能视频产品列表。
 
-        :param request: Request instance for DescribeProductDynamicRegister.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductDynamicRegisterRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductDynamicRegisterResponse`
+        :param request: Request instance for DescribeProducts.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeProductDynamicRegister", params, headers=headers)
+            body = self.call("DescribeProducts", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeProductDynamicRegisterResponse()
+            model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeProducts(self, request):
-        """获取产品列表
+    def DescribePubVersions(self, request):
+        """本接口（DescribePubVersions）用于获取某一产品发布过的全部固件版本。
 
-        :param request: Request instance for DescribeProducts.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductsResponse`
+        :param request: Request instance for DescribePubVersions.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribePubVersionsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribePubVersionsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeProducts", params, headers=headers)
+            body = self.call("DescribePubVersions", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeProductsResponse()
+            model = models.DescribePubVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeSDKLog(self, request):
-        """获取设备sdk日志
+    def DescribeRechargeRecords(self, request):
+        """客户可通过本接口获取充值记录信息, 一次最多返回50条记录。
 
-        :param request: Request instance for DescribeSDKLog.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeSDKLogRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeSDKLogResponse`
+        :param request: Request instance for DescribeRechargeRecords.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRechargeRecordsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRechargeRecordsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeSDKLog", params, headers=headers)
+            body = self.call("DescribeRechargeRecords", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeSDKLogResponse()
+            model = models.DescribeRechargeRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def EditFirmware(self, request):
-        """本接口用于编辑固件信息
+    def DescribeRegistrationStatus(self, request):
+        """本接口（DescribeRegistrationStatus）用于查询终端用户的注册状态。
 
-        :param request: Request instance for EditFirmware.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.EditFirmwareRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.EditFirmwareResponse`
+        :param request: Request instance for DescribeRegistrationStatus.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRegistrationStatusRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRegistrationStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("EditFirmware", params, headers=headers)
+            body = self.call("DescribeRegistrationStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.EditFirmwareResponse()
+            model = models.DescribeRegistrationStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def GenerateSignedVideoURL(self, request):
-        """获取视频防盗链播放URL
+    def DescribeRunLog(self, request):
+        """本接口（DescribeRunLog）用于获取设备运行日志。
 
-        :param request: Request instance for GenerateSignedVideoURL.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GenerateSignedVideoURLRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GenerateSignedVideoURLResponse`
+        :param request: Request instance for DescribeRunLog.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRunLogRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRunLogResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("GenerateSignedVideoURL", params, headers=headers)
+            body = self.call("DescribeRunLog", params, headers=headers)
             response = json.loads(body)
-            model = models.GenerateSignedVideoURLResponse()
+            model = models.DescribeRunLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def GetAllFirmwareVersion(self, request):
-        """本接口（GetAllFirmwareVersion）用于获取所有的版本列表
+    def DescribeStorageService(self, request):
+        """查询云存服务
 
-        :param request: Request instance for GetAllFirmwareVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GetAllFirmwareVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GetAllFirmwareVersionResponse`
+        :param request: Request instance for DescribeStorageService.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStorageServiceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStorageServiceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("GetAllFirmwareVersion", params, headers=headers)
+            body = self.call("DescribeStorageService", params, headers=headers)
             response = json.loads(body)
-            model = models.GetAllFirmwareVersionResponse()
+            model = models.DescribeStorageServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def GetFirmwareURL(self, request):
-        """本接口（GetFirmwareURL）用于获取固件存储的URL
+    def DescribeStream(self, request):
+        """请求设备直播流地址
 
-        :param request: Request instance for GetFirmwareURL.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GetFirmwareURLRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GetFirmwareURLResponse`
+        :param request: Request instance for DescribeStream.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStreamRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStreamResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("GetFirmwareURL", params, headers=headers)
+            body = self.call("DescribeStream", params, headers=headers)
             response = json.loads(body)
-            model = models.GetFirmwareURLResponse()
+            model = models.DescribeStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ImportModelDefinition(self, request):
-        """导入其它产品的数据模板，覆盖现有数据模板的物模型和产品分类信息
+    def DescribeTraceIds(self, request):
+        """本接口（DescribeTraceIds）用于查询设备日志跟踪白名单。
 
-        :param request: Request instance for ImportModelDefinition.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ImportModelDefinitionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ImportModelDefinitionResponse`
+        :param request: Request instance for DescribeTraceIds.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceIdsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceIdsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ImportModelDefinition", params, headers=headers)
+            body = self.call("DescribeTraceIds", params, headers=headers)
             response = json.loads(body)
-            model = models.ImportModelDefinitionResponse()
+            model = models.DescribeTraceIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def InheritCloudStorageUser(self, request):
-        """继承云存用户
+    def DescribeTraceStatus(self, request):
+        """本接口（DescribeTraceStatus）用于查询指定设备是否在白名单中。
 
-        :param request: Request instance for InheritCloudStorageUser.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.InheritCloudStorageUserRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.InheritCloudStorageUserResponse`
+        :param request: Request instance for DescribeTraceStatus.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceStatusRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("InheritCloudStorageUser", params, headers=headers)
+            body = self.call("DescribeTraceStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.InheritCloudStorageUserResponse()
+            model = models.DescribeTraceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ListFirmwares(self, request):
-        """本接口（ListFirmwares）用于获取固件列表
+    def DisableDevice(self, request):
+        """本接口（DisableDevice）用于禁用设备，可进行批量操作，每次操作最多100台设备。
 
-        :param request: Request instance for ListFirmwares.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ListFirmwaresRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ListFirmwaresResponse`
+        :param request: Request instance for DisableDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ListFirmwares", params, headers=headers)
+            body = self.call("DisableDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.ListFirmwaresResponse()
+            model = models.DisableDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyDataForward(self, request):
-        """修改数据转发
+    def DisableDeviceStream(self, request):
+        """本接口（DisableDeviceStream）用于停止设备推流，可进行批量操作，每次操作最多100台设备。
 
-        :param request: Request instance for ModifyDataForward.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardResponse`
+        :param request: Request instance for DisableDeviceStream.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceStreamRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceStreamResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDataForward", params, headers=headers)
+            body = self.call("DisableDeviceStream", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDataForwardResponse()
+            model = models.DisableDeviceStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyDataForwardStatus(self, request):
-        """设置数据转发状态
+    def DisableOtaVersion(self, request):
+        """本接口（DisableOtaVersion）用于禁用固件版本。
 
-        :param request: Request instance for ModifyDataForwardStatus.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardStatusRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardStatusResponse`
+        :param request: Request instance for DisableOtaVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableOtaVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableOtaVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDataForwardStatus", params, headers=headers)
+            body = self.call("DisableOtaVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDataForwardStatusResponse()
+            model = models.DisableOtaVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDevice(self, request):
         """修改设备信息
 
         :param request: Request instance for ModifyDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyDevice", params, headers=headers)
             response = json.loads(body)
             model = models.ModifyDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
 
+    def ModifyDeviceAction(self, request):
+        """本接口（ModifyDeviceAction）用于修改设备物模型的行为（Action）。
 
-    def ModifyDeviceLogLevel(self, request):
-        """更新设备日志级别
+        可对ctlVal数据属性进行写入,如:Action.takePhoto.ctlVal,设备在线且成功发送到设备才返回,物模型写入数据时,不需要传入时标信息,平台以当前时标作为数据的时标更新物模型中的时标信息。
+        注意:
+          1.若设备当前不在线,会直接返回错误
+          2.若设备网络出现异常时,消息发送可能超时,超时等待最长时间为3秒
+          3.value的内容必须与实际物模型的定义一致
 
-        :param request: Request instance for ModifyDeviceLogLevel.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceLogLevelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceLogLevelResponse`
+        :param request: Request instance for ModifyDeviceAction.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceActionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceActionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDeviceLogLevel", params, headers=headers)
+            body = self.call("ModifyDeviceAction", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDeviceLogLevelResponse()
+            model = models.ModifyDeviceActionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyForwardRule(self, request):
-        """修改转发规则
+    def ModifyDeviceProperty(self, request):
+        """本接口（ModifyDeviceProperty）用于修改设备物模型的属性（ProWritable）。
+        可对setVal数据属性进行写入,如:
+        ProWritable.Pos.setVal
+        对于嵌套类型的可写属性，可以仅对其部分数据内容进行写入，如:
+        ProWritable.Pos.setVal.x;
+        可写属性云端写入成功即返回;云端向设备端发布属性变更参数;若当前设备不在线,在设备下次上线时会自动更新这些属性参数;
+        物模型写入数据时,不需要传入时标信息,平台以当前时标作为数据的时标更新物模型中的时标信息。
 
-        :param request: Request instance for ModifyForwardRule.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyForwardRuleRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyForwardRuleResponse`
+        :param request: Request instance for ModifyDeviceProperty.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDevicePropertyRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDevicePropertyResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyForwardRule", params, headers=headers)
+            body = self.call("ModifyDeviceProperty", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyForwardRuleResponse()
+            model = models.ModifyDevicePropertyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyModelDefinition(self, request):
-        """提供修改产品的数据模板的能力
+    def ModifyProduct(self, request):
+        """本接口（ModifyProduct）用于编辑物联网智能视频产品的相关信息。
 
-        :param request: Request instance for ModifyModelDefinition.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyModelDefinitionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyModelDefinitionResponse`
+        :param request: Request instance for ModifyProduct.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyModelDefinition", params, headers=headers)
+            body = self.call("ModifyProduct", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyModelDefinitionResponse()
+            model = models.ModifyProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyProduct(self, request):
-        """修改产品信息
+    def ModifyVerContent(self, request):
+        """编辑版本描述信息
 
-        :param request: Request instance for ModifyProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductResponse`
+        :param request: Request instance for ModifyVerContent.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyVerContentRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyVerContentResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyProduct", params, headers=headers)
+            body = self.call("ModifyVerContent", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyProductResponse()
+            model = models.ModifyVerContentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyProductDynamicRegister(self, request):
-        """修改产品动态注册
+    def RefundStorageService(self, request):
+        """本接口（RefundStorageService）用于退订已购买的云存服务。
+        退订时，云存服务对应订单的处理方式 :
+        1. 未开始的订单自动回到已付费订单池
+        2. 已开始的订单自动失效
+        3. 购买云存接口,优先从已付费订单池中分配订单
 
-        :param request: Request instance for ModifyProductDynamicRegister.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductDynamicRegisterRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductDynamicRegisterResponse`
+        :param request: Request instance for RefundStorageService.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RefundStorageServiceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RefundStorageServiceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyProductDynamicRegister", params, headers=headers)
+            body = self.call("RefundStorageService", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyProductDynamicRegisterResponse()
+            model = models.RefundStorageServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def PublishMessage(self, request):
-        """本接口（PublishMessage）用于使用自定义透传协议进行设备远控
+    def RunDevice(self, request):
+        """本接口（RunDevice）用于启用设备，可进行批量操作，每次操作最多100台设备。
 
-        :param request: Request instance for PublishMessage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.PublishMessageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.PublishMessageResponse`
+        :param request: Request instance for RunDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("PublishMessage", params, headers=headers)
+            body = self.call("RunDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.PublishMessageResponse()
+            model = models.RunDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ReportAliveDevice(self, request):
-        """上报活跃设备
+    def RunDeviceStream(self, request):
+        """本接口（RunDeviceStream）用于开启设备推流，可进行批量操作，每次操作最多100台设备。
 
-        :param request: Request instance for ReportAliveDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ReportAliveDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ReportAliveDeviceResponse`
+        :param request: Request instance for RunDeviceStream.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceStreamRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceStreamResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ReportAliveDevice", params, headers=headers)
+            body = self.call("RunDeviceStream", params, headers=headers)
             response = json.loads(body)
-            model = models.ReportAliveDeviceResponse()
+            model = models.RunDeviceStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ResetCloudStorage(self, request):
-        """重置云存服务
+    def RunIotModel(self, request):
+        """本接口（RunIotModel）用于对定义的物模型进行发布。
 
-        :param request: Request instance for ResetCloudStorage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ResetCloudStorageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ResetCloudStorageResponse`
+        :param request: Request instance for RunIotModel.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunIotModelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunIotModelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ResetCloudStorage", params, headers=headers)
+            body = self.call("RunIotModel", params, headers=headers)
             response = json.loads(body)
-            model = models.ResetCloudStorageResponse()
+            model = models.RunIotModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RetryDeviceFirmwareTask(self, request):
-        """本接口用于重试设备升级任务
+    def RunOtaVersion(self, request):
+        """本接口（RunOtaVersion）用于固件版本正式发布。
 
-        :param request: Request instance for RetryDeviceFirmwareTask.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.RetryDeviceFirmwareTaskRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.RetryDeviceFirmwareTaskResponse`
+        :param request: Request instance for RunOtaVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunOtaVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunOtaVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RetryDeviceFirmwareTask", params, headers=headers)
+            body = self.call("RunOtaVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.RetryDeviceFirmwareTaskResponse()
+            model = models.RunOtaVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def SetForwardAuth(self, request):
-        """设置转发权限
+    def RunTestOtaVersion(self, request):
+        """本接口（RunTestOtaVersion）用于固件版本测试发布。
 
-        :param request: Request instance for SetForwardAuth.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.SetForwardAuthRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.SetForwardAuthResponse`
+        :param request: Request instance for RunTestOtaVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunTestOtaVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunTestOtaVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("SetForwardAuth", params, headers=headers)
+            body = self.call("RunTestOtaVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.SetForwardAuthResponse()
+            model = models.RunTestOtaVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def TransferCloudStorage(self, request):
-        """转移云存服务
+    def SendOnlineMsg(self, request):
+        """本接口（SendOnlineMsg）用于向设备发送在线消息。
+        注意：
+        若设备当前不在线,会直接返回错误;
+        若设备网络出现异常时,消息发送可能超时,超时等待最长时间为3秒.waitresp非0情况下,会导致本接口阻塞3秒。
 
-        :param request: Request instance for TransferCloudStorage.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.TransferCloudStorageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.TransferCloudStorageResponse`
+        :param request: Request instance for SendOnlineMsg.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.SendOnlineMsgRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.SendOnlineMsgResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("TransferCloudStorage", params, headers=headers)
+            body = self.call("SendOnlineMsg", params, headers=headers)
             response = json.loads(body)
-            model = models.TransferCloudStorageResponse()
+            model = models.SendOnlineMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def UpdateAIModelChannel(self, request):
-        """更新AI推理结果推送配置
+    def SetMessageQueue(self, request):
+        """本接口（SetMessageQueue）用于配置物联网智能视频产品的转发消息队列。
 
-        :param request: Request instance for UpdateAIModelChannel.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.UpdateAIModelChannelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.UpdateAIModelChannelResponse`
+        :param request: Request instance for SetMessageQueue.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.SetMessageQueueRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.SetMessageQueueResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("UpdateAIModelChannel", params, headers=headers)
+            body = self.call("SetMessageQueue", params, headers=headers)
             response = json.loads(body)
-            model = models.UpdateAIModelChannelResponse()
+            model = models.SetMessageQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def UploadFirmware(self, request):
-        """本接口（UploadFirmware）用于上传设备固件信息
+    def UpgradeDevice(self, request):
+        """本接口（UpgradeDevice）用于对设备进行固件升级。
+        该接口向指定的设备下发固件更新指令,可将固件升级到任意版本(可实现固件降级)。
+        警告:使能UpgradeNow参数存在一定的风险性！建议仅在debug场景下使用!
 
-        :param request: Request instance for UploadFirmware.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.UploadFirmwareRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.UploadFirmwareResponse`
+        :param request: Request instance for UpgradeDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.UpgradeDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.UpgradeDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("UploadFirmware", params, headers=headers)
+            body = self.call("UpgradeDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.UploadFirmwareResponse()
+            model = models.UpgradeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def WakeUpDevice(self, request):
-        """设备唤醒
+    def UploadOtaVersion(self, request):
+        """本接口（UploadOtaVersion）接收上传到控制台的固件版本信息。
 
-        :param request: Request instance for WakeUpDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20201215.models.WakeUpDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.WakeUpDeviceResponse`
+        :param request: Request instance for UploadOtaVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20191126.models.UploadOtaVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.UploadOtaVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("WakeUpDevice", params, headers=headers)
+            body = self.call("UploadOtaVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.WakeUpDeviceResponse()
+            model = models.UploadOtaVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20201215/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,1560 +13,1831 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.abstract_client import AbstractClient
-from tencentcloud.iotvideo.v20191126 import models
+from tencentcloud.iotvideo.v20201215 import models
 
 
 class IotvideoClient(AbstractClient):
-    _apiVersion = '2019-11-26'
+    _apiVersion = '2020-12-15'
     _endpoint = 'iotvideo.tencentcloudapi.com'
     _service = 'iotvideo'
 
 
-    def ClearDeviceActiveCode(self, request):
-        """清除设备激活码
+    def ApplyAIModel(self, request):
+        """申请AI模型
 
-        :param request: Request instance for ClearDeviceActiveCode.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ClearDeviceActiveCodeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ClearDeviceActiveCodeResponse`
+        :param request: Request instance for ApplyAIModel.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ApplyAIModelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ApplyAIModelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ClearDeviceActiveCode", params, headers=headers)
+            body = self.call("ApplyAIModel", params, headers=headers)
             response = json.loads(body)
-            model = models.ClearDeviceActiveCodeResponse()
+            model = models.ApplyAIModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateAnonymousAccessToken(self, request):
-        """创建匿名访问Token
+    def BatchUpdateFirmware(self, request):
+        """本接口（BatchUpdateFirmware）用于批量更新设备固件
 
-        :param request: Request instance for CreateAnonymousAccessToken.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateAnonymousAccessTokenRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateAnonymousAccessTokenResponse`
+        :param request: Request instance for BatchUpdateFirmware.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.BatchUpdateFirmwareRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.BatchUpdateFirmwareResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateAnonymousAccessToken", params, headers=headers)
+            body = self.call("BatchUpdateFirmware", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateAnonymousAccessTokenResponse()
+            model = models.BatchUpdateFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateAppUsr(self, request):
-        """本接口（CreateAppUsr）用于接收由厂商云发送过来的注册请求,建立厂商云终端用户与IoT Video终端用户的映射关系。
+    def BindCloudStorageUser(self, request):
+        """绑定云存用户
 
-        :param request: Request instance for CreateAppUsr.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateAppUsrRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateAppUsrResponse`
+        :param request: Request instance for BindCloudStorageUser.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.BindCloudStorageUserRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.BindCloudStorageUserResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateAppUsr", params, headers=headers)
+            body = self.call("BindCloudStorageUser", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateAppUsrResponse()
+            model = models.BindCloudStorageUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateBinding(self, request):
-        """本接口（CreateBinding）用于终端用户和设备进行绑定，具体的应用场景如下：
-            终端用户与设备具有“强关联”关系。用户与设备绑定之后，用户终端即具备了该设备的访问权限,访问或操作设备时，无需获取设备访问Token。
+    def CancelAIModelApplication(self, request):
+        """取消AI模型申请
 
-        :param request: Request instance for CreateBinding.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateBindingRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateBindingResponse`
+        :param request: Request instance for CancelAIModelApplication.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CancelAIModelApplicationRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CancelAIModelApplicationResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateBinding", params, headers=headers)
+            body = self.call("CancelAIModelApplication", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateBindingResponse()
+            model = models.CancelAIModelApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateDevToken(self, request):
-        """本接口（CreateDevToken）用于以下场景：
-        终端用户与设备没有强绑定关联关系;
-        允许终端用户短时或一次性临时访问设备;
-        当终端用户与设备有强绑定关系时，可以不用调用此接口
+    def CancelDeviceFirmwareTask(self, request):
+        """本接口用于取消设备升级任务
 
-        :param request: Request instance for CreateDevToken.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevTokenRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevTokenResponse`
+        :param request: Request instance for CancelDeviceFirmwareTask.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CancelDeviceFirmwareTaskRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CancelDeviceFirmwareTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateDevToken", params, headers=headers)
+            body = self.call("CancelDeviceFirmwareTask", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateDevTokenResponse()
+            model = models.CancelDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateDevices(self, request):
-        """本接口（CreateDevices）用于批量创建新的物联网视频通信设备。
-        注意：腾讯云不会对设备私钥进行保存，请自行保管好您的设备私钥。
+    def CheckForwardAuth(self, request):
+        """判断是否开启转发的权限
 
-        :param request: Request instance for CreateDevices.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevicesRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateDevicesResponse`
+        :param request: Request instance for CheckForwardAuth.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CheckForwardAuthRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CheckForwardAuthResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateDevices", params, headers=headers)
+            body = self.call("CheckForwardAuth", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateDevicesResponse()
+            model = models.CheckForwardAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateGencode(self, request):
-        """本接口（CreateGencode）用于生成设备物模型源代码
+    def ControlDeviceData(self, request):
+        """根据设备产品ID、设备名称，设置控制设备的属性数据。
 
-        :param request: Request instance for CreateGencode.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateGencodeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateGencodeResponse`
+        :param request: Request instance for ControlDeviceData.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ControlDeviceDataRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ControlDeviceDataResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateGencode", params, headers=headers)
+            body = self.call("ControlDeviceData", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateGencodeResponse()
+            model = models.ControlDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateIotDataType(self, request):
-        """本接口（CreateIotDataType）用于创建自定义物模型数据类型。
+    def CreateAIDetection(self, request):
+        """发起AI推理请求
 
-        :param request: Request instance for CreateIotDataType.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotDataTypeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotDataTypeResponse`
+        :param request: Request instance for CreateAIDetection.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateAIDetectionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateAIDetectionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateIotDataType", params, headers=headers)
+            body = self.call("CreateAIDetection", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateIotDataTypeResponse()
+            model = models.CreateAIDetectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateIotModel(self, request):
-        """本接口（CreateIotModel）用于定义的物模型提交。
-        该接口实现了物模型草稿箱的功能，保存用户最后一次编辑的物模型数据。
+    def CreateBatch(self, request):
+        """创建批次
 
-        :param request: Request instance for CreateIotModel.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotModelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateIotModelResponse`
+        :param request: Request instance for CreateBatch.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateBatchRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateBatchResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateIotModel", params, headers=headers)
+            body = self.call("CreateBatch", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateIotModelResponse()
+            model = models.CreateBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateCOSCredentials(self, request):
+        """创建COS上传密钥
+
+        :param request: Request instance for CreateCOSCredentials.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateCOSCredentialsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateCOSCredentialsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCOSCredentials", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCOSCredentialsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateCloudStorage(self, request):
+        """开通云存服务
+
+        :param request: Request instance for CreateCloudStorage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateCloudStorageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateCloudStorageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCloudStorage", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCloudStorageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateDataForward(self, request):
+        """创建数据转发
+
+        :param request: Request instance for CreateDataForward.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateDataForwardRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateDataForwardResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDataForward", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDataForwardResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateForwardRule(self, request):
+        """创建转发规则
+
+        :param request: Request instance for CreateForwardRule.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateForwardRuleRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateForwardRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateForwardRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateForwardRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
-        """本接口（CreateProduct）用于创建一个新的物联网智能视频产品。
+        """创建产品
 
         :param request: Request instance for CreateProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateProductResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("CreateProduct", params, headers=headers)
             response = json.loads(body)
             model = models.CreateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateStorage(self, request):
-        """该接口已经停止维护，请勿使用
+    def CreateTaskFileUrl(self, request):
+        """本接口（CreateTaskFileUrl）用于获取产品级任务文件上传链接
 
-        :param request: Request instance for CreateStorage.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageResponse`
+        :param request: Request instance for CreateTaskFileUrl.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.CreateTaskFileUrlRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.CreateTaskFileUrlResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateStorage", params, headers=headers)
+            body = self.call("CreateTaskFileUrl", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateStorageResponse()
+            model = models.CreateTaskFileUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateStorageService(self, request):
-        """购买云存服务
+    def DeleteDevice(self, request):
+        """删除设备
 
-        :param request: Request instance for CreateStorageService.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageServiceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateStorageServiceResponse`
+        :param request: Request instance for DeleteDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateStorageService", params, headers=headers)
+            body = self.call("DeleteDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateStorageServiceResponse()
+            model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateTraceIds(self, request):
-        """本接口（CreateTraceIds）用于将设备加到日志跟踪白名单。
+    def DeleteFirmware(self, request):
+        """本接口（DeleteFirmware）用于删除固件
 
-        :param request: Request instance for CreateTraceIds.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateTraceIdsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateTraceIdsResponse`
+        :param request: Request instance for DeleteFirmware.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteFirmwareRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteFirmwareResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateTraceIds", params, headers=headers)
+            body = self.call("DeleteFirmware", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateTraceIdsResponse()
+            model = models.DeleteFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateUploadPath(self, request):
-        """本接口（CreateUploadPath）用于获取固件上传路径。
+    def DeleteForwardRule(self, request):
+        """删除转发规则
 
-        :param request: Request instance for CreateUploadPath.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateUploadPathRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateUploadPathResponse`
+        :param request: Request instance for DeleteForwardRule.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteForwardRuleRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteForwardRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateUploadPath", params, headers=headers)
+            body = self.call("DeleteForwardRule", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateUploadPathResponse()
+            model = models.DeleteForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def CreateUsrToken(self, request):
-        """本接口（CreateUsrToken）用于终端用户获取IoT Video平台的accessToken，初始化SDK,连接到IoT Video接入服务器。
+    def DeleteProduct(self, request):
+        """删除产品
 
-        :param request: Request instance for CreateUsrToken.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.CreateUsrTokenRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.CreateUsrTokenResponse`
+        :param request: Request instance for DeleteProduct.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DeleteProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DeleteProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("CreateUsrToken", params, headers=headers)
+            body = self.call("DeleteProduct", params, headers=headers)
             response = json.loads(body)
-            model = models.CreateUsrTokenResponse()
+            model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteAppUsr(self, request):
-        """本接口（DeleteAppUsr）用于删除终端用户。
+    def DescribeAIModelApplications(self, request):
+        """用户AI模型申请记录
 
-        :param request: Request instance for DeleteAppUsr.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteAppUsrRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteAppUsrResponse`
+        :param request: Request instance for DescribeAIModelApplications.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelApplicationsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelApplicationsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteAppUsr", params, headers=headers)
+            body = self.call("DescribeAIModelApplications", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteAppUsrResponse()
+            model = models.DescribeAIModelApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteBinding(self, request):
-        """本接口（DeleteBinding）用于终端用户和设备进行解绑定。
+    def DescribeAIModelChannel(self, request):
+        """查看AI推理结果推送配置
 
-        :param request: Request instance for DeleteBinding.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteBindingRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteBindingResponse`
+        :param request: Request instance for DescribeAIModelChannel.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelChannelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelChannelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteBinding", params, headers=headers)
+            body = self.call("DescribeAIModelChannel", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteBindingResponse()
+            model = models.DescribeAIModelChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteDevice(self, request):
-        """本接口（DeleteDevice）用于删除设备，可进行批量操作，每次操作最多100台设备。
+    def DescribeAIModelUsage(self, request):
+        """查看AI模型资源包
 
-        :param request: Request instance for DeleteDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteDeviceResponse`
+        :param request: Request instance for DescribeAIModelUsage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelUsageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelUsageResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteDevice", params, headers=headers)
+            body = self.call("DescribeAIModelUsage", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteDeviceResponse()
+            model = models.DescribeAIModelUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteIotDataType(self, request):
-        """本接口（DeleteIotDataType）用于删除自定义物模型数据类型。
+    def DescribeAIModels(self, request):
+        """拉取AI模型列表
 
-        :param request: Request instance for DeleteIotDataType.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteIotDataTypeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteIotDataTypeResponse`
+        :param request: Request instance for DescribeAIModels.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeAIModelsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteIotDataType", params, headers=headers)
+            body = self.call("DescribeAIModels", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteIotDataTypeResponse()
+            model = models.DescribeAIModelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteMessageQueue(self, request):
-        """本接口（DeleteMessageQueue）用于删除物联网智能视频产品的转发消息配置信息。
+    def DescribeBalance(self, request):
+        """查询账户余额
 
-        :param request: Request instance for DeleteMessageQueue.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteMessageQueueRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteMessageQueueResponse`
+        :param request: Request instance for DescribeBalance.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteMessageQueue", params, headers=headers)
+            body = self.call("DescribeBalance", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteMessageQueueResponse()
+            model = models.DescribeBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteOtaVersion(self, request):
-        """本接口（DeleteOtaVersion）用于删除固件版本信息。
+    def DescribeBalanceTransactions(self, request):
+        """拉取账户流水
 
-        :param request: Request instance for DeleteOtaVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteOtaVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteOtaVersionResponse`
+        :param request: Request instance for DescribeBalanceTransactions.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceTransactionsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBalanceTransactionsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteOtaVersion", params, headers=headers)
+            body = self.call("DescribeBalanceTransactions", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteOtaVersionResponse()
+            model = models.DescribeBalanceTransactionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteProduct(self, request):
-        """本接口（DeleteProduct）用于删除一个物联网智能视频产品。
+    def DescribeBatch(self, request):
+        """获取批次详情
 
-        :param request: Request instance for DeleteProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteProductResponse`
+        :param request: Request instance for DescribeBatch.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteProduct", params, headers=headers)
+            body = self.call("DescribeBatch", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteProductResponse()
+            model = models.DescribeBatchResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeBatchs(self, request):
+        """获取批次列表
+
+        :param request: Request instance for DescribeBatchs.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeBatchsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBatchs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBatchsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeCategory(self, request):
+        """获取Category详情
+
+        :param request: Request instance for DescribeCategory.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCategoryRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCategoryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCategory", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCategoryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeCloudStorage(self, request):
+        """获取设备云存服务详情
+
+        :param request: Request instance for DescribeCloudStorage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCloudStorage", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeleteTraceIds(self, request):
-        """本接口（DeleteTraceIds）用于将设备从日志跟踪白名单中删除，该接口可批量操作，最多支持同时操作100台设备。
+    def DescribeCloudStorageDate(self, request):
+        """获取具有云存的日期
 
-        :param request: Request instance for DeleteTraceIds.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeleteTraceIdsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeleteTraceIdsResponse`
+        :param request: Request instance for DescribeCloudStorageDate.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageDateRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageDateResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeleteTraceIds", params, headers=headers)
+            body = self.call("DescribeCloudStorageDate", params, headers=headers)
             response = json.loads(body)
-            model = models.DeleteTraceIdsResponse()
+            model = models.DescribeCloudStorageDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DeliverStorageService(self, request):
-        """将已购买的云存服务转移到另一设备
+    def DescribeCloudStorageEvents(self, request):
+        """拉取云存事件列表
 
-        :param request: Request instance for DeliverStorageService.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DeliverStorageServiceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DeliverStorageServiceResponse`
+        :param request: Request instance for DescribeCloudStorageEvents.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageEventsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageEventsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DeliverStorageService", params, headers=headers)
+            body = self.call("DescribeCloudStorageEvents", params, headers=headers)
             response = json.loads(body)
-            model = models.DeliverStorageServiceResponse()
+            model = models.DescribeCloudStorageEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeAccountBalance(self, request):
-        """客户可通过本接口获取账户余额信息, 默认接口请求频率限制：1次/秒
+    def DescribeCloudStorageThumbnail(self, request):
+        """拉取云存事件缩略图
 
-        :param request: Request instance for DescribeAccountBalance.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeAccountBalanceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeAccountBalanceResponse`
+        :param request: Request instance for DescribeCloudStorageThumbnail.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageThumbnailRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageThumbnailResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeAccountBalance", params, headers=headers)
+            body = self.call("DescribeCloudStorageThumbnail", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeAccountBalanceResponse()
+            model = models.DescribeCloudStorageThumbnailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBindDev(self, request):
-        """本接口（DescribeBindDev）用于查询终端用户绑定的设备列表。
+    def DescribeCloudStorageTime(self, request):
+        """获取某一天云存时间轴
 
-        :param request: Request instance for DescribeBindDev.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindDevRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindDevResponse`
+        :param request: Request instance for DescribeCloudStorageTime.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageTimeRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageTimeResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBindDev", params, headers=headers)
+            body = self.call("DescribeCloudStorageTime", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBindDevResponse()
+            model = models.DescribeCloudStorageTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeBindUsr(self, request):
-        """本接口（DescribeBindUsr）用于查询设备被分享的所有用户列表。
+    def DescribeCloudStorageUsers(self, request):
+        """拉取云存用户列表
 
-        :param request: Request instance for DescribeBindUsr.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindUsrRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeBindUsrResponse`
+        :param request: Request instance for DescribeCloudStorageUsers.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageUsersRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeCloudStorageUsersResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeBindUsr", params, headers=headers)
+            body = self.call("DescribeCloudStorageUsers", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeBindUsrResponse()
+            model = models.DescribeCloudStorageUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDataForwardList(self, request):
+        """获取数据转发列表
+
+        :param request: Request instance for DescribeDataForwardList.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDataForwardListRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDataForwardListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDataForwardList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDataForwardListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
-        """本接口（DescribeDevice）获取设备信息。
+        """查看设备详情
 
         :param request: Request instance for DescribeDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDevice", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDeviceActionHistory(self, request):
+        """为用户提供获取动作历史的能力。
+
+        :param request: Request instance for DescribeDeviceActionHistory.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceActionHistoryRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceActionHistoryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDeviceActionHistory", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDeviceActionHistoryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDeviceCommLog(self, request):
+        """获取设备在指定时间范围内的通讯日志
+
+        :param request: Request instance for DescribeDeviceCommLog.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceCommLogRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceCommLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDeviceCommLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDeviceCommLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDeviceData(self, request):
+        """获取设备属性数据
+
+        :param request: Request instance for DescribeDeviceData.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDeviceData", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDeviceDataResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeDeviceModel(self, request):
-        """本接口（DescribeDeviceModel）用于获取设备物模型。
+    def DescribeDeviceDataHistory(self, request):
+        """获取设备在指定时间范围内上报的历史数据。
 
-        :param request: Request instance for DescribeDeviceModel.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceModelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDeviceModelResponse`
+        :param request: Request instance for DescribeDeviceDataHistory.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataHistoryRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceDataHistoryResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeDeviceModel", params, headers=headers)
+            body = self.call("DescribeDeviceDataHistory", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeDeviceModelResponse()
+            model = models.DescribeDeviceDataHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDeviceEventHistory(self, request):
+        """获取设备的历史事件
+
+        :param request: Request instance for DescribeDeviceEventHistory.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceEventHistoryRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceEventHistoryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDeviceEventHistory", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDeviceEventHistoryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDeviceStatusLog(self, request):
+        """获取设备上下线日志
+
+        :param request: Request instance for DescribeDeviceStatusLog.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceStatusLogRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDeviceStatusLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDeviceStatusLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDeviceStatusLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
-        """本接口（DescribeDevices）用于获取设备信息列表。
+        """获取设备列表
 
         :param request: Request instance for DescribeDevices.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDevicesRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeDevicesResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDevicesRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeDevicesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeDevices", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeIotDataType(self, request):
-        """本接口（DescribeIotDataType）用于查询自定义的物模型数据类型。
+    def DescribeFirmware(self, request):
+        """本接口（DescribeFirmware）用于查询固件信息
 
-        :param request: Request instance for DescribeIotDataType.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotDataTypeRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotDataTypeResponse`
+        :param request: Request instance for DescribeFirmware.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeIotDataType", params, headers=headers)
+            body = self.call("DescribeFirmware", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeIotDataTypeResponse()
+            model = models.DescribeFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeIotModel(self, request):
-        """本接口（DescribeIotModel）用于获取物模型定义详情。
+    def DescribeFirmwareTask(self, request):
+        """此接口查询固件升级任务详情
 
-        :param request: Request instance for DescribeIotModel.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelResponse`
+        :param request: Request instance for DescribeFirmwareTask.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeIotModel", params, headers=headers)
+            body = self.call("DescribeFirmwareTask", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeIotModelResponse()
+            model = models.DescribeFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeIotModels(self, request):
-        """本接口（DescribeIotModels）用于列出物模型历史版本列表。
+    def DescribeFirmwareTaskDevices(self, request):
+        """本接口用于查询固件升级任务的设备列表
 
-        :param request: Request instance for DescribeIotModels.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeIotModelsResponse`
+        :param request: Request instance for DescribeFirmwareTaskDevices.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDevicesRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDevicesResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeIotModels", params, headers=headers)
+            body = self.call("DescribeFirmwareTaskDevices", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeIotModelsResponse()
+            model = models.DescribeFirmwareTaskDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeLogs(self, request):
-        """本接口（DescribeLogs）用于查询设备日志列表。
-        设备日志最长保留时长为15天,超期自动清除。
+    def DescribeFirmwareTaskDistribution(self, request):
+        """本接口用于查询固件升级任务状态分布
 
-        :param request: Request instance for DescribeLogs.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeLogsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeLogsResponse`
+        :param request: Request instance for DescribeFirmwareTaskDistribution.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDistributionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskDistributionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeLogs", params, headers=headers)
+            body = self.call("DescribeFirmwareTaskDistribution", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeLogsResponse()
+            model = models.DescribeFirmwareTaskDistributionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeMessageQueue(self, request):
-        """本接口（DescribeMessageQueue）用于查询物联网智能视频产品转发消息配置。
+    def DescribeFirmwareTaskStatistics(self, request):
+        """本接口用于查询固件升级任务统计信息
 
-        :param request: Request instance for DescribeMessageQueue.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeMessageQueueRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeMessageQueueResponse`
+        :param request: Request instance for DescribeFirmwareTaskStatistics.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskStatisticsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTaskStatisticsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeMessageQueue", params, headers=headers)
+            body = self.call("DescribeFirmwareTaskStatistics", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeMessageQueueResponse()
+            model = models.DescribeFirmwareTaskStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeModelDataRet(self, request):
-        """本接口（DescribeModelDataRet）用于根据TaskId获取对设备物模型操作最终响应的结果。
+    def DescribeFirmwareTasks(self, request):
+        """本接口用于查询固件升级任务列表
 
-        :param request: Request instance for DescribeModelDataRet.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeModelDataRetRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeModelDataRetResponse`
+        :param request: Request instance for DescribeFirmwareTasks.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTasksRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeFirmwareTasksResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeModelDataRet", params, headers=headers)
+            body = self.call("DescribeFirmwareTasks", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeModelDataRetResponse()
+            model = models.DescribeFirmwareTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeOsList(self, request):
-        """查看操作系统支持的芯片列表
+    def DescribeForwardRule(self, request):
+        """获取产品转发规则
 
-        :param request: Request instance for DescribeOsList.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOsListRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOsListResponse`
+        :param request: Request instance for DescribeForwardRule.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeForwardRuleRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeForwardRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeOsList", params, headers=headers)
+            body = self.call("DescribeForwardRule", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeOsListResponse()
+            model = models.DescribeForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeOtaVersions(self, request):
-        """本接口（DescribeOtaVersions）用于查询固件版本信息列表。
+    def DescribeModelDefinition(self, request):
+        """查询产品配置的数据模板信息
 
-        :param request: Request instance for DescribeOtaVersions.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOtaVersionsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeOtaVersionsResponse`
+        :param request: Request instance for DescribeModelDefinition.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeModelDefinitionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeModelDefinitionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeOtaVersions", params, headers=headers)
+            body = self.call("DescribeModelDefinition", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeOtaVersionsResponse()
+            model = models.DescribeModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProduct(self, request):
-        """本接口（DescribeProduct）用于获取单个产品的详细信息。
+        """获取产品详情
 
         :param request: Request instance for DescribeProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("DescribeProduct", params, headers=headers)
             response = json.loads(body)
             model = models.DescribeProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeProducts(self, request):
-        """本接口（DescribeProducts）用于列出用户账号下的物联网智能视频产品列表。
+    def DescribeProductDynamicRegister(self, request):
+        """获取产品动态注册详情
 
-        :param request: Request instance for DescribeProducts.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeProductsResponse`
+        :param request: Request instance for DescribeProductDynamicRegister.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductDynamicRegisterRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductDynamicRegisterResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeProducts", params, headers=headers)
+            body = self.call("DescribeProductDynamicRegister", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeProductsResponse()
+            model = models.DescribeProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribePubVersions(self, request):
-        """本接口（DescribePubVersions）用于获取某一产品发布过的全部固件版本。
+    def DescribeProducts(self, request):
+        """获取产品列表
 
-        :param request: Request instance for DescribePubVersions.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribePubVersionsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribePubVersionsResponse`
+        :param request: Request instance for DescribeProducts.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductsRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeProductsResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribePubVersions", params, headers=headers)
+            body = self.call("DescribeProducts", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribePubVersionsResponse()
+            model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeRechargeRecords(self, request):
-        """客户可通过本接口获取充值记录信息, 一次最多返回50条记录。
+    def DescribeSDKLog(self, request):
+        """获取设备sdk日志
 
-        :param request: Request instance for DescribeRechargeRecords.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRechargeRecordsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRechargeRecordsResponse`
+        :param request: Request instance for DescribeSDKLog.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.DescribeSDKLogRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.DescribeSDKLogResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeRechargeRecords", params, headers=headers)
+            body = self.call("DescribeSDKLog", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeRechargeRecordsResponse()
+            model = models.DescribeSDKLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeRegistrationStatus(self, request):
-        """本接口（DescribeRegistrationStatus）用于查询终端用户的注册状态。
+    def EditFirmware(self, request):
+        """本接口用于编辑固件信息
 
-        :param request: Request instance for DescribeRegistrationStatus.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRegistrationStatusRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRegistrationStatusResponse`
+        :param request: Request instance for EditFirmware.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.EditFirmwareRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.EditFirmwareResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeRegistrationStatus", params, headers=headers)
+            body = self.call("EditFirmware", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeRegistrationStatusResponse()
+            model = models.EditFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeRunLog(self, request):
-        """本接口（DescribeRunLog）用于获取设备运行日志。
+    def GenerateSignedVideoURL(self, request):
+        """获取视频防盗链播放URL
 
-        :param request: Request instance for DescribeRunLog.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRunLogRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeRunLogResponse`
+        :param request: Request instance for GenerateSignedVideoURL.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GenerateSignedVideoURLRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GenerateSignedVideoURLResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeRunLog", params, headers=headers)
+            body = self.call("GenerateSignedVideoURL", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeRunLogResponse()
+            model = models.GenerateSignedVideoURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeStorageService(self, request):
-        """查询云存服务
+    def GetAllFirmwareVersion(self, request):
+        """本接口（GetAllFirmwareVersion）用于获取所有的版本列表
 
-        :param request: Request instance for DescribeStorageService.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStorageServiceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStorageServiceResponse`
+        :param request: Request instance for GetAllFirmwareVersion.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GetAllFirmwareVersionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GetAllFirmwareVersionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeStorageService", params, headers=headers)
+            body = self.call("GetAllFirmwareVersion", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeStorageServiceResponse()
+            model = models.GetAllFirmwareVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeStream(self, request):
-        """请求设备直播流地址
+    def GetFirmwareURL(self, request):
+        """本接口（GetFirmwareURL）用于获取固件存储的URL
 
-        :param request: Request instance for DescribeStream.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStreamRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeStreamResponse`
+        :param request: Request instance for GetFirmwareURL.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.GetFirmwareURLRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.GetFirmwareURLResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeStream", params, headers=headers)
+            body = self.call("GetFirmwareURL", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeStreamResponse()
+            model = models.GetFirmwareURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeTraceIds(self, request):
-        """本接口（DescribeTraceIds）用于查询设备日志跟踪白名单。
+    def ImportModelDefinition(self, request):
+        """导入其它产品的数据模板，覆盖现有数据模板的物模型和产品分类信息
 
-        :param request: Request instance for DescribeTraceIds.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceIdsRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceIdsResponse`
+        :param request: Request instance for ImportModelDefinition.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ImportModelDefinitionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ImportModelDefinitionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeTraceIds", params, headers=headers)
+            body = self.call("ImportModelDefinition", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeTraceIdsResponse()
+            model = models.ImportModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DescribeTraceStatus(self, request):
-        """本接口（DescribeTraceStatus）用于查询指定设备是否在白名单中。
+    def InheritCloudStorageUser(self, request):
+        """继承云存用户
 
-        :param request: Request instance for DescribeTraceStatus.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceStatusRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DescribeTraceStatusResponse`
+        :param request: Request instance for InheritCloudStorageUser.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.InheritCloudStorageUserRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.InheritCloudStorageUserResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DescribeTraceStatus", params, headers=headers)
+            body = self.call("InheritCloudStorageUser", params, headers=headers)
             response = json.loads(body)
-            model = models.DescribeTraceStatusResponse()
+            model = models.InheritCloudStorageUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DisableDevice(self, request):
-        """本接口（DisableDevice）用于禁用设备，可进行批量操作，每次操作最多100台设备。
+    def ListFirmwares(self, request):
+        """本接口（ListFirmwares）用于获取固件列表
 
-        :param request: Request instance for DisableDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceResponse`
+        :param request: Request instance for ListFirmwares.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ListFirmwaresRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ListFirmwaresResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DisableDevice", params, headers=headers)
+            body = self.call("ListFirmwares", params, headers=headers)
             response = json.loads(body)
-            model = models.DisableDeviceResponse()
+            model = models.ListFirmwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DisableDeviceStream(self, request):
-        """本接口（DisableDeviceStream）用于停止设备推流，可进行批量操作，每次操作最多100台设备。
+    def ModifyDataForward(self, request):
+        """修改数据转发
 
-        :param request: Request instance for DisableDeviceStream.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceStreamRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableDeviceStreamResponse`
+        :param request: Request instance for ModifyDataForward.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DisableDeviceStream", params, headers=headers)
+            body = self.call("ModifyDataForward", params, headers=headers)
             response = json.loads(body)
-            model = models.DisableDeviceStreamResponse()
+            model = models.ModifyDataForwardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def DisableOtaVersion(self, request):
-        """本接口（DisableOtaVersion）用于禁用固件版本。
+    def ModifyDataForwardStatus(self, request):
+        """设置数据转发状态
 
-        :param request: Request instance for DisableOtaVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.DisableOtaVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.DisableOtaVersionResponse`
+        :param request: Request instance for ModifyDataForwardStatus.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardStatusRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDataForwardStatusResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("DisableOtaVersion", params, headers=headers)
+            body = self.call("ModifyDataForwardStatus", params, headers=headers)
             response = json.loads(body)
-            model = models.DisableOtaVersionResponse()
+            model = models.ModifyDataForwardStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDevice(self, request):
         """修改设备信息
 
         :param request: Request instance for ModifyDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceResponse`
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
             body = self.call("ModifyDevice", params, headers=headers)
             response = json.loads(body)
             model = models.ModifyDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
-    def ModifyDeviceAction(self, request):
-        """本接口（ModifyDeviceAction）用于修改设备物模型的行为（Action）。
 
-        可对ctlVal数据属性进行写入,如:Action.takePhoto.ctlVal,设备在线且成功发送到设备才返回,物模型写入数据时,不需要传入时标信息,平台以当前时标作为数据的时标更新物模型中的时标信息。
-        注意:
-          1.若设备当前不在线,会直接返回错误
-          2.若设备网络出现异常时,消息发送可能超时,超时等待最长时间为3秒
-          3.value的内容必须与实际物模型的定义一致
+    def ModifyDeviceLogLevel(self, request):
+        """更新设备日志级别
 
-        :param request: Request instance for ModifyDeviceAction.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceActionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDeviceActionResponse`
+        :param request: Request instance for ModifyDeviceLogLevel.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceLogLevelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyDeviceLogLevelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDeviceAction", params, headers=headers)
+            body = self.call("ModifyDeviceLogLevel", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDeviceActionResponse()
+            model = models.ModifyDeviceLogLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyDeviceProperty(self, request):
-        """本接口（ModifyDeviceProperty）用于修改设备物模型的属性（ProWritable）。
-        可对setVal数据属性进行写入,如:
-        ProWritable.Pos.setVal
-        对于嵌套类型的可写属性，可以仅对其部分数据内容进行写入，如:
-        ProWritable.Pos.setVal.x;
-        可写属性云端写入成功即返回;云端向设备端发布属性变更参数;若当前设备不在线,在设备下次上线时会自动更新这些属性参数;
-        物模型写入数据时,不需要传入时标信息,平台以当前时标作为数据的时标更新物模型中的时标信息。
+    def ModifyForwardRule(self, request):
+        """修改转发规则
 
-        :param request: Request instance for ModifyDeviceProperty.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDevicePropertyRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyDevicePropertyResponse`
+        :param request: Request instance for ModifyForwardRule.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyForwardRuleRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyForwardRuleResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyDeviceProperty", params, headers=headers)
+            body = self.call("ModifyForwardRule", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyDevicePropertyResponse()
+            model = models.ModifyForwardRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyProduct(self, request):
-        """本接口（ModifyProduct）用于编辑物联网智能视频产品的相关信息。
+    def ModifyModelDefinition(self, request):
+        """提供修改产品的数据模板的能力
 
-        :param request: Request instance for ModifyProduct.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyProductRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyProductResponse`
+        :param request: Request instance for ModifyModelDefinition.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyModelDefinitionRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyModelDefinitionResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyProduct", params, headers=headers)
+            body = self.call("ModifyModelDefinition", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyProductResponse()
+            model = models.ModifyModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def ModifyVerContent(self, request):
-        """编辑版本描述信息
+    def ModifyProduct(self, request):
+        """修改产品信息
 
-        :param request: Request instance for ModifyVerContent.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.ModifyVerContentRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.ModifyVerContentResponse`
+        :param request: Request instance for ModifyProduct.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("ModifyVerContent", params, headers=headers)
+            body = self.call("ModifyProduct", params, headers=headers)
             response = json.loads(body)
-            model = models.ModifyVerContentResponse()
+            model = models.ModifyProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RefundStorageService(self, request):
-        """本接口（RefundStorageService）用于退订已购买的云存服务。
-        退订时，云存服务对应订单的处理方式 :
-        1. 未开始的订单自动回到已付费订单池
-        2. 已开始的订单自动失效
-        3. 购买云存接口,优先从已付费订单池中分配订单
+    def ModifyProductDynamicRegister(self, request):
+        """修改产品动态注册
 
-        :param request: Request instance for RefundStorageService.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RefundStorageServiceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RefundStorageServiceResponse`
+        :param request: Request instance for ModifyProductDynamicRegister.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductDynamicRegisterRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ModifyProductDynamicRegisterResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RefundStorageService", params, headers=headers)
+            body = self.call("ModifyProductDynamicRegister", params, headers=headers)
             response = json.loads(body)
-            model = models.RefundStorageServiceResponse()
+            model = models.ModifyProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RunDevice(self, request):
-        """本接口（RunDevice）用于启用设备，可进行批量操作，每次操作最多100台设备。
+    def PublishMessage(self, request):
+        """本接口（PublishMessage）用于使用自定义透传协议进行设备远控
 
-        :param request: Request instance for RunDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceResponse`
+        :param request: Request instance for PublishMessage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.PublishMessageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.PublishMessageResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RunDevice", params, headers=headers)
+            body = self.call("PublishMessage", params, headers=headers)
             response = json.loads(body)
-            model = models.RunDeviceResponse()
+            model = models.PublishMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RunDeviceStream(self, request):
-        """本接口（RunDeviceStream）用于开启设备推流，可进行批量操作，每次操作最多100台设备。
+    def ReportAliveDevice(self, request):
+        """上报活跃设备
 
-        :param request: Request instance for RunDeviceStream.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceStreamRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunDeviceStreamResponse`
+        :param request: Request instance for ReportAliveDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ReportAliveDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ReportAliveDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RunDeviceStream", params, headers=headers)
+            body = self.call("ReportAliveDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.RunDeviceStreamResponse()
+            model = models.ReportAliveDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RunIotModel(self, request):
-        """本接口（RunIotModel）用于对定义的物模型进行发布。
+    def ResetCloudStorage(self, request):
+        """重置云存服务
 
-        :param request: Request instance for RunIotModel.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunIotModelRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunIotModelResponse`
+        :param request: Request instance for ResetCloudStorage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.ResetCloudStorageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.ResetCloudStorageResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RunIotModel", params, headers=headers)
+            body = self.call("ResetCloudStorage", params, headers=headers)
             response = json.loads(body)
-            model = models.RunIotModelResponse()
+            model = models.ResetCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RunOtaVersion(self, request):
-        """本接口（RunOtaVersion）用于固件版本正式发布。
+    def RetryDeviceFirmwareTask(self, request):
+        """本接口用于重试设备升级任务
 
-        :param request: Request instance for RunOtaVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunOtaVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunOtaVersionResponse`
+        :param request: Request instance for RetryDeviceFirmwareTask.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.RetryDeviceFirmwareTaskRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.RetryDeviceFirmwareTaskResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RunOtaVersion", params, headers=headers)
+            body = self.call("RetryDeviceFirmwareTask", params, headers=headers)
             response = json.loads(body)
-            model = models.RunOtaVersionResponse()
+            model = models.RetryDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def RunTestOtaVersion(self, request):
-        """本接口（RunTestOtaVersion）用于固件版本测试发布。
+    def SetForwardAuth(self, request):
+        """设置转发权限
 
-        :param request: Request instance for RunTestOtaVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.RunTestOtaVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.RunTestOtaVersionResponse`
+        :param request: Request instance for SetForwardAuth.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.SetForwardAuthRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.SetForwardAuthResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("RunTestOtaVersion", params, headers=headers)
+            body = self.call("SetForwardAuth", params, headers=headers)
             response = json.loads(body)
-            model = models.RunTestOtaVersionResponse()
+            model = models.SetForwardAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def SendOnlineMsg(self, request):
-        """本接口（SendOnlineMsg）用于向设备发送在线消息。
-        注意：
-        若设备当前不在线,会直接返回错误;
-        若设备网络出现异常时,消息发送可能超时,超时等待最长时间为3秒.waitresp非0情况下,会导致本接口阻塞3秒。
+    def TransferCloudStorage(self, request):
+        """转移云存服务
 
-        :param request: Request instance for SendOnlineMsg.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.SendOnlineMsgRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.SendOnlineMsgResponse`
+        :param request: Request instance for TransferCloudStorage.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.TransferCloudStorageRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.TransferCloudStorageResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("SendOnlineMsg", params, headers=headers)
+            body = self.call("TransferCloudStorage", params, headers=headers)
             response = json.loads(body)
-            model = models.SendOnlineMsgResponse()
+            model = models.TransferCloudStorageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def SetMessageQueue(self, request):
-        """本接口（SetMessageQueue）用于配置物联网智能视频产品的转发消息队列。
+    def UpdateAIModelChannel(self, request):
+        """更新AI推理结果推送配置
 
-        :param request: Request instance for SetMessageQueue.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.SetMessageQueueRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.SetMessageQueueResponse`
+        :param request: Request instance for UpdateAIModelChannel.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.UpdateAIModelChannelRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.UpdateAIModelChannelResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("SetMessageQueue", params, headers=headers)
+            body = self.call("UpdateAIModelChannel", params, headers=headers)
             response = json.loads(body)
-            model = models.SetMessageQueueResponse()
+            model = models.UpdateAIModelChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def UpgradeDevice(self, request):
-        """本接口（UpgradeDevice）用于对设备进行固件升级。
-        该接口向指定的设备下发固件更新指令,可将固件升级到任意版本(可实现固件降级)。
-        警告:使能UpgradeNow参数存在一定的风险性！建议仅在debug场景下使用!
+    def UploadFirmware(self, request):
+        """本接口（UploadFirmware）用于上传设备固件信息
 
-        :param request: Request instance for UpgradeDevice.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.UpgradeDeviceRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.UpgradeDeviceResponse`
+        :param request: Request instance for UploadFirmware.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.UploadFirmwareRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.UploadFirmwareResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("UpgradeDevice", params, headers=headers)
+            body = self.call("UploadFirmware", params, headers=headers)
             response = json.loads(body)
-            model = models.UpgradeDeviceResponse()
+            model = models.UploadFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def UploadOtaVersion(self, request):
-        """本接口（UploadOtaVersion）接收上传到控制台的固件版本信息。
+    def WakeUpDevice(self, request):
+        """设备唤醒
 
-        :param request: Request instance for UploadOtaVersion.
-        :type request: :class:`tencentcloud.iotvideo.v20191126.models.UploadOtaVersionRequest`
-        :rtype: :class:`tencentcloud.iotvideo.v20191126.models.UploadOtaVersionResponse`
+        :param request: Request instance for WakeUpDevice.
+        :type request: :class:`tencentcloud.iotvideo.v20201215.models.WakeUpDeviceRequest`
+        :rtype: :class:`tencentcloud.iotvideo.v20201215.models.WakeUpDeviceResponse`
 
         """
         try:
             params = request._serialize()
             headers = request.headers
-            body = self.call("UploadOtaVersion", params, headers=headers)
+            body = self.call("WakeUpDevice", params, headers=headers)
             response = json.loads(body)
-            model = models.UploadOtaVersionResponse()
+            model = models.WakeUpDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/iotvideo/v20191126/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/iotvideo/v20191126/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/README.rst` & `tencentcloud-sdk-python-iotvideo-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.937/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.938/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

