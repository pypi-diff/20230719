# Comparing `tmp/tencentcloud-sdk-python-cpdp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cpdp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.937.tar", last modified: Tue Jul 18 00:21:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.938.tar", last modified: Wed Jul 19 00:25:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cpdp-3.0.937.tar` & `tencentcloud-sdk-python-cpdp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/
--rw-r--r--   0 root         (0) root         (0)   210732 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/cpdp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19183 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  2040467 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:12.000000 tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/
+-rw-r--r--   0 root         (0) root         (0)   211612 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/cpdp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19183 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  2040467 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:18.000000 tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/setup.py` & `tencentcloud-sdk-python-cpdp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/cpdp_client.py` & `tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/cpdp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddFlexFundingAccount(self, request):
         """灵云V2-绑定收款用户资金账号信息
 
         :param request: Request instance for AddFlexFundingAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.AddFlexFundingAccountRequest`
@@ -65,15 +65,15 @@
             model = models.AddFlexFundingAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddFlexIdInfo(self, request):
         """灵云V2-补充证件信息
 
         :param request: Request instance for AddFlexIdInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.AddFlexIdInfoRequest`
@@ -88,15 +88,15 @@
             model = models.AddFlexIdInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddFlexPhoneNo(self, request):
         """灵云V2-补充手机号信息
 
         :param request: Request instance for AddFlexPhoneNo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.AddFlexPhoneNoRequest`
@@ -111,15 +111,15 @@
             model = models.AddFlexPhoneNoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddMerchant(self, request):
         """云支付-添加商户接口
 
         :param request: Request instance for AddMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.AddMerchantRequest`
@@ -134,15 +134,15 @@
             model = models.AddMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddShop(self, request):
         """云支付-添加门店接口
 
         :param request: Request instance for AddShop.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.AddShopRequest`
@@ -157,15 +157,15 @@
             model = models.AddShopResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyApplicationMaterial(self, request):
         """跨境-提交申报材料。申报材料的主体是付款人，需要提前调用【跨境-付款人申请】接口提交付款人信息且审核通过后调用。
 
         :param request: Request instance for ApplyApplicationMaterial.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyApplicationMaterialRequest`
@@ -180,15 +180,15 @@
             model = models.ApplyApplicationMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyFlexPayment(self, request):
         """灵云V2-付款
 
         :param request: Request instance for ApplyFlexPayment.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyFlexPaymentRequest`
@@ -203,15 +203,15 @@
             model = models.ApplyFlexPaymentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyFlexSettlement(self, request):
         """灵云V2-结算
 
         :param request: Request instance for ApplyFlexSettlement.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyFlexSettlementRequest`
@@ -226,15 +226,15 @@
             model = models.ApplyFlexSettlementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyFlexWechatPreAuth(self, request):
         """微工卡开通预核身接口
 
         :param request: Request instance for ApplyFlexWechatPreAuth.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyFlexWechatPreAuthRequest`
@@ -249,15 +249,15 @@
             model = models.ApplyFlexWechatPreAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyOpenBankOrderDetailReceipt(self, request):
         """云企付-申请单笔交易回单
 
         :param request: Request instance for ApplyOpenBankOrderDetailReceipt.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyOpenBankOrderDetailReceiptRequest`
@@ -272,15 +272,15 @@
             model = models.ApplyOpenBankOrderDetailReceiptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyOpenBankSettleOrder(self, request):
         """云企付-结算申请接口
 
         :param request: Request instance for ApplyOpenBankSettleOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyOpenBankSettleOrderRequest`
@@ -295,15 +295,15 @@
             model = models.ApplyOpenBankSettleOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyOpenBankSubMerchantSignOnline(self, request):
         """子商户在线签约
 
         :param request: Request instance for ApplyOpenBankSubMerchantSignOnline.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyOpenBankSubMerchantSignOnlineRequest`
@@ -318,15 +318,15 @@
             model = models.ApplyOpenBankSubMerchantSignOnlineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyOutwardOrder(self, request):
         """跨境-汇出指令申请。通过该接口可将对接方账户中的人民币余额汇兑成外币，再汇出至指定银行账户。
 
         :param request: Request instance for ApplyOutwardOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyOutwardOrderRequest`
@@ -341,15 +341,15 @@
             model = models.ApplyOutwardOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyPayerInfo(self, request):
         """跨境-付款人申请。通过该接口提交付款人信息并进行 kyc 审核。
 
         :param request: Request instance for ApplyPayerInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyPayerInfoRequest`
@@ -364,15 +364,15 @@
             model = models.ApplyPayerInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyReWithdrawal(self, request):
         """正常结算提现失败情况下，发起重新提现的请求接口
 
         :param request: Request instance for ApplyReWithdrawal.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyReWithdrawalRequest`
@@ -387,15 +387,15 @@
             model = models.ApplyReWithdrawalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyReconciliationFile(self, request):
         """聚鑫-申请对账文件
 
         :param request: Request instance for ApplyReconciliationFile.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyReconciliationFileRequest`
@@ -410,15 +410,15 @@
             model = models.ApplyReconciliationFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyTrade(self, request):
         """跨境-提交贸易材料。通过提交贸易材料接口可为对接方累计贸易额度，在额度范围内可发起汇兑汇出交易。
 
         :param request: Request instance for ApplyTrade.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyTradeRequest`
@@ -433,15 +433,15 @@
             model = models.ApplyTradeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyWithdrawal(self, request):
         """商户提现
 
         :param request: Request instance for ApplyWithdrawal.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ApplyWithdrawalRequest`
@@ -456,15 +456,15 @@
             model = models.ApplyWithdrawalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindAccount(self, request):
         """灵云-绑定账号
 
         :param request: Request instance for BindAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.BindAccountRequest`
@@ -479,15 +479,15 @@
             model = models.BindAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindAcct(self, request):
         """商户绑定提现银行卡，每个商户只能绑定一张提现银行卡
 
         :param request: Request instance for BindAcct.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.BindAcctRequest`
@@ -502,15 +502,15 @@
             model = models.BindAcctResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindOpenBankExternalSubMerchantBankAccount(self, request):
         """云企付-子商户银行卡绑定
 
         :param request: Request instance for BindOpenBankExternalSubMerchantBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.BindOpenBankExternalSubMerchantBankAccountRequest`
@@ -525,15 +525,15 @@
             model = models.BindOpenBankExternalSubMerchantBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindOpenBankProfitSharePayee(self, request):
         """云企付-绑定分账收款方
 
         :param request: Request instance for BindOpenBankProfitSharePayee.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.BindOpenBankProfitSharePayeeRequest`
@@ -548,15 +548,15 @@
             model = models.BindOpenBankProfitSharePayeeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindRelateAccReUnionPay(self, request):
         """会员绑定提现账户-回填银联鉴权短信码。用于会员填写动态验证码后，发往银行进行验证，验证成功则完成绑定。
 
         :param request: Request instance for BindRelateAccReUnionPay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.BindRelateAccReUnionPayRequest`
@@ -571,15 +571,15 @@
             model = models.BindRelateAccReUnionPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindRelateAcctSmallAmount(self, request):
         """会员绑定提现账户-小额鉴权。会员申请绑定提现账户，绑定后从会员子账户中提现到绑定账户。
         转账鉴权有两种形式：往账鉴权和来账鉴权。
         往账鉴权：该接口发起成功后，银行会向提现账户转入小于等于0.5元的随机金额，并短信通知客户查看，客户查看后，需将收到的金额大小，在电商平台页面上回填，并通知银行。银行验证通过后，完成提现账户绑定。
         来账鉴权：该接口发起成功后，银行以短信通知客户查看，客户查看后，需通过待绑定的账户往市场的监管账户转入短信上指定的金额。银行检索到该笔指定金额的来账是源自待绑定账户，则绑定成功。平安银行的账户，即BankType送1时，大小额行号和超级网银号都不用送。
@@ -597,15 +597,15 @@
             model = models.BindRelateAcctSmallAmountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindRelateAcctUnionPay(self, request):
         """会员绑定提现账户-银联鉴权。用于会员申请绑定提现账户，申请后银行前往银联验证卡信息：姓名、证件、卡号、银行预留手机是否相符，相符则发送给会员手机动态验证码并返回成功，不相符则返回失败。
         平台接收到银行返回成功后，进入输入动态验证码的页面，有效期120秒，若120秒未输入，客户可点击重新发送动态验证码，这个步骤重新调用该接口即可。
         平安银行的账户，大小额行号和超级网银号都不用送。
         超级网银号：单笔转账金额不超过5万，不限制笔数，只用选XX银行，不用具体到支行，可实时知道对方是否收款成功。
@@ -624,15 +624,15 @@
             model = models.BindRelateAcctUnionPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckAcct(self, request):
         """商户绑定提现银行卡的验证接口
 
         :param request: Request instance for CheckAcct.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CheckAcctRequest`
