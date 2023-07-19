# Comparing `tmp/tencentcloud-sdk-python-cloudhsm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cloudhsm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudhsm-3.0.937.tar", last modified: Tue Jul 18 00:20:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudhsm-3.0.938.tar", last modified: Wed Jul 19 00:24:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937.tar` & `tencentcloud-sdk-python-cloudhsm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/
--rw-r--r--   0 root         (0) root         (0)    13291 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    81651 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:20:38.000000 tencentcloud-sdk-python-cloudhsm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/
+-rw-r--r--   0 root         (0) root         (0)    13347 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    81651 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:24:44.000000 tencentcloud-sdk-python-cloudhsm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/setup.py` & `tencentcloud-sdk-python-cloudhsm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudhsm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudhsm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py` & `tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeHSMBySubnetIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHSMByVpcId(self, request):
         """通过VpcId获取Hsm资源数
 
         :param request: Request instance for DescribeHSMByVpcId.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeHSMByVpcIdRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeHSMByVpcIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubnet(self, request):
         """查询子网列表
 
         :param request: Request instance for DescribeSubnet.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeSubnetRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeSubnetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSupportedHsm(self, request):
         """获取当前地域所支持的设备列表
 
         :param request: Request instance for DescribeSupportedHsm.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeSupportedHsmRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeSupportedHsmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsg(self, request):
         """根据用户的AppId获取用户安全组列表
 
         :param request: Request instance for DescribeUsg.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeUsgRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeUsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsgRule(self, request):
         """获取安全组详情
 
         :param request: Request instance for DescribeUsgRule.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeUsgRuleRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeUsgRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpc(self, request):
         """查询用户的私有网络列表
 
         :param request: Request instance for DescribeVpc.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeVpcRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVsmAttributes(self, request):
         """获取VSM属性
 
         :param request: Request instance for DescribeVsmAttributes.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeVsmAttributesRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeVsmAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVsms(self, request):
         """获取用户VSM列表
 
         :param request: Request instance for DescribeVsms.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.DescribeVsmsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeVsmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAlarmEvent(self, request):
         """获取告警事件
 
         :param request: Request instance for GetAlarmEvent.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.GetAlarmEventRequest`
@@ -249,15 +249,15 @@
             model = models.GetAlarmEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetVsmMonitorInfo(self, request):
         """获取VSM监控信息
 
         :param request: Request instance for GetVsmMonitorInfo.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.GetVsmMonitorInfoRequest`
@@ -272,15 +272,15 @@
             model = models.GetVsmMonitorInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceBuyVsm(self, request):
         """购买询价接口
 
         :param request: Request instance for InquiryPriceBuyVsm.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.InquiryPriceBuyVsmRequest`
@@ -295,15 +295,15 @@
             model = models.InquiryPriceBuyVsmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmEvent(self, request):
         """修改告警事件
 
         :param request: Request instance for ModifyAlarmEvent.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.ModifyAlarmEventRequest`
@@ -318,15 +318,15 @@
             model = models.ModifyAlarmEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVsmAttributes(self, request):
         """修改VSM属性
 
         :param request: Request instance for ModifyVsmAttributes.
         :type request: :class:`tencentcloud.cloudhsm.v20191112.models.ModifyVsmAttributesRequest`
@@ -341,8 +341,8 @@
             model = models.ModifyVsmAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/errorcodes.py` & `tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/tencentcloud/cloudhsm/v20191112/models.py` & `tencentcloud-sdk-python-cloudhsm-3.0.938/tencentcloud/cloudhsm/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cloudhsm-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudhsm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudhsm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.937/README.rst` & `tencentcloud-sdk-python-cloudhsm-3.0.938/README.rst`

 * *Files identical despite different names*

