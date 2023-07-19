# Comparing `tmp/tencentcloud-sdk-python-dayu-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dayu-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dayu-3.0.937.tar", last modified: Tue Jul 18 00:22:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dayu-3.0.938.tar", last modified: Wed Jul 19 00:37:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dayu-3.0.937.tar` & `tencentcloud-sdk-python-dayu-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   102618 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/dayu_client.py
--rw-r--r--   0 root         (0) root         (0)   545180 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:22:04.000000 tencentcloud-sdk-python-dayu-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   103066 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/dayu_client.py
+-rw-r--r--   0 root         (0) root         (0)   545180 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:37:18.000000 tencentcloud-sdk-python-dayu-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/setup.py` & `tencentcloud-sdk-python-dayu-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/errorcodes.py` & `tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/dayu_client.py` & `tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/dayu_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateBasicDDoSAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBoundIP(self, request):
         """绑定IP到高防包实例，支持独享包、共享包；需要注意的是此接口绑定或解绑IP是异步接口，当处于绑定或解绑中时，则不允许再进行绑定或解绑，需要等待当前绑定或解绑完成。
 
         :param request: Request instance for CreateBoundIP.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateBoundIPRequest`
@@ -65,15 +65,15 @@
             model = models.CreateBoundIPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCCFrequencyRules(self, request):
         """添加CC防护的访问频率控制规则
 
         :param request: Request instance for CreateCCFrequencyRules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateCCFrequencyRulesRequest`
@@ -88,15 +88,15 @@
             model = models.CreateCCFrequencyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCCSelfDefinePolicy(self, request):
         """创建CC自定义策略
 
         :param request: Request instance for CreateCCSelfDefinePolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateCCSelfDefinePolicyRequest`
@@ -111,15 +111,15 @@
             model = models.CreateCCSelfDefinePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSPolicy(self, request):
         """添加DDoS高级策略
 
         :param request: Request instance for CreateDDoSPolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateDDoSPolicyRequest`
@@ -134,15 +134,15 @@
             model = models.CreateDDoSPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSPolicyCase(self, request):
         """添加策略场景
 
         :param request: Request instance for CreateDDoSPolicyCase.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateDDoSPolicyCaseRequest`
@@ -157,15 +157,15 @@
             model = models.CreateDDoSPolicyCaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstanceName(self, request):
         """资源实例重命名，支持独享包、共享包、高防IP、高防IP专业版；
 
         :param request: Request instance for CreateInstanceName.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateInstanceNameRequest`
@@ -180,15 +180,15 @@
             model = models.CreateInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL4HealthConfig(self, request):
         """上传四层健康检查配置
 
         :param request: Request instance for CreateL4HealthConfig.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL4HealthConfigRequest`
@@ -203,15 +203,15 @@
             model = models.CreateL4HealthConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL4Rules(self, request):
         """添加L4转发规则
 
         :param request: Request instance for CreateL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL4RulesRequest`
@@ -226,15 +226,15 @@
             model = models.CreateL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7CCRule(self, request):
         """此接口是7层CC的访问频控自定义规则（IP+Host维度，不支持具体的URI），此接口已弃用，请调用新接口CreateCCFrequencyRules，新接口同时支持IP+Host维度以及具体的URI；
 
         :param request: Request instance for CreateL7CCRule.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL7CCRuleRequest`
@@ -249,15 +249,15 @@
             model = models.CreateL7CCRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7HealthConfig(self, request):
         """上传七层健康检查配置
 
         :param request: Request instance for CreateL7HealthConfig.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL7HealthConfigRequest`
@@ -272,15 +272,15 @@
             model = models.CreateL7HealthConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7RuleCert(self, request):
         """配置7层转发规则的证书
 
         :param request: Request instance for CreateL7RuleCert.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL7RuleCertRequest`
@@ -295,15 +295,15 @@
             model = models.CreateL7RuleCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7Rules(self, request):
         """添加7层(网站)转发规则
 
         :param request: Request instance for CreateL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL7RulesRequest`
@@ -318,15 +318,15 @@
             model = models.CreateL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7RulesUpload(self, request):
         """批量上传7层转发规则
 
         :param request: Request instance for CreateL7RulesUpload.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateL7RulesUploadRequest`
@@ -341,15 +341,15 @@
             model = models.CreateL7RulesUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetReturn(self, request):
         """高防IP专业版一键切回源站
 
         :param request: Request instance for CreateNetReturn.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateNetReturnRequest`
@@ -364,15 +364,15 @@
             model = models.CreateNetReturnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNewL4Rules(self, request):
         """添加L4转发规则
 
         :param request: Request instance for CreateNewL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateNewL4RulesRequest`
