# Comparing `tmp/tencentcloud-sdk-python-iotcloud-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iotcloud-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.937.tar", last modified: Tue Jul 18 00:25:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.938.tar", last modified: Wed Jul 19 00:41:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotcloud-3.0.937.tar` & `tencentcloud-sdk-python-iotcloud-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66885 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12818 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   278249 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64286 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12668 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   281180 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:25:43.000000 tencentcloud-sdk-python-iotcloud-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67173 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   278249 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64562 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   281180 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:41:08.000000 tencentcloud-sdk-python-iotcloud-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/setup.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchUpdateFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDevices(self, request):
         """本接口（BindDevices）用于网关设备批量绑定子设备
 
         :param request: Request instance for BindDevices.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.BindDevicesRequest`
@@ -65,15 +65,15 @@
             model = models.BindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelDeviceFirmwareTask(self, request):
         """取消设备升级任务
 
         :param request: Request instance for CancelDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CancelDeviceFirmwareTaskRequest`
@@ -88,15 +88,15 @@
             model = models.CancelDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDevice(self, request):
         """本接口（CreateDevice）用于新建一个物联网通信设备。
 
         :param request: Request instance for CreateDevice.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateDeviceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultiDevicesTask(self, request):
         """本接口（CreateMultiDevicesTask）用于创建产品级别的批量创建设备任务
 
         :param request: Request instance for CreateMultiDevicesTask.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateMultiDevicesTaskRequest`
@@ -134,15 +134,15 @@
             model = models.CreateMultiDevicesTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrivateCA(self, request):
         """创建私有CA证书
 
         :param request: Request instance for CreatePrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreatePrivateCARequest`
@@ -157,15 +157,15 @@
             model = models.CreatePrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
         """本接口（CreateProduct）用于创建一个新的物联网通信产品
 
         :param request: Request instance for CreateProduct.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateProductRequest`
@@ -180,15 +180,15 @@
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
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateTaskFileUrlRequest`
@@ -203,15 +203,15 @@
             model = models.CreateTaskFileUrlResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateTopicPolicyRequest`
@@ -226,15 +226,15 @@
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
         """本接口（CreateTopicRule）用于创建一个规则
 
         :param request: Request instance for CreateTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.CreateTopicRuleRequest`
@@ -249,15 +249,15 @@
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
         """本接口（DeleteDevice）用于删除物联网通信设备。
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteDeviceRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceResource(self, request):
         """本接口（DeleteDeviceResource）用于删除设备资源
 
         :param request: Request instance for DeleteDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteDeviceResourceRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceShadow(self, request):
         """本接口（DeleteDeviceShadow）用于删除设备影子
 
         :param request: Request instance for DeleteDeviceShadow.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteDeviceShadowRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteDeviceShadowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivateCA(self, request):
         """删除私有CA证书
 
         :param request: Request instance for DeletePrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeletePrivateCARequest`
@@ -341,15 +341,15 @@
             model = models.DeletePrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProduct(self, request):
         """本接口（DeleteProduct）用于删除一个物联网通信产品
 
         :param request: Request instance for DeleteProduct.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteProductRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProductPrivateCA(self, request):
         """删除产品的私有CA证书
 
         :param request: Request instance for DeleteProductPrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteProductPrivateCARequest`
@@ -387,15 +387,15 @@
             model = models.DeleteProductPrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopicRule(self, request):
         """本接口（DeleteTopicRule）用于删除规则
 
         :param request: Request instance for DeleteTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DeleteTopicRuleRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
         """本接口（DescribeDevice）用于查看设备信息
 
         :param request: Request instance for DescribeDevice.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDeviceRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceClientKey(self, request):
         """获取证书认证类型设备的私钥，刚生成或者重置设备后仅可调用一次
 
         :param request: Request instance for DescribeDeviceClientKey.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDeviceClientKeyRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeDeviceClientKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceResource(self, request):
         """本接口（DescribeDeviceResource）用于查询设备资源详情。
 
         :param request: Request instance for DescribeDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDeviceResourceRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceResources(self, request):
         """本接口（DescribeDeviceResources）用于查询设备资源列表。
 
         :param request: Request instance for DescribeDeviceResources.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDeviceResourcesRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeDeviceResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceShadow(self, request):
         """本接口（DescribeDeviceShadow）用于查询虚拟设备信息。
 
         :param request: Request instance for DescribeDeviceShadow.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDeviceShadowRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeDeviceShadowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
         """本接口（DescribeDevices）用于查询物联网通信设备的设备列表。
 
         :param request: Request instance for DescribeDevices.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeDevicesRequest`
@@ -548,15 +548,15 @@
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
         """查询固件信息
 
         :param request: Request instance for DescribeFirmware.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareRequest`
@@ -571,15 +571,15 @@
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
         """查询固件升级任务详情
 
         :param request: Request instance for DescribeFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareTaskRequest`
