# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.937.tar", last modified: Tue Jul 18 00:23:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.938.tar", last modified: Wed Jul 19 00:39:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.937.tar` & `tencentcloud-sdk-python-essbasic-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54861 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   386802 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    55045 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   386805 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:06.000000 tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             model = models.ChannelBatchCancelFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCancelFlow(self, request):
         """撤销签署流程接口，可以撤回：未全部签署完成；不可以撤回（终态）：已全部签署完成、已拒签、已过期、已撤回。
         注意:
         能撤回合同的只能是合同的发起人或者发起企业的超管、法人
 
@@ -75,15 +75,15 @@
             model = models.ChannelCancelFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCancelMultiFlowSignQRCode(self, request):
         """此接口（ChannelCancelMultiFlowSignQRCode）用于取消一码多扫二维码。该接口对传入的二维码ID，若还在有效期内，可以提前失效。
 
         :param request: Request instance for ChannelCancelMultiFlowSignQRCode.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCancelMultiFlowSignQRCodeRequest`
@@ -98,15 +98,15 @@
             model = models.ChannelCancelMultiFlowSignQRCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateBatchCancelFlowUrl(self, request):
         """指定需要批量撤销的签署流程Id，获取批量撤销链接 - 不建议使用此接口，可使用ChannelBatchCancelFlows
         客户指定需要撤销的签署流程Id，最多100个，超过100不处理；
         接口调用成功返回批量撤销合同的链接，通过链接跳转到电子签小程序完成批量撤销;
         可以撤回：未全部签署完成；不可以撤回（终态）：已全部签署完成、已拒签、已过期、已撤回。
@@ -126,15 +126,15 @@
             model = models.ChannelCreateBatchCancelFlowUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateBoundFlows(self, request):
         """此接口（ChannelCreateBoundFlows）用于子客领取合同，经办人需要有相应的角色，合同不能重复领取。
 
         :param request: Request instance for ChannelCreateBoundFlows.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateBoundFlowsRequest`
@@ -149,15 +149,15 @@
             model = models.ChannelCreateBoundFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateConvertTaskApi(self, request):
         """上传了word、excel、图片文件后，通过该接口发起文件转换任务，将word、excel、图片文件转换为pdf文件。
 
         :param request: Request instance for ChannelCreateConvertTaskApi.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateConvertTaskApiRequest`
@@ -172,15 +172,15 @@
             model = models.ChannelCreateConvertTaskApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateEmbedWebUrl(self, request):
         """本接口（ChannelCreateEmbedWebUrl）用于创建常规模块嵌入web的链接
         本接口支持创建：创建印章，创建模板，修改模板，预览模板，预览合同流程的web链接
         进入web连接后与当前控制台操作保持一致
 
@@ -197,15 +197,15 @@
             model = models.ChannelCreateEmbedWebUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowByFiles(self, request):
         """接口（ChannelCreateFlowByFiles）用于通过文件创建签署流程。此接口静默签能力不可直接使用，请联系客户经理申请使用
 
         :param request: Request instance for ChannelCreateFlowByFiles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowByFilesRequest`
@@ -220,15 +220,15 @@
             model = models.ChannelCreateFlowByFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowGroupByFiles(self, request):
         """接口（ChannelCreateFlowGroupByFiles）用于通过多文件创建合同组签署流程。
 
         :param request: Request instance for ChannelCreateFlowGroupByFiles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowGroupByFilesRequest`
@@ -243,15 +243,15 @@
             model = models.ChannelCreateFlowGroupByFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowGroupByTemplates(self, request):
         """接口（ChannelCreateFlowGroupByTemplates）用于通过多模板创建合同组签署流程。
 
         :param request: Request instance for ChannelCreateFlowGroupByTemplates.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowGroupByTemplatesRequest`
