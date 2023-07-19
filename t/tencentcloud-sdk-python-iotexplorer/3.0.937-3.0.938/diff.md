# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.937.tar", last modified: Tue Jul 18 00:25:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.938.tar", last modified: Wed Jul 19 00:41:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82835 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)    20510 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   360219 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-18 00:25:49.000000 tencentcloud-sdk-python-iotexplorer-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83195 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)    20510 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360219 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-19 00:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindProducts(self, request):
         """批量绑定子产品
 
         :param request: Request instance for BindProducts.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.BindProductsRequest`
@@ -65,15 +65,15 @@
             model = models.BindProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallDeviceActionAsync(self, request):
         """提供给用户异步调用设备行为的能力
 
         :param request: Request instance for CallDeviceActionAsync.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CallDeviceActionAsyncRequest`
@@ -88,15 +88,15 @@
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
         """为用户提供同步调用设备行为的能力。
 
         :param request: Request instance for CallDeviceActionSync.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CallDeviceActionSyncRequest`
@@ -111,15 +111,15 @@
             model = models.CallDeviceActionSyncResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ControlDeviceDataRequest`
@@ -134,15 +134,15 @@
             model = models.ControlDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBatchProduction(self, request):
         """用于新建批量生产设备
 
         :param request: Request instance for CreateBatchProduction.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateBatchProductionRequest`
@@ -157,15 +157,15 @@
             model = models.CreateBatchProductionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDevice(self, request):
         """创建设备
 
         :param request: Request instance for CreateDevice.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateDeviceRequest`
@@ -180,15 +180,15 @@
             model = models.CreateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFenceBind(self, request):
         """创建围栏绑定信息
 
         :param request: Request instance for CreateFenceBind.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateFenceBindRequest`
@@ -203,15 +203,15 @@
             model = models.CreateFenceBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLoRaFrequency(self, request):
         """创建 LoRa 自定义频点
 
         :param request: Request instance for CreateLoRaFrequency.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateLoRaFrequencyRequest`
@@ -226,15 +226,15 @@
             model = models.CreateLoRaFrequencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLoRaGateway(self, request):
         """创建新 LoRa 网关设备接口
 
         :param request: Request instance for CreateLoRaGateway.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateLoRaGatewayRequest`
@@ -249,15 +249,15 @@
             model = models.CreateLoRaGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePositionFence(self, request):
         """创建围栏
 
         :param request: Request instance for CreatePositionFence.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreatePositionFenceRequest`
@@ -272,15 +272,15 @@
             model = models.CreatePositionFenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePositionSpace(self, request):
         """创建位置空间
 
         :param request: Request instance for CreatePositionSpace.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreatePositionSpaceRequest`
@@ -295,15 +295,15 @@
             model = models.CreatePositionSpaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProject(self, request):
         """为用户提供新建项目的能力，用于集中管理产品和应用。
 
         :param request: Request instance for CreateProject.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateProjectRequest`
@@ -318,15 +318,15 @@
             model = models.CreateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStudioProduct(self, request):
         """为用户提供新建产品的能力，用于管理用户的设备
 
         :param request: Request instance for CreateStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateStudioProductRequest`
@@ -341,15 +341,15 @@
             model = models.CreateStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopicPolicy(self, request):
         """本接口（CreateTopicPolicy）用于创建一个Topic
 
         :param request: Request instance for CreateTopicPolicy.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateTopicPolicyRequest`
@@ -364,15 +364,15 @@
             model = models.CreateTopicPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopicRule(self, request):
         """创建规则
 
         :param request: Request instance for CreateTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.CreateTopicRuleRequest`
@@ -387,15 +387,15 @@
             model = models.CreateTopicRuleResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteDeviceRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDevices(self, request):
         """批量删除设备
 
         :param request: Request instance for DeleteDevices.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteDevicesRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFenceBind(self, request):
         """删除围栏绑定信息
 
         :param request: Request instance for DeleteFenceBind.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteFenceBindRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteFenceBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoRaFrequency(self, request):
         """提供删除LoRa自定义频点的能力
 
         :param request: Request instance for DeleteLoRaFrequency.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteLoRaFrequencyRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteLoRaFrequencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoRaGateway(self, request):
         """删除  LoRa 网关的接口
 
         :param request: Request instance for DeleteLoRaGateway.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteLoRaGatewayRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteLoRaGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePositionFence(self, request):
         """删除围栏
 
         :param request: Request instance for DeletePositionFence.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeletePositionFenceRequest`
@@ -525,15 +525,15 @@
             model = models.DeletePositionFenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePositionSpace(self, request):
         """删除位置空间
 
         :param request: Request instance for DeletePositionSpace.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeletePositionSpaceRequest`
