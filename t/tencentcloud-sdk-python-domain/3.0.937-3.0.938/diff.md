# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.937.tar", last modified: Tue Jul 18 00:22:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.938.tar", last modified: Wed Jul 19 00:37:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.937.tar` & `tencentcloud-sdk-python-domain-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25103 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)   121377 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25207 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)   121377 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:37:58.000000 tencentcloud-sdk-python-domain-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:37:57.000000 tencentcloud-sdk-python-domain-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-domain-3.0.937/setup.py` & `tencentcloud-sdk-python-domain-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/domain_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchModifyDomainInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBatchStatus(self, request):
         """本接口 ( CheckBatchStatus ) 用于查询批量操作日志状态 。
 
         :param request: Request instance for CheckBatchStatus.
         :type request: :class:`tencentcloud.domain.v20180808.models.CheckBatchStatusRequest`
@@ -65,15 +65,15 @@
             model = models.CheckBatchStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckDomain(self, request):
         """检查域名是否可以注册。
 
         :param request: Request instance for CheckDomain.
         :type request: :class:`tencentcloud.domain.v20180808.models.CheckDomainRequest`
@@ -88,15 +88,15 @@
             model = models.CheckDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomainBatch(self, request):
         """本接口 ( CreateDomainBatch ) 用于批量域名注册 。
 
         :param request: Request instance for CreateDomainBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.CreateDomainBatchRequest`
@@ -111,15 +111,15 @@
             model = models.CreateDomainBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePhoneEmail(self, request):
         """此接口用于创建有效的手机、邮箱
 
         :param request: Request instance for CreatePhoneEmail.
         :type request: :class:`tencentcloud.domain.v20180808.models.CreatePhoneEmailRequest`
@@ -134,15 +134,15 @@
             model = models.CreatePhoneEmailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTemplate(self, request):
         """本接口 ( CreateTemplate ) 用于添加域名信息模板 。
 
         :param request: Request instance for CreateTemplate.
         :type request: :class:`tencentcloud.domain.v20180808.models.CreateTemplateRequest`
@@ -157,15 +157,15 @@
             model = models.CreateTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePhoneEmail(self, request):
         """此接口用于删除已验证的手机邮箱
 
         :param request: Request instance for DeletePhoneEmail.
         :type request: :class:`tencentcloud.domain.v20180808.models.DeletePhoneEmailRequest`