@@ -266,15 +266,15 @@
             model = models.ChannelCreateFlowGroupByTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowReminds(self, request):
         """指定需要批量催办的签署流程Id，批量催办合同，最多100个；接口失败后返回错误信息
         注意:
         该接口不可直接调用，请联系客户经理申请使用
         仅能催办当前状态为“待签署”的签署人，且只能催办一次
@@ -292,15 +292,15 @@
             model = models.ChannelCreateFlowRemindsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowSignReview(self, request):
         """提交企业流程审批结果
         目前存在两种审核操作，签署审核，发起审核
         签署审核：通过接口（CreateFlowsByTemplates或ChannelCreateFlowByFiles或ChannelCreatePrepareFlow）发起签署流程后，若指定了参数 NeedSignReview 为true,则可以调用此接口，指定operate=SignReview，提交企业内部签署审批结果；若签署流程状态正常，且本企业存在签署方未签署，同一签署流程可以多次提交签署审批结果，签署时的最后一个“审批结果”有效
 
@@ -319,15 +319,15 @@
             model = models.ChannelCreateFlowSignReviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateFlowSignUrl(self, request):
         """创建个人签署H5签署链接，请联系客户经理申请使用<br/>
         该接口用于发起合同后，生成C端签署人的签署链接<br/>
         注意：该接口目前签署人类型仅支持个人签署方（PERSON）<br/>
         注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
@@ -346,15 +346,15 @@
             model = models.ChannelCreateFlowSignUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateMultiFlowSignQRCode(self, request):
         """此接口（ChannelCreateMultiFlowSignQRCode）用于创建一码多扫流程签署二维码。 适用场景：无需填写签署人信息，可通过模板id生成签署二维码，签署人可通过扫描二维码补充签署信息进行实名签署。常用于提前不知道签署人的身份信息场景，例如：劳务工招工、大批量员工入职等场景。
 
         **本接口适用于发起方没有填写控件的 B2C或者单C模板**
 
@@ -377,15 +377,15 @@
             model = models.ChannelCreateMultiFlowSignQRCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateOrganizationModifyQrCode(self, request):
         """生成渠道子客编辑企业信息二维码
 
         :param request: Request instance for ChannelCreateOrganizationModifyQrCode.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateOrganizationModifyQrCodeRequest`
@@ -400,15 +400,15 @@
             model = models.ChannelCreateOrganizationModifyQrCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreatePrepareFlow(self, request):
         """创建预发起合同
         通过此接口指定：合同，签署人，填写控件信息，生成预创建合同链接，点击后跳转到web页面完成合同创建并发起
         可指定合同信息不可更改，签署人信息不可更改
         合同发起后，填写及签署流程与现有操作流程一致
@@ -427,15 +427,15 @@
             model = models.ChannelCreatePrepareFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateReleaseFlow(self, request):
         """发起解除协议，主要应用场景为：基于一份已经签署的合同，进行解除操作。
         合同发起人必须在电子签已经进行实名。
 
         :param request: Request instance for ChannelCreateReleaseFlow.
@@ -451,15 +451,15 @@
             model = models.ChannelCreateReleaseFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateSealPolicy(self, request):
         """将指定印章授权给第三方平台子客企业下的某些员工
 
         :param request: Request instance for ChannelCreateSealPolicy.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateSealPolicyRequest`
@@ -474,15 +474,15 @@
             model = models.ChannelCreateSealPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateUserRoles(self, request):
         """通过此接口，绑定员工角色，支持以电子签userId、客户系统userId两种方式调用。
 
         :param request: Request instance for ChannelCreateUserRoles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateUserRolesRequest`
@@ -497,15 +497,15 @@
             model = models.ChannelCreateUserRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDeleteRoleUsers(self, request):
         """通过此接口，删除员工绑定的角色，支持以电子签userId、客户系统userId两种方式调用。
 
         :param request: Request instance for ChannelDeleteRoleUsers.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteRoleUsersRequest`
@@ -520,15 +520,15 @@
             model = models.ChannelDeleteRoleUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDeleteSealPolicies(self, request):
         """删除指定印章下多个授权信息
 
         :param request: Request instance for ChannelDeleteSealPolicies.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteSealPoliciesRequest`
@@ -543,15 +543,15 @@
             model = models.ChannelDeleteSealPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeEmployees(self, request):
         """查询企业员工列表
 
         :param request: Request instance for ChannelDescribeEmployees.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeEmployeesRequest`
