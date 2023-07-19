# Comparing `tmp/tencentcloud-sdk-python-mna-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mna-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.937.tar", last modified: Tue Jul 18 00:27:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.938.tar", last modified: Wed Jul 19 00:42:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mna-3.0.937.tar` & `tencentcloud-sdk-python-mna-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/
--rw-r--r--   0 root         (0) root         (0)    12081 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/mna_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    66678 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:27:23.000000 tencentcloud-sdk-python-mna-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/
+-rw-r--r--   0 root         (0) root         (0)    12133 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/mna_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    66678 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:42:46.000000 tencentcloud-sdk-python-mna-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-mna-3.0.937/setup.py` & `tencentcloud-sdk-python-mna-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mna-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/mna_client.py` & `tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/mna_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEncryptedKey(self, request):
         """通过此接口设置和更新预置密钥
 
         :param request: Request instance for CreateEncryptedKey.
         :type request: :class:`tencentcloud.mna.v20210119.models.CreateEncryptedKeyRequest`
@@ -65,15 +65,15 @@
             model = models.CreateEncryptedKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateQos(self, request):
         """移动网络发起Qos加速过程
 
         :param request: Request instance for CreateQos.
         :type request: :class:`tencentcloud.mna.v20210119.models.CreateQosRequest`
@@ -88,15 +88,15 @@
             model = models.CreateQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDevice(self, request):
         """删除设备信息
 
         :param request: Request instance for DeleteDevice.
         :type request: :class:`tencentcloud.mna.v20210119.models.DeleteDeviceRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteQos(self, request):
         """移动网络停止Qos加速过程
 
         :param request: Request instance for DeleteQos.
         :type request: :class:`tencentcloud.mna.v20210119.models.DeleteQosRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQos(self, request):
         """获取Qos加速状态
 
         :param request: Request instance for DescribeQos.
         :type request: :class:`tencentcloud.mna.v20210119.models.DescribeQosRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeQosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDevice(self, request):
         """通过指定设备的ID查找设备详细信息
 
         :param request: Request instance for GetDevice.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetDeviceRequest`
@@ -180,15 +180,15 @@
             model = models.GetDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDevices(self, request):
         """获取设备信息列表
 
         :param request: Request instance for GetDevices.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetDevicesRequest`
@@ -203,15 +203,15 @@
             model = models.GetDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFlowStatistic(self, request):
         """获取指定设备Id，指定时间点数据流量使用情况
 
         :param request: Request instance for GetFlowStatistic.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetFlowStatisticRequest`
@@ -226,15 +226,15 @@
             model = models.GetFlowStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetMultiFlowStatistic(self, request):
         """批量获取设备流量统计曲线
 
         :param request: Request instance for GetMultiFlowStatistic.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetMultiFlowStatisticRequest`
@@ -249,15 +249,15 @@
             model = models.GetMultiFlowStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPublicKey(self, request):
         """获取公钥用于验签
 
         :param request: Request instance for GetPublicKey.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetPublicKeyRequest`
@@ -272,15 +272,15 @@
             model = models.GetPublicKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetStatisticData(self, request):
         """在用量统计页面下载流量数据
 
         :param request: Request instance for GetStatisticData.
         :type request: :class:`tencentcloud.mna.v20210119.models.GetStatisticDataRequest`
@@ -295,15 +295,15 @@
             model = models.GetStatisticDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDevice(self, request):
         """更新设备信息
 
         :param request: Request instance for UpdateDevice.
         :type request: :class:`tencentcloud.mna.v20210119.models.UpdateDeviceRequest`
@@ -318,8 +318,8 @@
             model = models.UpdateDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/errorcodes.py` & `tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.937/tencentcloud/mna/v20210119/models.py` & `tencentcloud-sdk-python-mna-3.0.938/tencentcloud/mna/v20210119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.937/tencentcloud_sdk_python_mna.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.938/tencentcloud_sdk_python_mna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.937/README.rst` & `tencentcloud-sdk-python-mna-3.0.938/README.rst`

 * *Files identical despite different names*