@@ -180,15 +180,15 @@
             model = models.DeletePhoneEmailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTemplate(self, request):
         """本接口 ( DeleteTemplate ) 用于删除信息模板。
 
         :param request: Request instance for DeleteTemplate.
         :type request: :class:`tencentcloud.domain.v20180808.models.DeleteTemplateRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchOperationLogDetails(self, request):
         """本接口 ( DescribeBatchOperationLogDetails ) 用于获取批量操作日志详情。
 
         :param request: Request instance for DescribeBatchOperationLogDetails.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeBatchOperationLogDetailsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeBatchOperationLogDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchOperationLogs(self, request):
         """本接口 ( DescribeBatchOperationLogs ) 用于获取批量操作日志 。
 
         :param request: Request instance for DescribeBatchOperationLogs.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeBatchOperationLogsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeBatchOperationLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainBaseInfo(self, request):
         """本接口 (  DescribeDomainBaseInfo) 获取域名基本信息。
 
         :param request: Request instance for DescribeDomainBaseInfo.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeDomainBaseInfoRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeDomainBaseInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainNameList(self, request):
         """本接口 (  DescribeDomainNameList ) 我的域名列表。
 
         :param request: Request instance for DescribeDomainNameList.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeDomainNameListRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeDomainNameListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainPriceList(self, request):
         """按照域名后缀获取对应的价格列表
 
         :param request: Request instance for DescribeDomainPriceList.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeDomainPriceListRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeDomainPriceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainSimpleInfo(self, request):
         """获取域名实名信息详情
 
         :param request: Request instance for DescribeDomainSimpleInfo.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeDomainSimpleInfoRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeDomainSimpleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePhoneEmailList(self, request):
         """本接口用于获取已验证的手机邮箱列表
 
         :param request: Request instance for DescribePhoneEmailList.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribePhoneEmailListRequest`
@@ -364,15 +364,15 @@
             model = models.DescribePhoneEmailListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplate(self, request):
         """本接口 (DescribeTemplate) 用于获取模板信息。
 
         :param request: Request instance for DescribeTemplate.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeTemplateRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplateList(self, request):
         """本接口 (DescribeTemplateList) 用于获取信息模板列表。
 
         :param request: Request instance for DescribeTemplateList.
         :type request: :class:`tencentcloud.domain.v20180808.models.DescribeTemplateListRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeTemplateListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainDNSBatch(self, request):
         """本接口 ( ModifyDomainDNSBatch) 用于批量域名 DNS 修改 。
 
         :param request: Request instance for ModifyDomainDNSBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.ModifyDomainDNSBatchRequest`
@@ -433,15 +433,15 @@
             model = models.ModifyDomainDNSBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainOwnerBatch(self, request):
         """本接口 ( ModifyDomainOwnerBatch) 用于域名批量账号间转移 。
 
         :param request: Request instance for ModifyDomainOwnerBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.ModifyDomainOwnerBatchRequest`
@@ -456,15 +456,15 @@
             model = models.ModifyDomainOwnerBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDomainBatch(self, request):
         """本接口 ( RenewDomainBatch ) 用于批量续费域名 。
 
         :param request: Request instance for RenewDomainBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.RenewDomainBatchRequest`
@@ -479,15 +479,15 @@
             model = models.RenewDomainBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendPhoneEmailCode(self, request):
         """此接口用于发送手机邮箱验证码。
 
         :param request: Request instance for SendPhoneEmailCode.
         :type request: :class:`tencentcloud.domain.v20180808.models.SendPhoneEmailCodeRequest`
@@ -502,15 +502,15 @@
             model = models.SendPhoneEmailCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetDomainAutoRenew(self, request):
         """本接口 ( SetDomainAutoRenew ) 用于设置域名自动续费。
 
         :param request: Request instance for SetDomainAutoRenew.
         :type request: :class:`tencentcloud.domain.v20180808.models.SetDomainAutoRenewRequest`
@@ -525,15 +525,15 @@
             model = models.SetDomainAutoRenewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransferInDomainBatch(self, request):
         """本接口 ( TransferInDomainBatch ) 用于批量转入域名 。
 
         :param request: Request instance for TransferInDomainBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.TransferInDomainBatchRequest`
@@ -548,15 +548,15 @@
             model = models.TransferInDomainBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransferProhibitionBatch(self, request):
         """本接口 ( TransferProhibitionBatch ) 用于批量禁止域名转移 。
 
         :param request: Request instance for TransferProhibitionBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.TransferProhibitionBatchRequest`
@@ -571,15 +571,15 @@
             model = models.TransferProhibitionBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateProhibitionBatch(self, request):
         """本接口 ( UpdateProhibitionBatch ) 用于批量禁止更新锁。
 
         :param request: Request instance for UpdateProhibitionBatch.
         :type request: :class:`tencentcloud.domain.v20180808.models.UpdateProhibitionBatchRequest`
@@ -594,15 +594,15 @@
             model = models.UpdateProhibitionBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadImage(self, request):
         """本接口 ( UploadImage ) 用于证件图片上传 。
 
         :param request: Request instance for UploadImage.
         :type request: :class:`tencentcloud.domain.v20180808.models.UploadImageRequest`
@@ -617,8 +617,8 @@
             model = models.UploadImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.938/tencentcloud/domain/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.938/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.937/README.rst` & `tencentcloud-sdk-python-domain-3.0.938/README.rst`

 * *Files identical despite different names*