@@ -566,15 +566,15 @@
             model = models.ChannelDescribeEmployeesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeFlowComponents(self, request):
         """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
 
         :param request: Request instance for ChannelDescribeFlowComponents.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeFlowComponentsRequest`
@@ -589,15 +589,15 @@
             model = models.ChannelDescribeFlowComponentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeOrganizationSeals(self, request):
         """查询子客企业电子印章，需要操作者具有管理印章权限
         客户指定需要获取的印章数量和偏移量，数量最多100，超过100按100处理；入参InfoType控制印章是否携带授权人信息，为1则携带，为0则返回的授权人信息为空数组。接口调用成功返回印章的信息列表还有企业印章的总数。
 
         :param request: Request instance for ChannelDescribeOrganizationSeals.
@@ -613,15 +613,15 @@
             model = models.ChannelDescribeOrganizationSealsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeRoles(self, request):
         """查询角色列表，支持根据类型和状态过滤角色列表
 
         :param request: Request instance for ChannelDescribeRoles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeRolesRequest`
@@ -636,15 +636,15 @@
             model = models.ChannelDescribeRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelGetTaskResultApi(self, request):
         """通过发起转换任务接口（ChannelCreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for ChannelGetTaskResultApi.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelGetTaskResultApiRequest`
@@ -659,15 +659,15 @@
             model = models.ChannelGetTaskResultApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelUpdateSealStatus(self, request):
         """本接口（ChannelUpdateSealStatus）用于第三方应用平台为子客企业更新印章状态
 
         :param request: Request instance for ChannelUpdateSealStatus.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelUpdateSealStatusRequest`
@@ -682,15 +682,15 @@
             model = models.ChannelUpdateSealStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelVerifyPdf(self, request):
         """对流程的合同文件进行验证，判断文件是否合法。
 
         :param request: Request instance for ChannelVerifyPdf.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelVerifyPdfRequest`
@@ -705,15 +705,15 @@
             model = models.ChannelVerifyPdfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateChannelFlowEvidenceReport(self, request):
         """创建出证报告，返回报告 ID。需要配合出证套餐才能调用。
         出证需要一定时间，建议调用创建出证24小时之后再通过DescribeChannelFlowEvidenceReport进行查询。
 
         :param request: Request instance for CreateChannelFlowEvidenceReport.
@@ -729,15 +729,15 @@
             model = models.CreateChannelFlowEvidenceReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConsoleLoginUrl(self, request):
         """此接口（CreateConsoleLoginUrl）用于创建第三方平台子客企业控制台Web/移动登录链接。登录链接是子客控制台的唯一入口。
         若子客企业未激活，会进入企业激活流程，首次参与激活流程的经办人会成为超管。（若企业激活过程中填写信息有误，需要重置激活流程，可以换一个经办人OpenId获取新的链接进入。）
         若子客企业已激活，使用了新的经办人OpenId进入，则会进入经办人的实名流程。
         若子客企业、经办人均已完成认证，则会直接进入子客Web控制台。
@@ -755,15 +755,15 @@
             model = models.CreateConsoleLoginUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowsByTemplates(self, request):
         """接口（CreateFlowsByTemplates）用于使用模板批量创建签署流程。当前可批量发起合同（签署流程）数量为1-20个。
         如若在模板中配置了动态表格, 上传的附件必须为A4大小
         合同发起人必须在电子签已经进行实名。
 
@@ -780,15 +780,15 @@
             model = models.CreateFlowsByTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSealByImage(self, request):
         """通过图片为子客企业代创建印章，图片最大5MB
 
         :param request: Request instance for CreateSealByImage.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.CreateSealByImageRequest`
@@ -803,15 +803,15 @@
             model = models.CreateSealByImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSignUrls(self, request):
         """创建跳转小程序查看或签署的链接。
 
         跳转小程序的几种方式：主要是设置不同的EndPoint
         1. 通过链接Url直接跳转到小程序，不需要返回
