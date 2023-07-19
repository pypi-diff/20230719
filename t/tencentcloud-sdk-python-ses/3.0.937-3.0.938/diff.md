# Comparing `tmp/tencentcloud-sdk-python-ses-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ses-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.937.tar", last modified: Tue Jul 18 00:29:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.938.tar", last modified: Wed Jul 19 00:44:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ses-3.0.937.tar` & `tencentcloud-sdk-python-ses-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/
--rw-r--r--   0 root         (0) root         (0)    28299 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/ses_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11392 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   110814 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:36.000000 tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/
+-rw-r--r--   0 root         (0) root         (0)    28403 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/ses_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11392 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110814 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:52.000000 tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ses-3.0.937/setup.py` & `tencentcloud-sdk-python-ses-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/ses_client.py` & `tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/ses_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchSendEmailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEmailAddress(self, request):
         """在验证了发信域名之后，您需要一个发信地址来发送邮件。例如发信域名是mail.qcloud.com，那么发信地址可以为 service@mail.qcloud.com。如果您想要收件人在收件箱列表中显示您的别名，例如"腾讯云邮件通知"。那么发信地址为： 别名 空格 尖括号 邮箱地址。请注意中间需要有空格
 
         :param request: Request instance for CreateEmailAddress.
         :type request: :class:`tencentcloud.ses.v20201002.models.CreateEmailAddressRequest`
@@ -65,15 +65,15 @@
             model = models.CreateEmailAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEmailIdentity(self, request):
         """在使用身份发送电子邮件之前，您需要有一个电子邮件域名，该域名可以是您的网站或者移动应用的域名。您首先必须进行验证，证明自己是该域名的所有者，并且授权给腾讯云SES发送许可，才可以从该域名发送电子邮件。
 
         :param request: Request instance for CreateEmailIdentity.
         :type request: :class:`tencentcloud.ses.v20201002.models.CreateEmailIdentityRequest`
@@ -88,15 +88,15 @@
             model = models.CreateEmailIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEmailTemplate(self, request):
         """创建模板，该模板可以是TXT或者HTML，请注意如果HTML不要包含外部文件的CSS。模板中的变量使用 {{变量名}} 表示。
         注意：模板需要审核通过才可以使用。
 
         :param request: Request instance for CreateEmailTemplate.
@@ -112,15 +112,15 @@
             model = models.CreateEmailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReceiver(self, request):
         """创建收件人列表，收件人列表是发送批量邮件的目标邮件地址列表。创建列表后，需要上传收件人邮箱地址。之后创建发送任务，关联列表，便可以实现批量发送邮件的功能
 
         :param request: Request instance for CreateReceiver.
         :type request: :class:`tencentcloud.ses.v20201002.models.CreateReceiverRequest`
@@ -135,15 +135,15 @@
             model = models.CreateReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReceiverDetail(self, request):
         """在创建完收件人列表后，向这个收件人列表中批量增加收件人邮箱地址，一次最大支持2万，异步完成处理。数据量比较大的时候，上传可能需要一点时间，可以通过查询收件人列表了解上传状态和上传数量。本接口与接口CreateReceiverDetailWithData的功能特性基本一致，只是不支持上传发信时的模板参数。用户首先调用创建收件人列表接口-CreateReceiver后，然后调用本接口传入收件人地址，最后使用批量发送邮件接口-BatchSendEmail，即可完成批量发信。本接口也支持追加收件人地址，也不支持去重，需要用户自己保证收件人地址不重复。本接口一次请求的收件人地址数量限制为2W条，但收件人列表中收件人地址的总量不能超过一定的数量，目前是限制5万条。
 
         :param request: Request instance for CreateReceiverDetail.
         :type request: :class:`tencentcloud.ses.v20201002.models.CreateReceiverDetailRequest`
@@ -158,15 +158,15 @@
             model = models.CreateReceiverDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReceiverDetailWithData(self, request):
         """添加收件人地址附带模板参数，使用本接口在添加收件人地址的同时传入模板参数，使每一个收件人地址在发信的时候使用的模板变量取值不同。用户首先调用创建收件人列表接口-CreateReceiver后，然后调用本接口传入收件人地址和发信时的模板参数，最后使用批量发送邮件接口-BatchSendEmail，即可完成批量发信。需要注意的是在使用本接口后BatchSendEmail接口中的Template参数不需再传。用户也可以在控制台上邮件发送-收件人列表菜单中，通过导入文件的方式，导入收件人地址和模板变量和参数值。本接口一次请求的收件人地址数量限制为2W条，本接口同时也可以用来向已经上传完成的收件人列表追加收件人地址，但收件人列表中收件人地址的总量不能超过一定的数量，目前是限制5万条。本接口不支持去除重复的收件人地址，用户需要自己保证上传和追加地址不重复，不与之前上传的地址重复。
 
         :param request: Request instance for CreateReceiverDetailWithData.
         :type request: :class:`tencentcloud.ses.v20201002.models.CreateReceiverDetailWithDataRequest`