@@ -387,15 +387,15 @@
             model = models.CreateNewL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNewL7Rules(self, request):
         """添加7层转发规则
 
         :param request: Request instance for CreateNewL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateNewL7RulesRequest`
@@ -410,15 +410,15 @@
             model = models.CreateNewL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNewL7RulesUpload(self, request):
         """批量上传7层转发规则
 
         :param request: Request instance for CreateNewL7RulesUpload.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateNewL7RulesUploadRequest`
@@ -433,15 +433,15 @@
             model = models.CreateNewL7RulesUploadResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUnblockIp(self, request):
         """IP解封操作
 
         :param request: Request instance for CreateUnblockIp.
         :type request: :class:`tencentcloud.dayu.v20180709.models.CreateUnblockIpRequest`
@@ -456,15 +456,15 @@
             model = models.CreateUnblockIpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCFrequencyRules(self, request):
         """删除CC防护的访问频率控制规则
 
         :param request: Request instance for DeleteCCFrequencyRules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteCCFrequencyRulesRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteCCFrequencyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCSelfDefinePolicy(self, request):
         """删除CC自定义策略
 
         :param request: Request instance for DeleteCCSelfDefinePolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteCCSelfDefinePolicyRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteCCSelfDefinePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDDoSPolicy(self, request):
         """删除DDoS高级策略
 
         :param request: Request instance for DeleteDDoSPolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteDDoSPolicyRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteDDoSPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDDoSPolicyCase(self, request):
         """删除策略场景
 
         :param request: Request instance for DeleteDDoSPolicyCase.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteDDoSPolicyCaseRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteDDoSPolicyCaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteL4Rules(self, request):
         """删除四层转发规则
 
         :param request: Request instance for DeleteL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteL4RulesRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteL7Rules(self, request):
         """删除七层转发规则
 
         :param request: Request instance for DeleteL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteL7RulesRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNewL4Rules(self, request):
         """删除L4转发规则
 
         :param request: Request instance for DeleteNewL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteNewL4RulesRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteNewL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNewL7Rules(self, request):
         """删除L7转发规则
 
         :param request: Request instance for DeleteNewL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DeleteNewL7RulesRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteNewL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeActionLog(self, request):
         """获取操作日志
 
         :param request: Request instance for DescribeActionLog.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeActionLogRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeActionLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBGPIPL7RuleMaxCnt(self, request):
         """获取高防IP可添加的最多7层规则数量
 
         :param request: Request instance for DescribeBGPIPL7RuleMaxCnt.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBGPIPL7RuleMaxCntRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeBGPIPL7RuleMaxCntResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBaradData(self, request):
         """为大禹子产品提供业务转发指标数据的接口
 
         :param request: Request instance for DescribeBaradData.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBaradDataRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeBaradDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicCCThreshold(self, request):
         """获取基础防护CC防护阈值
 
         :param request: Request instance for DescribeBasicCCThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBasicCCThresholdRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeBasicCCThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicDeviceThreshold(self, request):
         """获取基础防护黑洞阈值
 
         :param request: Request instance for DescribeBasicDeviceThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBasicDeviceThresholdRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeBasicDeviceThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBizHttpStatus(self, request):
         """获取业务流量状态码统计
 
         :param request: Request instance for DescribeBizHttpStatus.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBizHttpStatusRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeBizHttpStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBizTrend(self, request):
         """获取业务流量曲线
 
         :param request: Request instance for DescribeBizTrend.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeBizTrendRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeBizTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCAlarmThreshold(self, request):
         """获取高防包、高防IP、高防IP专业版、棋牌盾产品设置CC攻击的告警通知阈值
 
         :param request: Request instance for DescribeCCAlarmThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCAlarmThresholdRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeCCAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCEvList(self, request):
         """获取CC攻击事件列表
 
         :param request: Request instance for DescribeCCEvList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCEvListRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeCCEvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCFrequencyRules(self, request):
         """获取CC防护的访问频率控制规则
 
         :param request: Request instance for DescribeCCFrequencyRules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCFrequencyRulesRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeCCFrequencyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCIpAllowDeny(self, request):
         """获取CC的IP黑白名单
 
         :param request: Request instance for DescribeCCIpAllowDeny.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCIpAllowDenyRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeCCIpAllowDenyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCSelfDefinePolicy(self, request):
         """获取CC自定义策略
 
         :param request: Request instance for DescribeCCSelfDefinePolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCSelfDefinePolicyRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeCCSelfDefinePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCTrend(self, request):
         """获取CC攻击指标数据，包括总请求峰值(QPS)和攻击请求(QPS)
 
         :param request: Request instance for DescribeCCTrend.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCTrendRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeCCTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCUrlAllow(self, request):
         """获取CC的Url白名单
 
         :param request: Request instance for DescribeCCUrlAllow.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeCCUrlAllowRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeCCUrlAllowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAlarmThreshold(self, request):
         """获取高防包、高防IP、高防IP专业版、棋牌盾产品设置DDoS攻击的告警通知阈值
 
         :param request: Request instance for DescribeDDoSAlarmThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSAlarmThresholdRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDDoSAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAttackIPRegionMap(self, request):
         """获取DDoS攻击源IP地域分布图，支持全球攻击分布和国内省份攻击分布；
 
         :param request: Request instance for DescribeDDoSAttackIPRegionMap.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSAttackIPRegionMapRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDDoSAttackIPRegionMapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAttackSource(self, request):
         """获取DDoS攻击源列表
 
         :param request: Request instance for DescribeDDoSAttackSource.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSAttackSourceRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeDDoSAttackSourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSCount(self, request):
         """获取DDoS攻击占比分析
 
         :param request: Request instance for DescribeDDoSCount.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSCountRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeDDoSCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSDefendStatus(self, request):
         """获取DDoS防护状态（临时关闭状态），支持产品：基础防护，独享包，共享包，高防IP，高防IP专业版；调用此接口是获取当前是否有设置临时关闭DDoS防护状态，如果有设置会返回临时关闭的时长等参数。
 
         :param request: Request instance for DescribeDDoSDefendStatus.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSDefendStatusRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeDDoSDefendStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSEvInfo(self, request):
         """获取DDoS攻击事件详情
 
         :param request: Request instance for DescribeDDoSEvInfo.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSEvInfoRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeDDoSEvInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSEvList(self, request):
         """获取DDoS攻击事件列表
 
         :param request: Request instance for DescribeDDoSEvList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSEvListRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeDDoSEvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSIpLog(self, request):
         """获取DDoSIP攻击日志
 
         :param request: Request instance for DescribeDDoSIpLog.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSIpLogRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeDDoSIpLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSNetCount(self, request):
         """获取高防IP专业版资源的DDoS攻击占比分析
 
         :param request: Request instance for DescribeDDoSNetCount.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSNetCountRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeDDoSNetCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSNetEvInfo(self, request):
         """获取高防IP专业版资源的DDoS攻击事件详情
 
         :param request: Request instance for DescribeDDoSNetEvInfo.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSNetEvInfoRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeDDoSNetEvInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSNetEvList(self, request):
         """获取高防IP专业版资源的DDoS攻击事件列表
 
         :param request: Request instance for DescribeDDoSNetEvList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSNetEvListRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeDDoSNetEvListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSNetIpLog(self, request):
         """获取高防IP专业版资源的DDoSIP攻击日志
 
         :param request: Request instance for DescribeDDoSNetIpLog.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSNetIpLogRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeDDoSNetIpLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSNetTrend(self, request):
         """获取高防IP专业版资源的DDoS攻击指标数据
 
         :param request: Request instance for DescribeDDoSNetTrend.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSNetTrendRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeDDoSNetTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSPolicy(self, request):
         """获取DDoS高级策略
 
         :param request: Request instance for DescribeDDoSPolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSPolicyRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeDDoSPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSTrend(self, request):
         """获取DDoS攻击流量带宽和攻击包速率数据
 
         :param request: Request instance for DescribeDDoSTrend.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSTrendRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeDDoSTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSUsedStatis(self, request):
         """统计用户的高防资源的使用天数和DDoS攻击防护次数
 
         :param request: Request instance for DescribeDDoSUsedStatis.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeDDoSUsedStatisRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeDDoSUsedStatisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIPProductInfo(self, request):
         """获取独享包或共享包IP对应的云资产信息，只支持独享包和共享包的IP
 
         :param request: Request instance for DescribeIPProductInfo.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeIPProductInfoRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeIPProductInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInsurePacks(self, request):
         """获取保险包套餐列表
 
         :param request: Request instance for DescribeInsurePacks.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeInsurePacksRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeInsurePacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpBlockList(self, request):
         """获取IP封堵列表
 
         :param request: Request instance for DescribeIpBlockList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeIpBlockListRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeIpBlockListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpUnBlockList(self, request):
         """获取IP解封记录
 
         :param request: Request instance for DescribeIpUnBlockList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeIpUnBlockListRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeIpUnBlockListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL4HealthConfig(self, request):
         """导出四层健康检查配置
 
         :param request: Request instance for DescribeL4HealthConfig.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeL4HealthConfigRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeL4HealthConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL4RulesErrHealth(self, request):
         """获取L4转发规则健康检查异常结果
 
         :param request: Request instance for DescribeL4RulesErrHealth.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeL4RulesErrHealthRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeL4RulesErrHealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7HealthConfig(self, request):
         """导出七层健康检查配置
 
         :param request: Request instance for DescribeL7HealthConfig.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeL7HealthConfigRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeL7HealthConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewL4Rules(self, request):
         """获取L4转发规则
 
         :param request: Request instance for DescribeNewL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeNewL4RulesRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeNewL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewL4RulesErrHealth(self, request):
         """获取L4转发规则健康检查异常结果
 
         :param request: Request instance for DescribeNewL4RulesErrHealth.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeNewL4RulesErrHealthRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeNewL4RulesErrHealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewL7RulesErrHealth(self, request):
         """获取L7转发规则健康检查异常结果
 
         :param request: Request instance for DescribeNewL7RulesErrHealth.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeNewL7RulesErrHealthRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeNewL7RulesErrHealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackIndex(self, request):
         """获取产品总览统计，支持高防包、高防IP、高防IP专业版；
 
         :param request: Request instance for DescribePackIndex.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribePackIndexRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribePackIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePcap(self, request):
         """下载攻击事件的pcap包
 
         :param request: Request instance for DescribePcap.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribePcapRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribePcapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicyCase(self, request):
         """获取策略场景
 
         :param request: Request instance for DescribePolicyCase.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribePolicyCaseRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribePolicyCaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResIpList(self, request):
         """获取资源的IP列表
 
         :param request: Request instance for DescribeResIpList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeResIpListRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeResIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceList(self, request):
         """获取资源列表
 
         :param request: Request instance for DescribeResourceList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeResourceListRequest`
