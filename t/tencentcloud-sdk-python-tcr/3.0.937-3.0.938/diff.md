# Comparing `tmp/tencentcloud-sdk-python-tcr-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcr-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.937.tar", last modified: Tue Jul 18 00:31:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.938.tar", last modified: Wed Jul 19 00:49:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcr-3.0.937.tar` & `tencentcloud-sdk-python-tcr-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)   104150 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/tcr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8520 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   443674 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:49.000000 tencentcloud-sdk-python-tcr-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)   104598 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/tcr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   443674 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:49:16.000000 tencentcloud-sdk-python-tcr-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/setup.py` & `tencentcloud-sdk-python-tcr-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchDeleteImagePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDeleteRepositoryPersonal(self, request):
         """用于个人版镜像仓库中批量删除镜像仓库
 
         :param request: Request instance for BatchDeleteRepositoryPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.BatchDeleteRepositoryPersonalRequest`
@@ -65,15 +65,15 @@
             model = models.BatchDeleteRepositoryPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckInstance(self, request):
         """用于校验企业版实例信息
 
         :param request: Request instance for CheckInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CheckInstanceRequest`
@@ -88,15 +88,15 @@
             model = models.CheckInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckInstanceName(self, request):
         """检查待创建的实例名称是否符合规范
 
         :param request: Request instance for CheckInstanceName.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CheckInstanceNameRequest`
@@ -111,15 +111,15 @@
             model = models.CheckInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationTriggerPersonal(self, request):
         """用于创建应用更新触发器
 
         :param request: Request instance for CreateApplicationTriggerPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateApplicationTriggerPersonalRequest`
@@ -134,15 +134,15 @@
             model = models.CreateApplicationTriggerPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomAccount(self, request):
         """创建自定义账户
 
         :param request: Request instance for CreateCustomAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateCustomAccountRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCustomAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImageAccelerationService(self, request):
         """创建镜像加速服务
 
         :param request: Request instance for CreateImageAccelerationService.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateImageAccelerationServiceRequest`
@@ -180,15 +180,15 @@
             model = models.CreateImageAccelerationServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImmutableTagRules(self, request):
         """创建镜像不可变规则
 
         :param request: Request instance for CreateImmutableTagRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateImmutableTagRulesRequest`
@@ -203,15 +203,15 @@
             model = models.CreateImmutableTagRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstance(self, request):
         """创建实例
 
         :param request: Request instance for CreateInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateInstanceRequest`
@@ -226,15 +226,15 @@
             model = models.CreateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstanceCustomizedDomain(self, request):
         """创建自定义域名
 
         :param request: Request instance for CreateInstanceCustomizedDomain.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateInstanceCustomizedDomainRequest`
@@ -249,15 +249,15 @@
             model = models.CreateInstanceCustomizedDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstanceToken(self, request):
         """创建实例的临时或长期访问凭证
 
         :param request: Request instance for CreateInstanceToken.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateInstanceTokenRequest`
@@ -272,15 +272,15 @@
             model = models.CreateInstanceTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInternalEndpointDns(self, request):
         """创建tcr内网私有域名解析
 
         :param request: Request instance for CreateInternalEndpointDns.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateInternalEndpointDnsRequest`
@@ -295,15 +295,15 @@
             model = models.CreateInternalEndpointDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMultipleSecurityPolicy(self, request):
         """用于在TCR实例中，创建多个白名单策略
 
         :param request: Request instance for CreateMultipleSecurityPolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateMultipleSecurityPolicyRequest`
@@ -318,15 +318,15 @@
             model = models.CreateMultipleSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespace(self, request):
         """用于在企业版中创建命名空间
 
         :param request: Request instance for CreateNamespace.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateNamespaceRequest`
@@ -341,15 +341,15 @@
             model = models.CreateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespacePersonal(self, request):
         """创建个人版镜像仓库命名空间，此命名空间全局唯一
 
         :param request: Request instance for CreateNamespacePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateNamespacePersonalRequest`