@@ -647,15 +647,15 @@
             model = models.CheckAcctResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckAmount(self, request):
         """验证鉴权金额。此接口可受理BindRelateAcctSmallAmount接口发起的转账金额（往账鉴权方式）的验证处理。若所回填的验证金额验证通过，则会绑定原申请中的银行账户作为提现账户。通过此接口也可以查得BindRelateAcctSmallAmount接口发起的来账鉴权方式的申请的当前状态。
 
         :param request: Request instance for CheckAmount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CheckAmountRequest`
@@ -670,15 +670,15 @@
             model = models.CheckAmountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseCloudOrder(self, request):
         """通过此接口关闭此前已创建的订单。关闭后，用户将无法继续付款，仅能关闭创建后未支付的订单。
 
         :param request: Request instance for CloseCloudOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CloseCloudOrderRequest`
@@ -693,15 +693,15 @@
             model = models.CloseCloudOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseOpenBankPaymentOrder(self, request):
         """云企付-关闭订单
 
         :param request: Request instance for CloseOpenBankPaymentOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CloseOpenBankPaymentOrderRequest`
@@ -716,15 +716,15 @@
             model = models.CloseOpenBankPaymentOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseOrder(self, request):
         """通过此接口关闭此前已创建的订单，关闭后，用户将无法继续付款。仅能关闭创建后未支付的订单
 
         :param request: Request instance for CloseOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CloseOrderRequest`
@@ -739,15 +739,15 @@
             model = models.CloseOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfirmOrder(self, request):
         """云鉴-消费订单确认接口
 
         :param request: Request instance for ConfirmOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ConfirmOrderRequest`
@@ -762,15 +762,15 @@
             model = models.ConfirmOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ContractOrder(self, request):
         """应用需要先带上签约信息调用本接口生成支付订单号，并将应答的PayInfo透传给聚鑫SDK，拉起客户端（包括微信公众号/微信小程序/客户端App）支付。
 
         :param request: Request instance for ContractOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ContractOrderRequest`
@@ -785,15 +785,15 @@
             model = models.ContractOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAcct(self, request):
         """子商户入驻聚鑫平台
 
         :param request: Request instance for CreateAcct.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateAcctRequest`
@@ -808,15 +808,15 @@
             model = models.CreateAcctResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAgentTaxPaymentInfos(self, request):
         """直播平台-代理商完税信息录入
 
         :param request: Request instance for CreateAgentTaxPaymentInfos.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateAgentTaxPaymentInfosRequest`
@@ -831,15 +831,15 @@
             model = models.CreateAgentTaxPaymentInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAnchor(self, request):
         """直播平台-主播入驻
 
         :param request: Request instance for CreateAnchor.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateAnchorRequest`
@@ -854,15 +854,15 @@
             model = models.CreateAnchorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBatchPayment(self, request):
         """灵云-批量主播转账接口
 
         :param request: Request instance for CreateBatchPayment.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateBatchPaymentRequest`
@@ -877,15 +877,15 @@
             model = models.CreateBatchPaymentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudSubMerchant(self, request):
         """创建子商户
 
         :param request: Request instance for CreateCloudSubMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateCloudSubMerchantRequest`
@@ -900,15 +900,15 @@
             model = models.CreateCloudSubMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustAcctId(self, request):
         """会员子账户开立。会员在银行注册，并开立会员子账户，交易网会员代码即会员在平台端系统的会员编号。
         平台需保存银行返回的子账户账号，后续交易接口都会用到。会员属性字段为预留扩展字段，当前必须送默认值。
 
         :param request: Request instance for CreateCustAcctId.
@@ -924,15 +924,15 @@
             model = models.CreateCustAcctIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateExternalAnchor(self, request):
         """灵云-主播入驻
 
         :param request: Request instance for CreateExternalAnchor.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateExternalAnchorRequest`
@@ -947,15 +947,15 @@
             model = models.CreateExternalAnchorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlexPayee(self, request):
         """灵云V2-收款用户开立
 
         :param request: Request instance for CreateFlexPayee.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateFlexPayeeRequest`
@@ -970,15 +970,15 @@
             model = models.CreateFlexPayeeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInvoice(self, request):
         """智慧零售-发票开具
 
         :param request: Request instance for CreateInvoice.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateInvoiceRequest`
@@ -993,15 +993,15 @@
             model = models.CreateInvoiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInvoiceV2(self, request):
         """智慧零售-发票开具V2
 
         :param request: Request instance for CreateInvoiceV2.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateInvoiceV2Request`
@@ -1016,15 +1016,15 @@
             model = models.CreateInvoiceV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMerchant(self, request):
         """智慧零售-商户注册
 
         :param request: Request instance for CreateMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateMerchantRequest`
@@ -1039,15 +1039,15 @@
             model = models.CreateMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankAggregatedSubMerchantRegistration(self, request):
         """云企付-子商户进件V2
 
         :param request: Request instance for CreateOpenBankAggregatedSubMerchantRegistration.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankAggregatedSubMerchantRegistrationRequest`
@@ -1062,15 +1062,15 @@
             model = models.CreateOpenBankAggregatedSubMerchantRegistrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankExternalSubMerchantAccountBook(self, request):
         """第三方子商户电子记账本创建接口
 
         :param request: Request instance for CreateOpenBankExternalSubMerchantAccountBook.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankExternalSubMerchantAccountBookRequest`
@@ -1085,15 +1085,15 @@
             model = models.CreateOpenBankExternalSubMerchantAccountBookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankExternalSubMerchantRegistration(self, request):
         """云企付-子商户进件
 
         :param request: Request instance for CreateOpenBankExternalSubMerchantRegistration.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankExternalSubMerchantRegistrationRequest`
@@ -1108,15 +1108,15 @@
             model = models.CreateOpenBankExternalSubMerchantRegistrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankGlobalPaymentOrder(self, request):
         """云企付-跨境支付下单
 
         :param request: Request instance for CreateOpenBankGlobalPaymentOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankGlobalPaymentOrderRequest`
@@ -1131,15 +1131,15 @@
             model = models.CreateOpenBankGlobalPaymentOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankMerchant(self, request):
         """云企付-创建商户
 
         :param request: Request instance for CreateOpenBankMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankMerchantRequest`
@@ -1154,15 +1154,15 @@
             model = models.CreateOpenBankMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankPaymentOrder(self, request):
         """云企付-创建支付订单。支持B2B网关支付，B2C转账下单。
 
         :param request: Request instance for CreateOpenBankPaymentOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankPaymentOrderRequest`
@@ -1177,15 +1177,15 @@
             model = models.CreateOpenBankPaymentOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankRechargeOrder(self, request):
         """云企付-创建充值订单
 
         :param request: Request instance for CreateOpenBankRechargeOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankRechargeOrderRequest`
@@ -1200,15 +1200,15 @@
             model = models.CreateOpenBankRechargeOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankSubMerchantRateConfigure(self, request):
         """云企付-子商户费率配置
 
         :param request: Request instance for CreateOpenBankSubMerchantRateConfigure.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankSubMerchantRateConfigureRequest`
@@ -1223,15 +1223,15 @@
             model = models.CreateOpenBankSubMerchantRateConfigureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankUnifiedOrder(self, request):
         """云企付-聚合下单
 
         :param request: Request instance for CreateOpenBankUnifiedOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankUnifiedOrderRequest`
@@ -1246,15 +1246,15 @@
             model = models.CreateOpenBankUnifiedOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOpenBankVerificationOrder(self, request):
         """云企付-创建核销申请，适用于针对支付订单维度的确认收货，解冻等业务场景。目前支持的渠道有TENPAY下的EBANK_PAYMENT付款方式创建支付订单时，选择担保支付下单的订单进行解冻。
 
         :param request: Request instance for CreateOpenBankVerificationOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOpenBankVerificationOrderRequest`
@@ -1269,15 +1269,15 @@
             model = models.CreateOpenBankVerificationOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrder(self, request):
         """云鉴-消费订单发起的接口
 
         :param request: Request instance for CreateOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateOrderRequest`
@@ -1292,15 +1292,15 @@
             model = models.CreateOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePayMerchant(self, request):
         """商户新增的接口
 
         :param request: Request instance for CreatePayMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreatePayMerchantRequest`
@@ -1315,15 +1315,15 @@
             model = models.CreatePayMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePayRollPreOrder(self, request):
         """务工卡-核身预下单
 
         :param request: Request instance for CreatePayRollPreOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreatePayRollPreOrderRequest`
@@ -1338,15 +1338,15 @@
             model = models.CreatePayRollPreOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePayRollPreOrderWithAuth(self, request):
         """务工卡-核身预下单带授权
 
         :param request: Request instance for CreatePayRollPreOrderWithAuth.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreatePayRollPreOrderWithAuthRequest`
@@ -1361,15 +1361,15 @@
             model = models.CreatePayRollPreOrderWithAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePayRollToken(self, request):
         """务工卡-生成授权令牌
 
         :param request: Request instance for CreatePayRollToken.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreatePayRollTokenRequest`
@@ -1384,15 +1384,15 @@
             model = models.CreatePayRollTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRedInvoice(self, request):
         """智慧零售-发票红冲
 
         :param request: Request instance for CreateRedInvoice.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateRedInvoiceRequest`
@@ -1407,15 +1407,15 @@
             model = models.CreateRedInvoiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRedInvoiceV2(self, request):
         """智慧零售-发票红冲V2
 
         :param request: Request instance for CreateRedInvoiceV2.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateRedInvoiceV2Request`
@@ -1430,15 +1430,15 @@
             model = models.CreateRedInvoiceV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSinglePayment(self, request):
         """灵云-单笔主播转账接口
 
         :param request: Request instance for CreateSinglePayment.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateSinglePaymentRequest`
@@ -1453,15 +1453,15 @@
             model = models.CreateSinglePaymentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTransferBatch(self, request):
         """微信商户发起批量转账
 
         :param request: Request instance for CreateTransferBatch.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.CreateTransferBatchRequest`
@@ -1476,15 +1476,15 @@
             model = models.CreateTransferBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeduceQuota(self, request):
         """直播平台-扣减额度
 
         :param request: Request instance for DeduceQuota.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DeduceQuotaRequest`
@@ -1499,15 +1499,15 @@
             model = models.DeduceQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAgentTaxPaymentInfo(self, request):
         """直播平台-删除代理商完税信息
 
         :param request: Request instance for DeleteAgentTaxPaymentInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DeleteAgentTaxPaymentInfoRequest`
@@ -1522,15 +1522,15 @@
             model = models.DeleteAgentTaxPaymentInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAgentTaxPaymentInfos(self, request):
         """直播平台-删除代理商完税信息
 
         :param request: Request instance for DeleteAgentTaxPaymentInfos.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DeleteAgentTaxPaymentInfosRequest`
@@ -1545,15 +1545,15 @@
             model = models.DeleteAgentTaxPaymentInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChargeDetail(self, request):
         """查询充值明细接口
 
         :param request: Request instance for DescribeChargeDetail.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DescribeChargeDetailRequest`
@@ -1568,15 +1568,15 @@
             model = models.DescribeChargeDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrderStatus(self, request):
         """查询单笔订单交易状态
 
         :param request: Request instance for DescribeOrderStatus.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DescribeOrderStatusRequest`
@@ -1591,15 +1591,15 @@
             model = models.DescribeOrderStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeAccreditQuery(self, request):
         """云支付-分账授权申请查询接口
 
         :param request: Request instance for DistributeAccreditQuery.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeAccreditQueryRequest`
@@ -1614,15 +1614,15 @@
             model = models.DistributeAccreditQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeAccreditTlinx(self, request):
         """云支付-分账授权申请接口
 
         :param request: Request instance for DistributeAccreditTlinx.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeAccreditTlinxRequest`
@@ -1637,15 +1637,15 @@
             model = models.DistributeAccreditTlinxResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeAddReceiver(self, request):
         """云支付-分账添加分账接收方接口
 
         :param request: Request instance for DistributeAddReceiver.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeAddReceiverRequest`
@@ -1660,15 +1660,15 @@
             model = models.DistributeAddReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeApply(self, request):
         """云支付-分账请求接口
 
         :param request: Request instance for DistributeApply.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeApplyRequest`
@@ -1683,15 +1683,15 @@
             model = models.DistributeApplyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeCancel(self, request):
         """云支付-分账撤销接口
 
         :param request: Request instance for DistributeCancel.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeCancelRequest`
@@ -1706,15 +1706,15 @@
             model = models.DistributeCancelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeQuery(self, request):
         """云支付-分账结果查询接口
 
         :param request: Request instance for DistributeQuery.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeQueryRequest`
@@ -1729,15 +1729,15 @@
             model = models.DistributeQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeQueryReceiver(self, request):
         """云支付-查询已添加分账接收方接口
 
         :param request: Request instance for DistributeQueryReceiver.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeQueryReceiverRequest`
@@ -1752,15 +1752,15 @@
             model = models.DistributeQueryReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DistributeRemoveReceiver(self, request):
         """云支付-分账解除分账接收方接口
 
         :param request: Request instance for DistributeRemoveReceiver.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DistributeRemoveReceiverRequest`
@@ -1775,15 +1775,15 @@
             model = models.DistributeRemoveReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadBill(self, request):
         """账单下载接口，根据本接口返回的URL地址，在D+1日下载对账单。注意，本接口返回的URL地址有时效，请尽快下载。URL超时时效后，请重新调用本接口再次获取。
 
         :param request: Request instance for DownloadBill.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DownloadBillRequest`
@@ -1798,15 +1798,15 @@
             model = models.DownloadBillResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadOrgFile(self, request):
         """云支付-下载机构文件接口
 
         :param request: Request instance for DownloadOrgFile.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DownloadOrgFileRequest`
@@ -1821,15 +1821,15 @@
             model = models.DownloadOrgFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadReconciliationUrl(self, request):
         """获取对账中心账单下载地址的接口
 
         :param request: Request instance for DownloadReconciliationUrl.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.DownloadReconciliationUrlRequest`
@@ -1844,15 +1844,15 @@
             model = models.DownloadReconciliationUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteMemberTransaction(self, request):
         """会员间交易接口
 
         :param request: Request instance for ExecuteMemberTransaction.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ExecuteMemberTransactionRequest`
@@ -1867,15 +1867,15 @@
             model = models.ExecuteMemberTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FreezeFlexBalance(self, request):
         """灵云V2-冻结余额
 
         :param request: Request instance for FreezeFlexBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.FreezeFlexBalanceRequest`
@@ -1890,15 +1890,15 @@
             model = models.FreezeFlexBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetBillDownloadUrl(self, request):
         """调用该接口返回对账单下载地址，对账单下载URL通过GET方式访问，返回zip包，解压后为csv格式文件。文件首行如下：
         订单号,订单归属日期,机构编号,订单描述,交易类型,订单状态,支付场景,原始金额,折扣金额,实际交易金额,支付渠道优惠金额,抹零金额,币种,下单时间,付款成功时间,商户编号,门店编号,付款方式编号,付款方式名称,商户手续费T1,商户扣率,是否信用卡交易,原始订单号,用户账号,外部订单号,订单备注
 
         :param request: Request instance for GetBillDownloadUrl.
@@ -1914,15 +1914,15 @@
             model = models.GetBillDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDistributeBillDownloadUrl(self, request):
         """调用该接口返回对账单下载地址，对账单下载URL通过GET方式访问，返回zip包，解压后为csv格式文件。文件首行如下：
         商户号,订单号,支付订单号,分账订单总金额,分账详情（通过|分割每笔明细：商户号1#分账金额1|商户号2#分账金额2）,交易手续费承担方商户号,交易手续费,发起时间,分账状态,结算日期,非交易主体分账金额,商户退款订单号,商户分账单号
 
         :param request: Request instance for GetDistributeBillDownloadUrl.
@@ -1938,15 +1938,15 @@
             model = models.GetDistributeBillDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPayRollAuth(self, request):
         """务工卡-查询授权关系
 
         :param request: Request instance for GetPayRollAuth.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.GetPayRollAuthRequest`
