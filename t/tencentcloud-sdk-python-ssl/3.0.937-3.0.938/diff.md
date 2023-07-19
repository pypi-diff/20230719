# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.937.tar", last modified: Tue Jul 18 00:30:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.938.tar", last modified: Wed Jul 19 00:45:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.937.tar` & `tencentcloud-sdk-python-ssl-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9587 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   366108 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    49507 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:20.000000 tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9587 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   366108 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    49715 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:33.000000 tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/setup.py` & `tencentcloud-sdk-python-ssl-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.938/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelCertificateOrder(self, request):
         """取消证书订单。
 
         :param request: Request instance for CancelCertificateOrder.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CancelCertificateOrderRequest`
@@ -65,15 +65,15 @@
             model = models.CancelCertificateOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckCertificateChain(self, request):
         """本接口（CheckCertificateChain）用于检查证书链是否完整。
 
         :param request: Request instance for CheckCertificateChain.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CheckCertificateChainRequest`
@@ -88,15 +88,15 @@
             model = models.CheckCertificateChainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CommitCertificateInformation(self, request):
         """提交证书订单。
 
         :param request: Request instance for CommitCertificateInformation.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CommitCertificateInformationRequest`
@@ -111,15 +111,15 @@
             model = models.CommitCertificateInformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompleteCertificate(self, request):
         """本接口（CompleteCertificate）用于主动触发证书验证。仅非DNSPod和Wotrus品牌证书支持使用此接口。
 
         :param request: Request instance for CompleteCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CompleteCertificateRequest`
@@ -134,15 +134,15 @@
             model = models.CompleteCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCertificate(self, request):
         """本接口（CreateCertificate）用于创建付费证书。
 
         :param request: Request instance for CreateCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CreateCertificateRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCertificateByPackage(self, request):
         """使用权益点创建证书
 
         :param request: Request instance for CreateCertificateByPackage.
         :type request: :class:`tencentcloud.ssl.v20191205.models.CreateCertificateByPackageRequest`
@@ -180,15 +180,15 @@
             model = models.CreateCertificateByPackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCertificate(self, request):
         """本接口（DeleteCertificate）用于删除证书。
 
         :param request: Request instance for DeleteCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeleteCertificateRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteManager(self, request):
         """删除管理人
 
         :param request: Request instance for DeleteManager.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeleteManagerRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteManagerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployCertificateInstance(self, request):
         """证书部署到云资源实例列表
 
         :param request: Request instance for DeployCertificateInstance.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateInstanceRequest`
@@ -249,15 +249,15 @@
             model = models.DeployCertificateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployCertificateRecordRetry(self, request):
         """云资源部署重试部署记录
 
         :param request: Request instance for DeployCertificateRecordRetry.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRetryRequest`