@@ -364,15 +364,15 @@
             model = models.CreateNamespacePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReplicationInstance(self, request):
         """创建从实例
 
         :param request: Request instance for CreateReplicationInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateReplicationInstanceRequest`
@@ -387,15 +387,15 @@
             model = models.CreateReplicationInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRepository(self, request):
         """用于企业版创建镜像仓库
 
         :param request: Request instance for CreateRepository.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateRepositoryRequest`
@@ -410,15 +410,15 @@
             model = models.CreateRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRepositoryPersonal(self, request):
         """用于在个人版仓库中创建镜像仓库
 
         :param request: Request instance for CreateRepositoryPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateRepositoryPersonalRequest`
@@ -433,15 +433,15 @@
             model = models.CreateRepositoryPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityPolicy(self, request):
         """创建实例公网访问白名单策略
 
         :param request: Request instance for CreateSecurityPolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateSecurityPolicyRequest`
@@ -456,15 +456,15 @@
             model = models.CreateSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceAccount(self, request):
         """创建自定义账户
 
         :param request: Request instance for CreateServiceAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateServiceAccountRequest`
@@ -479,15 +479,15 @@
             model = models.CreateServiceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSignature(self, request):
         """为一个镜像版本创建签名
 
         :param request: Request instance for CreateSignature.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateSignatureRequest`
@@ -502,15 +502,15 @@
             model = models.CreateSignatureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSignaturePolicy(self, request):
         """创建镜像签名策略
 
         :param request: Request instance for CreateSignaturePolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateSignaturePolicyRequest`
@@ -525,15 +525,15 @@
             model = models.CreateSignaturePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTagRetentionExecution(self, request):
         """手动执行版本保留
 
         :param request: Request instance for CreateTagRetentionExecution.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateTagRetentionExecutionRequest`
@@ -548,15 +548,15 @@
             model = models.CreateTagRetentionExecutionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTagRetentionRule(self, request):
         """创建版本保留规则
 
         :param request: Request instance for CreateTagRetentionRule.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateTagRetentionRuleRequest`
@@ -571,15 +571,15 @@
             model = models.CreateTagRetentionRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserPersonal(self, request):
         """创建个人用户
 
         :param request: Request instance for CreateUserPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateUserPersonalRequest`
@@ -594,15 +594,15 @@
             model = models.CreateUserPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWebhookTrigger(self, request):
         """创建触发器
 
         :param request: Request instance for CreateWebhookTrigger.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateWebhookTriggerRequest`
@@ -617,15 +617,15 @@
             model = models.CreateWebhookTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplicationTriggerPersonal(self, request):
         """用于删除应用更新触发器
 
         :param request: Request instance for DeleteApplicationTriggerPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteApplicationTriggerPersonalRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteApplicationTriggerPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomAccount(self, request):
         """删除自定义账号
 
         :param request: Request instance for DeleteCustomAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteCustomAccountRequest`
@@ -663,15 +663,15 @@
             model = models.DeleteCustomAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImage(self, request):
         """删除指定镜像
 
         :param request: Request instance for DeleteImage.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImageRequest`
@@ -686,15 +686,15 @@
             model = models.DeleteImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageAccelerateService(self, request):
         """删除镜像加速服务
 
         :param request: Request instance for DeleteImageAccelerateService.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImageAccelerateServiceRequest`
@@ -709,15 +709,15 @@
             model = models.DeleteImageAccelerateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageLifecycleGlobalPersonal(self, request):
         """用于删除个人版全局镜像版本自动清理策略
 
         :param request: Request instance for DeleteImageLifecycleGlobalPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImageLifecycleGlobalPersonalRequest`
@@ -732,15 +732,15 @@
             model = models.DeleteImageLifecycleGlobalPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImagePersonal(self, request):
         """用于在个人版中删除tag
 
         :param request: Request instance for DeleteImagePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImagePersonalRequest`
@@ -755,15 +755,15 @@
             model = models.DeleteImagePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImmutableTagRules(self, request):
         """删除镜像不可变规则
 
         :param request: Request instance for DeleteImmutableTagRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImmutableTagRulesRequest`
@@ -778,15 +778,15 @@
             model = models.DeleteImmutableTagRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstance(self, request):
         """删除镜像仓库企业版实例
 
         :param request: Request instance for DeleteInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteInstanceRequest`
