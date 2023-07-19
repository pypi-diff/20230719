# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.937.tar", last modified: Tue Jul 18 00:23:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.938.tar", last modified: Wed Jul 19 00:39:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.937.tar` & `tencentcloud-sdk-python-ess-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    61830 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   431046 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    62054 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   431541 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:39:00.000000 tencentcloud-sdk-python-ess-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.937/setup.py` & `tencentcloud-sdk-python-ess-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindEmployeeUserIdWithClientOpenIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelFlow(self, request):
         """用于撤销签署流程
         适用场景：如果某个合同流程当前至少还有一方没有签署，则可通过该接口取消该合同流程。常用于合同发错、内容填错，需要及时撤销的场景。
         注：如果合同流程中的参与方均已签署完毕，则无法通过该接口撤销合同。
 
@@ -67,15 +67,15 @@
             model = models.CancelFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelMultiFlowSignQRCode(self, request):
         """此接口（CancelMultiFlowSignQRCode）用于取消一码多扫二维码。该接口对传入的二维码ID，若还在有效期内，可以提前失效。
 
         :param request: Request instance for CancelMultiFlowSignQRCode.
         :type request: :class:`tencentcloud.ess.v20201111.models.CancelMultiFlowSignQRCodeRequest`
@@ -90,15 +90,15 @@
             model = models.CancelMultiFlowSignQRCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelUserAutoSignEnableUrl(self, request):
         """此接口（CancelUserAutoSignEnableUrl）用来撤销发送给个人用户的自动签开通链接，撤销后对应的个人用户开通链接失效。若个人用户已经完成开通，将无法撤销。（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for CancelUserAutoSignEnableUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CancelUserAutoSignEnableUrlRequest`
@@ -113,15 +113,15 @@
             model = models.CancelUserAutoSignEnableUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBatchCancelFlowUrl(self, request):
         """注：此接口将会废弃，请使用撤销单个签署流程（CancelFlow）接口。
         指定需要批量撤回的签署流程Id，获取批量撤销链接。
         客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回。
 