@@ -548,15 +548,15 @@
             model = models.DeletePositionSpaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProject(self, request):
         """提供删除某个项目的能力
 
         :param request: Request instance for DeleteProject.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteProjectRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStudioProduct(self, request):
         """提供删除某个项目下产品的能力
 
         :param request: Request instance for DeleteStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteStudioProductRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopicPolicy(self, request):
         """本接口（DeleteTopicPolicy）用于删除Topic
 
         :param request: Request instance for DeleteTopicPolicy.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteTopicPolicyRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteTopicPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopicRule(self, request):
         """删除规则
 
         :param request: Request instance for DeleteTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DeleteTopicRuleRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchProduction(self, request):
         """获取量产详情信息。
 
         :param request: Request instance for DescribeBatchProduction.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeBatchProductionRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeBatchProductionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBindedProducts(self, request):
         """获取网关产品已经绑定的子产品
 
         :param request: Request instance for DescribeBindedProducts.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeBindedProductsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeBindedProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
         """用于查看某个设备的详细信息
 
         :param request: Request instance for DescribeDevice.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDeviceRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceBindGateway(self, request):
         """查询设备绑定的网关设备
 
         :param request: Request instance for DescribeDeviceBindGateway.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDeviceBindGatewayRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeDeviceBindGatewayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceData(self, request):
         """根据设备产品ID、设备名称，获取设备上报的属性数据。
 
         :param request: Request instance for DescribeDeviceData.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDeviceDataRequest`
@@ -755,15 +755,15 @@
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDeviceDataHistoryRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeDeviceDataHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceLocationSolve(self, request):
         """获取实时位置解析
 
         :param request: Request instance for DescribeDeviceLocationSolve.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDeviceLocationSolveRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeDeviceLocationSolveResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevicePositionList(self, request):
         """获取设备位置列表
 
         :param request: Request instance for DescribeDevicePositionList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeDevicePositionListRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeDevicePositionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFenceBindList(self, request):
         """获取围栏绑定信息列表
 
         :param request: Request instance for DescribeFenceBindList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeFenceBindListRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeFenceBindListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFenceEventList(self, request):
         """获取围栏告警事件列表
 
         :param request: Request instance for DescribeFenceEventList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeFenceEventListRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeFenceEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirmwareTask(self, request):
         """查询固件升级任务列表
 
         :param request: Request instance for DescribeFirmwareTask.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeFirmwareTaskRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayBindDevices(self, request):
         """获取网关绑定的子设备列表
 
         :param request: Request instance for DescribeGatewayBindDevices.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeGatewayBindDevicesRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeGatewayBindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewaySubDeviceList(self, request):
         """查询绑定到家庭的网关设备的子设备列表
 
         :param request: Request instance for DescribeGatewaySubDeviceList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeGatewaySubDeviceListRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeGatewaySubDeviceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewaySubProducts(self, request):
         """用于获取网关可绑定或解绑的子产品
 
         :param request: Request instance for DescribeGatewaySubProducts.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeGatewaySubProductsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeGatewaySubProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoRaFrequency(self, request):
         """提供查询LoRa自定义频点详情的能力
 
         :param request: Request instance for DescribeLoRaFrequency.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeLoRaFrequencyRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeLoRaFrequencyResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeModelDefinitionRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePositionFenceList(self, request):
         """获取围栏列表
 
         :param request: Request instance for DescribePositionFenceList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribePositionFenceListRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribePositionFenceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProject(self, request):
         """查询项目详情
 
         :param request: Request instance for DescribeProject.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeProjectRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSpaceFenceEventList(self, request):
         """获取位置空间中围栏告警事件列表
 
         :param request: Request instance for DescribeSpaceFenceEventList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeSpaceFenceEventListRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeSpaceFenceEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStudioProduct(self, request):
         """提供查看产品详细信息的能力，包括产品的ID、数据协议、认证类型等重要参数
 
         :param request: Request instance for DescribeStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeStudioProductRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicPolicy(self, request):
         """本接口（DescribeTopicPolicy）用于查看Topic详细信息
 
         :param request: Request instance for DescribeTopicPolicy.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeTopicPolicyRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeTopicPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopicRule(self, request):
         """获取规则信息
 
         :param request: Request instance for DescribeTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DescribeTopicRuleRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DirectBindDeviceInFamily(self, request):
         """直接绑定设备和家庭
 
         :param request: Request instance for DirectBindDeviceInFamily.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DirectBindDeviceInFamilyRequest`
@@ -1169,15 +1169,15 @@
             model = models.DirectBindDeviceInFamilyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableTopicRule(self, request):
         """禁用规则
 
         :param request: Request instance for DisableTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.DisableTopicRuleRequest`
@@ -1192,15 +1192,15 @@
             model = models.DisableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableTopicRule(self, request):
         """启用规则
 
         :param request: Request instance for EnableTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.EnableTopicRuleRequest`