@@ -594,15 +594,15 @@
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
         """查询固件升级任务的设备列表
 
         :param request: Request instance for DescribeFirmwareTaskDevices.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareTaskDevicesRequest`
@@ -617,15 +617,15 @@
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
         """查询固件升级任务状态分布
 
         :param request: Request instance for DescribeFirmwareTaskDistribution.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareTaskDistributionRequest`
@@ -640,15 +640,15 @@
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
         """查询固件升级任务统计信息
 
         :param request: Request instance for DescribeFirmwareTaskStatistics.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareTaskStatisticsRequest`
@@ -663,15 +663,15 @@
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
         """查询固件升级任务列表
 
         :param request: Request instance for DescribeFirmwareTasks.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeFirmwareTasksRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeFirmwareTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayBindDevices(self, request):
         """本接口（DescribeGatewayBindDevices）用于获取网关绑定的子设备列表
 
         :param request: Request instance for DescribeGatewayBindDevices.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeGatewayBindDevicesRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeGatewayBindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateCA(self, request):
         """查询私有化CA信息
 
         :param request: Request instance for DescribePrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribePrivateCARequest`
@@ -732,15 +732,15 @@
             model = models.DescribePrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateCABindedProducts(self, request):
         """查询私有CA绑定的产品列表
 
         :param request: Request instance for DescribePrivateCABindedProducts.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribePrivateCABindedProductsRequest`
@@ -755,15 +755,15 @@
             model = models.DescribePrivateCABindedProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateCAs(self, request):
         """查询私有CA证书列表
 
         :param request: Request instance for DescribePrivateCAs.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribePrivateCAsRequest`
@@ -778,15 +778,15 @@
             model = models.DescribePrivateCAsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProduct(self, request):
         """本接口（DescribeProduct）用于查看产品详情
 
         :param request: Request instance for DescribeProduct.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductCA(self, request):
         """查询产品绑定的CA证书
 
         :param request: Request instance for DescribeProductCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductCARequest`
@@ -824,15 +824,15 @@
             model = models.DescribeProductCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductResource(self, request):
         """本接口（DescribeProductResource）用于查询产品资源详情。
 
         :param request: Request instance for DescribeProductResource.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductResourceRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeProductResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductResources(self, request):
         """本接口（DescribeProductResources）用于查询产品资源列表。
 
         :param request: Request instance for DescribeProductResources.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductResourcesRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeProductResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductTask(self, request):
         """本接口（DescribeProductTask）用于查看产品级别的任务信息
 
         :param request: Request instance for DescribeProductTask.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductTaskRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeProductTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductTasks(self, request):
         """本接口（DescribeProductTasks）用于查看产品级别的任务列表
 
         :param request: Request instance for DescribeProductTasks.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductTasksRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeProductTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProducts(self, request):
         """本接口（DescribeProducts）用于列出产品列表。
 
         :param request: Request instance for DescribeProducts.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeProductsRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushResourceTaskStatistics(self, request):
         """查询推送资源任务统计信息
 
         :param request: Request instance for DescribePushResourceTaskStatistics.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribePushResourceTaskStatisticsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribePushResourceTaskStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTasks(self, request):
         """查询资源推送任务列表
 
         :param request: Request instance for DescribeResourceTasks.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DescribeResourceTasksRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeResourceTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableTopicRule(self, request):
         """本接口（DisableTopicRule）用于禁用规则
 
         :param request: Request instance for DisableTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DisableTopicRuleRequest`