@@ -801,15 +801,15 @@
             model = models.DeleteInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstanceCustomizedDomain(self, request):
         """删除自定义域名
 
         :param request: Request instance for DeleteInstanceCustomizedDomain.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteInstanceCustomizedDomainRequest`
@@ -824,15 +824,15 @@
             model = models.DeleteInstanceCustomizedDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstanceToken(self, request):
         """删除长期访问凭证
 
         :param request: Request instance for DeleteInstanceToken.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteInstanceTokenRequest`
@@ -847,15 +847,15 @@
             model = models.DeleteInstanceTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInternalEndpointDns(self, request):
         """删除tcr内网私有域名解析
 
         :param request: Request instance for DeleteInternalEndpointDns.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteInternalEndpointDnsRequest`
@@ -870,15 +870,15 @@
             model = models.DeleteInternalEndpointDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMultipleSecurityPolicy(self, request):
         """用于删除实例多个公网访问白名单策略
 
         :param request: Request instance for DeleteMultipleSecurityPolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteMultipleSecurityPolicyRequest`
@@ -893,15 +893,15 @@
             model = models.DeleteMultipleSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNamespace(self, request):
         """删除命名空间
 
         :param request: Request instance for DeleteNamespace.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteNamespaceRequest`
@@ -916,15 +916,15 @@
             model = models.DeleteNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNamespacePersonal(self, request):
         """删除共享版命名空间
 
         :param request: Request instance for DeleteNamespacePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteNamespacePersonalRequest`
@@ -939,15 +939,15 @@
             model = models.DeleteNamespacePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReplicationInstance(self, request):
         """删除从实例
 
         :param request: Request instance for DeleteReplicationInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteReplicationInstanceRequest`
@@ -962,15 +962,15 @@
             model = models.DeleteReplicationInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRepository(self, request):
         """删除镜像仓库
 
         :param request: Request instance for DeleteRepository.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteRepositoryRequest`
@@ -985,15 +985,15 @@
             model = models.DeleteRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRepositoryPersonal(self, request):
         """用于个人版镜像仓库中删除
 
         :param request: Request instance for DeleteRepositoryPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteRepositoryPersonalRequest`
@@ -1008,15 +1008,15 @@
             model = models.DeleteRepositoryPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRepositoryTags(self, request):
         """用于企业版批量删除Repository Tag
 
         :param request: Request instance for DeleteRepositoryTags.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteRepositoryTagsRequest`
@@ -1031,15 +1031,15 @@
             model = models.DeleteRepositoryTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityPolicy(self, request):
         """删除实例公网访问白名单策略
 
         注意：当PolicyIndex和CidrBlock同时存在时，CidrBlock优先级更高
 
@@ -1056,15 +1056,15 @@
             model = models.DeleteSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceAccount(self, request):
         """删除服务级账号
 
         :param request: Request instance for DeleteServiceAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteServiceAccountRequest`
@@ -1079,15 +1079,15 @@
             model = models.DeleteServiceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSignaturePolicy(self, request):
         """删除命名空间加签策略
 
         :param request: Request instance for DeleteSignaturePolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteSignaturePolicyRequest`
@@ -1102,15 +1102,15 @@
             model = models.DeleteSignaturePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTagRetentionRule(self, request):
         """删除版本保留规则
 
         :param request: Request instance for DeleteTagRetentionRule.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteTagRetentionRuleRequest`
@@ -1125,15 +1125,15 @@
             model = models.DeleteTagRetentionRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWebhookTrigger(self, request):
         """删除触发器
 
         :param request: Request instance for DeleteWebhookTrigger.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteWebhookTriggerRequest`
@@ -1148,15 +1148,15 @@
             model = models.DeleteWebhookTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationTriggerLogPersonal(self, request):
         """用于查询应用更新触发器触发日志
 
         :param request: Request instance for DescribeApplicationTriggerLogPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeApplicationTriggerLogPersonalRequest`
@@ -1171,15 +1171,15 @@
             model = models.DescribeApplicationTriggerLogPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationTriggerPersonal(self, request):
         """用于查询应用更新触发器
 
         :param request: Request instance for DescribeApplicationTriggerPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeApplicationTriggerPersonalRequest`
@@ -1194,15 +1194,15 @@
             model = models.DescribeApplicationTriggerPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeChartDownloadInfo(self, request):
         """用于在企业版中返回Chart的下载信息
 
         :param request: Request instance for DescribeChartDownloadInfo.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeChartDownloadInfoRequest`
@@ -1217,15 +1217,15 @@
             model = models.DescribeChartDownloadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomAccounts(self, request):
         """查询自定义账号
 
         :param request: Request instance for DescribeCustomAccounts.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeCustomAccountsRequest`
@@ -1240,15 +1240,15 @@
             model = models.DescribeCustomAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExternalEndpointStatus(self, request):
         """查询实例公网访问入口状态
 
         :param request: Request instance for DescribeExternalEndpointStatus.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeExternalEndpointStatusRequest`
@@ -1263,15 +1263,15 @@
             model = models.DescribeExternalEndpointStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFavorRepositoryPersonal(self, request):
         """查询个人收藏仓库
 
         :param request: Request instance for DescribeFavorRepositoryPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeFavorRepositoryPersonalRequest`
@@ -1286,15 +1286,15 @@
             model = models.DescribeFavorRepositoryPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGCJobs(self, request):
         """GC 最近10条历史
 
         :param request: Request instance for DescribeGCJobs.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeGCJobsRequest`
@@ -1309,15 +1309,15 @@
             model = models.DescribeGCJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageAccelerateService(self, request):
         """查询镜像加速服务状态
 
         :param request: Request instance for DescribeImageAccelerateService.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImageAccelerateServiceRequest`
@@ -1332,15 +1332,15 @@
             model = models.DescribeImageAccelerateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageFilterPersonal(self, request):
         """用于在个人版中查询与指定tag镜像内容相同的tag列表
 
         :param request: Request instance for DescribeImageFilterPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImageFilterPersonalRequest`
@@ -1355,15 +1355,15 @@
             model = models.DescribeImageFilterPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageLifecycleGlobalPersonal(self, request):
         """用于获取个人版全局镜像版本自动清理策略
 
         :param request: Request instance for DescribeImageLifecycleGlobalPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImageLifecycleGlobalPersonalRequest`
@@ -1378,15 +1378,15 @@
             model = models.DescribeImageLifecycleGlobalPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageLifecyclePersonal(self, request):
         """用于获取个人版仓库中自动清理策略
 
         :param request: Request instance for DescribeImageLifecyclePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImageLifecyclePersonalRequest`
@@ -1401,15 +1401,15 @@
             model = models.DescribeImageLifecyclePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageManifests(self, request):
         """查询容器镜像Manifest信息
 
         :param request: Request instance for DescribeImageManifests.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImageManifestsRequest`
@@ -1424,15 +1424,15 @@
             model = models.DescribeImageManifestsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImagePersonal(self, request):
         """用于获取个人版镜像仓库tag列表
 
         :param request: Request instance for DescribeImagePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImagePersonalRequest`
@@ -1447,15 +1447,15 @@
             model = models.DescribeImagePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """查询镜像版本列表或指定容器镜像信息
 
         :param request: Request instance for DescribeImages.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImagesRequest`
@@ -1470,15 +1470,15 @@
             model = models.DescribeImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImmutableTagRules(self, request):
         """列出镜像不可变规则
 
         :param request: Request instance for DescribeImmutableTagRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeImmutableTagRulesRequest`
@@ -1493,15 +1493,15 @@
             model = models.DescribeImmutableTagRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceAllNamespaces(self, request):
         """查询所有实例命名空间列表
 
         :param request: Request instance for DescribeInstanceAllNamespaces.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInstanceAllNamespacesRequest`
@@ -1516,15 +1516,15 @@
             model = models.DescribeInstanceAllNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceCustomizedDomain(self, request):
         """查询实例自定义域名列表
 
         :param request: Request instance for DescribeInstanceCustomizedDomain.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInstanceCustomizedDomainRequest`
@@ -1539,15 +1539,15 @@
             model = models.DescribeInstanceCustomizedDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceStatus(self, request):
         """查询实例当前状态以及过程信息
 
         :param request: Request instance for DescribeInstanceStatus.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInstanceStatusRequest`
@@ -1562,15 +1562,15 @@
             model = models.DescribeInstanceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceToken(self, request):
         """查询长期访问凭证信息
 
         :param request: Request instance for DescribeInstanceToken.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInstanceTokenRequest`
@@ -1585,15 +1585,15 @@
             model = models.DescribeInstanceTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """查询实例信息
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInstancesRequest`
@@ -1608,15 +1608,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternalEndpointDnsStatus(self, request):
         """批量查询vpc是否已经添加私有域名解析
 
         :param request: Request instance for DescribeInternalEndpointDnsStatus.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInternalEndpointDnsStatusRequest`
@@ -1631,15 +1631,15 @@
             model = models.DescribeInternalEndpointDnsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInternalEndpoints(self, request):
         """查询实例内网访问VPC链接
 
         :param request: Request instance for DescribeInternalEndpoints.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeInternalEndpointsRequest`
@@ -1654,15 +1654,15 @@
             model = models.DescribeInternalEndpointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespacePersonal(self, request):
         """查询个人版命名空间信息
 
         :param request: Request instance for DescribeNamespacePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeNamespacePersonalRequest`
@@ -1677,15 +1677,15 @@
             model = models.DescribeNamespacePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespaces(self, request):
         """查询命名空间列表或指定命名空间信息
 
         :param request: Request instance for DescribeNamespaces.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeNamespacesRequest`
@@ -1700,15 +1700,15 @@
             model = models.DescribeNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """用于在TCR中获取可用区域
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeRegionsRequest`
@@ -1723,15 +1723,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReplicationInstanceCreateTasks(self, request):
         """查询创建从实例任务状态
 
         :param request: Request instance for DescribeReplicationInstanceCreateTasks.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeReplicationInstanceCreateTasksRequest`
@@ -1746,15 +1746,15 @@
             model = models.DescribeReplicationInstanceCreateTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReplicationInstanceSyncStatus(self, request):
         """查询从实例同步状态
 
         :param request: Request instance for DescribeReplicationInstanceSyncStatus.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeReplicationInstanceSyncStatusRequest`
@@ -1769,15 +1769,15 @@
             model = models.DescribeReplicationInstanceSyncStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReplicationInstances(self, request):
         """查询从实例列表
 
         :param request: Request instance for DescribeReplicationInstances.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeReplicationInstancesRequest`
@@ -1792,15 +1792,15 @@
             model = models.DescribeReplicationInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepositories(self, request):
         """查询镜像仓库列表或指定镜像仓库信息
 
         :param request: Request instance for DescribeRepositories.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeRepositoriesRequest`
@@ -1815,15 +1815,15 @@
             model = models.DescribeRepositoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepositoryFilterPersonal(self, request):
         """用于在个人版镜像仓库中，获取满足输入搜索条件的用户镜像仓库
 
         :param request: Request instance for DescribeRepositoryFilterPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeRepositoryFilterPersonalRequest`
@@ -1838,15 +1838,15 @@
             model = models.DescribeRepositoryFilterPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepositoryOwnerPersonal(self, request):
         """用于在个人版中获取用户全部的镜像仓库列表
 
         :param request: Request instance for DescribeRepositoryOwnerPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeRepositoryOwnerPersonalRequest`
@@ -1861,15 +1861,15 @@
             model = models.DescribeRepositoryOwnerPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepositoryPersonal(self, request):
         """查询个人版仓库信息
 
         :param request: Request instance for DescribeRepositoryPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeRepositoryPersonalRequest`
@@ -1884,15 +1884,15 @@
             model = models.DescribeRepositoryPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityPolicies(self, request):
         """查询实例公网访问白名单策略
 
         :param request: Request instance for DescribeSecurityPolicies.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeSecurityPoliciesRequest`
@@ -1907,15 +1907,15 @@
             model = models.DescribeSecurityPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceAccounts(self, request):
         """查询服务级账号
 
         :param request: Request instance for DescribeServiceAccounts.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeServiceAccountsRequest`
@@ -1930,15 +1930,15 @@
             model = models.DescribeServiceAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagRetentionExecution(self, request):
         """查询版本保留执行记录
 
         :param request: Request instance for DescribeTagRetentionExecution.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeTagRetentionExecutionRequest`
@@ -1953,15 +1953,15 @@
             model = models.DescribeTagRetentionExecutionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagRetentionExecutionTask(self, request):
         """查询版本保留执行任务
 
         :param request: Request instance for DescribeTagRetentionExecutionTask.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeTagRetentionExecutionTaskRequest`
@@ -1976,15 +1976,15 @@
             model = models.DescribeTagRetentionExecutionTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTagRetentionRules(self, request):
         """查询版本保留规则
 
         :param request: Request instance for DescribeTagRetentionRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeTagRetentionRulesRequest`
@@ -1999,15 +1999,15 @@
             model = models.DescribeTagRetentionRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserQuotaPersonal(self, request):
         """查询个人用户配额
 
         :param request: Request instance for DescribeUserQuotaPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeUserQuotaPersonalRequest`
@@ -2022,15 +2022,15 @@
             model = models.DescribeUserQuotaPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWebhookTrigger(self, request):
         """查询触发器
 
         :param request: Request instance for DescribeWebhookTrigger.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeWebhookTriggerRequest`
@@ -2045,15 +2045,15 @@
             model = models.DescribeWebhookTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWebhookTriggerLog(self, request):
         """获取触发器日志
 
         :param request: Request instance for DescribeWebhookTriggerLog.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DescribeWebhookTriggerLogRequest`
@@ -2068,15 +2068,15 @@
             model = models.DescribeWebhookTriggerLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadHelmChart(self, request):
         """用于在TCR中下载helm chart
 
         :param request: Request instance for DownloadHelmChart.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DownloadHelmChartRequest`
@@ -2091,15 +2091,15 @@
             model = models.DownloadHelmChartResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DuplicateImagePersonal(self, request):
         """用于在个人版镜像仓库中复制镜像版本
 
         :param request: Request instance for DuplicateImagePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DuplicateImagePersonalRequest`
@@ -2114,15 +2114,15 @@
             model = models.DuplicateImagePersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageExternalEndpoint(self, request):
         """管理实例公网访问
 
         :param request: Request instance for ManageExternalEndpoint.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ManageExternalEndpointRequest`
@@ -2137,15 +2137,15 @@
             model = models.ManageExternalEndpointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageImageLifecycleGlobalPersonal(self, request):
         """用于设置个人版全局镜像版本自动清理策略
 
         :param request: Request instance for ManageImageLifecycleGlobalPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ManageImageLifecycleGlobalPersonalRequest`
@@ -2160,15 +2160,15 @@
             model = models.ManageImageLifecycleGlobalPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageInternalEndpoint(self, request):
         """管理实例内网访问VPC链接
 
         :param request: Request instance for ManageInternalEndpoint.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ManageInternalEndpointRequest`
@@ -2183,15 +2183,15 @@
             model = models.ManageInternalEndpointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageReplication(self, request):
         """管理实例同步
 
         :param request: Request instance for ManageReplication.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ManageReplicationRequest`
@@ -2206,15 +2206,15 @@
             model = models.ManageReplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationTriggerPersonal(self, request):
         """用于修改应用更新触发器
 
         :param request: Request instance for ModifyApplicationTriggerPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyApplicationTriggerPersonalRequest`
@@ -2229,15 +2229,15 @@
             model = models.ModifyApplicationTriggerPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomAccount(self, request):
         """更新自定义账户
 
         :param request: Request instance for ModifyCustomAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyCustomAccountRequest`
@@ -2252,15 +2252,15 @@
             model = models.ModifyCustomAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImmutableTagRules(self, request):
         """更新镜像不可变规则
 
         :param request: Request instance for ModifyImmutableTagRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyImmutableTagRulesRequest`
@@ -2275,15 +2275,15 @@
             model = models.ModifyImmutableTagRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstance(self, request):
         """更新实例信息
 
         :param request: Request instance for ModifyInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyInstanceRequest`
@@ -2298,15 +2298,15 @@
             model = models.ModifyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceToken(self, request):
         """更新实例内指定长期访问凭证的启用状态
 
         :param request: Request instance for ModifyInstanceToken.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyInstanceTokenRequest`
@@ -2321,15 +2321,15 @@
             model = models.ModifyInstanceTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNamespace(self, request):
         """更新命名空间信息
 
         :param request: Request instance for ModifyNamespace.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyNamespaceRequest`
@@ -2344,15 +2344,15 @@
             model = models.ModifyNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRepository(self, request):
         """更新镜像仓库信息，可修改仓库描述信息
 
         :param request: Request instance for ModifyRepository.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyRepositoryRequest`
@@ -2367,15 +2367,15 @@
             model = models.ModifyRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRepositoryAccessPersonal(self, request):
         """用于更新个人版镜像仓库的访问属性
 
         :param request: Request instance for ModifyRepositoryAccessPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyRepositoryAccessPersonalRequest`
@@ -2390,15 +2390,15 @@
             model = models.ModifyRepositoryAccessPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRepositoryInfoPersonal(self, request):
         """用于在个人版镜像仓库中更新容器镜像描述
 
         :param request: Request instance for ModifyRepositoryInfoPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyRepositoryInfoPersonalRequest`
@@ -2413,15 +2413,15 @@
             model = models.ModifyRepositoryInfoPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityPolicy(self, request):
         """更新实例公网访问白名单
 
         :param request: Request instance for ModifySecurityPolicy.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifySecurityPolicyRequest`
@@ -2436,15 +2436,15 @@
             model = models.ModifySecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceAccount(self, request):
         """更新服务级账号
 
         :param request: Request instance for ModifyServiceAccount.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyServiceAccountRequest`
@@ -2459,15 +2459,15 @@
             model = models.ModifyServiceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTagRetentionRule(self, request):
         """更新版本保留规则
 
         :param request: Request instance for ModifyTagRetentionRule.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyTagRetentionRuleRequest`
@@ -2482,15 +2482,15 @@
             model = models.ModifyTagRetentionRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUserPasswordPersonal(self, request):
         """修改个人用户登录密码
 
         :param request: Request instance for ModifyUserPasswordPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyUserPasswordPersonalRequest`
@@ -2505,15 +2505,15 @@
             model = models.ModifyUserPasswordPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWebhookTrigger(self, request):
         """更新触发器
 
         :param request: Request instance for ModifyWebhookTrigger.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ModifyWebhookTriggerRequest`
@@ -2528,15 +2528,15 @@
             model = models.ModifyWebhookTriggerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstance(self, request):
         """预付费实例续费，同时支持按量计费转包年包月
 
         :param request: Request instance for RenewInstance.
         :type request: :class:`tencentcloud.tcr.v20190924.models.RenewInstanceRequest`
@@ -2551,15 +2551,15 @@
             model = models.RenewInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ValidateNamespaceExistPersonal(self, request):
         """查询个人版用户命名空间是否存在
 
         :param request: Request instance for ValidateNamespaceExistPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ValidateNamespaceExistPersonalRequest`
@@ -2574,15 +2574,15 @@
             model = models.ValidateNamespaceExistPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ValidateRepositoryExistPersonal(self, request):
         """用于判断个人版仓库是否存在
 
         :param request: Request instance for ValidateRepositoryExistPersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.ValidateRepositoryExistPersonalRequest`
@@ -2597,8 +2597,8 @@
             model = models.ValidateRepositoryExistPersonalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-tcr-3.0.938/tencentcloud/tcr/v20190924/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.938/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.938/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.937/README.rst` & `tencentcloud-sdk-python-tcr-3.0.938/README.rst`

 * *Files identical despite different names*