@@ -1215,15 +1215,15 @@
             model = models.EnableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenSingleDeviceSignatureOfPublic(self, request):
         """无
 
         :param request: Request instance for GenSingleDeviceSignatureOfPublic.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GenSingleDeviceSignatureOfPublicRequest`
@@ -1238,15 +1238,15 @@
             model = models.GenSingleDeviceSignatureOfPublicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetBatchProductionsList(self, request):
         """列出量产数据列表信息。
 
         :param request: Request instance for GetBatchProductionsList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetBatchProductionsListRequest`
@@ -1261,15 +1261,15 @@
             model = models.GetBatchProductionsListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCOSURL(self, request):
         """本接口（GetCOSURL）用于获取固件COS存储的上传请求URL地址
 
         :param request: Request instance for GetCOSURL.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetCOSURLRequest`
@@ -1284,15 +1284,15 @@
             model = models.GetCOSURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceList(self, request):
         """用于查询某个产品下的设备列表
 
         :param request: Request instance for GetDeviceList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceListRequest`
@@ -1307,15 +1307,15 @@
             model = models.GetDeviceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceLocationHistory(self, request):
         """获取设备历史位置
 
         :param request: Request instance for GetDeviceLocationHistory.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceLocationHistoryRequest`
@@ -1330,15 +1330,15 @@
             model = models.GetDeviceLocationHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFamilyDeviceUserList(self, request):
         """用于获取设备绑定的用户列表
 
         :param request: Request instance for GetFamilyDeviceUserList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetFamilyDeviceUserListRequest`
@@ -1353,15 +1353,15 @@
             model = models.GetFamilyDeviceUserListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetGatewaySubDeviceList(self, request):
         """获取指定网关设备的子设备列表
 
         :param request: Request instance for GetGatewaySubDeviceList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetGatewaySubDeviceListRequest`
@@ -1376,15 +1376,15 @@
             model = models.GetGatewaySubDeviceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLoRaGatewayList(self, request):
         """获取 LoRa 网关列表接口
 
         :param request: Request instance for GetLoRaGatewayList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetLoRaGatewayListRequest`
@@ -1399,15 +1399,15 @@
             model = models.GetLoRaGatewayListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPositionSpaceList(self, request):
         """获取位置空间列表
 
         :param request: Request instance for GetPositionSpaceList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetPositionSpaceListRequest`
@@ -1422,15 +1422,15 @@
             model = models.GetPositionSpaceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetProjectList(self, request):
         """提供查询用户所创建的项目列表查询功能。
 
         :param request: Request instance for GetProjectList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetProjectListRequest`
@@ -1445,15 +1445,15 @@
             model = models.GetProjectListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetStudioProductList(self, request):
         """提供查询某个项目下所有产品信息的能力。
 
         :param request: Request instance for GetStudioProductList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetStudioProductListRequest`
@@ -1468,15 +1468,15 @@
             model = models.GetStudioProductListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTopicRuleList(self, request):
         """获取规则列表
 
         :param request: Request instance for GetTopicRuleList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetTopicRuleListRequest`
@@ -1491,15 +1491,15 @@
             model = models.GetTopicRuleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEventHistory(self, request):
         """获取设备的历史事件
 
         :param request: Request instance for ListEventHistory.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ListEventHistoryRequest`
@@ -1514,15 +1514,15 @@
             model = models.ListEventHistoryResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ListFirmwaresRequest`
@@ -1537,15 +1537,15 @@
             model = models.ListFirmwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopicPolicy(self, request):
         """本接口（ListTopicPolicy）用于获取Topic列表
 
         :param request: Request instance for ListTopicPolicy.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ListTopicPolicyRequest`
@@ -1560,15 +1560,15 @@
             model = models.ListTopicPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFenceBind(self, request):
         """更新围栏绑定信息
 
         :param request: Request instance for ModifyFenceBind.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyFenceBindRequest`
@@ -1583,15 +1583,15 @@
             model = models.ModifyFenceBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoRaFrequency(self, request):
         """修改LoRa自定义频点
 
         :param request: Request instance for ModifyLoRaFrequency.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyLoRaFrequencyRequest`
@@ -1606,15 +1606,15 @@
             model = models.ModifyLoRaFrequencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoRaGateway(self, request):
         """修改 LoRa 网关信息
 
         :param request: Request instance for ModifyLoRaGateway.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyLoRaGatewayRequest`
@@ -1629,15 +1629,15 @@
             model = models.ModifyLoRaGatewayResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyModelDefinitionRequest`