@@ -1675,15 +1675,15 @@
             model = models.DescribeResourceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleSets(self, request):
         """获取资源的规则数
 
         :param request: Request instance for DescribeRuleSets.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeRuleSetsRequest`
@@ -1698,15 +1698,15 @@
             model = models.DescribeRuleSetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSchedulingDomainList(self, request):
         """获取调度域名列表
 
         :param request: Request instance for DescribeSchedulingDomainList.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeSchedulingDomainListRequest`
@@ -1721,15 +1721,15 @@
             model = models.DescribeSchedulingDomainListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecIndex(self, request):
         """获取本月安全统计
 
         :param request: Request instance for DescribeSecIndex.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeSecIndexRequest`
@@ -1744,15 +1744,15 @@
             model = models.DescribeSecIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSourceIpSegment(self, request):
         """获取回源IP段，支持的产品：高防IP，高防IP专业版；
 
         :param request: Request instance for DescribeSourceIpSegment.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeSourceIpSegmentRequest`
@@ -1767,15 +1767,15 @@
             model = models.DescribeSourceIpSegmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTransmitStatis(self, request):
         """获取业务转发统计数据，支持转发流量和转发包速率
 
         :param request: Request instance for DescribeTransmitStatis.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeTransmitStatisRequest`
@@ -1790,15 +1790,15 @@
             model = models.DescribeTransmitStatisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnBlockStatis(self, request):
         """获取黑洞解封次数
 
         :param request: Request instance for DescribeUnBlockStatis.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribeUnBlockStatisRequest`
@@ -1813,15 +1813,15 @@
             model = models.DescribeUnBlockStatisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribleL4Rules(self, request):
         """获取四层转发规则
 
         :param request: Request instance for DescribleL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribleL4RulesRequest`
@@ -1836,15 +1836,15 @@
             model = models.DescribleL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribleL7Rules(self, request):
         """获取七层转发规则
 
         :param request: Request instance for DescribleL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribleL7RulesRequest`
@@ -1859,15 +1859,15 @@
             model = models.DescribleL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribleNewL7Rules(self, request):
         """获取7层规则
 
         :param request: Request instance for DescribleNewL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribleNewL7RulesRequest`
@@ -1882,15 +1882,15 @@
             model = models.DescribleNewL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribleRegionCount(self, request):
         """获取地域的资源实例数
 
         :param request: Request instance for DescribleRegionCount.
         :type request: :class:`tencentcloud.dayu.v20180709.models.DescribleRegionCountRequest`
@@ -1905,15 +1905,15 @@
             model = models.DescribleRegionCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCAlarmThreshold(self, request):
         """为高防包、高防IP、高防IP专业版、棋牌盾产品设置CC攻击的告警通知阈值
 
         :param request: Request instance for ModifyCCAlarmThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCAlarmThresholdRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyCCAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCFrequencyRules(self, request):
         """修改CC防护的访问频率控制规则
 
         :param request: Request instance for ModifyCCFrequencyRules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCFrequencyRulesRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyCCFrequencyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCFrequencyRulesStatus(self, request):
         """开启或关闭CC防护的访问频率控制规则
 
         :param request: Request instance for ModifyCCFrequencyRulesStatus.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCFrequencyRulesStatusRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyCCFrequencyRulesStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCHostProtection(self, request):
         """开启或关闭CC域名防护
 
         :param request: Request instance for ModifyCCHostProtection.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCHostProtectionRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyCCHostProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCIpAllowDeny(self, request):
         """添加或删除CC的IP黑白名单
 
         :param request: Request instance for ModifyCCIpAllowDeny.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCIpAllowDenyRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyCCIpAllowDenyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCLevel(self, request):
         """修改CC防护等级
 
         :param request: Request instance for ModifyCCLevel.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCLevelRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyCCLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCPolicySwitch(self, request):
         """修改CC自定义策略开关
 
         :param request: Request instance for ModifyCCPolicySwitch.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCPolicySwitchRequest`
@@ -2066,15 +2066,15 @@
             model = models.ModifyCCPolicySwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCSelfDefinePolicy(self, request):
         """修改CC自定义策略
 
         :param request: Request instance for ModifyCCSelfDefinePolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCSelfDefinePolicyRequest`
@@ -2089,15 +2089,15 @@
             model = models.ModifyCCSelfDefinePolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCThreshold(self, request):
         """修改CC的防护阈值
 
         :param request: Request instance for ModifyCCThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCThresholdRequest`
@@ -2112,15 +2112,15 @@
             model = models.ModifyCCThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCUrlAllow(self, request):
         """添加或删除CC的URL白名单
 
         :param request: Request instance for ModifyCCUrlAllow.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyCCUrlAllowRequest`
@@ -2135,15 +2135,15 @@
             model = models.ModifyCCUrlAllowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSAIStatus(self, request):
         """读取或修改DDoS的AI防护状态
 
         :param request: Request instance for ModifyDDoSAIStatus.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSAIStatusRequest`
@@ -2158,15 +2158,15 @@
             model = models.ModifyDDoSAIStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSAlarmThreshold(self, request):
         """为高防包、高防IP、高防IP专业版、棋牌盾等产品设置DDoS攻击的告警通知阈值
 
         :param request: Request instance for ModifyDDoSAlarmThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSAlarmThresholdRequest`
@@ -2181,15 +2181,15 @@
             model = models.ModifyDDoSAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSDefendStatus(self, request):
         """开启或关闭DDoS防护状态，调用此接口允许临时关闭DDoS防护一段时间，等时间到了会自动开启DDoS防护；
 
         :param request: Request instance for ModifyDDoSDefendStatus.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSDefendStatusRequest`
@@ -2204,15 +2204,15 @@
             model = models.ModifyDDoSDefendStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSLevel(self, request):
         """读取或修改DDoS的防护等级
 
         :param request: Request instance for ModifyDDoSLevel.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSLevelRequest`