@@ -1961,15 +1961,15 @@
             model = models.GetPayRollAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPayRollAuthList(self, request):
         """务工卡-查询核身记录
 
         :param request: Request instance for GetPayRollAuthList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.GetPayRollAuthListRequest`
@@ -1984,15 +1984,15 @@
             model = models.GetPayRollAuthListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPayRollAuthResult(self, request):
         """务工卡-获取核身结果
 
         :param request: Request instance for GetPayRollAuthResult.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.GetPayRollAuthResultRequest`
@@ -2007,15 +2007,15 @@
             model = models.GetPayRollAuthResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MigrateOrderRefund(self, request):
         """山姆聚合支付项目-存量订单退款接口。可以通过本接口将支付款全部或部分退还给付款方，在收到用户退款请求并且验证成功之后，按照退款规则将支付款按原路退回到支付账号。
 
         :param request: Request instance for MigrateOrderRefund.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.MigrateOrderRefundRequest`
@@ -2030,15 +2030,15 @@
             model = models.MigrateOrderRefundResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MigrateOrderRefundQuery(self, request):
         """提交退款申请后，通过调用该接口查询退款状态。退款可能有一定延时。
 
         :param request: Request instance for MigrateOrderRefundQuery.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.MigrateOrderRefundQueryRequest`
@@ -2053,15 +2053,15 @@
             model = models.MigrateOrderRefundQueryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAgentTaxPaymentInfo(self, request):
         """直播平台-修改代理商完税信息
 
         :param request: Request instance for ModifyAgentTaxPaymentInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyAgentTaxPaymentInfoRequest`
@@ -2076,15 +2076,15 @@
             model = models.ModifyAgentTaxPaymentInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBindedAccount(self, request):
         """灵云-重新绑定账号
 
         :param request: Request instance for ModifyBindedAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyBindedAccountRequest`
@@ -2099,15 +2099,15 @@
             model = models.ModifyBindedAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFlexFundingAccount(self, request):
         """灵云V2-修改收款用户资金账号信息
 
         :param request: Request instance for ModifyFlexFundingAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyFlexFundingAccountRequest`
@@ -2122,15 +2122,15 @@
             model = models.ModifyFlexFundingAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFlexPayeeAccountRightStatus(self, request):
         """灵云V2-收款用户账户权益状态修改
 
         :param request: Request instance for ModifyFlexPayeeAccountRightStatus.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyFlexPayeeAccountRightStatusRequest`
@@ -2145,15 +2145,15 @@
             model = models.ModifyFlexPayeeAccountRightStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMerchant(self, request):
         """云鉴-商户信息修改的接口
 
         :param request: Request instance for ModifyMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyMerchantRequest`
@@ -2168,15 +2168,15 @@
             model = models.ModifyMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMntMbrBindRelateAcctBankCode(self, request):
         """维护会员绑定提现账户联行号。此接口可以支持市场修改会员的提现账户的开户行信息，具体包括开户行行名、开户行的银行联行号（大小额联行号）和超级网银行号。
 
         :param request: Request instance for ModifyMntMbrBindRelateAcctBankCode.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ModifyMntMbrBindRelateAcctBankCodeRequest`
@@ -2191,15 +2191,15 @@
             model = models.ModifyMntMbrBindRelateAcctBankCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAcctBinding(self, request):
         """聚鑫-查询子账户绑定银行卡
 
         :param request: Request instance for QueryAcctBinding.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAcctBindingRequest`
@@ -2214,15 +2214,15 @@
             model = models.QueryAcctBindingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAcctInfo(self, request):
         """聚鑫-开户信息查询
 
         :param request: Request instance for QueryAcctInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAcctInfoRequest`
@@ -2237,15 +2237,15 @@
             model = models.QueryAcctInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAcctInfoList(self, request):
         """聚鑫-开户信息列表查询, 查询某一段时间的开户信息
 
         :param request: Request instance for QueryAcctInfoList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAcctInfoListRequest`
@@ -2260,15 +2260,15 @@
             model = models.QueryAcctInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAgentStatements(self, request):
         """直播平台-查询代理商结算单链接
 
         :param request: Request instance for QueryAgentStatements.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAgentStatementsRequest`
@@ -2283,15 +2283,15 @@
             model = models.QueryAgentStatementsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAgentTaxPaymentBatch(self, request):
         """直播平台-查询批次信息
 
         :param request: Request instance for QueryAgentTaxPaymentBatch.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAgentTaxPaymentBatchRequest`
@@ -2306,15 +2306,15 @@
             model = models.QueryAgentTaxPaymentBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAnchorContractInfo(self, request):
         """直播平台-查询主播签约信息
 
         :param request: Request instance for QueryAnchorContractInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAnchorContractInfoRequest`
@@ -2329,15 +2329,15 @@
             model = models.QueryAnchorContractInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryApplicationMaterial(self, request):
         """跨境-成功申报材料查询。查询成功入库的申报材料。
 
         :param request: Request instance for QueryApplicationMaterial.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryApplicationMaterialRequest`
@@ -2352,15 +2352,15 @@
             model = models.QueryApplicationMaterialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryAssignment(self, request):
         """直播平台-查询分配关系
 
         :param request: Request instance for QueryAssignment.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryAssignmentRequest`
@@ -2375,15 +2375,15 @@
             model = models.QueryAssignmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBalance(self, request):
         """子商户余额查询
 
         :param request: Request instance for QueryBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBalanceRequest`
@@ -2398,15 +2398,15 @@
             model = models.QueryBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBankClear(self, request):
         """查询银行在途清算结果。查询时间段内交易网的在途清算结果。
 
         :param request: Request instance for QueryBankClear.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBankClearRequest`
@@ -2421,15 +2421,15 @@
             model = models.QueryBankClearResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBankTransactionDetails(self, request):
         """查询银行时间段内交易明细。查询时间段的会员成功交易。
 
         :param request: Request instance for QueryBankTransactionDetails.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBankTransactionDetailsRequest`
@@ -2444,15 +2444,15 @@
             model = models.QueryBankTransactionDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBankWithdrawCashDetails(self, request):
         """查询银行时间段内清分提现明细。查询银行时间段内清分提现明细接口：若为“见证+收单退款”“见证+收单充值”记录时备注Note为“见证+收单充值,订单号”“见证+收单退款,订单号”，此接口可以查到T0/T1的充值明细和退款记录。查询标志：充值记录仍用3清分选项查询，退款记录同提现用2选项查询。
 
         :param request: Request instance for QueryBankWithdrawCashDetails.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBankWithdrawCashDetailsRequest`
@@ -2467,15 +2467,15 @@
             model = models.QueryBankWithdrawCashDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBatchPaymentResult(self, request):
         """灵云-批量转账结果查询
 
         :param request: Request instance for QueryBatchPaymentResult.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBatchPaymentResultRequest`
@@ -2490,15 +2490,15 @@
             model = models.QueryBatchPaymentResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBillDownloadURL(self, request):
         """获取单笔代发转账对账单下载URL
 
         :param request: Request instance for QueryBillDownloadURL.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryBillDownloadURLRequest`
@@ -2513,15 +2513,15 @@
             model = models.QueryBillDownloadURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCityCode(self, request):
         """云支付-查询城市编码接口
 
         :param request: Request instance for QueryCityCode.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCityCodeRequest`
@@ -2536,15 +2536,15 @@
             model = models.QueryCityCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCloudChannelData(self, request):
         """发起支付等渠道操作后，可以调用该接口查询渠道的数据。
 
         :param request: Request instance for QueryCloudChannelData.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCloudChannelDataRequest`
@@ -2559,15 +2559,15 @@
             model = models.QueryCloudChannelDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCloudOrder(self, request):
         """根据订单号或用户ID，查询支付订单状态。
 
         :param request: Request instance for QueryCloudOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCloudOrderRequest`