@@ -848,15 +848,15 @@
             model = models.CreateSignUrlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChannelFlowEvidenceReport(self, request):
         """查询出证报告，返回报告 URL。
 
         :param request: Request instance for DescribeChannelFlowEvidenceReport.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeChannelFlowEvidenceReportRequest`
@@ -871,15 +871,15 @@
             model = models.DescribeChannelFlowEvidenceReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExtendedServiceAuthInfo(self, request):
         """查询企业扩展服务授权信息，企业经办人需要是企业超管或者法人
 
         :param request: Request instance for DescribeExtendedServiceAuthInfo.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeExtendedServiceAuthInfoRequest`
@@ -894,15 +894,15 @@
             model = models.DescribeExtendedServiceAuthInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowDetailInfo(self, request):
         """此接口（DescribeFlowDetailInfo）用于查询合同(签署流程)的详细信息。
 
         :param request: Request instance for DescribeFlowDetailInfo.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeFlowDetailInfoRequest`
@@ -917,15 +917,15 @@
             model = models.DescribeFlowDetailInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceUrlsByFlows(self, request):
         """根据签署流程信息批量获取资源下载链接，可以下载签署中、签署完的合同，需合作企业先进行授权。
         此接口直接返回下载的资源的url，与接口GetDownloadFlowUrl跳转到控制台的下载方式不同。
 
         :param request: Request instance for DescribeResourceUrlsByFlows.
@@ -941,15 +941,15 @@
             model = models.DescribeResourceUrlsByFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplates(self, request):
         """通过此接口（DescribeTemplates）查询该第三方平台子客企业在电子签拥有的有效模板，不包括第三方平台模板
 
         :param request: Request instance for DescribeTemplates.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeTemplatesRequest`
@@ -964,15 +964,15 @@
             model = models.DescribeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsage(self, request):
         """此接口（DescribeUsage）用于获取第三方平台所有合作企业流量消耗情况。
          注: 此接口每日限频2次，若要扩大限制次数,请提前与客服经理或邮件至e-contract@tencent.com进行联系。
 
         :param request: Request instance for DescribeUsage.
@@ -988,15 +988,15 @@
             model = models.DescribeUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetDownloadFlowUrl(self, request):
         """此接口（GetDownloadFlowUrl）用于创建电子签批量下载地址，让合作企业进入控制台直接下载，支持客户合同（流程）按照自定义文件夹形式 分类下载。
         当前接口限制最多合同（流程）50个.
         返回的链接只能使用一次
 
@@ -1013,15 +1013,15 @@
             model = models.GetDownloadFlowUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyExtendedService(self, request):
         """修改（操作）企业扩展服务 ，企业经办人需要是企业超管或者法人
 
         :param request: Request instance for ModifyExtendedService.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ModifyExtendedServiceRequest`
@@ -1036,15 +1036,15 @@
             model = models.ModifyExtendedServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OperateChannelTemplate(self, request):
         """此接口（OperateChannelTemplate）用于针对第三方应用平台模板库中的模板对子客企业可见性的查询和设置，不会直接分配第三方应用平台模板给子客企业。
         1、OperateType=select时：
         查询第三方应用平台模板库
         2、OperateType=update或者delete时：
@@ -1063,15 +1063,15 @@
             model = models.OperateChannelTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PrepareFlows(self, request):
         """该接口 (PrepareFlows) 用于创建待发起文件
         用户通过该接口进入签署流程发起的确认页面，进行发起信息二次确认， 如果确认则进行正常发起。
         目前该接口只支持B2C，不建议使用，将会废弃。
 
@@ -1088,15 +1088,15 @@
             model = models.PrepareFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncProxyOrganization(self, request):
         """此接口（SyncProxyOrganization）用于同步第三方平台子客企业信息，主要是子客企业的营业执照，便于子客企业开通过程中不用手动上传。若有需要调用此接口，需要在创建控制链接CreateConsoleLoginUrl之后即刻进行调用。
 
         :param request: Request instance for SyncProxyOrganization.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.SyncProxyOrganizationRequest`
@@ -1111,15 +1111,15 @@
             model = models.SyncProxyOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncProxyOrganizationOperators(self, request):
         """此接口（SyncProxyOrganizationOperators）用于同步 第三方平台子客企业经办人列表，主要是同步经办人的离职状态。子客Web控制台的组织架构管理，是依赖于第三方应用平台的，无法针对员工做新增/更新/离职等操作。
         若经办人信息有误，或者需要修改，也可以先将之前的经办人做离职操作，然后重新使用控制台链接CreateConsoleLoginUrl让经办人重新实名。
 
         :param request: Request instance for SyncProxyOrganizationOperators.
