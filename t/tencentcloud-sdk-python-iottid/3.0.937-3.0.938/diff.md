# Comparing `tmp/tencentcloud-sdk-python-iottid-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iottid-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.937.tar", last modified: Tue Jul 18 00:25:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.938.tar", last modified: Wed Jul 19 00:41:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iottid-3.0.937.tar` & `tencentcloud-sdk-python-iottid-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9130 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/iottid_client.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23421 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:25:54.000000 tencentcloud-sdk-python-iottid-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9166 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/iottid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23421 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:41:18.000000 tencentcloud-sdk-python-iottid-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/setup.py` & `tencentcloud-sdk-python-iottid-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/iottid_client.py` & `tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/iottid_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AuthTestTidResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BurnTidNotify(self, request):
         """安全芯片TID烧录回执
 
         :param request: Request instance for BurnTidNotify.
         :type request: :class:`tencentcloud.iottid.v20190411.models.BurnTidNotifyRequest`
@@ -65,15 +65,15 @@
             model = models.BurnTidNotifyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeliverTidNotify(self, request):
         """安全芯片为载体的TID空发回执，绑定TID与订单号。
 
         :param request: Request instance for DeliverTidNotify.
         :type request: :class:`tencentcloud.iottid.v20190411.models.DeliverTidNotifyRequest`
@@ -88,15 +88,15 @@
             model = models.DeliverTidNotifyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeliverTids(self, request):
         """设备服务商请求空发产品订单的TID信息
 
         :param request: Request instance for DeliverTids.
         :type request: :class:`tencentcloud.iottid.v20190411.models.DeliverTidsRequest`
@@ -111,15 +111,15 @@
             model = models.DeliverTidsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableLibCount(self, request):
         """查询指定订单的可空发的白盒密钥数量
 
         :param request: Request instance for DescribeAvailableLibCount.
         :type request: :class:`tencentcloud.iottid.v20190411.models.DescribeAvailableLibCountRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeAvailableLibCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePermission(self, request):
         """查询企业用户TID平台控制台权限
 
         :param request: Request instance for DescribePermission.
         :type request: :class:`tencentcloud.iottid.v20190411.models.DescribePermissionRequest`
@@ -157,15 +157,15 @@
             model = models.DescribePermissionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadTids(self, request):
         """下载芯片订单的TID
 
         :param request: Request instance for DownloadTids.
         :type request: :class:`tencentcloud.iottid.v20190411.models.DownloadTidsRequest`
@@ -180,15 +180,15 @@
             model = models.DownloadTidsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadDeviceUniqueCode(self, request):
         """上传硬件唯一标识码，是软加固设备身份参数。本接口如遇到错误数据，则所有当次上传数据失效。
 
         :param request: Request instance for UploadDeviceUniqueCode.
         :type request: :class:`tencentcloud.iottid.v20190411.models.UploadDeviceUniqueCodeRequest`
@@ -203,15 +203,15 @@
             model = models.UploadDeviceUniqueCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyChipBurnInfo(self, request):
         """下载控制台验证芯片烧录信息，保证TID与中心信息一致
 
         :param request: Request instance for VerifyChipBurnInfo.
         :type request: :class:`tencentcloud.iottid.v20190411.models.VerifyChipBurnInfoRequest`
@@ -226,8 +226,8 @@
             model = models.VerifyChipBurnInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/errorcodes.py` & `tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/tencentcloud/iottid/v20190411/models.py` & `tencentcloud-sdk-python-iottid-3.0.938/tencentcloud/iottid/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.938/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.937/README.rst` & `tencentcloud-sdk-python-iottid-3.0.938/README.rst`

 * *Files identical despite different names*

