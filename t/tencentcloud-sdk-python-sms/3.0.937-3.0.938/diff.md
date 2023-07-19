# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.937.tar", last modified: Tue Jul 18 00:29:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.938.tar", last modified: Wed Jul 19 00:45:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.937.tar` & `tencentcloud-sdk-python-sms-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28333 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)   104651 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26567 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    93545 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:53.000000 tencentcloud-sdk-python-sms-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28405 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)   104651 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26631 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    93545 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:45:09.000000 tencentcloud-sdk-python-sms-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-sms-3.0.937/setup.py` & `tencentcloud-sdk-python-sms-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/sms_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             model = models.AddSmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddSmsTemplate(self, request):
         """1. 添加短信模板，申请之前请先认真参阅 [腾讯云短信正文模板审核标准](https://cloud.tencent.com/document/product/382/39023)。
         2. ⚠️注意：个人认证用户不支持使用 API 申请短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 申请短信正文模板。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -71,15 +71,15 @@
             model = models.AddSmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallbackStatusStatistics(self, request):
         """统计用户回执的数据。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -96,15 +96,15 @@
             model = models.CallbackStatusStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSmsSign(self, request):
         """⚠️注意：个人认证用户不支持使用 API 删除短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，请登录 [控制台](https://console.cloud.tencent.com/smsv2) 删除短信签名。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -121,15 +121,15 @@
             model = models.DeleteSmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSmsTemplate(self, request):
         """⚠️注意：个人认证用户不支持使用 API 删除短信正文模板，请登录 [控制台](https://console.cloud.tencent.com/smsv2) 删除短信正文模板，如需了解请参阅 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -146,15 +146,15 @@
             model = models.DeleteSmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePhoneNumberInfo(self, request):
         """提供电话号码的信息查询，包括国家（或地区）码、规范的 E.164 格式号码等。
         >- 例如：查询号码 +86018845720123，可以得到国家码 86、规范的 E.164 号码 +8618845720123 等信息。
 
         :param request: Request instance for DescribePhoneNumberInfo.
@@ -170,15 +170,15 @@
             model = models.DescribePhoneNumberInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsSignList(self, request):
         """⚠️注意：个人认证用户不支持使用 API 查询短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629),如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 查询短信签名。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -195,15 +195,15 @@
             model = models.DescribeSmsSignListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsTemplateList(self, request):
         """⚠️注意：个人认证用户不支持使用 API 查询短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -220,15 +220,15 @@
             model = models.DescribeSmsTemplateListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySmsSign(self, request):
         """1. 修改短信签名，修改之前请先认真参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信签名。
         3. 修改短信签名，仅当签名为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的签名不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
@@ -247,15 +247,15 @@
             model = models.ModifySmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySmsTemplate(self, request):
         """1. 修改短信正文模板，修改之前请先认真参阅 [腾讯云短信正文模板审核标准](https://cloud.tencent.com/document/product/382/39023)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信正文模板。
         3. 修改短信模板，仅当正文模板为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的正文模板不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
@@ -274,15 +274,15 @@
             model = models.ModifySmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsReplyStatus(self, request):
         """拉取短信回复状态。
         目前也支持 [配置回复回调](https://cloud.tencent.com/document/product/382/42907) 的方式来获取上行回复。
         >- 注：此接口需要联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81) 开通。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
@@ -301,15 +301,15 @@
             model = models.PullSmsReplyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsReplyStatusByPhoneNumber(self, request):
         """拉取单个号码短信回复状态。
         目前也支持 [配置回复回调](https://cloud.tencent.com/document/product/382/42907) 的方式来获取上行回复。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -327,15 +327,15 @@
             model = models.PullSmsReplyStatusByPhoneNumberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsSendStatus(self, request):
         """拉取短信下发状态。
         目前也支持 [配置回调](https://cloud.tencent.com/document/product/382/37809#.E8.AE.BE.E7.BD.AE.E4.BA.8B.E4.BB.B6.E5.9B.9E.E8.B0.83.E9.85.8D.E7.BD.AE) 的方式来获取下发状态。
         >- 注：此接口需要联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81) 开通。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
@@ -354,15 +354,15 @@
             model = models.PullSmsSendStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsSendStatusByPhoneNumber(self, request):
         """拉取单个号码短信下发状态。
         目前也支持 [配置回调](https://cloud.tencent.com/document/product/382/37809#.E8.AE.BE.E7.BD.AE.E4.BA.8B.E4.BB.B6.E5.9B.9E.E8.B0.83.E9.85.8D.E7.BD.AE) 的方式来获取下发状态。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -380,15 +380,15 @@
             model = models.PullSmsSendStatusByPhoneNumberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReportConversion(self, request):
         """短信转化率上报。将已接收到短信的流水号上报到腾讯云短信服务。
         >- 注：当前接口以白名单方式对外开放，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81) 开通。
 
         :param request: Request instance for ReportConversion.