@@ -1135,15 +1135,15 @@
             model = models.SyncProxyOrganizationOperatorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFiles(self, request):
         """此接口（UploadFiles）用于文件上传。
         其中上传的文件，图片类型(png/jpg/jpeg)大小限制为5M，其他大小限制为60M。
         调用时需要设置Domain, 正式环境为 file.ess.tencent.cn。
         代码示例：
@@ -1163,8 +1163,8 @@
             model = models.UploadFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5662,15 +5662,15 @@
         self._ConsoleUrl = params.get("ConsoleUrl")
         self._IsActivated = params.get("IsActivated")
         self._ProxyOperatorIsVerified = params.get("ProxyOperatorIsVerified")
         self._RequestId = params.get("RequestId")
 
 
 class CreateFlowOption(AbstractModel):
-    """创建合同配置信息
+    """创建合同个性化参数
 
     """
 
     def __init__(self):
         r"""
         :param _CanEditFlow: 是否允许修改合同信息，true-是，false-否
         :type CanEditFlow: bool
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.ArchiveFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelFlow(self, request):
         """此接口（CancelFlow）用于撤销正在进行中的流程。
 
         注：已归档流程不可完成撤销动作。
 
@@ -69,15 +69,15 @@
             model = models.CancelFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBankCard2EVerification(self, request):
         """该接口为第三方平台向电子签平台验证银行卡二要素
 
         :param request: Request instance for CheckBankCard2EVerification.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckBankCard2EVerificationRequest`
@@ -92,15 +92,15 @@
             model = models.CheckBankCard2EVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBankCard3EVerification(self, request):
         """该接口为第三方平台向电子签平台验证银行卡三要素
 
         :param request: Request instance for CheckBankCard3EVerification.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckBankCard3EVerificationRequest`
@@ -115,15 +115,15 @@
             model = models.CheckBankCard3EVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBankCard4EVerification(self, request):
         """该接口为第三方平台向电子签平台验证银行卡四要素
 
         :param request: Request instance for CheckBankCard4EVerification.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckBankCard4EVerificationRequest`
@@ -138,15 +138,15 @@
             model = models.CheckBankCard4EVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckBankCardVerification(self, request):
         """该接口为第三方平台向电子签平台验证银行卡二/三/四要素
         银行卡二要素(同CheckBankCard2EVerification): bank_card + name
         银行卡三要素(同CheckBankCard3EVerification): bank_card + name + id_card_number
         银行卡四要素(同CheckBankCard4EVerification): bank_card + name + id_card_number + mobile
@@ -164,15 +164,15 @@
             model = models.CheckBankCardVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckFaceIdentify(self, request):
         """该接口为第三方平台向电子签平台检测慧眼或腾讯电子签小程序人脸核身结果
 
         :param request: Request instance for CheckFaceIdentify.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckFaceIdentifyRequest`
@@ -187,15 +187,15 @@
             model = models.CheckFaceIdentifyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIdCardVerification(self, request):
         """该接口为第三方平台向电子签平台验证姓名和身份证信息
 
         :param request: Request instance for CheckIdCardVerification.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckIdCardVerificationRequest`
@@ -210,15 +210,15 @@
             model = models.CheckIdCardVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckMobileAndName(self, request):
         """该接口为第三方平台向电子签平台验证手机号二要素
 
         :param request: Request instance for CheckMobileAndName.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckMobileAndNameRequest`
@@ -233,15 +233,15 @@
             model = models.CheckMobileAndNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckMobileVerification(self, request):
         """该接口为第三方平台向电子签平台验证手机号三要素
 
         :param request: Request instance for CheckMobileVerification.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckMobileVerificationRequest`
@@ -256,15 +256,15 @@
             model = models.CheckMobileVerificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckVerifyCodeMatchFlowId(self, request):
         """此接口用于确认验证码是否正确
 
         :param request: Request instance for CheckVerifyCodeMatchFlowId.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CheckVerifyCodeMatchFlowIdRequest`
