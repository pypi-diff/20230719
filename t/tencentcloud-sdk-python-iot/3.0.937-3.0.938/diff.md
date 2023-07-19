# Comparing `tmp/tencentcloud-sdk-python-iot-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iot-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iot-3.0.937.tar", last modified: Tue Jul 18 00:25:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iot-3.0.938.tar", last modified: Wed Jul 19 00:41:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iot-3.0.937.tar` & `tencentcloud-sdk-python-iot-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6163 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   171391 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/models.py
--rw-r--r--   0 root         (0) root         (0)    40724 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/iot_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:25:39.000000 tencentcloud-sdk-python-iot-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   171391 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/models.py
+-rw-r--r--   0 root         (0) root         (0)    40904 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/iot_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:41:02.000000 tencentcloud-sdk-python-iot-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-iot-3.0.937/setup.py` & `tencentcloud-sdk-python-iot-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.937/tencentcloud_sdk_python_iot.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iot-3.0.938/tencentcloud_sdk_python_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iot
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iot SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iot-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iot-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/errorcodes.py` & `tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/models.py` & `tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iot-3.0.937/tencentcloud/iot/v20180123/iot_client.py` & `tencentcloud-sdk-python-iot-3.0.938/tencentcloud/iot/v20180123/iot_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ActivateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddDevice(self, request):
         """提供在指定的产品Id下创建一个设备的能力，生成设备名称与设备秘钥。
 
         :param request: Request instance for AddDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.AddDeviceRequest`
@@ -65,15 +65,15 @@
             model = models.AddDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddProduct(self, request):
         """本接口(AddProduct)用于创建、定义某款硬件产品。
 
         :param request: Request instance for AddProduct.
         :type request: :class:`tencentcloud.iot.v20180123.models.AddProductRequest`
@@ -88,15 +88,15 @@
             model = models.AddProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddRule(self, request):
         """新增规则
 
         :param request: Request instance for AddRule.
         :type request: :class:`tencentcloud.iot.v20180123.models.AddRuleRequest`
@@ -111,15 +111,15 @@
             model = models.AddRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddTopic(self, request):
         """新增Topic，用于设备或应用发布消息至该Topic或订阅该Topic的消息。
 
         :param request: Request instance for AddTopic.
         :type request: :class:`tencentcloud.iot.v20180123.models.AddTopicRequest`
@@ -134,15 +134,15 @@
             model = models.AddTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppAddUser(self, request):
         """为APP提供用户注册功能
 
         :param request: Request instance for AppAddUser.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppAddUserRequest`
@@ -157,15 +157,15 @@
             model = models.AppAddUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppDeleteDevice(self, request):
         """用户解除与设备的关联关系，解除后APP用户无法控制设备，获取设备数据
 
         :param request: Request instance for AppDeleteDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppDeleteDeviceRequest`
@@ -180,15 +180,15 @@
             model = models.AppDeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetDevice(self, request):
         """获取绑定设备的基本信息与数据模板定义
 
         :param request: Request instance for AppGetDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetDeviceRequest`
@@ -203,15 +203,15 @@
             model = models.AppGetDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetDeviceData(self, request):
         """获取绑定设备数据，用于实时展示设备的最新数据
 
         :param request: Request instance for AppGetDeviceData.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetDeviceDataRequest`
@@ -226,15 +226,15 @@
             model = models.AppGetDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetDeviceStatuses(self, request):
         """获取绑定设备的上下线状态
 
         :param request: Request instance for AppGetDeviceStatuses.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetDeviceStatusesRequest`
@@ -249,15 +249,15 @@
             model = models.AppGetDeviceStatusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetDevices(self, request):
         """获取用户的绑定设备列表
 
         :param request: Request instance for AppGetDevices.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetDevicesRequest`
@@ -272,15 +272,15 @@
             model = models.AppGetDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetToken(self, request):
         """获取用户token
 
         :param request: Request instance for AppGetToken.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetTokenRequest`
@@ -295,15 +295,15 @@
             model = models.AppGetTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppGetUser(self, request):
         """获取用户信息
 
         :param request: Request instance for AppGetUser.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppGetUserRequest`
@@ -318,15 +318,15 @@
             model = models.AppGetUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppIssueDeviceControl(self, request):
         """用户通过APP控制设备
 
         :param request: Request instance for AppIssueDeviceControl.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppIssueDeviceControlRequest`
@@ -341,15 +341,15 @@
             model = models.AppIssueDeviceControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppResetPassword(self, request):
         """重置APP用户密码
 
         :param request: Request instance for AppResetPassword.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppResetPasswordRequest`
@@ -364,15 +364,15 @@
             model = models.AppResetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppSecureAddDevice(self, request):
         """用户绑定设备，绑定后可以在APP端进行控制。绑定设备前需调用“获取设备绑定签名”接口
 
         :param request: Request instance for AppSecureAddDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppSecureAddDeviceRequest`
@@ -387,15 +387,15 @@
             model = models.AppSecureAddDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppUpdateDevice(self, request):
         """修改设备别名，便于用户个性化定义设备的名称
 
         :param request: Request instance for AppUpdateDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppUpdateDeviceRequest`
@@ -410,15 +410,15 @@
             model = models.AppUpdateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AppUpdateUser(self, request):
         """修改用户信息
 
         :param request: Request instance for AppUpdateUser.
         :type request: :class:`tencentcloud.iot.v20180123.models.AppUpdateUserRequest`
@@ -433,15 +433,15 @@
             model = models.AppUpdateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSubDeviceToGatewayProduct(self, request):
         """关联子设备产品和网关产品
 
         :param request: Request instance for AssociateSubDeviceToGatewayProduct.
         :type request: :class:`tencentcloud.iot.v20180123.models.AssociateSubDeviceToGatewayProductRequest`
@@ -456,15 +456,15 @@
             model = models.AssociateSubDeviceToGatewayProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeactivateRule(self, request):
         """禁用规则
 
         :param request: Request instance for DeactivateRule.
         :type request: :class:`tencentcloud.iot.v20180123.models.DeactivateRuleRequest`
@@ -479,15 +479,15 @@
             model = models.DeactivateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDevice(self, request):
         """提供在指定的产品Id下删除一个设备的能力。
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.DeleteDeviceRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProduct(self, request):
         """删除用户指定的产品Id对应的信息。
 
         :param request: Request instance for DeleteProduct.
         :type request: :class:`tencentcloud.iot.v20180123.models.DeleteProductRequest`
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
 
 
     def DeleteRule(self, request):
         """删除规则
 
         :param request: Request instance for DeleteRule.
         :type request: :class:`tencentcloud.iot.v20180123.models.DeleteRuleRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopic(self, request):
         """删除Topic
 
         :param request: Request instance for DeleteTopic.
         :type request: :class:`tencentcloud.iot.v20180123.models.DeleteTopicRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDataHistory(self, request):
         """批量获取设备某一段时间范围的设备上报数据。该接口适用于使用高级版类型的产品
 
         :param request: Request instance for GetDataHistory.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDataHistoryRequest`
@@ -594,15 +594,15 @@
             model = models.GetDataHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDebugLog(self, request):
         """获取设备的调试日志，用于定位问题
 
         :param request: Request instance for GetDebugLog.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDebugLogRequest`
@@ -617,15 +617,15 @@
             model = models.GetDebugLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDevice(self, request):
         """提供查询某个设备详细信息的能力。
 
         :param request: Request instance for GetDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceRequest`
@@ -640,15 +640,15 @@
             model = models.GetDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceData(self, request):
         """获取某个设备当前上报到云端的数据，该接口适用于使用数据模板协议的产品。
 
         :param request: Request instance for GetDeviceData.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceDataRequest`
@@ -663,15 +663,15 @@
             model = models.GetDeviceDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceLog(self, request):
         """批量获取设备与云端的详细通信日志，该接口适用于使用高级版类型的产品。
 
         :param request: Request instance for GetDeviceLog.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceLogRequest`
@@ -686,15 +686,15 @@
             model = models.GetDeviceLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceSignatures(self, request):
         """获取设备绑定签名，用于用户绑定某个设备的应用场景
 
         :param request: Request instance for GetDeviceSignatures.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceSignaturesRequest`