@@ -1008,15 +1008,15 @@
             model = models.DisableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadDeviceResource(self, request):
         """本接口（DownloadDeviceResource）用于下载设备资源
 
         :param request: Request instance for DownloadDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.DownloadDeviceResourceRequest`
@@ -1031,15 +1031,15 @@
             model = models.DownloadDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditFirmware(self, request):
         """编辑固件信息
 
         :param request: Request instance for EditFirmware.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.EditFirmwareRequest`
@@ -1054,15 +1054,15 @@
             model = models.EditFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableTopicRule(self, request):
         """本接口（EnableTopicRule）用于启用规则
 
         :param request: Request instance for EnableTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.EnableTopicRuleRequest`
@@ -1077,15 +1077,15 @@
             model = models.EnableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAllVersion(self, request):
         """本接口（GetAllVersion）用于获取所有的版本列表
 
         :param request: Request instance for GetAllVersion.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.GetAllVersionRequest`
@@ -1100,15 +1100,15 @@
             model = models.GetAllVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCOSURL(self, request):
         """本接口（GetCOSURL）用于获取固件存储在COS的URL
 
         :param request: Request instance for GetCOSURL.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.GetCOSURLRequest`
@@ -1123,15 +1123,15 @@
             model = models.GetCOSURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetUserResourceInfo(self, request):
         """本接口（GetUserResourceInfo）用于查询用户资源使用信息。
 
         :param request: Request instance for GetUserResourceInfo.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.GetUserResourceInfoRequest`
@@ -1146,15 +1146,15 @@
             model = models.GetUserResourceInfoResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ListFirmwaresRequest`
@@ -1169,15 +1169,15 @@
             model = models.ListFirmwaresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLog(self, request):
         """本接口（ListLog）用于查看日志信息
 
         :param request: Request instance for ListLog.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ListLogRequest`
@@ -1192,15 +1192,15 @@
             model = models.ListLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLogPayload(self, request):
         """获取日志内容列表
 
         :param request: Request instance for ListLogPayload.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ListLogPayloadRequest`
@@ -1215,15 +1215,15 @@
             model = models.ListLogPayloadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListSDKLog(self, request):
         """获取设备上报的日志
 
         :param request: Request instance for ListSDKLog.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ListSDKLogRequest`
@@ -1238,15 +1238,15 @@
             model = models.ListSDKLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTopicRules(self, request):
         """本接口（ListTopicRules）用于分页获取规则列表
 
         :param request: Request instance for ListTopicRules.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ListTopicRulesRequest`
@@ -1261,15 +1261,15 @@
             model = models.ListTopicRulesResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.PublishBroadcastMessageRequest`
@@ -1284,15 +1284,15 @@
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
         """本接口（PublishMessage）用于向某个主题发消息。
 
         :param request: Request instance for PublishMessage.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.PublishMessageRequest`
@@ -1307,15 +1307,15 @@
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
         """发布RRPC消息
 
         :param request: Request instance for PublishRRPCMessage.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.PublishRRPCMessageRequest`
@@ -1330,15 +1330,15 @@
             model = models.PublishRRPCMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceTopicRule(self, request):
         """本接口（ReplaceTopicRule）用于修改替换规则
 
         :param request: Request instance for ReplaceTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ReplaceTopicRuleRequest`
@@ -1353,15 +1353,15 @@
             model = models.ReplaceTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDeviceState(self, request):
         """重置设备的连接状态
 
         :param request: Request instance for ResetDeviceState.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.ResetDeviceStateRequest`
@@ -1376,15 +1376,15 @@
             model = models.ResetDeviceStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryDeviceFirmwareTask(self, request):
         """重试设备升级任务
 
         :param request: Request instance for RetryDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.RetryDeviceFirmwareTaskRequest`
@@ -1399,15 +1399,15 @@
             model = models.RetryDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetProductsForbiddenStatus(self, request):
         """批量设置产品禁用状态
 
         :param request: Request instance for SetProductsForbiddenStatus.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.SetProductsForbiddenStatusRequest`
@@ -1422,15 +1422,15 @@
             model = models.SetProductsForbiddenStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindDevices(self, request):
         """本接口（UnbindDevices）用于网关设备批量解绑子设备
 
         :param request: Request instance for UnbindDevices.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UnbindDevicesRequest`