@@ -1652,15 +1652,15 @@
             model = models.ModifyModelDefinitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPositionFence(self, request):
         """更新围栏
 
         :param request: Request instance for ModifyPositionFence.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyPositionFenceRequest`
@@ -1675,15 +1675,15 @@
             model = models.ModifyPositionFenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPositionSpace(self, request):
         """更新位置空间
 
         :param request: Request instance for ModifyPositionSpace.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyPositionSpaceRequest`
@@ -1698,15 +1698,15 @@
             model = models.ModifyPositionSpaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProject(self, request):
         """修改项目
 
         :param request: Request instance for ModifyProject.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyProjectRequest`
@@ -1721,15 +1721,15 @@
             model = models.ModifyProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySpaceProperty(self, request):
         """更新位置空间产品属性
 
         :param request: Request instance for ModifySpaceProperty.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifySpacePropertyRequest`
@@ -1744,15 +1744,15 @@
             model = models.ModifySpacePropertyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyStudioProduct(self, request):
         """提供修改产品的名称和描述等信息的能力，对于已发布产品不允许进行修改。
 
         :param request: Request instance for ModifyStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyStudioProductRequest`
@@ -1767,15 +1767,15 @@
             model = models.ModifyStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopicPolicy(self, request):
         """本接口（UpdateTopicPolicy）用于更新Topic信息
 
         :param request: Request instance for ModifyTopicPolicy.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyTopicPolicyRequest`
@@ -1790,15 +1790,15 @@
             model = models.ModifyTopicPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopicRule(self, request):
         """修改规则
 
         :param request: Request instance for ModifyTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ModifyTopicRuleRequest`
@@ -1813,15 +1813,15 @@
             model = models.ModifyTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishBroadcastMessage(self, request):
         """发布广播消息
 
         :param request: Request instance for PublishBroadcastMessage.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.PublishBroadcastMessageRequest`
@@ -1836,15 +1836,15 @@
             model = models.PublishBroadcastMessageResponse()
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
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.PublishMessageRequest`
@@ -1859,15 +1859,15 @@
             model = models.PublishMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishRRPCMessage(self, request):
         """下发RRPC消息
 
         :param request: Request instance for PublishRRPCMessage.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.PublishRRPCMessageRequest`
@@ -1882,15 +1882,15 @@
             model = models.PublishRRPCMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseStudioProduct(self, request):
         """产品开发完成并测试通过后，通过发布产品将产品设置为发布状态
 
         :param request: Request instance for ReleaseStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.ReleaseStudioProductRequest`
@@ -1905,15 +1905,15 @@
             model = models.ReleaseStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchPositionSpace(self, request):
         """搜索位置空间
 
         :param request: Request instance for SearchPositionSpace.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.SearchPositionSpaceRequest`
@@ -1928,15 +1928,15 @@
             model = models.SearchPositionSpaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchStudioProduct(self, request):
         """提供根据产品名称查找产品的能力
 
         :param request: Request instance for SearchStudioProduct.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.SearchStudioProductRequest`
@@ -1951,15 +1951,15 @@
             model = models.SearchStudioProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchTopicRule(self, request):
         """搜索规则
 
         :param request: Request instance for SearchTopicRule.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.SearchTopicRuleRequest`
@@ -1974,15 +1974,15 @@
             model = models.SearchTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindDevices(self, request):
         """批量解绑子设备
 
         :param request: Request instance for UnbindDevices.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.UnbindDevicesRequest`
@@ -1997,15 +1997,15 @@
             model = models.UnbindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindProducts(self, request):
         """批量解绑子产品
 
         :param request: Request instance for UnbindProducts.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.UnbindProductsRequest`
@@ -2020,15 +2020,15 @@
             model = models.UnbindProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDevicesEnableState(self, request):
         """批量禁用启用设备
 
         :param request: Request instance for UpdateDevicesEnableState.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.UpdateDevicesEnableStateRequest`
@@ -2043,15 +2043,15 @@
             model = models.UpdateDevicesEnableStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFirmware(self, request):
         """本接口（UpdateFirmware）用于对指定设备发起固件升级请求
 
         :param request: Request instance for UpdateFirmware.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.UpdateFirmwareRequest`
@@ -2066,15 +2066,15 @@
             model = models.UpdateFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFirmware(self, request):
         """本接口（UploadFirmware）用于创建设备固件版本信息，在平台用于固件版本升级、固件资源下发等。
 
         :param request: Request instance for UploadFirmware.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.UploadFirmwareRequest`
@@ -2089,8 +2089,8 @@
             model = models.UploadFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.938/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.937/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.938/README.rst`

 * *Files identical despite different names*