@@ -181,15 +181,15 @@
             model = models.CreateReceiverDetailWithDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBlackList(self, request):
         """邮箱被拉黑之后，用户如果确认收件邮箱有效或者已经处于激活状态，可以从腾讯云地址库中删除该黑名单之后继续投递。
 
         :param request: Request instance for DeleteBlackList.
         :type request: :class:`tencentcloud.ses.v20201002.models.DeleteBlackListRequest`
@@ -204,15 +204,15 @@
             model = models.DeleteBlackListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEmailAddress(self, request):
         """删除发信人地址
 
         :param request: Request instance for DeleteEmailAddress.
         :type request: :class:`tencentcloud.ses.v20201002.models.DeleteEmailAddressRequest`
@@ -227,15 +227,15 @@
             model = models.DeleteEmailAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEmailIdentity(self, request):
         """删除发信域名，删除后，将不可再使用该域名进行发信
 
         :param request: Request instance for DeleteEmailIdentity.
         :type request: :class:`tencentcloud.ses.v20201002.models.DeleteEmailIdentityRequest`
@@ -250,15 +250,15 @@
             model = models.DeleteEmailIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEmailTemplate(self, request):
         """删除发信模板
 
         :param request: Request instance for DeleteEmailTemplate.
         :type request: :class:`tencentcloud.ses.v20201002.models.DeleteEmailTemplateRequest`
@@ -273,15 +273,15 @@
             model = models.DeleteEmailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReceiver(self, request):
         """根据收件id删除收件人列表,同时删除列表中的所有收件邮箱
 
         :param request: Request instance for DeleteReceiver.
         :type request: :class:`tencentcloud.ses.v20201002.models.DeleteReceiverRequest`
@@ -296,15 +296,15 @@
             model = models.DeleteReceiverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEmailIdentity(self, request):
         """获取某个发信域名的配置详情
 
         :param request: Request instance for GetEmailIdentity.
         :type request: :class:`tencentcloud.ses.v20201002.models.GetEmailIdentityRequest`
@@ -319,15 +319,15 @@
             model = models.GetEmailIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEmailTemplate(self, request):
         """根据模板ID获取模板详情
 
         :param request: Request instance for GetEmailTemplate.
         :type request: :class:`tencentcloud.ses.v20201002.models.GetEmailTemplateRequest`
@@ -342,15 +342,15 @@
             model = models.GetEmailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetSendEmailStatus(self, request):
         """获取邮件发送状态。仅支持查询30天之内的数据
         默认接口请求频率限制：1次/秒
 
         :param request: Request instance for GetSendEmailStatus.