@@ -1445,15 +1445,15 @@
             model = models.UnbindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDeviceAvailableState(self, request):
         """启用或者禁用设备
 
         :param request: Request instance for UpdateDeviceAvailableState.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateDeviceAvailableStateRequest`
@@ -1468,15 +1468,15 @@
             model = models.UpdateDeviceAvailableStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDeviceLogLevel(self, request):
         """设置设备上报的日志级别
 
         :param request: Request instance for UpdateDeviceLogLevel.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateDeviceLogLevelRequest`
@@ -1491,15 +1491,15 @@
             model = models.UpdateDeviceLogLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDevicePSK(self, request):
         """本接口（UpdateDevicePSK）用于更新设备的PSK
 
         :param request: Request instance for UpdateDevicePSK.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateDevicePSKRequest`
@@ -1514,15 +1514,15 @@
             model = models.UpdateDevicePSKResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDeviceShadow(self, request):
         """本接口（UpdateDeviceShadow）用于更新虚拟设备信息。
 
         :param request: Request instance for UpdateDeviceShadow.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateDeviceShadowRequest`
@@ -1537,15 +1537,15 @@
             model = models.UpdateDeviceShadowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDevicesEnableState(self, request):
         """批量启用或者禁用设备
 
         :param request: Request instance for UpdateDevicesEnableState.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateDevicesEnableStateRequest`
@@ -1560,15 +1560,15 @@
             model = models.UpdateDevicesEnableStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePrivateCA(self, request):
         """更新私有CA证书
 
         :param request: Request instance for UpdatePrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdatePrivateCARequest`
@@ -1583,15 +1583,15 @@
             model = models.UpdatePrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProductDynamicRegister(self, request):
         """更新产品动态注册的配置
 
         :param request: Request instance for UpdateProductDynamicRegister.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateProductDynamicRegisterRequest`
@@ -1606,15 +1606,15 @@
             model = models.UpdateProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProductPrivateCA(self, request):
         """更新产品的私有CA
 
         :param request: Request instance for UpdateProductPrivateCA.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateProductPrivateCARequest`
@@ -1629,15 +1629,15 @@
             model = models.UpdateProductPrivateCAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTopicPolicy(self, request):
         """本接口（UpdateTopicPolicy）用于更新Topic信息
 
         :param request: Request instance for UpdateTopicPolicy.
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UpdateTopicPolicyRequest`
@@ -1652,15 +1652,15 @@
             model = models.UpdateTopicPolicyResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20210408.models.UploadFirmwareRequest`
@@ -1675,8 +1675,8 @@
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

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchUpdateFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindDevices(self, request):
         """本接口（BindDevices）用于网关设备批量绑定子设备
 
         :param request: Request instance for BindDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.BindDevicesRequest`
@@ -65,15 +65,15 @@
             model = models.BindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelDeviceFirmwareTask(self, request):
         """取消设备升级任务
 
         :param request: Request instance for CancelDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CancelDeviceFirmwareTaskRequest`
@@ -88,15 +88,15 @@
             model = models.CancelDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelTask(self, request):
         """本接口（CancelTask）用于取消一个未被调度的任务。
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CancelTaskRequest`
@@ -111,15 +111,15 @@
             model = models.CancelTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDevice(self, request):
         """本接口（CreateDevice）用于新建一个物联网通信设备。
 
         :param request: Request instance for CreateDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateDeviceRequest`
@@ -134,15 +134,15 @@
             model = models.CreateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLoraDevice(self, request):
         """创建lora类型的设备
 
         :param request: Request instance for CreateLoraDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateLoraDeviceRequest`
@@ -157,15 +157,15 @@
             model = models.CreateLoraDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultiDevice(self, request):
         """本接口（CreateMultiDevice）用于批量创建物联云设备。
 
         :param request: Request instance for CreateMultiDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateMultiDeviceRequest`
@@ -180,15 +180,15 @@
             model = models.CreateMultiDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultiDevicesTask(self, request):
         """本接口（CreateMultiDevicesTask）用于创建产品级别的批量创建设备任务
 
         :param request: Request instance for CreateMultiDevicesTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateMultiDevicesTaskRequest`
@@ -203,15 +203,15 @@
             model = models.CreateMultiDevicesTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProduct(self, request):
         """本接口（CreateProduct）用于创建一个新的物联网通信产品
 
         :param request: Request instance for CreateProduct.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateProductRequest`
@@ -226,15 +226,15 @@
             model = models.CreateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTask(self, request):
         """本接口（CreateTask）用于创建一个批量任务。目前此接口可以创建批量更新影子以及批量下发消息的任务
 
         :param request: Request instance for CreateTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateTaskRequest`
@@ -249,15 +249,15 @@
             model = models.CreateTaskResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateTaskFileUrlRequest`
@@ -272,15 +272,15 @@
             model = models.CreateTaskFileUrlResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateTopicPolicyRequest`
@@ -295,15 +295,15 @@
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
         """本接口（CreateTopicRule）用于创建一个规则
 
         :param request: Request instance for CreateTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.CreateTopicRuleRequest`
@@ -318,15 +318,15 @@
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
         """本接口（DeleteDevice）用于删除物联网通信设备。
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DeleteDeviceRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDeviceResource(self, request):
         """本接口（DeleteDeviceResource）用于删除设备资源
 
         :param request: Request instance for DeleteDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DeleteDeviceResourceRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoraDevice(self, request):
         """删除lora类型的设备
 
         :param request: Request instance for DeleteLoraDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DeleteLoraDeviceRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteLoraDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProduct(self, request):
         """本接口（DeleteProduct）用于删除一个物联网通信产品
 
         :param request: Request instance for DeleteProduct.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DeleteProductRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopicRule(self, request):
         """本接口（DeleteTopicRule）用于删除规则
 
         :param request: Request instance for DeleteTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DeleteTopicRuleRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllDevices(self, request):
         """查询所有设备列表
 
         :param request: Request instance for DescribeAllDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeAllDevicesRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeAllDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevice(self, request):
         """本接口（DescribeDevice）用于查看设备信息
 
         :param request: Request instance for DescribeDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDeviceRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceClientKey(self, request):
         """获取证书认证类型设备的私钥，刚生成或者重置设备后仅可调用一次
 
         :param request: Request instance for DescribeDeviceClientKey.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDeviceClientKeyRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeDeviceClientKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceResource(self, request):
         """本接口（DescribeDeviceResource）用于查询设备资源详情。
 
         :param request: Request instance for DescribeDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDeviceResourceRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceResources(self, request):
         """本接口（DescribeDeviceResources）用于查询设备资源列表。
 
         :param request: Request instance for DescribeDeviceResources.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDeviceResourcesRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeDeviceResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeviceShadow(self, request):
         """本接口（DescribeDeviceShadow）用于查询虚拟设备信息。
 
         :param request: Request instance for DescribeDeviceShadow.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDeviceShadowRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeDeviceShadowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevices(self, request):
         """本接口（DescribeDevices）用于查询物联网通信设备的设备列表。
 
         :param request: Request instance for DescribeDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeDevicesRequest`
@@ -594,15 +594,15 @@
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
         """查询固件信息
 
         :param request: Request instance for DescribeFirmware.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareRequest`
@@ -617,15 +617,15 @@
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
         """查询固件升级任务详情
 
         :param request: Request instance for DescribeFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareTaskRequest`
@@ -640,15 +640,15 @@
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
         """查询固件升级任务的设备列表
 
         :param request: Request instance for DescribeFirmwareTaskDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareTaskDevicesRequest`
@@ -663,15 +663,15 @@
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
         """查询固件升级任务状态分布
 
         :param request: Request instance for DescribeFirmwareTaskDistribution.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareTaskDistributionRequest`