@@ -279,15 +279,15 @@
             model = models.CheckVerifyCodeMatchFlowIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFaceIdSign(self, request):
         """该接口为第三方平台向电子签平台获取慧眼慧眼API签名
 
         :param request: Request instance for CreateFaceIdSign.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CreateFaceIdSignRequest`
@@ -302,15 +302,15 @@
             model = models.CreateFaceIdSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowByFiles(self, request):
         """此接口（CreateFlowByFiles）用于通过PDF文件创建签署流程。
 
         注意：调用此接口前，请先调用多文件上传接口 (UploadFiles)，提前上传合同文件。
 
@@ -327,15 +327,15 @@
             model = models.CreateFlowByFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateH5FaceIdUrl(self, request):
         """该接口为第三方平台向电子签平台获取慧眼H5人脸核身Url
 
         :param request: Request instance for CreateH5FaceIdUrl.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CreateH5FaceIdUrlRequest`
@@ -350,15 +350,15 @@
             model = models.CreateH5FaceIdUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePreviewSignUrl(self, request):
         """此接口（CreatePreviewSignUrl）用于生成生成预览签署URL。
 
         注：调用此接口前，请确保您已提前调用了发送流程接口（SendFlow）指定相关签署方。
 
@@ -375,15 +375,15 @@
             model = models.CreatePreviewSignUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSeal(self, request):
         """此接口（CreateSeal）用于创建个人/企业印章。
 
         注意：使用FileId参数指定印章，需先调用多文件上传 (UploadFiles) 上传印章图片。
 
@@ -400,15 +400,15 @@
             model = models.CreateSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServerFlowSign(self, request):
         """此接口（CreateServerFlowSign）用于静默签署文件。
 
         注：
         1、此接口为白名单接口，调用前请提前与客服经理或邮件至e-contract@tencent.com进行联系。
@@ -427,15 +427,15 @@
             model = models.CreateServerFlowSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSignUrl(self, request):
         """此接口（CreateSignUrl）用于生成指定用户的签署URL。
 
         注：调用此接口前，请确保您已提前调用了发送流程接口（SendFlow）指定相关签署方。
 
@@ -452,15 +452,15 @@
             model = models.CreateSignUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubOrganization(self, request):
         """此接口（CreateSubOrganization）用于在腾讯电子签内注册子机构。
 
         :param request: Request instance for CreateSubOrganization.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CreateSubOrganizationRequest`
@@ -475,15 +475,15 @@
             model = models.CreateSubOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubOrganizationAndSeal(self, request):
         """此接口（CreateSubOrganizationAndSeal）用于注册子机构，同时系统将为该子企业自动生成一个默认电子印章图片。
 
         注意：
         1. 在后续的签署流程中，若未指定签署使用的印章ID，则默认调用自动生成的印章图片进行签署。
@@ -502,15 +502,15 @@
             model = models.CreateSubOrganizationAndSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUser(self, request):
         """此接口（CreateUser）用于注册腾讯电子签个人用户。
 
         :param request: Request instance for CreateUser.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.CreateUserRequest`
@@ -525,15 +525,15 @@
             model = models.CreateUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserAndSeal(self, request):
         """第三方应用可通过此接口（CreateUserAndSeal）注册腾讯电子签实名个人用户，同时系统将为该用户自动生成一个默认电子签名图片。
 
         注意：
         1. 在后续的签署流程中，若未指定签署使用的印章ID，则默认调用自动生成的签名图片进行签署。
@@ -552,15 +552,15 @@
             model = models.CreateUserAndSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSeal(self, request):
         """此接口 (DeleteSeal) 用于删除指定ID的印章。
 
         注意：默认印章不支持删除
 
@@ -577,15 +577,15 @@
             model = models.DeleteSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCatalogApprovers(self, request):
         """第三方应用可通过此接口（DescribeCatalogApprovers）查询指定目录的参与者列表
 
         :param request: Request instance for DescribeCatalogApprovers.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeCatalogApproversRequest`
@@ -600,15 +600,15 @@
             model = models.DescribeCatalogApproversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCatalogSignComponents(self, request):
         """第三方应用可通过此接口（DescribeCatalogSignComponents）拉取目录签署区
 
         :param request: Request instance for DescribeCatalogSignComponents.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeCatalogSignComponentsRequest`
@@ -623,15 +623,15 @@
             model = models.DescribeCatalogSignComponentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomFlowIds(self, request):
         """此接口（DescribeCustomFlowIds）用于通过自定义流程id来查询对应的电子签流程id
 
         :param request: Request instance for DescribeCustomFlowIds.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeCustomFlowIdsRequest`
@@ -646,15 +646,15 @@
             model = models.DescribeCustomFlowIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomFlowIdsByFlowId(self, request):
         """此接口（DescribeCustomFlowIdsByFlowId）用于根据流程id反查自定义流程id
 
         :param request: Request instance for DescribeCustomFlowIdsByFlowId.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeCustomFlowIdsByFlowIdRequest`
@@ -669,15 +669,15 @@
             model = models.DescribeCustomFlowIdsByFlowIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFaceIdPhotos(self, request):
         """该接口为第三方平台向电子签平台获取慧眼人脸核身照片
 
         :param request: Request instance for DescribeFaceIdPhotos.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFaceIdPhotosRequest`
@@ -692,15 +692,15 @@
             model = models.DescribeFaceIdPhotosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFaceIdResults(self, request):
         """该接口为第三方平台向电子签平台获取慧眼人脸核身结果
 
         :param request: Request instance for DescribeFaceIdResults.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFaceIdResultsRequest`
@@ -715,15 +715,15 @@
             model = models.DescribeFaceIdResultsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileIdsByCustomIds(self, request):
         """根据用户自定义id查询文件id
 
         :param request: Request instance for DescribeFileIdsByCustomIds.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFileIdsByCustomIdsRequest`
@@ -738,15 +738,15 @@
             model = models.DescribeFileIdsByCustomIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileUrls(self, request):
         """此接口（DescribeFileUrls）用于获取签署文件下载的URL。
 
         :param request: Request instance for DescribeFileUrls.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFileUrlsRequest`
@@ -761,15 +761,15 @@
             model = models.DescribeFileUrlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlow(self, request):
         """通过此接口（DescribeFlow）可查询签署流程的详细信息。
 
         :param request: Request instance for DescribeFlow.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFlowRequest`
@@ -784,15 +784,15 @@
             model = models.DescribeFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowApprovers(self, request):
         """第三方应用可通过此接口（DescribeFlowApprovers）查询流程参与者信息。
 
         :param request: Request instance for DescribeFlowApprovers.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFlowApproversRequest`
@@ -807,15 +807,15 @@
             model = models.DescribeFlowApproversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowFiles(self, request):
         """查询流程文件
 
         :param request: Request instance for DescribeFlowFiles.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeFlowFilesRequest`
@@ -830,15 +830,15 @@
             model = models.DescribeFlowFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSeals(self, request):
         """此接口（DescribeSeals）用于查询指定ID的印章信息。
 
         :param request: Request instance for DescribeSeals.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.DescribeSealsRequest`
@@ -853,15 +853,15 @@
             model = models.DescribeSealsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubOrganizations(self, request):
         """此接口（DescribeSubOrganizations）用于查询子机构信息。
 
         注：此接口仅可查询您所属机构应用号创建的子机构信息，不可跨应用/跨机构查询。
 
@@ -878,15 +878,15 @@
             model = models.DescribeSubOrganizationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsers(self, request):
         """此接口（DescribeUsers）用于查询应用号下的个人用户信息。
 
         注：此接口仅可查询您所属机构应用号创建的个人用户信息，不可跨应用/跨机构查询。
 
@@ -903,15 +903,15 @@
             model = models.DescribeUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyFlowFile(self, request):
         """通过此接口（DestroyFlowFile）可删除指定流程中的合同文件。
 
         注：调用此接口前，请确保此流程已属于归档状态。您可通过查询流程信息接口（DescribeFlow）进行查询。
 
@@ -928,15 +928,15 @@
             model = models.DestroyFlowFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateOrganizationSeal(self, request):
         """生成企业电子印章
 
         :param request: Request instance for GenerateOrganizationSeal.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.GenerateOrganizationSealRequest`
@@ -951,15 +951,15 @@
             model = models.GenerateOrganizationSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateUserSeal(self, request):
         """此接口（GenerateUserSeal）用于生成个人签名图片。
 
         注意：
         1. 个人签名由用户注册时预留的姓名信息生成，不支持自定义签名内容。
@@ -978,15 +978,15 @@
             model = models.GenerateUserSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyOrganizationDefaultSeal(self, request):
         """此接口 (ModifyOrganizationDefaultSeal) 用于重新指定企业默认印章。
 
         :param request: Request instance for ModifyOrganizationDefaultSeal.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.ModifyOrganizationDefaultSealRequest`