@@ -272,15 +272,15 @@
             model = models.DeployCertificateRecordRetryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployCertificateRecordRollback(self, request):
         """云资源部署一键回滚
 
         :param request: Request instance for DeployCertificateRecordRollback.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DeployCertificateRecordRollbackRequest`
@@ -295,15 +295,15 @@
             model = models.DeployCertificateRecordRollbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificate(self, request):
         """本接口（DescribeCertificate）用于获取证书信息。
 
         :param request: Request instance for DescribeCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificateRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificateDetail(self, request):
         """获取证书详情。
 
         :param request: Request instance for DescribeCertificateDetail.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificateDetailRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeCertificateDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificateOperateLogs(self, request):
         """获取用户账号下有关证书的操作日志。
 
         :param request: Request instance for DescribeCertificateOperateLogs.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificateOperateLogsRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeCertificateOperateLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificates(self, request):
         """本接口（DescribeCertificates）用于获取证书列表。
 
         :param request: Request instance for DescribeCertificates.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCertificatesRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeCertificatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompanies(self, request):
         """查询公司列表
 
         :param request: Request instance for DescribeCompanies.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCompaniesRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeCompaniesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeployedResources(self, request):
         """证书查询关联资源
 
         :param request: Request instance for DescribeDeployedResources.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeDeployedResourcesRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeDeployedResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostApiGatewayInstanceList(self, request):
         """查询证书apiGateway云资源部署实例列表
 
         :param request: Request instance for DescribeHostApiGatewayInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostApiGatewayInstanceListRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeHostApiGatewayInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostCdnInstanceList(self, request):
         """查询证书cdn云资源部署实例列表
 
         :param request: Request instance for DescribeHostCdnInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCdnInstanceListRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeHostCdnInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostClbInstanceList(self, request):
         """查询证书clb云资源部署实例列表
 
         :param request: Request instance for DescribeHostClbInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostClbInstanceListRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeHostClbInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostCosInstanceList(self, request):
         """查询证书cos云资源部署实例列表
 
         :param request: Request instance for DescribeHostCosInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostCosInstanceListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeHostCosInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostDdosInstanceList(self, request):
         """查询证书ddos云资源部署实例列表
 
         :param request: Request instance for DescribeHostDdosInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDdosInstanceListRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeHostDdosInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostDeployRecord(self, request):
         """查询证书云资源部署记录列表
 
         :param request: Request instance for DescribeHostDeployRecord.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeHostDeployRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostDeployRecordDetail(self, request):
         """查询证书云资源部署记录详情列表
 
         :param request: Request instance for DescribeHostDeployRecordDetail.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostDeployRecordDetailRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeHostDeployRecordDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostLighthouseInstanceList(self, request):
         """查询证书Lighthouse云资源部署实例列表
 
         :param request: Request instance for DescribeHostLighthouseInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLighthouseInstanceListRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeHostLighthouseInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostLiveInstanceList(self, request):
         """查询证书live云资源部署实例列表
 
         :param request: Request instance for DescribeHostLiveInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostLiveInstanceListRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeHostLiveInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostTeoInstanceList(self, request):
         """查询证书EdgeOne云资源部署实例列表
 
         :param request: Request instance for DescribeHostTeoInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTeoInstanceListRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeHostTeoInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostTkeInstanceList(self, request):
         """查询证书tke云资源部署实例列表
 
         :param request: Request instance for DescribeHostTkeInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostTkeInstanceListRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeHostTkeInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostUpdateRecord(self, request):
         """查询证书云资源更新记录列表
 
         :param request: Request instance for DescribeHostUpdateRecord.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeHostUpdateRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostUpdateRecordDetail(self, request):
         """查询证书云资源更新记录详情列表
 
         :param request: Request instance for DescribeHostUpdateRecordDetail.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostUpdateRecordDetailRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeHostUpdateRecordDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostVodInstanceList(self, request):
         """查询证书Vod云资源部署实例列表
 
         :param request: Request instance for DescribeHostVodInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostVodInstanceListRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeHostVodInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostWafInstanceList(self, request):
         """查询证书waf云资源部署实例列表
 
         :param request: Request instance for DescribeHostWafInstanceList.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeHostWafInstanceListRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeHostWafInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeManagerDetail(self, request):
         """查询管理人详情
 
         :param request: Request instance for DescribeManagerDetail.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeManagerDetailRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeManagerDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeManagers(self, request):
         """查询管理人列表
 
         :param request: Request instance for DescribeManagers.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeManagersRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeManagersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackages(self, request):
         """获得权益包列表
 
         :param request: Request instance for DescribePackages.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribePackagesRequest`
@@ -847,15 +847,15 @@
             model = models.DescribePackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadCertificate(self, request):
         """本接口（DownloadCertificate）用于下载证书。
 
         :param request: Request instance for DownloadCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DownloadCertificateRequest`
@@ -870,15 +870,15 @@
             model = models.DownloadCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def HostCertificate(self, request):
         """云资源托管
 
         :param request: Request instance for HostCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.HostCertificateRequest`
@@ -893,15 +893,15 @@
             model = models.HostCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCertificateAlias(self, request):
         """用户传入证书id和备注来修改证书备注。
 
         :param request: Request instance for ModifyCertificateAlias.
         :type request: :class:`tencentcloud.ssl.v20191205.models.ModifyCertificateAliasRequest`
@@ -916,15 +916,15 @@
             model = models.ModifyCertificateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCertificateProject(self, request):
         """批量修改证书所属项目。
 
         :param request: Request instance for ModifyCertificateProject.
         :type request: :class:`tencentcloud.ssl.v20191205.models.ModifyCertificateProjectRequest`