@@ -686,15 +686,15 @@
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
         """查询固件升级任务统计信息
 
         :param request: Request instance for DescribeFirmwareTaskStatistics.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareTaskStatisticsRequest`
@@ -709,15 +709,15 @@
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
         """查询固件升级任务列表
 
         :param request: Request instance for DescribeFirmwareTasks.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeFirmwareTasksRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeFirmwareTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoraDevice(self, request):
         """获取lora类型设备的详细信息
 
         :param request: Request instance for DescribeLoraDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeLoraDeviceRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeLoraDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMultiDevTask(self, request):
         """本接口（DescribeMultiDevTask）用于查询批量创建设备任务的执行状态。
 
         :param request: Request instance for DescribeMultiDevTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeMultiDevTaskRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeMultiDevTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMultiDevices(self, request):
         """本接口（DescribeMultiDevices）用于查询批量创建设备的执行结果。
 
         :param request: Request instance for DescribeMultiDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeMultiDevicesRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeMultiDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProduct(self, request):
         """本接口（DescribeProduct）用于查看产品详情
 
         :param request: Request instance for DescribeProduct.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductResource(self, request):
         """本接口（DescribeProductResource）用于查询产品资源详情。
 
         :param request: Request instance for DescribeProductResource.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductResourceRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeProductResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductResources(self, request):
         """本接口（DescribeProductResources）用于查询产品资源列表。
 
         :param request: Request instance for DescribeProductResources.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductResourcesRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeProductResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductTask(self, request):
         """本接口（DescribeProductTask）用于查看产品级别的任务信息
 
         :param request: Request instance for DescribeProductTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductTaskRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeProductTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductTasks(self, request):
         """本接口（DescribeProductTasks）用于查看产品级别的任务列表
 
         :param request: Request instance for DescribeProductTasks.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductTasksRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeProductTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProducts(self, request):
         """本接口（DescribeProducts）用于列出产品列表。
 
         :param request: Request instance for DescribeProducts.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeProductsRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePushResourceTaskStatistics(self, request):
         """查询推送资源任务统计信息
 
         :param request: Request instance for DescribePushResourceTaskStatistics.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribePushResourceTaskStatisticsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribePushResourceTaskStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTasks(self, request):
         """查询资源推送任务列表
 
         :param request: Request instance for DescribeResourceTasks.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeResourceTasksRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeResourceTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTask(self, request):
         """本接口（DescribeTask）用于查询一个已创建任务的详情，任务保留一个月
 
         :param request: Request instance for DescribeTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeTaskRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """本接口（DescribeTasks）用于查询已创建的任务列表，任务保留一个月
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DescribeTasksRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableTopicRule(self, request):
         """本接口（DisableTopicRule）用于禁用规则
 
         :param request: Request instance for DisableTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DisableTopicRuleRequest`
@@ -1054,15 +1054,15 @@
             model = models.DisableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadDeviceResource(self, request):
         """本接口（DownloadDeviceResource）用于下载设备资源
 
         :param request: Request instance for DownloadDeviceResource.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.DownloadDeviceResourceRequest`
@@ -1077,15 +1077,15 @@
             model = models.DownloadDeviceResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditFirmware(self, request):
         """编辑固件信息
 
         :param request: Request instance for EditFirmware.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.EditFirmwareRequest`
@@ -1100,15 +1100,15 @@
             model = models.EditFirmwareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableTopicRule(self, request):
         """本接口（EnableTopicRule）用于启用规则
 
         :param request: Request instance for EnableTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.EnableTopicRuleRequest`
@@ -1123,15 +1123,15 @@
             model = models.EnableTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCOSURL(self, request):
         """本接口（GetCOSURL）用于获取固件存储在COS的URL
 
         :param request: Request instance for GetCOSURL.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.GetCOSURLRequest`
@@ -1146,15 +1146,15 @@
             model = models.GetCOSURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetUserResourceInfo(self, request):
         """本接口（GetUserResourceInfo）用于查询用户资源使用信息。
 
         :param request: Request instance for GetUserResourceInfo.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.GetUserResourceInfoRequest`
@@ -1169,15 +1169,15 @@
             model = models.GetUserResourceInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLog(self, request):
         """本接口（ListLog）用于查看日志信息
 
         :param request: Request instance for ListLog.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.ListLogRequest`
@@ -1192,15 +1192,15 @@
             model = models.ListLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListLogPayload(self, request):
         """获取日志内容列表
 
         :param request: Request instance for ListLogPayload.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.ListLogPayloadRequest`