@@ -1001,15 +1001,15 @@
             model = models.ModifyOrganizationDefaultSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySeal(self, request):
         """此接口（ModifySeal）用于修改指定印章ID的印章图片和名称。
 
         注：印章类型暂不支持修改，如需调整，请联系客服经理或通过创建印章接口（CreateSeal）进行创建新印章。
 
@@ -1026,15 +1026,15 @@
             model = models.ModifySealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubOrganizationInfo(self, request):
         """此接口（ModifySubOrganizationInfo）用于更新子机构信息。
 
         注：若修改子机构名称或更新机构证件照片，需要重新通过子机构实名接口（VerifySubOrganization）进行重新实名。
 
@@ -1051,15 +1051,15 @@
             model = models.ModifySubOrganizationInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUser(self, request):
         """此接口（ModifyUser）用于更新个人用户信息。
 
         注：若修改用户姓名，需要重新通过个人用户实名接口（VerifyUser）进行重新实名。
 
@@ -1076,15 +1076,15 @@
             model = models.ModifyUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserDefaultSeal(self, request):
         """此接口 (ModifyUserDefaultSeal) 用于重新指定个人默认印章。
 
         :param request: Request instance for ModifyUserDefaultSeal.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.ModifyUserDefaultSealRequest`
@@ -1099,15 +1099,15 @@
             model = models.ModifyUserDefaultSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RejectFlow(self, request):
         """此接口（RejectFlow）用于用户拒绝签署合同流程。
 
         :param request: Request instance for RejectFlow.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.RejectFlowRequest`
@@ -1122,15 +1122,15 @@
             model = models.RejectFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendFlow(self, request):
         """此接口（SendFlow）用于指定签署者及签署内容，后续可通过生成签署接口（CreateSignUrl）获取签署url。
 
         :param request: Request instance for SendFlow.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.SendFlowRequest`
@@ -1145,15 +1145,15 @@
             model = models.SendFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendFlowUrl(self, request):
         """发送流程并获取签署URL
 
         :param request: Request instance for SendFlowUrl.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.SendFlowUrlRequest`
@@ -1168,15 +1168,15 @@
             model = models.SendFlowUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendSignInnerVerifyCode(self, request):
         """此接口用于发送签署验证码
 
         :param request: Request instance for SendSignInnerVerifyCode.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.SendSignInnerVerifyCodeRequest`
@@ -1191,15 +1191,15 @@
             model = models.SendSignInnerVerifyCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SignFlow(self, request):
         """此接口（SignFlow）可用于对流程文件进行签署。
 
         :param request: Request instance for SignFlow.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.SignFlowRequest`
@@ -1214,15 +1214,15 @@
             model = models.SignFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFiles(self, request):
         """此接口（UploadFiles）用于文件上传。
 
         :param request: Request instance for UploadFiles.
         :type request: :class:`tencentcloud.essbasic.v20201222.models.UploadFilesRequest`
@@ -1237,15 +1237,15 @@
             model = models.UploadFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifySubOrganization(self, request):
         """此接口（VerifySubOrganization）用于通过子机构的实名认证。
 
         注：此接口为白名单接口，如您需要使用此能力，请提前与客户经理沟通或邮件至e-contract@tencent.com与我们联系。
 
@@ -1262,15 +1262,15 @@
             model = models.VerifySubOrganizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyUser(self, request):
         """第三方应用可通过此接口（VerifyUser）将腾讯电子签个人用户的实名认证状态设为通过。
 
         注：此接口为白名单接口，如您需要使用此能力，请提前与客户经理沟通或邮件至e-contract@tencent.com与我们联系。
 
@@ -1287,8 +1287,8 @@
             model = models.VerifyUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.938/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.938/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