@@ -366,15 +366,15 @@
             model = models.GetSendEmailStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetStatisticsReport(self, request):
         """获取近期发送的统计情况，包含发送量、送达率、打开率、退信率等一系列数据。
 
         :param request: Request instance for GetStatisticsReport.
         :type request: :class:`tencentcloud.ses.v20201002.models.GetStatisticsReportRequest`
@@ -389,15 +389,15 @@
             model = models.GetStatisticsReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListBlackEmailAddress(self, request):
         """腾讯云发送的邮件一旦被收件方判断为硬退(Hard Bounce)，腾讯云会拉黑该地址，并不允许所有用户向该地址发送邮件。成为邮箱黑名单。如果业务方确认是误判，可以从黑名单中删除。
 
         :param request: Request instance for ListBlackEmailAddress.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListBlackEmailAddressRequest`
@@ -412,15 +412,15 @@
             model = models.ListBlackEmailAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEmailAddress(self, request):
         """获取发信地址列表
 
         :param request: Request instance for ListEmailAddress.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListEmailAddressRequest`
@@ -435,15 +435,15 @@
             model = models.ListEmailAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEmailIdentities(self, request):
         """获取当前发信域名列表，包含已验证通过与未验证的域名
 
         :param request: Request instance for ListEmailIdentities.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListEmailIdentitiesRequest`
@@ -458,15 +458,15 @@
             model = models.ListEmailIdentitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEmailTemplates(self, request):
         """获取当前邮件模板列表
 
         :param request: Request instance for ListEmailTemplates.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListEmailTemplatesRequest`
@@ -481,15 +481,15 @@
             model = models.ListEmailTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListReceivers(self, request):
         """根据条件查询收件人列表，支持分页，模糊查询，状态查询
 
         :param request: Request instance for ListReceivers.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListReceiversRequest`
@@ -504,15 +504,15 @@
             model = models.ListReceiversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListSendTasks(self, request):
         """分页查询批量发送邮件任务，包含即时发送任务，定时发送任务，周期重复发送任务，查询发送情况，包括请求数量，已发数量，缓存数量，任务状态等信息
 
         :param request: Request instance for ListSendTasks.
         :type request: :class:`tencentcloud.ses.v20201002.models.ListSendTasksRequest`
@@ -527,15 +527,15 @@
             model = models.ListSendTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendEmail(self, request):
         """您可以通过此API发送HTML或者TEXT邮件，适用于触发类邮件（验证码、交易类）。默认仅支持使用模板发送邮件。
 
         :param request: Request instance for SendEmail.
         :type request: :class:`tencentcloud.ses.v20201002.models.SendEmailRequest`
@@ -550,15 +550,15 @@
             model = models.SendEmailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEmailIdentity(self, request):
         """您已经成功配置好了您的DNS，接下来请求腾讯云验证您的DNS配置是否正确
 
         :param request: Request instance for UpdateEmailIdentity.
         :type request: :class:`tencentcloud.ses.v20201002.models.UpdateEmailIdentityRequest`
@@ -573,15 +573,15 @@
             model = models.UpdateEmailIdentityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEmailSmtpPassWord(self, request):
         """设置邮箱的smtp密码。若要通过smtp发送邮件，必须为邮箱设置smtp密码。初始时，邮箱没有设置smtp密码，不能使用smtp的方式发送邮件。设置smtp密码后，可以修改密码。
 
         :param request: Request instance for UpdateEmailSmtpPassWord.
         :type request: :class:`tencentcloud.ses.v20201002.models.UpdateEmailSmtpPassWordRequest`
@@ -596,15 +596,15 @@
             model = models.UpdateEmailSmtpPassWordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEmailTemplate(self, request):
         """更新邮件模板，更新后需再次审核
 
         :param request: Request instance for UpdateEmailTemplate.
         :type request: :class:`tencentcloud.ses.v20201002.models.UpdateEmailTemplateRequest`
@@ -619,8 +619,8 @@
             model = models.UpdateEmailTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/errorcodes.py` & `tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.937/tencentcloud/ses/v20201002/models.py` & `tencentcloud-sdk-python-ses-3.0.938/tencentcloud/ses/v20201002/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ses-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ses-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ses-3.0.937/README.rst` & `tencentcloud-sdk-python-ses-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.937/tencentcloud_sdk_python_ses.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.938/tencentcloud_sdk_python_ses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