@@ -138,15 +138,15 @@
             model = models.CreateBatchCancelFlowUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateChannelSubOrganizationModifyQrCode(self, request):
         """根据产品要求，调整接口目录
 
         新接口：ChannelCreateOrganizationModifyQrCode
 
@@ -167,15 +167,15 @@
             model = models.CreateChannelSubOrganizationModifyQrCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConvertTaskApi(self, request):
         """上传了word、excel、图片文件后，通过该接口发起文件转换任务，将word、excel、图片文件转换为pdf文件。
 
         :param request: Request instance for CreateConvertTaskApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiRequest`
@@ -190,15 +190,15 @@
             model = models.CreateConvertTaskApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDocument(self, request):
         """创建签署流程电子文档
         适用场景：见创建签署流程接口。
         注：该接口需要给对应的流程指定一个模板id，并且填充该模板中需要补充的信息。是“发起流程”接口的前置接口。
 
@@ -215,15 +215,15 @@
             model = models.CreateDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlow(self, request):
         """通过模板创建签署流程<br/>
         适用场景：在标准制式的合同场景中，可通过提前预制好模板文件，每次调用模板文件的id，补充合同内容信息及签署信息生成电子合同。<br/>
         注：该接口是通过模板生成合同流程的前置接口，先创建一个不包含签署文件的流程。<br/>
         配合“创建电子文档”接口和“发起流程”接口使用。<br/>
@@ -241,15 +241,15 @@
             model = models.CreateFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowApprovers(self, request):
         """补充签署流程本企业签署人信息
         适用场景：在通过模板或者文件发起合同时，若未指定本企业签署人信息，则流程发起后，可以调用此接口补充签署人。
         同一签署人可以补充多个员工作为候选签署人,最终签署人取决于谁先领取合同完成签署。
 
@@ -268,15 +268,15 @@
             model = models.CreateFlowApproversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowByFiles(self, request):
         """此接口（CreateFlowByFiles）用来通过上传后的pdf资源编号来创建待签署的合同流程。<br/>
         适用场景1：适用非制式的合同文件签署。一般开发者自己有完整的签署文件，可以通过该接口传入完整的PDF文件及流程信息生成待签署的合同流程。<br/>
         适用场景2：可通过该接口传入制式合同文件，同时在指定位置添加签署控件。可以起到接口创建临时模板的效果。如果是标准的制式文件，建议使用模板功能生成模板ID进行合同流程的生成。<br/>
         注意事项：该接口需要依赖“多文件上传”接口生成pdf资源编号（FileIds）进行使用。<br/>
@@ -294,15 +294,15 @@
             model = models.CreateFlowByFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowEvidenceReport(self, request):
         """创建出证报告，返回报告 ID。需要配合出证套餐才能调用。
         出证需要一定时间，建议调用创建出证24小时之后再通过DescribeFlowEvidenceReport进行查询。
 
         :param request: Request instance for CreateFlowEvidenceReport.
@@ -318,15 +318,15 @@
             model = models.CreateFlowEvidenceReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowGroupByFiles(self, request):
         """此接口（CreateFlowGroupByFiles）通过多文件创建合同组签署流程。<br/>
         PDF资源Id 通过上传文件接口获取
         此接口合同组中的子合同必须都是文件发起的合同
 
@@ -343,15 +343,15 @@
             model = models.CreateFlowGroupByFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowGroupByTemplates(self, request):
         """此接口（CreateFlowGroupByTemplates）通过多模板创建合同组签署流程。<br/>
         此接口合同组中的子合同必须都是模板发起的合同。 <br/>目前最大仅支持50个子合同
 
         :param request: Request instance for CreateFlowGroupByTemplates.
@@ -367,15 +367,15 @@
             model = models.CreateFlowGroupByTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowReminds(self, request):
         """指定需要批量催办的签署流程Id，批量催办合同，最多100个; 接口失败后返回错误信息
         注意:
         该接口不可直接调用，请联系客户经理申请使用
         仅能催办当前状态为“待签署”的签署人，且只能催办一次
@@ -394,15 +394,15 @@
             model = models.CreateFlowRemindsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowSignReview(self, request):
         """提交企业签署流程审批结果
         适用场景:
         在通过接口(CreateFlow 或者CreateFlowByFiles)创建签署流程时，若指定了参数 NeedSignReview 为true，且发起方企业作为签署方参与了流程签署，则可以调用此接口提交企业内部签署审批结果。
         若签署流程状态正常，且本企业存在签署方未签署，同一签署流程可以多次提交签署审批结果，签署时的最后一个“审批结果”有效。
@@ -420,15 +420,15 @@
             model = models.CreateFlowSignReviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowSignUrl(self, request):
         """创建个人H5签署链接，请联系客户经理申请使用 <br/>
         该接口用于发起合同后，生成C端签署人的签署链接 <br/>
         注意：该接口目前签署人类型仅支持个人签署方（PERSON） <br/>
         注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
@@ -447,15 +447,15 @@
             model = models.CreateFlowSignUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationDepartment(self, request):
         """通过此接口，创建企业的部门，支持绑定客户系统部门ID。
 
         :param request: Request instance for CreateIntegrationDepartment.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationDepartmentRequest`
@@ -470,15 +470,15 @@
             model = models.CreateIntegrationDepartmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationEmployees(self, request):
         """创建员工,此接口会发送提醒员工实名的短信
 
         :param request: Request instance for CreateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesRequest`
@@ -493,15 +493,15 @@
             model = models.CreateIntegrationEmployeesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationUserRoles(self, request):
         """绑定员工与对应角色
 
         :param request: Request instance for CreateIntegrationUserRoles.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationUserRolesRequest`
@@ -516,15 +516,15 @@
             model = models.CreateIntegrationUserRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultiFlowSignQRCode(self, request):
         """此接口（CreateMultiFlowSignQRCode）用于创建一码多扫流程签署二维码。
         适用场景：无需填写签署人信息，可通过模板id生成签署二维码，签署人可通过扫描二维码补充签署信息进行实名签署。常用于提前不知道签署人的身份信息场景，例如：劳务工招工、大批量员工入职等场景。
 
         **本接口适用于发起方没有填写控件的 B2C或者单C模板**
@@ -547,15 +547,15 @@
             model = models.CreateMultiFlowSignQRCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrepareFlow(self, request):
         """创建快速发起流程
         适用场景：用户通过API 合同文件及签署信息，并可通过我们返回的URL在页面完成签署控件等信息的编辑与确认，快速发起合同.
         注：该接口文件的resourceId 是通过上传文件之后获取的。
 
@@ -572,15 +572,15 @@
             model = models.CreatePrepareFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePreparedPersonalEsign(self, request):
         """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章（处方单场景专用，使用此接口请与客户经理确认）。
 
         :param request: Request instance for CreatePreparedPersonalEsign.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignRequest`
