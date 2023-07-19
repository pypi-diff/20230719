# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.937.tar", last modified: Tue Jul 18 00:24:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.938.tar", last modified: Wed Jul 19 00:39:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.937.tar` & `tencentcloud-sdk-python-faceid-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34030 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)   212180 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:24:04.000000 tencentcloud-sdk-python-faceid-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)   212180 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:39:19.000000 tencentcloud-sdk-python-faceid-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.938/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/setup.py` & `tencentcloud-sdk-python-faceid-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BankCard2EVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BankCard4EVerification(self, request):
         """本接口用于输入银行卡号、姓名、开户证件号、开户手机号，校验信息的真实性和一致性。
 
         :param request: Request instance for BankCard4EVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.BankCard4EVerificationRequest`
@@ -65,15 +65,15 @@
             model = models.BankCard4EVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BankCardVerification(self, request):
         """本接口用于银行卡号、姓名、开户证件号信息的真实性和一致性。
 
         :param request: Request instance for BankCardVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.BankCardVerificationRequest`
@@ -88,15 +88,15 @@
             model = models.BankCardVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBankCardInformation(self, request):
         """银行卡基础信息查询
 
         :param request: Request instance for CheckBankCardInformation.
         :type request: :class:`tencentcloud.faceid.v20180301.models.CheckBankCardInformationRequest`
@@ -111,15 +111,15 @@
             model = models.CheckBankCardInformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckEidTokenStatus(self, request):
         """用于轮询E证通H5场景EidToken验证状态。
 
         :param request: Request instance for CheckEidTokenStatus.
         :type request: :class:`tencentcloud.faceid.v20180301.models.CheckEidTokenStatusRequest`
@@ -134,15 +134,15 @@
             model = models.CheckEidTokenStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIdCardInformation(self, request):
         """传入身份证人像面照片，识别身份证照片上的信息，并将姓名、身份证号、身份证人像照片与权威库的证件照进行比对，是否属于同一个人，从而验证身份证信息的真实性。
 
         :param request: Request instance for CheckIdCardInformation.
         :type request: :class:`tencentcloud.faceid.v20180301.models.CheckIdCardInformationRequest`
@@ -157,15 +157,15 @@
             model = models.CheckIdCardInformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIdNameDate(self, request):
         """本接口用于校验姓名、身份证号、身份证有效期的真实性和一致性。
 
         :param request: Request instance for CheckIdNameDate.
         :type request: :class:`tencentcloud.faceid.v20180301.models.CheckIdNameDateRequest`
@@ -180,15 +180,15 @@
             model = models.CheckIdNameDateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckPhoneAndName(self, request):
         """手机号二要素核验接口用于校验手机号和姓名的真实性和一致性，支持的手机号段详情请查阅<a href="https://cloud.tencent.com/document/product/1007/46063">运营商类</a>文档。
 
         :param request: Request instance for CheckPhoneAndName.
         :type request: :class:`tencentcloud.faceid.v20180301.models.CheckPhoneAndNameRequest`
@@ -203,15 +203,15 @@
             model = models.CheckPhoneAndNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectAuth(self, request):
         """每次调用人脸核身SaaS化服务前，需先调用本接口获取BizToken，用来串联核身流程，在验证完成后，用于获取验证结果信息。
 
         :param request: Request instance for DetectAuth.
         :type request: :class:`tencentcloud.faceid.v20180301.models.DetectAuthRequest`
@@ -226,15 +226,15 @@
             model = models.DetectAuthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EncryptedPhoneVerification(self, request):
         """本接口用于校验手机号、姓名和身份证号的真实性和一致性，入参支持明文、MD5和SHA256加密传输。
 
         :param request: Request instance for EncryptedPhoneVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.EncryptedPhoneVerificationRequest`
@@ -249,15 +249,15 @@
             model = models.EncryptedPhoneVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetActionSequence(self, request):
         """使用动作活体检测模式前，需调用本接口获取动作顺序。
 
         :param request: Request instance for GetActionSequence.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetActionSequenceRequest`
@@ -272,15 +272,15 @@
             model = models.GetActionSequenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDetectInfo(self, request):
         """完成验证后，用BizToken调用本接口获取结果信息，BizToken生成后三天内（3\*24\*3,600秒）可多次拉取。
 
         :param request: Request instance for GetDetectInfo.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetDetectInfoRequest`
@@ -295,15 +295,15 @@
             model = models.GetDetectInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDetectInfoEnhanced(self, request):
         """完成验证后，用BizToken调用本接口获取结果信息，BizToken生成后三天内（3\*24\*3,600秒）可多次拉取。
 
         :param request: Request instance for GetDetectInfoEnhanced.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetDetectInfoEnhancedRequest`
@@ -318,15 +318,15 @@
             model = models.GetDetectInfoEnhancedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEidResult(self, request):
         """完成验证后，用EidToken调用本接口获取结果信息，EidToken生成后三天内（3\*24\*3,600秒）可多次拉取。
 
         :param request: Request instance for GetEidResult.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetEidResultRequest`
@@ -341,15 +341,15 @@
             model = models.GetEidResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEidToken(self, request):
         """每次调用E证通服务前，需先调用本接口获取EidToken，用来串联E证通流程，在验证完成后，用于获取E证通结果信息。
 
         :param request: Request instance for GetEidToken.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetEidTokenRequest`
@@ -364,15 +364,15 @@
             model = models.GetEidTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFaceIdResult(self, request):
         """完成验证后，用FaceIdToken调用本接口获取结果信息，FaceIdToken生成后三天内（3\*24\*3,600秒）可多次拉取。
 
         :param request: Request instance for GetFaceIdResult.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetFaceIdResultRequest`
@@ -387,15 +387,15 @@
             model = models.GetFaceIdResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFaceIdToken(self, request):
         """每次调用人脸核身SDK服务前，需先调用本接口获取SDKToken，用来串联核身流程，在验证完成后，用于获取验证结果信息，该token仅能核身一次。
 
         :param request: Request instance for GetFaceIdToken.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetFaceIdTokenRequest`
@@ -410,15 +410,15 @@
             model = models.GetFaceIdTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetLiveCode(self, request):
         """使用数字活体检测模式前，需调用本接口获取数字验证码。
 
         :param request: Request instance for GetLiveCode.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetLiveCodeRequest`
@@ -433,15 +433,15 @@
             model = models.GetLiveCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetWeChatBillDetails(self, request):
         """查询微信渠道服务（微信小程序、微信原生H5、微信普通H5）的账单明细及计费状态。
 
         :param request: Request instance for GetWeChatBillDetails.
         :type request: :class:`tencentcloud.faceid.v20180301.models.GetWeChatBillDetailsRequest`
@@ -456,15 +456,15 @@
             model = models.GetWeChatBillDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IdCardOCRVerification(self, request):
         """本接口用于校验姓名和身份证号的真实性和一致性，您可以通过输入姓名和身份证号或传入身份证人像面照片提供所需验证信息。
 
         :param request: Request instance for IdCardOCRVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.IdCardOCRVerificationRequest`
@@ -479,15 +479,15 @@
             model = models.IdCardOCRVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IdCardVerification(self, request):
         """传入姓名和身份证号，校验两者的真实性和一致性。
 
         :param request: Request instance for IdCardVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.IdCardVerificationRequest`
@@ -502,15 +502,15 @@
             model = models.IdCardVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageRecognition(self, request):
         """传入照片和身份信息，判断该照片与权威库的证件照是否属于同一个人。
 
         :param request: Request instance for ImageRecognition.
         :type request: :class:`tencentcloud.faceid.v20180301.models.ImageRecognitionRequest`
@@ -525,15 +525,15 @@
             model = models.ImageRecognitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Liveness(self, request):
         """活体检测
 
         :param request: Request instance for Liveness.
         :type request: :class:`tencentcloud.faceid.v20180301.models.LivenessRequest`
@@ -548,15 +548,15 @@
             model = models.LivenessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LivenessCompare(self, request):
         """传入视频和照片，先判断视频中是否为真人，判断为真人后，再判断该视频中的人与上传照片是否属于同一个人。
 
         :param request: Request instance for LivenessCompare.
         :type request: :class:`tencentcloud.faceid.v20180301.models.LivenessCompareRequest`