@@ -939,15 +939,15 @@
             model = models.ModifyCertificateProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCertificatesExpiringNotificationSwitch(self, request):
         """修改忽略证书到期通知。打开或关闭证书到期通知。
 
         :param request: Request instance for ModifyCertificatesExpiringNotificationSwitch.
         :type request: :class:`tencentcloud.ssl.v20191205.models.ModifyCertificatesExpiringNotificationSwitchRequest`
@@ -962,15 +962,15 @@
             model = models.ModifyCertificatesExpiringNotificationSwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceCertificate(self, request):
         """本接口（ReplaceCertificate）用于重颁发证书。已申请的免费证书仅支持 RSA 算法、密钥对参数为2048的证书重颁发，并且目前仅支持1次重颁发。
 
         :param request: Request instance for ReplaceCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.ReplaceCertificateRequest`
@@ -985,15 +985,15 @@
             model = models.ReplaceCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeCertificate(self, request):
         """本接口（RevokeCertificate）用于吊销证书。
 
         :param request: Request instance for RevokeCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.RevokeCertificateRequest`
@@ -1008,15 +1008,15 @@
             model = models.RevokeCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitAuditManager(self, request):
         """重新提交审核管理人
 
         :param request: Request instance for SubmitAuditManager.
         :type request: :class:`tencentcloud.ssl.v20191205.models.SubmitAuditManagerRequest`
@@ -1031,15 +1031,15 @@
             model = models.SubmitAuditManagerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SubmitCertificateInformation(self, request):
         """提交证书资料。输入参数信息可以分多次提交，但提交的证书资料应最低限度保持完整。
 
         :param request: Request instance for SubmitCertificateInformation.
         :type request: :class:`tencentcloud.ssl.v20191205.models.SubmitCertificateInformationRequest`
@@ -1054,15 +1054,15 @@
             model = models.SubmitCertificateInformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCertificateInstance(self, request):
         """一键更新旧证书资源
 
         :param request: Request instance for UpdateCertificateInstance.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateInstanceRequest`
@@ -1077,15 +1077,15 @@
             model = models.UpdateCertificateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCertificateRecordRetry(self, request):
         """云资源更新重试部署记录
 
         :param request: Request instance for UpdateCertificateRecordRetry.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRetryRequest`
@@ -1100,15 +1100,15 @@
             model = models.UpdateCertificateRecordRetryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCertificateRecordRollback(self, request):
         """云资源更新一键回滚
 
         :param request: Request instance for UpdateCertificateRecordRollback.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UpdateCertificateRecordRollbackRequest`
@@ -1123,15 +1123,15 @@
             model = models.UpdateCertificateRecordRollbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadCertificate(self, request):
         """本接口（UploadCertificate）用于上传证书。
 
         :param request: Request instance for UploadCertificate.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UploadCertificateRequest`
@@ -1146,15 +1146,15 @@
             model = models.UploadCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadConfirmLetter(self, request):
         """本接口（UploadConfirmLetter）用于上传证书确认函。
 
         :param request: Request instance for UploadConfirmLetter.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UploadConfirmLetterRequest`
@@ -1169,15 +1169,15 @@
             model = models.UploadConfirmLetterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadRevokeLetter(self, request):
         """本接口（UploadRevokeLetter）用于上传证书吊销确认函。
 
         :param request: Request instance for UploadRevokeLetter.
         :type request: :class:`tencentcloud.ssl.v20191205.models.UploadRevokeLetterRequest`
@@ -1192,15 +1192,15 @@
             model = models.UploadRevokeLetterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyManager(self, request):
         """重新核验管理人
 
         :param request: Request instance for VerifyManager.
         :type request: :class:`tencentcloud.ssl.v20191205.models.VerifyManagerRequest`
@@ -1215,8 +1215,8 @@
             model = models.VerifyManagerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/README.rst` & `tencentcloud-sdk-python-ssl-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.937/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.938/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