@@ -2582,15 +2582,15 @@
             model = models.QueryCloudOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCloudRefundOrder(self, request):
         """提交退款申请后，通过调用该接口查询退款状态。退款可能有一定延时，用微信零钱支付的退款约20分钟内到账，银行卡支付的退款约3个工作日后到账。
 
         :param request: Request instance for QueryCloudRefundOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCloudRefundOrderRequest`
@@ -2605,15 +2605,15 @@
             model = models.QueryCloudRefundOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCommonTransferRecharge(self, request):
         """查询普通转账充值明细。接口用于查询会员主动转账进资金汇总账户的明细情况。若会员使用绑定账号转入，则直接入账到会员子账户。若未使用绑定账号转入，则系统无法自动清分到对应子账户，则转入挂账子账户由平台自行清分。若是 “见证+收单充值”T0充值记录时备注Note为“见证+收单充值,订单号” 此接口可以查到T0到账的“见证+收单充值”充值记录。
 
         :param request: Request instance for QueryCommonTransferRecharge.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCommonTransferRechargeRequest`
@@ -2628,15 +2628,15 @@
             model = models.QueryCommonTransferRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCompanyTitle(self, request):
         """智慧零售-查询公司抬头
 
         :param request: Request instance for QueryCompanyTitle.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCompanyTitleRequest`
@@ -2651,15 +2651,15 @@
             model = models.QueryCompanyTitleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryContract(self, request):
         """通过此接口查询签约数据
 
         :param request: Request instance for QueryContract.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryContractRequest`
@@ -2674,15 +2674,15 @@
             model = models.QueryContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryContractPayFee(self, request):
         """云支付-查询支付方式费率及自定义表单项接口
 
         :param request: Request instance for QueryContractPayFee.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryContractPayFeeRequest`
@@ -2697,15 +2697,15 @@
             model = models.QueryContractPayFeeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryContractPayWayList(self, request):
         """云支付-查询合同支付方式列表接口
 
         :param request: Request instance for QueryContractPayWayList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryContractPayWayListRequest`
@@ -2720,15 +2720,15 @@
             model = models.QueryContractPayWayListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryContractRelateShop(self, request):
         """云支付-查询合同可关联门店接口
 
         :param request: Request instance for QueryContractRelateShop.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryContractRelateShopRequest`
@@ -2743,15 +2743,15 @@
             model = models.QueryContractRelateShopResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryCustAcctIdBalance(self, request):
         """查询银行子账户余额。查询会员子账户以及平台的功能子账户的余额。
 
         :param request: Request instance for QueryCustAcctIdBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryCustAcctIdBalanceRequest`
@@ -2766,15 +2766,15 @@
             model = models.QueryCustAcctIdBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryDownloadBillURL(self, request):
         """云鉴-查询对账单下载地址的接口
 
         :param request: Request instance for QueryDownloadBillURL.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryDownloadBillURLRequest`
@@ -2789,15 +2789,15 @@
             model = models.QueryDownloadBillURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExceedingInfo(self, request):
         """灵云-查询超额信息
 
         :param request: Request instance for QueryExceedingInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryExceedingInfoRequest`
@@ -2812,15 +2812,15 @@
             model = models.QueryExceedingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryExchangeRate(self, request):
         """跨境-查询汇率
 
         :param request: Request instance for QueryExchangeRate.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryExchangeRateRequest`
@@ -2835,15 +2835,15 @@
             model = models.QueryExchangeRateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFinancialDataUrl(self, request):
         """财税-查询金融数据文件下载链接
 
         :param request: Request instance for QueryFinancialDataUrl.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFinancialDataUrlRequest`
@@ -2858,15 +2858,15 @@
             model = models.QueryFinancialDataUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexAmountBeforeTax(self, request):
         """灵云V2-查询税前金额
 
         :param request: Request instance for QueryFlexAmountBeforeTax.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexAmountBeforeTaxRequest`
@@ -2881,15 +2881,15 @@
             model = models.QueryFlexAmountBeforeTaxResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexBillDownloadUrl(self, request):
         """灵云V2-查询对账单文件下载链接
 
         :param request: Request instance for QueryFlexBillDownloadUrl.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexBillDownloadUrlRequest`
@@ -2904,15 +2904,15 @@
             model = models.QueryFlexBillDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexFreezeOrderList(self, request):
         """灵云V2-查询冻结订单列表
 
         :param request: Request instance for QueryFlexFreezeOrderList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexFreezeOrderListRequest`
@@ -2927,15 +2927,15 @@
             model = models.QueryFlexFreezeOrderListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexOrderSummaryList(self, request):
         """灵云V2-订单汇总列表查询
 
         :param request: Request instance for QueryFlexOrderSummaryList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexOrderSummaryListRequest`
@@ -2950,15 +2950,15 @@
             model = models.QueryFlexOrderSummaryListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPayeeAccountBalance(self, request):
         """灵云V2-收款用户账户余额查询
 
         :param request: Request instance for QueryFlexPayeeAccountBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPayeeAccountBalanceRequest`
@@ -2973,15 +2973,15 @@
             model = models.QueryFlexPayeeAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPayeeAccountInfo(self, request):
         """灵云V2-收款用户账户信息查询
 
         :param request: Request instance for QueryFlexPayeeAccountInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPayeeAccountInfoRequest`
@@ -2996,15 +2996,15 @@
             model = models.QueryFlexPayeeAccountInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPayeeAccountList(self, request):
         """灵云V2-收款用户账户列表查询
 
         :param request: Request instance for QueryFlexPayeeAccountList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPayeeAccountListRequest`
@@ -3019,15 +3019,15 @@
             model = models.QueryFlexPayeeAccountListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPayeeInfo(self, request):
         """灵云V2-收款用户信息查询
 
         :param request: Request instance for QueryFlexPayeeInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPayeeInfoRequest`
@@ -3042,15 +3042,15 @@
             model = models.QueryFlexPayeeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPaymentOrderList(self, request):
         """灵云V2-查询付款订单列表
 
         :param request: Request instance for QueryFlexPaymentOrderList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPaymentOrderListRequest`
@@ -3065,15 +3065,15 @@
             model = models.QueryFlexPaymentOrderListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPaymentOrderStatus(self, request):
         """灵云V2-查询付款订单状态
 
         :param request: Request instance for QueryFlexPaymentOrderStatus.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPaymentOrderStatusRequest`
@@ -3088,15 +3088,15 @@
             model = models.QueryFlexPaymentOrderStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexPlatformAccountBalance(self, request):
         """灵云V2-平台账户余额查询
 
         :param request: Request instance for QueryFlexPlatformAccountBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexPlatformAccountBalanceRequest`
@@ -3111,15 +3111,15 @@
             model = models.QueryFlexPlatformAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexServiceProviderAccountBalance(self, request):
         """灵云V2-查询服务商账户余额
 
         :param request: Request instance for QueryFlexServiceProviderAccountBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexServiceProviderAccountBalanceRequest`
@@ -3134,15 +3134,15 @@
             model = models.QueryFlexServiceProviderAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexSettlementOrderList(self, request):
         """灵云V2-查询结算订单列表
 
         :param request: Request instance for QueryFlexSettlementOrderList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexSettlementOrderListRequest`
@@ -3157,15 +3157,15 @@
             model = models.QueryFlexSettlementOrderListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFlexWechatAuthResult(self, request):
         """查询微工卡核身结果
 
         :param request: Request instance for QueryFlexWechatAuthResult.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFlexWechatAuthResultRequest`
@@ -3180,15 +3180,15 @@
             model = models.QueryFlexWechatAuthResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFundsTransactionDetails(self, request):
         """聚鑫-查询会员资金交易信息列表
 
         :param request: Request instance for QueryFundsTransactionDetails.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryFundsTransactionDetailsRequest`
@@ -3203,15 +3203,15 @@
             model = models.QueryFundsTransactionDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryInvoice(self, request):
         """智慧零售-发票查询
 
         :param request: Request instance for QueryInvoice.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryInvoiceRequest`
@@ -3226,15 +3226,15 @@
             model = models.QueryInvoiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryInvoiceV2(self, request):
         """智慧零售-发票查询V2
 
         :param request: Request instance for QueryInvoiceV2.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryInvoiceV2Request`
@@ -3249,15 +3249,15 @@
             model = models.QueryInvoiceV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMaliciousRegistration(self, request):
         """商户恶意注册接口
 
         :param request: Request instance for QueryMaliciousRegistration.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMaliciousRegistrationRequest`
@@ -3272,15 +3272,15 @@
             model = models.QueryMaliciousRegistrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMemberBind(self, request):
         """会员绑定信息查询。查询标志为“单个会员”的情况下，返回该会员的有效的绑定账户信息。
         查询标志为“全部会员”的情况下，返回市场下的全部的有效的绑定账户信息。查询标志为“单个会员的证件信息”的情况下，返回市场下的指定的会员的留存在电商见证宝系统的证件信息。
 
         :param request: Request instance for QueryMemberBind.
@@ -3296,15 +3296,15 @@
             model = models.QueryMemberBindResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMemberTransaction(self, request):
         """会员间交易-不验证。此接口可以实现会员间的余额的交易，实现资金在会员之间流动。
 
         :param request: Request instance for QueryMemberTransaction.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMemberTransactionRequest`
@@ -3319,15 +3319,15 @@
             model = models.QueryMemberTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMemberTransactionDetails(self, request):
         """聚鑫-查询会员间交易信息列表
 
         :param request: Request instance for QueryMemberTransactionDetails.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMemberTransactionDetailsRequest`
@@ -3342,15 +3342,15 @@
             model = models.QueryMemberTransactionDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchant(self, request):
         """云鉴-商户信息查询接口
 
         :param request: Request instance for QueryMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantRequest`
@@ -3365,15 +3365,15 @@
             model = models.QueryMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchantBalance(self, request):
         """跨境-对接方账户余额查询
 
         :param request: Request instance for QueryMerchantBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantBalanceRequest`
@@ -3388,15 +3388,15 @@
             model = models.QueryMerchantBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchantClassification(self, request):
         """云支付-查询商户分类接口
 
         :param request: Request instance for QueryMerchantClassification.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantClassificationRequest`
@@ -3411,15 +3411,15 @@
             model = models.QueryMerchantClassificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchantInfoForManagement(self, request):
         """智慧零售-查询管理端商户
 
         :param request: Request instance for QueryMerchantInfoForManagement.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantInfoForManagementRequest`
@@ -3434,15 +3434,15 @@
             model = models.QueryMerchantInfoForManagementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchantOrder(self, request):
         """云鉴-消费订单查询接口
 
         :param request: Request instance for QueryMerchantOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantOrderRequest`
@@ -3457,15 +3457,15 @@
             model = models.QueryMerchantOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMerchantPayWayList(self, request):
         """商户查询已开通的支付方式列表
 
         :param request: Request instance for QueryMerchantPayWayList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryMerchantPayWayListRequest`
@@ -3480,15 +3480,15 @@
             model = models.QueryMerchantPayWayListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankBankAccountBalance(self, request):
         """云企付-子商户银行卡余额查询
 
         :param request: Request instance for QueryOpenBankBankAccountBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankBankAccountBalanceRequest`
@@ -3503,15 +3503,15 @@
             model = models.QueryOpenBankBankAccountBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankBankBranchList(self, request):
         """云企付-查询联行号
 
         :param request: Request instance for QueryOpenBankBankBranchList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankBankBranchListRequest`
@@ -3526,15 +3526,15 @@
             model = models.QueryOpenBankBankBranchListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankBillDataPage(self, request):
         """云企付-分页查询对账单数据
 
         :param request: Request instance for QueryOpenBankBillDataPage.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankBillDataPageRequest`
@@ -3549,15 +3549,15 @@
             model = models.QueryOpenBankBillDataPageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankBindExternalSubMerchantBankAccount(self, request):
         """云企付-子商户银行卡绑定结果查询
 
         :param request: Request instance for QueryOpenBankBindExternalSubMerchantBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankBindExternalSubMerchantBankAccountRequest`
@@ -3572,15 +3572,15 @@
             model = models.QueryOpenBankBindExternalSubMerchantBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankDailyReceiptDownloadUrl(self, request):
         """云企付-按日期批量查询回单下载地址
 
         :param request: Request instance for QueryOpenBankDailyReceiptDownloadUrl.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankDailyReceiptDownloadUrlRequest`
@@ -3595,15 +3595,15 @@
             model = models.QueryOpenBankDailyReceiptDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankDownLoadUrl(self, request):
         """云企付-查询对账单下载地址
 
         :param request: Request instance for QueryOpenBankDownLoadUrl.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankDownLoadUrlRequest`
@@ -3618,15 +3618,15 @@
             model = models.QueryOpenBankDownLoadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankExternalSubAccountBookBalance(self, request):
         """第三方子商户电子记账本余额查询接口
 
         :param request: Request instance for QueryOpenBankExternalSubAccountBookBalance.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankExternalSubAccountBookBalanceRequest`
@@ -3641,15 +3641,15 @@
             model = models.QueryOpenBankExternalSubAccountBookBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankExternalSubMerchantBankAccount(self, request):
         """云企付-子商户银行卡列表查询
 
         :param request: Request instance for QueryOpenBankExternalSubMerchantBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankExternalSubMerchantBankAccountRequest`
@@ -3664,15 +3664,15 @@
             model = models.QueryOpenBankExternalSubMerchantBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankExternalSubMerchantRegistration(self, request):
         """云企付-子商户进件结果查询
 
         :param request: Request instance for QueryOpenBankExternalSubMerchantRegistration.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankExternalSubMerchantRegistrationRequest`
@@ -3687,15 +3687,15 @@
             model = models.QueryOpenBankExternalSubMerchantRegistrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankOrderDetailReceiptInfo(self, request):
         """云企付-单笔交易回单申请结果查询
 
         :param request: Request instance for QueryOpenBankOrderDetailReceiptInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankOrderDetailReceiptInfoRequest`
@@ -3710,15 +3710,15 @@
             model = models.QueryOpenBankOrderDetailReceiptInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankPaymentOrder(self, request):
         """云企付-查询订单支付结果
 
         :param request: Request instance for QueryOpenBankPaymentOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankPaymentOrderRequest`
@@ -3733,15 +3733,15 @@
             model = models.QueryOpenBankPaymentOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankProfitSharePayee(self, request):
         """云企付-绑定分账收款方查询
 
         :param request: Request instance for QueryOpenBankProfitSharePayee.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankProfitSharePayeeRequest`
@@ -3756,15 +3756,15 @@
             model = models.QueryOpenBankProfitSharePayeeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankRefundOrder(self, request):
         """云企付-退款结果查询
 
         :param request: Request instance for QueryOpenBankRefundOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankRefundOrderRequest`
@@ -3779,15 +3779,15 @@
             model = models.QueryOpenBankRefundOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankSettleOrder(self, request):
         """云企付-结算单查询结果
 
         :param request: Request instance for QueryOpenBankSettleOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankSettleOrderRequest`
@@ -3802,15 +3802,15 @@
             model = models.QueryOpenBankSettleOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankSubMerchantCredential(self, request):
         """云企付-子商户资质文件查询
 
         :param request: Request instance for QueryOpenBankSubMerchantCredential.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankSubMerchantCredentialRequest`
@@ -3825,15 +3825,15 @@
             model = models.QueryOpenBankSubMerchantCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankSubMerchantRateConfigure(self, request):
         """云企付-子商户费率配置结果查询
 
         :param request: Request instance for QueryOpenBankSubMerchantRateConfigure.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankSubMerchantRateConfigureRequest`
@@ -3848,15 +3848,15 @@
             model = models.QueryOpenBankSubMerchantRateConfigureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankSubMerchantSignOnline(self, request):
         """子商户在线签约查询
 
         :param request: Request instance for QueryOpenBankSubMerchantSignOnline.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankSubMerchantSignOnlineRequest`
@@ -3871,15 +3871,15 @@
             model = models.QueryOpenBankSubMerchantSignOnlineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankSupportBankList(self, request):
         """云企付-查询支持银行列表
 
         :param request: Request instance for QueryOpenBankSupportBankList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankSupportBankListRequest`