@@ -571,15 +571,15 @@
             model = models.LivenessCompareResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LivenessRecognition(self, request):
         """传入视频和身份信息，先判断视频中是否为真人，判断为真人后，再判断该视频中的人与权威库的证件照是否属于同一个人。
 
         :param request: Request instance for LivenessRecognition.
         :type request: :class:`tencentcloud.faceid.v20180301.models.LivenessRecognitionRequest`
@@ -594,15 +594,15 @@
             model = models.LivenessRecognitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MinorsVerification(self, request):
         """通过传入手机号或姓名和身份证号，结合权威数据源和腾讯健康守护可信模型，判断该信息是否真实且年满18周岁。腾讯健康守护可信模型覆盖了上十亿手机库源，覆盖率高、准确率高，如果不在库中的手机号，还可以通过姓名+身份证进行兜底验证。
 
         :param request: Request instance for MinorsVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.MinorsVerificationRequest`
@@ -617,15 +617,15 @@
             model = models.MinorsVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MobileNetworkTimeVerification(self, request):
         """本接口用于查询手机号在网时长，输入手机号进行查询。
 
         :param request: Request instance for MobileNetworkTimeVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.MobileNetworkTimeVerificationRequest`
@@ -640,15 +640,15 @@
             model = models.MobileNetworkTimeVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MobileStatus(self, request):
         """本接口用于验证手机号的状态，您可以输入手机号进行查询。
 
         :param request: Request instance for MobileStatus.
         :type request: :class:`tencentcloud.faceid.v20180301.models.MobileStatusRequest`
@@ -663,15 +663,15 @@
             model = models.MobileStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseNfcData(self, request):
         """解析SDK获取到的证件NFC数据，接口传入SDK返回的ReqId，返回证件信息（个别字段为特定证件类型特有）。SDK生成的ReqId五分钟内有效，重复查询仅收一次费。支持身份证类证件（二代身份证、港澳居住证、台湾居住证、外国人永居证）以及旅行类证件（港澳通行证、台湾通行证、台胞证、回乡证）的NFC识别及核验。
 
         :param request: Request instance for ParseNfcData.
         :type request: :class:`tencentcloud.faceid.v20180301.models.ParseNfcDataRequest`
@@ -686,15 +686,15 @@
             model = models.ParseNfcDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PhoneVerification(self, request):
         """本接口用于校验手机号、姓名和身份证号的真实性和一致性。支持的手机号段详情请查阅<a href="https://cloud.tencent.com/document/product/1007/46063">运营商类</a>文档。
 
         :param request: Request instance for PhoneVerification.
         :type request: :class:`tencentcloud.faceid.v20180301.models.PhoneVerificationRequest`
@@ -709,15 +709,15 @@
             model = models.PhoneVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PhoneVerificationCMCC(self, request):
         """本接口用于校验中国移动手机号、姓名和身份证号的真实性和一致性。中国移动支持的手机号段详情请查阅<a href="https://cloud.tencent.com/document/product/1007/46063">运营商类</a>文档。
 
         :param request: Request instance for PhoneVerificationCMCC.
         :type request: :class:`tencentcloud.faceid.v20180301.models.PhoneVerificationCMCCRequest`
@@ -732,15 +732,15 @@
             model = models.PhoneVerificationCMCCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PhoneVerificationCTCC(self, request):
         """本接口用于校验中国电信手机号、姓名和身份证号的真实性和一致性。中国电信支持的手机号段详情请查阅<a href="https://cloud.tencent.com/document/product/1007/46063">运营商类</a>文档。
 
         :param request: Request instance for PhoneVerificationCTCC.
         :type request: :class:`tencentcloud.faceid.v20180301.models.PhoneVerificationCTCCRequest`
@@ -755,15 +755,15 @@
             model = models.PhoneVerificationCTCCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PhoneVerificationCUCC(self, request):
         """本接口用于校验中国联通手机号、姓名和身份证号的真实性和一致性。中国联通支持的手机号段详情请查阅<a href="https://cloud.tencent.com/document/product/1007/46063">运营商类</a>文档。
 
         :param request: Request instance for PhoneVerificationCUCC.
         :type request: :class:`tencentcloud.faceid.v20180301.models.PhoneVerificationCUCCRequest`
@@ -778,8 +778,8 @@
             model = models.PhoneVerificationCUCCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.938/tencentcloud/faceid/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.937/README.rst` & `tencentcloud-sdk-python-faceid-3.0.938/README.rst`

 * *Files identical despite different names*