@@ -595,15 +595,15 @@
             model = models.CreatePreparedPersonalEsignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReleaseFlow(self, request):
         """发起解除协议，主要应用场景为：基于一份已经签署的合同(签署流程)，进行解除操作。
 
         :param request: Request instance for CreateReleaseFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateReleaseFlowRequest`
@@ -618,15 +618,15 @@
             model = models.CreateReleaseFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSchemeUrl(self, request):
         """获取小程序签署链接
 
         适用场景：如果需要签署人在自己的APP、小程序、H5应用中签署，可以通过此接口获取跳转腾讯电子签小程序的签署跳转链接。
 
@@ -651,15 +651,15 @@
             model = models.CreateSchemeUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSeal(self, request):
         """创建电子印章
 
         :param request: Request instance for CreateSeal.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateSealRequest`
@@ -674,15 +674,15 @@
             model = models.CreateSealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSealPolicy(self, request):
         """对企业员工进行印章授权
 
         :param request: Request instance for CreateSealPolicy.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateSealPolicyRequest`
@@ -697,15 +697,15 @@
             model = models.CreateSealPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserAutoSignEnableUrl(self, request):
         """企业方可以通过此接口获取个人用户开启自动签的跳转链接（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for CreateUserAutoSignEnableUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateUserAutoSignEnableUrlRequest`
@@ -720,15 +720,15 @@
             model = models.CreateUserAutoSignEnableUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationDepartment(self, request):
         """通过此接口，删除企业的部门。
 
         :param request: Request instance for DeleteIntegrationDepartment.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationDepartmentRequest`
@@ -743,15 +743,15 @@
             model = models.DeleteIntegrationDepartmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationEmployees(self, request):
         """移除员工
 
         :param request: Request instance for DeleteIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationEmployeesRequest`
@@ -766,15 +766,15 @@
             model = models.DeleteIntegrationEmployeesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationRoleUsers(self, request):
         """解绑员工与对应角色关系
 
         :param request: Request instance for DeleteIntegrationRoleUsers.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationRoleUsersRequest`
@@ -789,15 +789,15 @@
             model = models.DeleteIntegrationRoleUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSealPolicies(self, request):
         """撤销员工持有的印章权限
 
         :param request: Request instance for DeleteSealPolicies.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteSealPoliciesRequest`
@@ -812,15 +812,15 @@
             model = models.DeleteSealPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExtendedServiceAuthInfos(self, request):
         """查询企业扩展服务授权信息，目前支持查询：企业静默签，企业与港澳台居民签署合同，使用手机号验证签署方身份，骑缝章，批量签署能力是否已经开通
 
         :param request: Request instance for DescribeExtendedServiceAuthInfos.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeExtendedServiceAuthInfosRequest`
@@ -835,15 +835,15 @@
             model = models.DescribeExtendedServiceAuthInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileUrls(self, request):
         """查询文件下载URL。
         适用场景：通过传参合同流程编号，下载对应的合同PDF文件流到本地。
 
         :param request: Request instance for DescribeFileUrls.
@@ -859,15 +859,15 @@
             model = models.DescribeFileUrlsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowBriefs(self, request):
         """查询流程摘要
         适用场景：可用于主动查询某个合同流程的签署状态信息。可以配合回调通知使用。
         日调用量限制：10W
 
@@ -884,15 +884,15 @@
             model = models.DescribeFlowBriefsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowComponents(self, request):
         """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
 
         :param request: Request instance for DescribeFlowComponents.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowComponentsRequest`