@@ -709,15 +709,15 @@
             model = models.GetDeviceSignaturesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceStatistics(self, request):
         """查询某段时间范围内产品的在线、激活设备数
 
         :param request: Request instance for GetDeviceStatistics.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceStatisticsRequest`
@@ -732,15 +732,15 @@
             model = models.GetDeviceStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDeviceStatuses(self, request):
         """批量获取设备的当前状态，状态包括在线、离线或未激活状态。
 
         :param request: Request instance for GetDeviceStatuses.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDeviceStatusesRequest`
@@ -755,15 +755,15 @@
             model = models.GetDeviceStatusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDevices(self, request):
         """提供分页查询某个产品Id下设备信息的能力。
 
         :param request: Request instance for GetDevices.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetDevicesRequest`
@@ -778,15 +778,15 @@
             model = models.GetDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetProduct(self, request):
         """获取产品定义的详细信息，包括产品名称、产品描述，鉴权模式等信息。
 
         :param request: Request instance for GetProduct.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetProductRequest`
@@ -801,15 +801,15 @@
             model = models.GetProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetProducts(self, request):
         """获取用户在物联网套件所创建的所有产品信息。
 
         :param request: Request instance for GetProducts.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetProductsRequest`
@@ -824,15 +824,15 @@
             model = models.GetProductsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRule(self, request):
         """获取转发规则信息
 
         :param request: Request instance for GetRule.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetRuleRequest`
@@ -847,15 +847,15 @@
             model = models.GetRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRules(self, request):
         """获取转发规则列表
 
         :param request: Request instance for GetRules.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetRulesRequest`
@@ -870,15 +870,15 @@
             model = models.GetRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTopic(self, request):
         """获取Topic信息
 
         :param request: Request instance for GetTopic.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetTopicRequest`
@@ -893,15 +893,15 @@
             model = models.GetTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTopics(self, request):
         """获取Topic列表
 
         :param request: Request instance for GetTopics.
         :type request: :class:`tencentcloud.iot.v20180123.models.GetTopicsRequest`
@@ -916,15 +916,15 @@
             model = models.GetTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IssueDeviceControl(self, request):
         """提供下发控制指令到指定设备的能力，该接口适用于使用高级版类型的产品。
 
         :param request: Request instance for IssueDeviceControl.
         :type request: :class:`tencentcloud.iot.v20180123.models.IssueDeviceControlRequest`
@@ -939,15 +939,15 @@
             model = models.IssueDeviceControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishMsg(self, request):
         """提供向指定的Topic发布消息的能力，常用于向设备下发控制指令。该接口只适用于产品版本为“基础版”类型的产品，使用高级版的产品需使用“下发设备控制指令”接口
 
         :param request: Request instance for PublishMsg.
         :type request: :class:`tencentcloud.iot.v20180123.models.PublishMsgRequest`
@@ -962,15 +962,15 @@
             model = models.PublishMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDevice(self, request):
         """重置设备操作，将会为设备生成新的证书及清空最新数据，需谨慎操作。
 
         :param request: Request instance for ResetDevice.
         :type request: :class:`tencentcloud.iot.v20180123.models.ResetDeviceRequest`
@@ -985,15 +985,15 @@
             model = models.ResetDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnassociateSubDeviceFromGatewayProduct(self, request):
         """业务无客户使用，下线接口。
 
         取消子设备产品与网关设备产品的关联
 
@@ -1010,15 +1010,15 @@
             model = models.UnassociateSubDeviceFromGatewayProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProduct(self, request):
         """提供修改产品信息及数据模板的能力。
 
         :param request: Request instance for UpdateProduct.
         :type request: :class:`tencentcloud.iot.v20180123.models.UpdateProductRequest`
@@ -1033,15 +1033,15 @@
             model = models.UpdateProductResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRule(self, request):
         """更新规则
 
         :param request: Request instance for UpdateRule.
         :type request: :class:`tencentcloud.iot.v20180123.models.UpdateRuleRequest`
@@ -1056,8 +1056,8 @@
             model = models.UpdateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iot-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iot-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iot
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iot SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iot-3.0.937/README.rst` & `tencentcloud-sdk-python-iot-3.0.938/README.rst`

 * *Files identical despite different names*

