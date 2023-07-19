# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.937.tar", last modified: Tue Jul 18 00:28:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.938.tar", last modified: Wed Jul 19 00:43:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.937.tar` & `tencentcloud-sdk-python-partners-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)    19334 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   107514 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:37.000000 tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)    19410 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   107514 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:57.000000 tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-partners-3.0.937/setup.py` & `tencentcloud-sdk-python-partners-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/partners_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AgentPayDealsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AgentTransferMoney(self, request):
         """为合作伙伴提供转账给客户能力。仅支持合作伙伴为自己名下客户转账。
 
         :param request: Request instance for AgentTransferMoney.
         :type request: :class:`tencentcloud.partners.v20180321.models.AgentTransferMoneyRequest`
@@ -65,15 +65,15 @@
             model = models.AgentTransferMoneyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssignClientsToSales(self, request):
         """为代客or申请中代客分派跟进人（业务员），入参可从以下API获取
         - 代客列表获取API： [DescribeAgentAuditedClients](https://cloud.tencent.com/document/product/563/19184)
         - 申请中代客列表获取API：[DescribeAgentClients](https://cloud.tencent.com/document/product/563/16046)
         - 业务员列表获取API：[DescribeSalesmans](https://cloud.tencent.com/document/product/563/35196) <br><br>
@@ -91,15 +91,15 @@
             model = models.AssignClientsToSalesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AuditApplyClient(self, request):
         """代理商可以审核其名下申请中代客
 
         :param request: Request instance for AuditApplyClient.
         :type request: :class:`tencentcloud.partners.v20180321.models.AuditApplyClientRequest`
@@ -114,15 +114,15 @@
             model = models.AuditApplyClientResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePayRelationForClient(self, request):
         """合作伙伴为客户创建强代付关系
 
         :param request: Request instance for CreatePayRelationForClient.
         :type request: :class:`tencentcloud.partners.v20180321.models.CreatePayRelationForClientRequest`
@@ -137,15 +137,15 @@
             model = models.CreatePayRelationForClientResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentAuditedClients(self, request):
         """查询已审核客户列表
 
         :param request: Request instance for DescribeAgentAuditedClients.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentAuditedClientsRequest`
@@ -160,15 +160,15 @@
             model = models.DescribeAgentAuditedClientsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentBills(self, request):
         """代理商可查询自己及名下代客所有业务明细
 
         :param request: Request instance for DescribeAgentBills.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentBillsRequest`
@@ -183,15 +183,15 @@
             model = models.DescribeAgentBillsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentClientGrade(self, request):
         """传入代客uin，查客户级别，客户审核状态，客户实名认证状态
 
         :param request: Request instance for DescribeAgentClientGrade.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentClientGradeRequest`
@@ -206,15 +206,15 @@
             model = models.DescribeAgentClientGradeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentClients(self, request):
         """代理商可查询自己名下待审核客户列表
 
         :param request: Request instance for DescribeAgentClients.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentClientsRequest`
@@ -229,15 +229,15 @@
             model = models.DescribeAgentClientsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentDealsByCache(self, request):
         """供代理商拉取缓存的全量预付费客户订单
 
         :param request: Request instance for DescribeAgentDealsByCache.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentDealsByCacheRequest`
@@ -252,15 +252,15 @@
             model = models.DescribeAgentDealsByCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentPayDealsV2(self, request):
         """可以查询代理商代付的预付费订单
 
         :param request: Request instance for DescribeAgentPayDealsV2.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsV2Request`
@@ -275,15 +275,15 @@
             model = models.DescribeAgentPayDealsV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentSelfPayDealsV2(self, request):
         """查询代理商名下指定代客的自付订单（预付费）
 
         :param request: Request instance for DescribeAgentSelfPayDealsV2.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsV2Request`
@@ -298,15 +298,15 @@
             model = models.DescribeAgentSelfPayDealsV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClientBalanceNew(self, request):
         """为合作伙伴提供查询客户余额能力。调用者必须是合作伙伴，只能查询自己名下客户余额
 
         :param request: Request instance for DescribeClientBalanceNew.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeClientBalanceNewRequest`
@@ -321,15 +321,15 @@
             model = models.DescribeClientBalanceNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRebateInfos(self, request):
         """【该接口已下线，请切换使用升级版本DescribeRebateInfosNew】代理商可查询自己名下全部返佣信息
 
         :param request: Request instance for DescribeRebateInfos.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeRebateInfosRequest`
@@ -344,15 +344,15 @@
             model = models.DescribeRebateInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRebateInfosNew(self, request):
         """代理商可查询自己名下全部返佣信息
 
         :param request: Request instance for DescribeRebateInfosNew.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeRebateInfosNewRequest`
@@ -367,15 +367,15 @@
             model = models.DescribeRebateInfosNewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSalesmans(self, request):
         """代理商查询名下业务员列表信息
 
         :param request: Request instance for DescribeSalesmans.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeSalesmansRequest`
@@ -390,15 +390,15 @@
             model = models.DescribeSalesmansResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnbindClientList(self, request):
         """代理商名下客户解绑记录查询接口
 
         :param request: Request instance for DescribeUnbindClientList.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeUnbindClientListRequest`
@@ -413,15 +413,15 @@
             model = models.DescribeUnbindClientListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClientRemark(self, request):
         """代理商可以对名下客户添加备注、修改备注
 
         :param request: Request instance for ModifyClientRemark.
         :type request: :class:`tencentcloud.partners.v20180321.models.ModifyClientRemarkRequest`
@@ -436,15 +436,15 @@
             model = models.ModifyClientRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemovePayRelationForClient(self, request):
         """合作伙伴为客户消除强代付关系
 
         :param request: Request instance for RemovePayRelationForClient.
         :type request: :class:`tencentcloud.partners.v20180321.models.RemovePayRelationForClientRequest`
@@ -459,8 +459,8 @@
             model = models.RemovePayRelationForClientResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.937/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.938/tencentcloud/partners/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-partners-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.937/README.rst` & `tencentcloud-sdk-python-partners-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.937/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.938/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