@@ -907,15 +907,15 @@
             model = models.DescribeFlowComponentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowEvidenceReport(self, request):
         """查询出证报告，返回报告 URL。
 
         :param request: Request instance for DescribeFlowEvidenceReport.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowEvidenceReportRequest`
@@ -930,15 +930,15 @@
             model = models.DescribeFlowEvidenceReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowInfo(self, request):
         """查询合同详情
         适用场景：可用于主动查询某个合同详情信息。
 
         :param request: Request instance for DescribeFlowInfo.
@@ -954,15 +954,15 @@
             model = models.DescribeFlowInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowTemplates(self, request):
         """当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。<br/>
         该接口常用来配合“创建电子文档”接口作为前置的接口使用。<br/>
 
         :param request: Request instance for DescribeFlowTemplates.
@@ -978,15 +978,15 @@
             model = models.DescribeFlowTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationDepartments(self, request):
         """通过此接口，查询企业的部门，支持查询单个部门节点或单个部门节点及一级子节点部门列表。
 
         :param request: Request instance for DescribeIntegrationDepartments.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationDepartmentsRequest`
@@ -1001,15 +1001,15 @@
             model = models.DescribeIntegrationDepartmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationEmployees(self, request):
         """查询企业员工列表，每次返回的数据量最大为20
 
         :param request: Request instance for DescribeIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationEmployeesRequest`
@@ -1024,15 +1024,15 @@
             model = models.DescribeIntegrationEmployeesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationMainOrganizationUser(self, request):
         """通过子企业影子账号查询主企业员工账号
 
         :param request: Request instance for DescribeIntegrationMainOrganizationUser.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationMainOrganizationUserRequest`
@@ -1047,15 +1047,15 @@
             model = models.DescribeIntegrationMainOrganizationUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationRoles(self, request):
         """查询企业角色列表
 
         :param request: Request instance for DescribeIntegrationRoles.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationRolesRequest`
@@ -1070,15 +1070,15 @@
             model = models.DescribeIntegrationRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationGroupOrganizations(self, request):
         """此API接口用户查询加入集团的成员企业
 
         :param request: Request instance for DescribeOrganizationGroupOrganizations.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeOrganizationGroupOrganizationsRequest`
@@ -1093,15 +1093,15 @@
             model = models.DescribeOrganizationGroupOrganizationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrganizationSeals(self, request):
         """查询企业印章的列表，需要操作者具有查询印章权限
         客户指定需要获取的印章数量和偏移量，数量最多100，超过100按100处理；入参InfoType控制印章是否携带授权人信息，为1则携带，为0则返回的授权人信息为空数组。接口调用成功返回印章的信息列表还有企业印章的总数。
 
         :param request: Request instance for DescribeOrganizationSeals.
@@ -1117,15 +1117,15 @@
             model = models.DescribeOrganizationSealsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeThirdPartyAuthCode(self, request):
         """通过AuthCode查询用户是否实名
 
         :param request: Request instance for DescribeThirdPartyAuthCode.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeThirdPartyAuthCodeRequest`
@@ -1140,15 +1140,15 @@
             model = models.DescribeThirdPartyAuthCodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserAutoSignStatus(self, request):
         """企业方可以通过此接口查询个人用户自动签开启状态。（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for DescribeUserAutoSignStatus.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeUserAutoSignStatusRequest`
@@ -1163,15 +1163,15 @@
             model = models.DescribeUserAutoSignStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableUserAutoSign(self, request):
         """企业方可以通过此接口关闭个人的自动签功能（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for DisableUserAutoSign.
         :type request: :class:`tencentcloud.ess.v20201111.models.DisableUserAutoSignRequest`
@@ -1186,15 +1186,15 @@
             model = models.DisableUserAutoSignResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTaskResultApi(self, request):
         """通过发起转换任务接口（CreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。<br/>
         大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for GetTaskResultApi.