@@ -3894,15 +3894,15 @@
             model = models.QueryOpenBankSupportBankListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankUnbindExternalSubMerchantBankAccount(self, request):
         """云企付-子商户银行卡解绑结果查询
 
         :param request: Request instance for QueryOpenBankUnbindExternalSubMerchantBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankUnbindExternalSubMerchantBankAccountRequest`
@@ -3917,15 +3917,15 @@
             model = models.QueryOpenBankUnbindExternalSubMerchantBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOpenBankVerificationOrder(self, request):
         """云企付-查询核销订单状态，客户可以使用该接口来查询核销申请的订单状态。目前仅支持TENPAY渠道EBANK_PAYMENT付款方式的担保支付订单查询。
 
         :param request: Request instance for QueryOpenBankVerificationOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOpenBankVerificationOrderRequest`
@@ -3940,15 +3940,15 @@
             model = models.QueryOpenBankVerificationOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOrder(self, request):
         """根据订单号，或者用户Id，查询支付订单状态
 
         :param request: Request instance for QueryOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOrderRequest`
@@ -3963,15 +3963,15 @@
             model = models.QueryOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOrderStatus(self, request):
         """云支付-查询订单付款状态
 
         :param request: Request instance for QueryOrderStatus.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOrderStatusRequest`
@@ -3986,15 +3986,15 @@
             model = models.QueryOrderStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryOutwardOrder(self, request):
         """跨境-查询汇出结果
 
         :param request: Request instance for QueryOutwardOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryOutwardOrderRequest`
@@ -4009,15 +4009,15 @@
             model = models.QueryOutwardOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryPayerInfo(self, request):
         """跨境-付款人查询
 
         :param request: Request instance for QueryPayerInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryPayerInfoRequest`
@@ -4032,15 +4032,15 @@
             model = models.QueryPayerInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryReconciliationDocument(self, request):
         """查询对账文件信息。平台调用该接口获取需下载对账文件的文件名称以及密钥。 平台获取到信息后， 可以再调用OPENAPI的文件下载功能。
 
         :param request: Request instance for QueryReconciliationDocument.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryReconciliationDocumentRequest`
@@ -4055,15 +4055,15 @@
             model = models.QueryReconciliationDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryReconciliationFileApplyInfo(self, request):
         """聚鑫-查询对账文件申请结果
 
         :param request: Request instance for QueryReconciliationFileApplyInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryReconciliationFileApplyInfoRequest`
@@ -4078,15 +4078,15 @@
             model = models.QueryReconciliationFileApplyInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryRefund(self, request):
         """提交退款申请后，通过调用该接口查询退款状态。退款可能有一定延时，用微信零钱支付的退款约20分钟内到账，银行卡支付的退款约3个工作日后到账。
 
         :param request: Request instance for QueryRefund.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryRefundRequest`
@@ -4101,15 +4101,15 @@
             model = models.QueryRefundResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryShopOpenId(self, request):
         """云支付-获取门店OpenId接口
 
         :param request: Request instance for QueryShopOpenId.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryShopOpenIdRequest`
@@ -4124,15 +4124,15 @@
             model = models.QueryShopOpenIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QuerySinglePaymentResult(self, request):
         """灵云-单笔转账结果查询
 
         :param request: Request instance for QuerySinglePaymentResult.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QuerySinglePaymentResultRequest`
@@ -4147,15 +4147,15 @@
             model = models.QuerySinglePaymentResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QuerySingleTransactionStatus(self, request):
         """查询银行单笔交易状态。查询单笔交易的状态。
 
         :param request: Request instance for QuerySingleTransactionStatus.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QuerySingleTransactionStatusRequest`
@@ -4170,15 +4170,15 @@
             model = models.QuerySingleTransactionStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QuerySmallAmountTransfer(self, request):
         """查询小额鉴权转账结果。查询小额往账鉴权的转账状态。
 
         :param request: Request instance for QuerySmallAmountTransfer.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QuerySmallAmountTransferRequest`
@@ -4193,15 +4193,15 @@
             model = models.QuerySmallAmountTransferResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryTrade(self, request):
         """跨境-贸易材料明细查询。
 
         :param request: Request instance for QueryTrade.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryTradeRequest`
@@ -4216,15 +4216,15 @@
             model = models.QueryTradeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryTransferBatch(self, request):
         """通过商家批次单号或者微信批次号查询批次单
 
         :param request: Request instance for QueryTransferBatch.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryTransferBatchRequest`
@@ -4239,15 +4239,15 @@
             model = models.QueryTransferBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryTransferDetail(self, request):
         """通过商家或者微信批次明细单号查询明细单
 
         :param request: Request instance for QueryTransferDetail.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryTransferDetailRequest`
@@ -4262,15 +4262,15 @@
             model = models.QueryTransferDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryTransferResult(self, request):
         """智能代发-单笔代发转账查询接口
 
         :param request: Request instance for QueryTransferResult.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.QueryTransferResultRequest`
@@ -4285,15 +4285,15 @@
             model = models.QueryTransferResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RechargeByThirdPay(self, request):
         """会员在途充值(经第三方支付渠道)接口
 
         :param request: Request instance for RechargeByThirdPay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RechargeByThirdPayRequest`
@@ -4308,15 +4308,15 @@
             model = models.RechargeByThirdPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RechargeMemberThirdPay(self, request):
         """见证宝-会员在途充值(经第三方支付渠道)
 
         :param request: Request instance for RechargeMemberThirdPay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RechargeMemberThirdPayRequest`
@@ -4331,15 +4331,15 @@
             model = models.RechargeMemberThirdPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Refund(self, request):
         """如交易订单需退款，可以通过本接口将支付款全部或部分退还给付款方，聚鑫将在收到退款请求并且验证成功之后，按照退款规则将支付款按原路退回到支付帐号。最长支持1年的订单退款。在订单包含多个子订单的情况下，如果使用本接口传入OutTradeNo或TransactionId退款，则只支持全单退款；如果需要部分退款，请通过传入子订单的方式来指定部分金额退款。
 
         :param request: Request instance for Refund.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundRequest`
@@ -4354,15 +4354,15 @@
             model = models.RefundResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundCloudOrder(self, request):
         """如交易订单需退款，可以通过本接口将支付款全部或部分退还给付款方，聚鑫将在收到退款请求并且验证成功之后，按照退款规则将支付款按原路退回到支付帐号。最长支持1年的订单退款。在订单包含多个子订单的情况下，如果使用本接口传入OutTradeNo或TransactionId退款，则只支持全单退款；如果需要部分退款，请通过传入子订单的方式来指定部分金额退款。
 
         :param request: Request instance for RefundCloudOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundCloudOrderRequest`
@@ -4377,15 +4377,15 @@
             model = models.RefundCloudOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundMemberTransaction(self, request):
         """会员间交易退款
 
         :param request: Request instance for RefundMemberTransaction.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundMemberTransactionRequest`
@@ -4400,15 +4400,15 @@
             model = models.RefundMemberTransactionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundOpenBankOrder(self, request):
         """云企付-退款申请
 
         :param request: Request instance for RefundOpenBankOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundOpenBankOrderRequest`
@@ -4423,15 +4423,15 @@
             model = models.RefundOpenBankOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundOrder(self, request):
         """云鉴-消费订单退款的接口
 
         :param request: Request instance for RefundOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundOrderRequest`
@@ -4446,15 +4446,15 @@
             model = models.RefundOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundTlinxOrder(self, request):
         """云支付订单退款接口
 
         :param request: Request instance for RefundTlinxOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RefundTlinxOrderRequest`
@@ -4469,15 +4469,15 @@
             model = models.RefundTlinxOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterBehavior(self, request):
         """商户查询是否签约和签约行为上报
 
         :param request: Request instance for RegisterBehavior.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RegisterBehaviorRequest`
@@ -4492,15 +4492,15 @@
             model = models.RegisterBehaviorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterBill(self, request):
         """登记挂账(支持撤销)
 
         :param request: Request instance for RegisterBill.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RegisterBillRequest`