@@ -2227,15 +2227,15 @@
             model = models.ModifyDDoSLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSPolicy(self, request):
         """修改DDoS高级策略
 
         :param request: Request instance for ModifyDDoSPolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSPolicyRequest`
@@ -2250,15 +2250,15 @@
             model = models.ModifyDDoSPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSPolicyCase(self, request):
         """修改策略场景
 
         :param request: Request instance for ModifyDDoSPolicyCase.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSPolicyCaseRequest`
@@ -2273,15 +2273,15 @@
             model = models.ModifyDDoSPolicyCaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSPolicyName(self, request):
         """修改DDoS高级策略名称
 
         :param request: Request instance for ModifyDDoSPolicyName.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSPolicyNameRequest`
@@ -2296,15 +2296,15 @@
             model = models.ModifyDDoSPolicyNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSSwitch(self, request):
         """开启或关闭DDoS防护，只支持基础防护产品；
 
         :param request: Request instance for ModifyDDoSSwitch.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSSwitchRequest`
@@ -2319,15 +2319,15 @@
             model = models.ModifyDDoSSwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSThreshold(self, request):
         """修改DDoS清洗阈值
 
         :param request: Request instance for ModifyDDoSThreshold.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSThresholdRequest`
@@ -2342,15 +2342,15 @@
             model = models.ModifyDDoSThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSWaterKey(self, request):
         """支持水印密钥的添加，删除，开启，关闭
 
         :param request: Request instance for ModifyDDoSWaterKey.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyDDoSWaterKeyRequest`
@@ -2365,15 +2365,15 @@
             model = models.ModifyDDoSWaterKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyElasticLimit(self, request):
         """修改弹性防护阈值
 
         :param request: Request instance for ModifyElasticLimit.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyElasticLimitRequest`
@@ -2388,15 +2388,15 @@
             model = models.ModifyElasticLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4Health(self, request):
         """修改L4转发规则健康检查参数，支持的子产品：高防IP、高防IP专业版
 
         :param request: Request instance for ModifyL4Health.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyL4HealthRequest`
@@ -2411,15 +2411,15 @@
             model = models.ModifyL4HealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4KeepTime(self, request):
         """修改L4转发规则的会话保持，支持的子产品：高防IP、高防IP专业版
 
         :param request: Request instance for ModifyL4KeepTime.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyL4KeepTimeRequest`
@@ -2434,15 +2434,15 @@
             model = models.ModifyL4KeepTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4Rules(self, request):
         """修改L4转发规则
 
         :param request: Request instance for ModifyL4Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyL4RulesRequest`
@@ -2457,15 +2457,15 @@
             model = models.ModifyL4RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL7Rules(self, request):
         """修改L7转发规则
 
         :param request: Request instance for ModifyL7Rules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyL7RulesRequest`
@@ -2480,15 +2480,15 @@
             model = models.ModifyL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetReturnSwitch(self, request):
         """在客户收攻击或者被封堵时，切回到源站，并设置回切的时长
 
         :param request: Request instance for ModifyNetReturnSwitch.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyNetReturnSwitchRequest`
@@ -2503,15 +2503,15 @@
             model = models.ModifyNetReturnSwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNewDomainRules(self, request):
         """修改7层转发规则
 
         :param request: Request instance for ModifyNewDomainRules.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyNewDomainRulesRequest`
@@ -2526,15 +2526,15 @@
             model = models.ModifyNewDomainRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNewL4Rule(self, request):
         """修改4层转发规则
 
         :param request: Request instance for ModifyNewL4Rule.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyNewL4RuleRequest`
@@ -2549,15 +2549,15 @@
             model = models.ModifyNewL4RuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResBindDDoSPolicy(self, request):
         """资源实例绑定DDoS高级策略
 
         :param request: Request instance for ModifyResBindDDoSPolicy.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyResBindDDoSPolicyRequest`
@@ -2572,15 +2572,15 @@
             model = models.ModifyResBindDDoSPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourceRenewFlag(self, request):
         """修改资源自动续费标记
 
         :param request: Request instance for ModifyResourceRenewFlag.
         :type request: :class:`tencentcloud.dayu.v20180709.models.ModifyResourceRenewFlagRequest`
@@ -2595,8 +2595,8 @@
             model = models.ModifyResourceRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/tencentcloud/dayu/v20180709/models.py` & `tencentcloud-sdk-python-dayu-3.0.938/tencentcloud/dayu/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dayu-3.0.938/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dayu
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dayu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dayu-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dayu
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dayu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.937/README.rst` & `tencentcloud-sdk-python-dayu-3.0.938/README.rst`

 * *Files identical despite different names*