@@ -1210,15 +1210,15 @@
             model = models.GetTaskResultApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationCallbackInfo(self, request):
         """新增/删除应用callbackinfo
         callbackinfo包含： 回调地址和签名key
         操作：新增/删除
 
@@ -1235,15 +1235,15 @@
             model = models.ModifyApplicationCallbackInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIntegrationDepartment(self, request):
         """通过此接口，更新企业的部门信息，支持更新部门名、客户系统部门ID、部门序列号。
 
         :param request: Request instance for ModifyIntegrationDepartment.
         :type request: :class:`tencentcloud.ess.v20201111.models.ModifyIntegrationDepartmentRequest`
@@ -1258,15 +1258,15 @@
             model = models.ModifyIntegrationDepartmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartFlow(self, request):
         """此接口用于发起流程
         适用场景：见创建签署流程接口。
         注：该接口是“创建电子文档”接口的后置接口，用于激活包含完整合同信息（模板及内容信息）的流程。激活后的流程就是一份待签署的电子合同。
 
@@ -1283,15 +1283,15 @@
             model = models.StartFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindEmployeeUserIdWithClientOpenId(self, request):
         """将存在绑定关系的电子签系统员工userId与客户系统员工openId进行解绑
 
         :param request: Request instance for UnbindEmployeeUserIdWithClientOpenId.
         :type request: :class:`tencentcloud.ess.v20201111.models.UnbindEmployeeUserIdWithClientOpenIdRequest`
@@ -1306,15 +1306,15 @@
             model = models.UnbindEmployeeUserIdWithClientOpenIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateIntegrationEmployees(self, request):
         """更新员工信息(姓名，手机号，邮件、部门)，用户实名后无法更改姓名与手机号
 
         :param request: Request instance for UpdateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesRequest`
@@ -1329,15 +1329,15 @@
             model = models.UpdateIntegrationEmployeesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadFiles(self, request):
         """此接口（UploadFiles）用于文件上传。<br/>
         适用场景：用于生成pdf资源编号（FileIds）来配合“用PDF创建流程”接口使用，使用场景可详见“用PDF创建流程”接口说明。<br/>
 
         其中上传的文件，图片类型(png/jpg/jpeg)大小限制为5M，其他大小限制为60M。<br/>
@@ -1358,15 +1358,15 @@
             model = models.UploadFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyPdf(self, request):
         """对流程的合同文件进行验证，判断文件是否合法。
 
         :param request: Request instance for VerifyPdf.
         :type request: :class:`tencentcloud.ess.v20201111.models.VerifyPdfRequest`
@@ -1381,8 +1381,8 @@
             model = models.VerifyPdfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.938/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4789,20 +4789,23 @@
         :type ReliveInfo: :class:`tencentcloud.ess.v20201111.models.RelieveInfo`
         :param _ReleasedApprovers: 非必须，解除协议的本企业签署人列表，
 默认使用原流程的签署人列表,当解除协议的签署人与原流程的签署人不能相同时（例如原流程签署人离职了），需要指定本企业其他已实名员工来替换原流程中的原签署人，注意需要指明原签署人的编号(ReceiptId,通过DescribeFlowInfo接口获取)来代表需要替换哪一个签署人
 解除协议的签署人数量不能多于原流程的签署人数量
         :type ReleasedApprovers: list of ReleasedApprover
         :param _Deadline: 签署流程的签署截止时间。 值为unix时间戳,精确到秒,不传默认为当前时间七天后
         :type Deadline: int
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._NeedRelievedFlowId = None
         self._ReliveInfo = None
         self._ReleasedApprovers = None
         self._Deadline = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -4836,14 +4839,22 @@
     def Deadline(self):
         return self._Deadline
 
     @Deadline.setter
     def Deadline(self, Deadline):
         self._Deadline = Deadline
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._NeedRelievedFlowId = params.get("NeedRelievedFlowId")
         if params.get("ReliveInfo") is not None:
@@ -4852,14 +4863,17 @@
         if params.get("ReleasedApprovers") is not None:
             self._ReleasedApprovers = []
             for item in params.get("ReleasedApprovers"):
                 obj = ReleasedApprover()
                 obj._deserialize(item)
                 self._ReleasedApprovers.append(obj)
         self._Deadline = params.get("Deadline")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.938/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.937/README.rst` & `tencentcloud-sdk-python-ess-3.0.938/README.rst`

 * *Files identical despite different names*