@@ -4515,15 +4515,15 @@
             model = models.RegisterBillResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterBillSupportWithdraw(self, request):
         """登记挂账(支持撤销)。此接口可实现把不明来账或自有资金等已登记在挂账子账户下的资金调整到普通会员子账户。即通过申请调用此接口，将会减少挂账子账户的资金，调增指定的普通会员子账户的可提现余额及可用余额。此接口不支持把挂账子账户资金清分到功能子账户。
 
         :param request: Request instance for RegisterBillSupportWithdraw.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RegisterBillSupportWithdrawRequest`
@@ -4538,15 +4538,15 @@
             model = models.RegisterBillSupportWithdrawResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevResigterBillSupportWithdraw(self, request):
         """登记挂账撤销。此接口可以实现把RegisterBillSupportWithdraw接口完成的登记挂账进行撤销，即调减普通会员子账户的可提现和可用余额，调增挂账子账户的可用余额。
 
         :param request: Request instance for RevResigterBillSupportWithdraw.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RevResigterBillSupportWithdrawRequest`
@@ -4561,15 +4561,15 @@
             model = models.RevResigterBillSupportWithdrawResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReviseMbrProperty(self, request):
         """修改会员属性-普通商户子账户。修改会员的会员属性。
 
         :param request: Request instance for ReviseMbrProperty.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ReviseMbrPropertyRequest`
@@ -4584,15 +4584,15 @@
             model = models.ReviseMbrPropertyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeMemberRechargeThirdPay(self, request):
         """撤销会员在途充值(经第三方支付渠道)
 
         :param request: Request instance for RevokeMemberRechargeThirdPay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RevokeMemberRechargeThirdPayRequest`
@@ -4607,15 +4607,15 @@
             model = models.RevokeMemberRechargeThirdPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeRechargeByThirdPay(self, request):
         """撤销会员在途充值(经第三方支付渠道)接口
 
         :param request: Request instance for RevokeRechargeByThirdPay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.RevokeRechargeByThirdPayRequest`
@@ -4630,15 +4630,15 @@
             model = models.RevokeRechargeByThirdPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncContractData(self, request):
         """对于存量的签约关系导入或者部分场景下米大师无法收到签约通知的场景，需要由调用方主动将签约状态同步至米大师
 
         :param request: Request instance for SyncContractData.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.SyncContractDataRequest`
@@ -4653,15 +4653,15 @@
             model = models.SyncContractDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateContract(self, request):
         """通过此接口进行解约
 
         :param request: Request instance for TerminateContract.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.TerminateContractRequest`
@@ -4676,15 +4676,15 @@
             model = models.TerminateContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransferSinglePay(self, request):
         """智能代发-单笔代发转账接口
 
         :param request: Request instance for TransferSinglePay.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.TransferSinglePayRequest`
@@ -4699,15 +4699,15 @@
             model = models.TransferSinglePayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindAcct(self, request):
         """商户解除绑定的提现银行卡
 
         :param request: Request instance for UnBindAcct.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnBindAcctRequest`
@@ -4722,15 +4722,15 @@
             model = models.UnBindAcctResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindOpenBankExternalSubMerchantBankAccount(self, request):
         """云企付-子商户银行卡解绑
 
         :param request: Request instance for UnbindOpenBankExternalSubMerchantBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnbindOpenBankExternalSubMerchantBankAccountRequest`
@@ -4745,15 +4745,15 @@
             model = models.UnbindOpenBankExternalSubMerchantBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindRelateAcct(self, request):
         """会员解绑提现账户。此接口可以支持会员解除名下的绑定账户关系。
 
         :param request: Request instance for UnbindRelateAcct.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnbindRelateAcctRequest`
@@ -4768,15 +4768,15 @@
             model = models.UnbindRelateAcctResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnifiedCloudOrder(self, request):
         """应用需要先调用本接口生成支付订单号，并将应答的PayInfo透传给聚鑫SDK，拉起客户端（包括微信公众号/微信小程序/客户端App）支付。
 
         :param request: Request instance for UnifiedCloudOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnifiedCloudOrderRequest`
@@ -4791,15 +4791,15 @@
             model = models.UnifiedCloudOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnifiedOrder(self, request):
         """应用需要先调用本接口生成支付订单号，并将应答的PayInfo透传给聚鑫SDK，拉起客户端（包括微信公众号/微信小程序/客户端App）支付。
 
         :param request: Request instance for UnifiedOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnifiedOrderRequest`
@@ -4814,15 +4814,15 @@
             model = models.UnifiedOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnifiedTlinxOrder(self, request):
         """云支付-统一下单接口
 
         :param request: Request instance for UnifiedTlinxOrder.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UnifiedTlinxOrderRequest`
@@ -4837,15 +4837,15 @@
             model = models.UnifiedTlinxOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadExternalAnchorInfo(self, request):
         """灵云-上传主播信息
 
         :param request: Request instance for UploadExternalAnchorInfo.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadExternalAnchorInfoRequest`
@@ -4860,15 +4860,15 @@
             model = models.UploadExternalAnchorInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFile(self, request):
         """直播平台-文件上传
 
         :param request: Request instance for UploadFile.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadFileRequest`
@@ -4883,15 +4883,15 @@
             model = models.UploadFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadOpenBankSubMerchantCredential(self, request):
         """云企付-子商户资质文件上传
 
         :param request: Request instance for UploadOpenBankSubMerchantCredential.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadOpenBankSubMerchantCredentialRequest`
@@ -4906,15 +4906,15 @@
             model = models.UploadOpenBankSubMerchantCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadOrgFile(self, request):
         """云支付-上传机构文件接口
 
         :param request: Request instance for UploadOrgFile.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadOrgFileRequest`
@@ -4929,15 +4929,15 @@
             model = models.UploadOrgFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadTaxList(self, request):
         """直播平台-上传代理商完税列表
 
         :param request: Request instance for UploadTaxList.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadTaxListRequest`
@@ -4952,15 +4952,15 @@
             model = models.UploadTaxListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadTaxPayment(self, request):
         """直播平台-上传代理商完税证明
 
         :param request: Request instance for UploadTaxPayment.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.UploadTaxPaymentRequest`
@@ -4975,15 +4975,15 @@
             model = models.UploadTaxPaymentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyOpenBankAccount(self, request):
         """云企付-子商户银行卡打款验证，在接入TENPAY渠道EBANK_PAYMENT付款时，若客户期望接入担保支付，需在接入前先完成，收款商户绑定的银行卡进行打款验证。验证成功后，才可以调用CreateOpenBankPaymentOrder接口进行担保支付下单。
 
         :param request: Request instance for VerifyOpenBankAccount.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.VerifyOpenBankAccountRequest`
@@ -4998,15 +4998,15 @@
             model = models.VerifyOpenBankAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ViewContract(self, request):
         """云支付-查询合同明细接口
 
         :param request: Request instance for ViewContract.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ViewContractRequest`
@@ -5021,15 +5021,15 @@
             model = models.ViewContractResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ViewMerchant(self, request):
         """云支付-查询商户明细接口
 
         :param request: Request instance for ViewMerchant.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ViewMerchantRequest`
@@ -5044,15 +5044,15 @@
             model = models.ViewMerchantResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ViewShop(self, request):
         """云支付-查询门店明细接口
 
         :param request: Request instance for ViewShop.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.ViewShopRequest`
@@ -5067,15 +5067,15 @@
             model = models.ViewShopResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WithdrawCashMembership(self, request):
         """会员提现-不验证。此接口受理会员发起的提现申请。会员子账户的可提现余额、可用余额会减少，市场的资金汇总账户(监管账户)会减少相应的发生金额，提现到会员申请的收款账户。
 
         :param request: Request instance for WithdrawCashMembership.
         :type request: :class:`tencentcloud.cpdp.v20190820.models.WithdrawCashMembershipRequest`
@@ -5090,8 +5090,8 @@
             model = models.WithdrawCashMembershipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/errorcodes.py` & `tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud/cpdp/v20190820/models.py` & `tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud/cpdp/v20190820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/README.rst` & `tencentcloud-sdk-python-cpdp-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.937/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.938/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

