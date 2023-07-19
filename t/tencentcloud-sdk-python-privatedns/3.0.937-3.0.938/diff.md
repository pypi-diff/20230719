# Comparing `tmp/tencentcloud-sdk-python-privatedns-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-privatedns-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.937.tar", last modified: Tue Jul 18 00:28:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.938.tar", last modified: Wed Jul 19 00:44:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-privatedns-3.0.937.tar` & `tencentcloud-sdk-python-privatedns-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21077 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/privatedns_client.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    91015 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-18 00:28:51.000000 tencentcloud-sdk-python-privatedns-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21165 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/privatedns_client.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    91015 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-19 00:44:11.000000 tencentcloud-sdk-python-privatedns-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/setup.py` & `tencentcloud-sdk-python-privatedns-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/privatedns_client.py` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/privatedns_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreatePrivateDNSAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrivateZone(self, request):
         """创建私有域
 
         :param request: Request instance for CreatePrivateZone.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.CreatePrivateZoneRequest`
@@ -65,15 +65,15 @@
             model = models.CreatePrivateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrivateZoneRecord(self, request):
         """添加私有域解析记录
 
         :param request: Request instance for CreatePrivateZoneRecord.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.CreatePrivateZoneRecordRequest`
@@ -88,15 +88,15 @@
             model = models.CreatePrivateZoneRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEndPoint(self, request):
         """删除终端节点
 
         :param request: Request instance for DeleteEndPoint.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DeleteEndPointRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteEndPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivateDNSAccount(self, request):
         """删除私有域解析账号
 
         :param request: Request instance for DeletePrivateDNSAccount.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DeletePrivateDNSAccountRequest`
@@ -134,15 +134,15 @@
             model = models.DeletePrivateDNSAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivateZone(self, request):
         """删除私有域并停止解析
 
         :param request: Request instance for DeletePrivateZone.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DeletePrivateZoneRequest`
@@ -157,15 +157,15 @@
             model = models.DeletePrivateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrivateZoneRecord(self, request):
         """删除私有域解析记录
 
         :param request: Request instance for DeletePrivateZoneRecord.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DeletePrivateZoneRecordRequest`
@@ -180,15 +180,15 @@
             model = models.DeletePrivateZoneRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountVpcList(self, request):
         """获取私有域解析账号的VPC列表
 
         :param request: Request instance for DescribeAccountVpcList.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribeAccountVpcListRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeAccountVpcListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditLog(self, request):
         """获取操作日志列表
 
         :param request: Request instance for DescribeAuditLog.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribeAuditLogRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeAuditLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDashboard(self, request):
         """获取私有域解析概览
 
         :param request: Request instance for DescribeDashboard.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribeDashboardRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateDNSAccountList(self, request):
         """获取私有域解析账号列表
 
         :param request: Request instance for DescribePrivateDNSAccountList.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribePrivateDNSAccountListRequest`
@@ -272,15 +272,15 @@
             model = models.DescribePrivateDNSAccountListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateZone(self, request):
         """获取私有域信息
 
         :param request: Request instance for DescribePrivateZone.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribePrivateZoneRequest`
@@ -295,15 +295,15 @@
             model = models.DescribePrivateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateZoneList(self, request):
         """获取私有域列表
 
         :param request: Request instance for DescribePrivateZoneList.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribePrivateZoneListRequest`
@@ -318,15 +318,15 @@
             model = models.DescribePrivateZoneListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateZoneRecordList(self, request):
         """获取私有域记录列表
 
         :param request: Request instance for DescribePrivateZoneRecordList.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribePrivateZoneRecordListRequest`
@@ -341,15 +341,15 @@
             model = models.DescribePrivateZoneRecordListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrivateZoneService(self, request):
         """查询私有域解析开通状态
 
         :param request: Request instance for DescribePrivateZoneService.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribePrivateZoneServiceRequest`
@@ -364,15 +364,15 @@
             model = models.DescribePrivateZoneServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQuotaUsage(self, request):
         """查询额度使用情况
 
         :param request: Request instance for DescribeQuotaUsage.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribeQuotaUsageRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeQuotaUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRequestData(self, request):
         """获取私有域解析请求量
 
         :param request: Request instance for DescribeRequestData.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DescribeRequestDataRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeRequestDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrivateZone(self, request):
         """修改私有域信息
 
         :param request: Request instance for ModifyPrivateZone.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.ModifyPrivateZoneRequest`
@@ -433,15 +433,15 @@
             model = models.ModifyPrivateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrivateZoneRecord(self, request):
         """修改私有域解析记录
 
         :param request: Request instance for ModifyPrivateZoneRecord.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.ModifyPrivateZoneRecordRequest`
@@ -456,15 +456,15 @@
             model = models.ModifyPrivateZoneRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrivateZoneVpc(self, request):
         """修改私有域关联的VPC
 
         :param request: Request instance for ModifyPrivateZoneVpc.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.ModifyPrivateZoneVpcRequest`
@@ -479,15 +479,15 @@
             model = models.ModifyPrivateZoneVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordsStatus(self, request):
         """修改解析记录状态
 
         :param request: Request instance for ModifyRecordsStatus.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.ModifyRecordsStatusRequest`
@@ -502,15 +502,15 @@
             model = models.ModifyRecordsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubscribePrivateZoneService(self, request):
         """开通私有域解析
 
         :param request: Request instance for SubscribePrivateZoneService.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.SubscribePrivateZoneServiceRequest`
@@ -525,8 +525,8 @@
             model = models.SubscribePrivateZoneServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/errorcodes.py` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud/privatedns/v20201028/models.py` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud/privatedns/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.938/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.937/README.rst` & `tencentcloud-sdk-python-privatedns-3.0.938/README.rst`

 * *Files identical despite different names*