@@ -1215,15 +1215,15 @@
             model = models.ListLogPayloadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListSDKLog(self, request):
         """获取设备上报的日志
 
         :param request: Request instance for ListSDKLog.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.ListSDKLogRequest`
@@ -1238,15 +1238,15 @@
             model = models.ListSDKLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishAsDevice(self, request):
         """模拟lora类型的设备端向服务器端发送消息
 
         :param request: Request instance for PublishAsDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.PublishAsDeviceRequest`
@@ -1261,15 +1261,15 @@
             model = models.PublishAsDeviceResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.PublishBroadcastMessageRequest`
@@ -1284,15 +1284,15 @@
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
         """本接口（PublishMessage）用于向某个主题发消息。
 
         :param request: Request instance for PublishMessage.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.PublishMessageRequest`
@@ -1307,15 +1307,15 @@
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
         """发布RRPC消息
 
         :param request: Request instance for PublishRRPCMessage.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.PublishRRPCMessageRequest`
@@ -1330,15 +1330,15 @@
             model = models.PublishRRPCMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishToDevice(self, request):
         """服务器端下发消息给lora类型的设备
 
         :param request: Request instance for PublishToDevice.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.PublishToDeviceRequest`
@@ -1353,15 +1353,15 @@
             model = models.PublishToDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceTopicRule(self, request):
         """本接口（ReplaceTopicRule）用于修改替换规则
 
         :param request: Request instance for ReplaceTopicRule.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.ReplaceTopicRuleRequest`
@@ -1376,15 +1376,15 @@
             model = models.ReplaceTopicRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDeviceState(self, request):
         """重置设备的连接状态
 
         :param request: Request instance for ResetDeviceState.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.ResetDeviceStateRequest`
@@ -1399,15 +1399,15 @@
             model = models.ResetDeviceStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryDeviceFirmwareTask(self, request):
         """重试设备升级任务
 
         :param request: Request instance for RetryDeviceFirmwareTask.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.RetryDeviceFirmwareTaskRequest`
@@ -1422,15 +1422,15 @@
             model = models.RetryDeviceFirmwareTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetProductsForbiddenStatus(self, request):
         """批量设置产品禁用状态
 
         :param request: Request instance for SetProductsForbiddenStatus.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.SetProductsForbiddenStatusRequest`
@@ -1445,15 +1445,15 @@
             model = models.SetProductsForbiddenStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindDevices(self, request):
         """本接口（UnbindDevices）用于网关设备批量解绑子设备
 
         :param request: Request instance for UnbindDevices.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UnbindDevicesRequest`
@@ -1468,15 +1468,15 @@
             model = models.UnbindDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDeviceAvailableState(self, request):
         """启用或者禁用设备
 
         :param request: Request instance for UpdateDeviceAvailableState.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UpdateDeviceAvailableStateRequest`
@@ -1491,15 +1491,15 @@
             model = models.UpdateDeviceAvailableStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDeviceShadow(self, request):
         """本接口（UpdateDeviceShadow）用于更新虚拟设备信息。
 
         :param request: Request instance for UpdateDeviceShadow.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UpdateDeviceShadowRequest`
@@ -1514,15 +1514,15 @@
             model = models.UpdateDeviceShadowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDevicesEnableState(self, request):
         """批量启用或者禁用设备
 
         :param request: Request instance for UpdateDevicesEnableState.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UpdateDevicesEnableStateRequest`
@@ -1537,15 +1537,15 @@
             model = models.UpdateDevicesEnableStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProductDynamicRegister(self, request):
         """更新产品动态注册的配置
 
         :param request: Request instance for UpdateProductDynamicRegister.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UpdateProductDynamicRegisterRequest`
@@ -1560,15 +1560,15 @@
             model = models.UpdateProductDynamicRegisterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTopicPolicy(self, request):
         """本接口（UpdateTopicPolicy）用于更新Topic信息
 
         :param request: Request instance for UpdateTopicPolicy.
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UpdateTopicPolicyRequest`
@@ -1583,15 +1583,15 @@
             model = models.UpdateTopicPolicyResponse()
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
         :type request: :class:`tencentcloud.iotcloud.v20180614.models.UploadFirmwareRequest`
@@ -1606,8 +1606,8 @@
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

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.938/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.937/README.rst` & `tencentcloud-sdk-python-iotcloud-3.0.938/README.rst`

 * *Files identical despite different names*