@@ -404,15 +404,15 @@
             model = models.ReportConversionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSms(self, request):
         """短信发送接口，用于给用户发短信验证码、通知类短信或营销短信。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 注：您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
         >- 注：当前接口属于 2021-01-11 版本，如果您仍在使用 [2019-07-11 版本](https://cloud.tencent.com/document/product/382/38778)，建议您使用当前最新版本的接口，版本差异可参考[版本描述](https://cloud.tencent.com/document/product/382/63195#.E7.89.88.E6.9C.AC.E6.8F.8F.E8.BF.B0)。
@@ -430,15 +430,15 @@
             model = models.SendSmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendStatusStatistics(self, request):
         """统计用户发送短信的数据。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -455,15 +455,15 @@
             model = models.SendStatusStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SmsPackagesStatistics(self, request):
         """用户套餐包信息统计。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -480,8 +480,8 @@
             model = models.SmsPackagesStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/sms_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             model = models.AddSmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddSmsTemplate(self, request):
         """1. 添加短信模板，申请之前请先认真参阅 [腾讯云短信正文模板审核标准](https://cloud.tencent.com/document/product/382/39023)。
         2. ⚠️注意：个人认证用户不支持使用 API 申请短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 申请短信正文模板。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -71,15 +71,15 @@
             model = models.AddSmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CallbackStatusStatistics(self, request):
         """统计用户回执的数据。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -96,15 +96,15 @@
             model = models.CallbackStatusStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSmsSign(self, request):
         """⚠️注意：个人认证用户不支持使用 API 删除短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，请登录 [控制台](https://console.cloud.tencent.com/smsv2) 删除短信签名。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -121,15 +121,15 @@
             model = models.DeleteSmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSmsTemplate(self, request):
         """⚠️注意：个人认证用户不支持使用 API 删除短信正文模板，请登录 [控制台](https://console.cloud.tencent.com/smsv2) 删除短信正文模板，如需了解请参阅 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -146,15 +146,15 @@
             model = models.DeleteSmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsSignList(self, request):
         """⚠️注意：个人认证用户不支持使用 API 查询短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629),如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 查询短信签名。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -171,15 +171,15 @@
             model = models.DescribeSmsSignListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSmsTemplateList(self, request):
         """⚠️注意：个人认证用户不支持使用 API 查询短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -196,15 +196,15 @@
             model = models.DescribeSmsTemplateListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySmsSign(self, request):
         """1. 修改短信签名，修改之前请先认真参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信签名。
         3. 修改短信签名，仅当签名为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的签名不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
@@ -223,15 +223,15 @@
             model = models.ModifySmsSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySmsTemplate(self, request):
         """1. 修改短信正文模板，修改之前请先认真参阅 [腾讯云短信正文模板审核标准](https://cloud.tencent.com/document/product/382/39023)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信正文模板，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信正文模板。
         3. 修改短信模板，仅当正文模板为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的正文模板不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
@@ -250,15 +250,15 @@
             model = models.ModifySmsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsReplyStatus(self, request):
         """拉取短信回复状态。
         目前也支持 [配置回复回调](https://cloud.tencent.com/document/product/382/42907) 的方式来获取上行回复。
         >- 注：此接口需要联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81) 开通。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
@@ -277,15 +277,15 @@
             model = models.PullSmsReplyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsReplyStatusByPhoneNumber(self, request):
         """拉取单个号码短信回复状态。
         目前也支持 [配置回复回调](https://cloud.tencent.com/document/product/382/42907) 的方式来获取上行回复。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -303,15 +303,15 @@
             model = models.PullSmsReplyStatusByPhoneNumberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsSendStatus(self, request):
         """拉取短信下发状态。
         目前也支持 [配置回调](https://cloud.tencent.com/document/product/382/37809#.E8.AE.BE.E7.BD.AE.E4.BA.8B.E4.BB.B6.E5.9B.9E.E8.B0.83.E9.85.8D.E7.BD.AE) 的方式来获取下发状态。
         >- 注：此接口需要联系 [sms helper](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81) 开通。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
@@ -330,15 +330,15 @@
             model = models.PullSmsSendStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PullSmsSendStatusByPhoneNumber(self, request):
         """拉取单个号码短信下发状态。
         目前也支持 [配置回调](https://cloud.tencent.com/document/product/382/37809#.E8.AE.BE.E7.BD.AE.E4.BA.8B.E4.BB.B6.E5.9B.9E.E8.B0.83.E9.85.8D.E7.BD.AE) 的方式来获取下发状态。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
@@ -356,15 +356,15 @@
             model = models.PullSmsSendStatusByPhoneNumberResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSms(self, request):
         """短信发送接口，用于给用户发短信验证码、通知类短信或营销短信。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -381,15 +381,15 @@
             model = models.SendSmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendStatusStatistics(self, request):
         """统计用户发送短信的数据。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -406,15 +406,15 @@
             model = models.SendStatusStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SmsPackagesStatistics(self, request):
         """用户套餐包信息统计。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
@@ -431,8 +431,8 @@
             model = models.SmsPackagesStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.937/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.938/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.937/README.rst` & `tencentcloud-sdk-python-sms-3.0.938/README.rst`

 * *Files identical despite different names*

