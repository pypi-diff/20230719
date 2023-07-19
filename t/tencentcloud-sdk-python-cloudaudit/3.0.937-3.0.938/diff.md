# Comparing `tmp/tencentcloud-sdk-python-cloudaudit-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cloudaudit-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudaudit-3.0.937.tar", last modified: Tue Jul 18 00:20:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudaudit-3.0.938.tar", last modified: Wed Jul 19 00:24:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937.tar` & `tencentcloud-sdk-python-cloudaudit-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18502 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    90257 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-18 00:20:33.000000 tencentcloud-sdk-python-cloudaudit-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90257 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-19 00:24:39.000000 tencentcloud-sdk-python-cloudaudit-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/setup.py` & `tencentcloud-sdk-python-cloudaudit-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             model = models.CreateAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAuditTrack(self, request):
         """创建跟踪集
 
         :param request: Request instance for CreateAuditTrack.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.CreateAuditTrackRequest`
@@ -69,15 +69,15 @@
             model = models.CreateAuditTrackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAudit(self, request):
         """删除跟踪集
 
         :param request: Request instance for DeleteAudit.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DeleteAuditRequest`
@@ -92,15 +92,15 @@
             model = models.DeleteAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAuditTrack(self, request):
         """删除云审计跟踪集
 
         :param request: Request instance for DeleteAuditTrack.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DeleteAuditTrackRequest`
@@ -115,15 +115,15 @@
             model = models.DeleteAuditTrackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAudit(self, request):
         """查询跟踪集详情
 
         :param request: Request instance for DescribeAudit.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DescribeAuditRequest`
@@ -138,15 +138,15 @@
             model = models.DescribeAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditTrack(self, request):
         """查询云审计跟踪集详情
 
         :param request: Request instance for DescribeAuditTrack.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DescribeAuditTrackRequest`
@@ -161,15 +161,15 @@
             model = models.DescribeAuditTrackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditTracks(self, request):
         """查询云审计跟踪集列表
 
         :param request: Request instance for DescribeAuditTracks.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DescribeAuditTracksRequest`
@@ -184,15 +184,15 @@
             model = models.DescribeAuditTracksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEvents(self, request):
         """查询云审计日志
 
         :param request: Request instance for DescribeEvents.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.DescribeEventsRequest`
@@ -207,15 +207,15 @@
             model = models.DescribeEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAttributeKey(self, request):
         """查询AttributeKey的有效取值范围
 
         :param request: Request instance for GetAttributeKey.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.GetAttributeKeyRequest`
@@ -230,15 +230,15 @@
             model = models.GetAttributeKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquireAuditCredit(self, request):
         """查询用户可创建跟踪集的数量
 
         :param request: Request instance for InquireAuditCredit.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.InquireAuditCreditRequest`
@@ -253,15 +253,15 @@
             model = models.InquireAuditCreditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAudits(self, request):
         """查询跟踪集概要
 
         :param request: Request instance for ListAudits.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.ListAuditsRequest`
@@ -276,15 +276,15 @@
             model = models.ListAuditsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListCmqEnableRegion(self, request):
         """查询云审计支持的cmq的可用区
 
         :param request: Request instance for ListCmqEnableRegion.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.ListCmqEnableRegionRequest`
@@ -299,15 +299,15 @@
             model = models.ListCmqEnableRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListCosEnableRegion(self, request):
         """查询云审计支持的cos可用区
 
         :param request: Request instance for ListCosEnableRegion.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.ListCosEnableRegionRequest`
@@ -322,15 +322,15 @@
             model = models.ListCosEnableRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListKeyAliasByRegion(self, request):
         """根据地域获取KMS密钥别名
 
         :param request: Request instance for ListKeyAliasByRegion.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.ListKeyAliasByRegionRequest`
@@ -345,15 +345,15 @@
             model = models.ListKeyAliasByRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LookUpEvents(self, request):
         """用于对操作日志进行检索，便于用户进行查询相关的操作信息。
 
         :param request: Request instance for LookUpEvents.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.LookUpEventsRequest`
@@ -368,15 +368,15 @@
             model = models.LookUpEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAuditTrack(self, request):
         """修改云审计跟踪
 
         :param request: Request instance for ModifyAuditTrack.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.ModifyAuditTrackRequest`
@@ -391,15 +391,15 @@
             model = models.ModifyAuditTrackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartLogging(self, request):
         """开启跟踪集
 
         :param request: Request instance for StartLogging.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.StartLoggingRequest`
@@ -414,15 +414,15 @@
             model = models.StartLoggingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopLogging(self, request):
         """关闭跟踪集
 
         :param request: Request instance for StopLogging.
         :type request: :class:`tencentcloud.cloudaudit.v20190319.models.StopLoggingRequest`
@@ -437,15 +437,15 @@
             model = models.StopLoggingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAudit(self, request):
         """参数要求：
         1、如果IsCreateNewBucket的值存在的话，cosRegion和cosBucketName都是必填参数。
         2、如果IsEnableCmqNotify的值是1的话，IsCreateNewQueue、CmqRegion和CmqQueueName都是必填参数。
         3、如果IsEnableCmqNotify的值是0的话，IsCreateNewQueue、CmqRegion和CmqQueueName都不能传。
@@ -464,8 +464,8 @@
             model = models.UpdateAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/errorcodes.py` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud/cloudaudit/v20190319/models.py` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud/cloudaudit/v20190319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudaudit-3.0.938/tencentcloud_sdk_python_cloudaudit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudaudit
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudaudit SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cloudaudit-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudaudit
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cloudaudit SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudaudit-3.0.937/README.rst` & `tencentcloud-sdk-python-cloudaudit-3.0.938/README.rst`

 * *Files identical despite different names*

