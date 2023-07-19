# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.937.tar", last modified: Tue Jul 18 00:34:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.938.tar", last modified: Wed Jul 19 00:52:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.937.tar` & `tencentcloud-sdk-python-tsf-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)   196318 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50111 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1288536 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:23.000000 tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)   197194 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50111 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1288536 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:52:58.000000 tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/setup.py` & `tencentcloud-sdk-python-tsf-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddInstances(self, request):
         """添加云主机节点至TSF集群
 
         :param request: Request instance for AddInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.AddInstancesRequest`
@@ -65,15 +65,15 @@
             model = models.AddInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateBusinessLogConfig(self, request):
         """关联日志配置项到应用
 
         :param request: Request instance for AssociateBusinessLogConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.AssociateBusinessLogConfigRequest`
@@ -88,15 +88,15 @@
             model = models.AssociateBusinessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateConfigWithGroup(self, request):
         """关联投递配置到部署组
 
         :param request: Request instance for AssociateConfigWithGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.AssociateConfigWithGroupRequest`
@@ -111,15 +111,15 @@
             model = models.AssociateConfigWithGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindApiGroup(self, request):
         """网关与API分组批量绑定
 
         :param request: Request instance for BindApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.BindApiGroupRequest`
@@ -134,15 +134,15 @@
             model = models.BindApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindPlugin(self, request):
         """插件与网关分组/API批量绑定
 
         :param request: Request instance for BindPlugin.
         :type request: :class:`tencentcloud.tsf.v20180326.models.BindPluginRequest`
@@ -157,15 +157,15 @@
             model = models.BindPluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeApiUsableStatus(self, request):
         """启用或禁用API
 
         :param request: Request instance for ChangeApiUsableStatus.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ChangeApiUsableStatusRequest`
@@ -180,15 +180,15 @@
             model = models.ChangeApiUsableStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ContinueRunFailedTaskBatch(self, request):
         """对执行失败的任务批次执行续跑
 
         :param request: Request instance for ContinueRunFailedTaskBatch.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ContinueRunFailedTaskBatchRequest`
@@ -203,15 +203,15 @@
             model = models.ContinueRunFailedTaskBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAllGatewayApiAsync(self, request):
         """一键导入API分组
 
         :param request: Request instance for CreateAllGatewayApiAsync.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateAllGatewayApiAsyncRequest`
@@ -226,15 +226,15 @@
             model = models.CreateAllGatewayApiAsyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApiGroup(self, request):
         """创建API分组
 
         :param request: Request instance for CreateApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateApiGroupRequest`
@@ -249,15 +249,15 @@
             model = models.CreateApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApiRateLimitRule(self, request):
         """创建API限流规则
 
         :param request: Request instance for CreateApiRateLimitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateApiRateLimitRuleRequest`
@@ -272,15 +272,15 @@
             model = models.CreateApiRateLimitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApiRateLimitRuleWithDetailResp(self, request):
         """创建API限流规则,并返回规则信息
 
         :param request: Request instance for CreateApiRateLimitRuleWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateApiRateLimitRuleWithDetailRespRequest`
@@ -295,15 +295,15 @@
             model = models.CreateApiRateLimitRuleWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplication(self, request):
         """创建应用
 
         :param request: Request instance for CreateApplication.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateApplicationRequest`
@@ -318,15 +318,15 @@
             model = models.CreateApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """创建集群
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateClusterRequest`
@@ -341,15 +341,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfig(self, request):
         """创建配置项
 
         :param request: Request instance for CreateConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateConfigRequest`
@@ -364,15 +364,15 @@
             model = models.CreateConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigTemplate(self, request):
         """创建参数模板
 
         :param request: Request instance for CreateConfigTemplate.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateConfigTemplateRequest`
@@ -387,15 +387,15 @@
             model = models.CreateConfigTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigTemplateWithDetailResp(self, request):
         """创建参数模板,并返回模版详细信息
 
         :param request: Request instance for CreateConfigTemplateWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateConfigTemplateWithDetailRespRequest`
@@ -410,15 +410,15 @@
             model = models.CreateConfigTemplateWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigWithDetailResp(self, request):
         """创建配置项，返回详细信息
 
         :param request: Request instance for CreateConfigWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateConfigWithDetailRespRequest`
@@ -433,15 +433,15 @@
             model = models.CreateConfigWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateContainGroup(self, request):
         """（已废弃，请使用 CreateGroup 和 DeployContainerGroup 创建和部署容器部署组）创建容器部署组
 
         :param request: Request instance for CreateContainGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateContainGroupRequest`
@@ -456,15 +456,15 @@
             model = models.CreateContainGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFileConfig(self, request):
         """创建文件配置项
 
         :param request: Request instance for CreateFileConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateFileConfigRequest`
@@ -479,15 +479,15 @@
             model = models.CreateFileConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFileConfigWithDetailResp(self, request):
         """创建文件配置项，返回详细信息
 
         :param request: Request instance for CreateFileConfigWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateFileConfigWithDetailRespRequest`
@@ -502,15 +502,15 @@
             model = models.CreateFileConfigWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGatewayApi(self, request):
         """批量导入API至api分组(也支持新建API到分组)
 
         :param request: Request instance for CreateGatewayApi.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateGatewayApiRequest`
@@ -525,15 +525,15 @@
             model = models.CreateGatewayApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGroup(self, request):
         """创建虚拟机部署组
 
         :param request: Request instance for CreateGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateGroupRequest`
@@ -548,15 +548,15 @@
             model = models.CreateGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLane(self, request):
         """创建泳道
 
         :param request: Request instance for CreateLane.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateLaneRequest`
@@ -571,15 +571,15 @@
             model = models.CreateLaneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLaneRule(self, request):
         """创建泳道规则
 
         :param request: Request instance for CreateLaneRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateLaneRuleRequest`
@@ -594,15 +594,15 @@
             model = models.CreateLaneRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMicroservice(self, request):
         """新增微服务
 
         :param request: Request instance for CreateMicroservice.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateMicroserviceRequest`
@@ -617,15 +617,15 @@
             model = models.CreateMicroserviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMicroserviceWithDetailResp(self, request):
         """新增微服务返回id
 
         :param request: Request instance for CreateMicroserviceWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateMicroserviceWithDetailRespRequest`
@@ -640,15 +640,15 @@
             model = models.CreateMicroserviceWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespace(self, request):
         """创建命名空间
 
         :param request: Request instance for CreateNamespace.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateNamespaceRequest`
@@ -663,15 +663,15 @@
             model = models.CreateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePathRewrites(self, request):
         """创建路径重写
 
         :param request: Request instance for CreatePathRewrites.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreatePathRewritesRequest`
@@ -686,15 +686,15 @@
             model = models.CreatePathRewritesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePathRewritesWithDetailResp(self, request):
         """创建路径重写，并返回路径重写规则信息
 
         :param request: Request instance for CreatePathRewritesWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreatePathRewritesWithDetailRespRequest`
@@ -709,15 +709,15 @@
             model = models.CreatePathRewritesWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePublicConfig(self, request):
         """创建公共配置项
 
         :param request: Request instance for CreatePublicConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreatePublicConfigRequest`
@@ -732,15 +732,15 @@
             model = models.CreatePublicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePublicConfigWithDetailResp(self, request):
         """创建公共配置项，并返回配置项详细信息
 
         :param request: Request instance for CreatePublicConfigWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreatePublicConfigWithDetailRespRequest`
@@ -755,15 +755,15 @@
             model = models.CreatePublicConfigWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRepository(self, request):
         """创建仓库
 
         :param request: Request instance for CreateRepository.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateRepositoryRequest`
@@ -778,15 +778,15 @@
             model = models.CreateRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTask(self, request):
         """创建任务
 
         :param request: Request instance for CreateTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateTaskRequest`
@@ -801,15 +801,15 @@
             model = models.CreateTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTaskFlow(self, request):
         """创建工作流
 
         :param request: Request instance for CreateTaskFlow.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateTaskFlowRequest`
@@ -824,15 +824,15 @@
             model = models.CreateTaskFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUnitNamespaces(self, request):
         """批量创建单元化命名空间
 
         :param request: Request instance for CreateUnitNamespaces.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateUnitNamespacesRequest`
@@ -847,15 +847,15 @@
             model = models.CreateUnitNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUnitRule(self, request):
         """创建单元化规则
 
         :param request: Request instance for CreateUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateUnitRuleRequest`
@@ -870,15 +870,15 @@
             model = models.CreateUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUnitRuleWithDetailResp(self, request):
         """创建单元化规则, 并返回详细信息
 
         :param request: Request instance for CreateUnitRuleWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.CreateUnitRuleWithDetailRespRequest`
@@ -893,15 +893,15 @@
             model = models.CreateUnitRuleWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApiGroup(self, request):
         """删除Api分组
 
         :param request: Request instance for DeleteApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteApiGroupRequest`
@@ -916,15 +916,15 @@
             model = models.DeleteApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApiRateLimitRule(self, request):
         """删除API限流规则
 
         :param request: Request instance for DeleteApiRateLimitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteApiRateLimitRuleRequest`
@@ -939,15 +939,15 @@
             model = models.DeleteApiRateLimitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplication(self, request):
         """删除应用
 
         :param request: Request instance for DeleteApplication.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteApplicationRequest`
@@ -962,15 +962,15 @@
             model = models.DeleteApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """删除集群
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteClusterRequest`
@@ -985,15 +985,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfig(self, request):
         """删除配置项
 
         :param request: Request instance for DeleteConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteConfigRequest`
@@ -1008,15 +1008,15 @@
             model = models.DeleteConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfigTemplate(self, request):
         """删除模板
 
         :param request: Request instance for DeleteConfigTemplate.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteConfigTemplateRequest`
@@ -1031,15 +1031,15 @@
             model = models.DeleteConfigTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteContainerGroup(self, request):
         """删除容器部署组
 
         :param request: Request instance for DeleteContainerGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteContainerGroupRequest`
@@ -1054,15 +1054,15 @@
             model = models.DeleteContainerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFileConfig(self, request):
         """删除文件配置项
 
         :param request: Request instance for DeleteFileConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteFileConfigRequest`
@@ -1077,15 +1077,15 @@
             model = models.DeleteFileConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGatewayApi(self, request):
         """批量删除API
 
         :param request: Request instance for DeleteGatewayApi.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteGatewayApiRequest`
@@ -1100,15 +1100,15 @@
             model = models.DeleteGatewayApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGroup(self, request):
         """删除容器部署组
 
         :param request: Request instance for DeleteGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteGroupRequest`
@@ -1123,15 +1123,15 @@
             model = models.DeleteGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageTags(self, request):
         """批量删除镜像版本
 
         :param request: Request instance for DeleteImageTags.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteImageTagsRequest`
@@ -1146,15 +1146,15 @@
             model = models.DeleteImageTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLane(self, request):
         """删除泳道
 
         :param request: Request instance for DeleteLane.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteLaneRequest`
@@ -1169,15 +1169,15 @@
             model = models.DeleteLaneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLaneRule(self, request):
         """删除泳道规则
 
         :param request: Request instance for DeleteLaneRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteLaneRuleRequest`
@@ -1192,15 +1192,15 @@
             model = models.DeleteLaneRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMicroservice(self, request):
         """删除微服务
 
         :param request: Request instance for DeleteMicroservice.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteMicroserviceRequest`
@@ -1215,15 +1215,15 @@
             model = models.DeleteMicroserviceResponse()
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
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteNamespaceRequest`
@@ -1238,15 +1238,15 @@
             model = models.DeleteNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePathRewrites(self, request):
         """删除路径重写
 
         :param request: Request instance for DeletePathRewrites.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeletePathRewritesRequest`
@@ -1261,15 +1261,15 @@
             model = models.DeletePathRewritesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePkgs(self, request):
         """从软件仓库批量删除程序包。
         一次最多支持删除1000个包，数量超过1000，返回UpperDeleteLimit错误。
 
         :param request: Request instance for DeletePkgs.
@@ -1285,15 +1285,15 @@
             model = models.DeletePkgsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePublicConfig(self, request):
         """删除公共配置项
 
         :param request: Request instance for DeletePublicConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeletePublicConfigRequest`
@@ -1308,15 +1308,15 @@
             model = models.DeletePublicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRepository(self, request):
         """删除仓库
 
         :param request: Request instance for DeleteRepository.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteRepositoryRequest`
@@ -1331,15 +1331,15 @@
             model = models.DeleteRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServerlessGroup(self, request):
         """删除Serverless部署组
 
         :param request: Request instance for DeleteServerlessGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteServerlessGroupRequest`
@@ -1354,15 +1354,15 @@
             model = models.DeleteServerlessGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTask(self, request):
         """删除任务
 
         :param request: Request instance for DeleteTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteTaskRequest`
@@ -1377,15 +1377,15 @@
             model = models.DeleteTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUnitNamespaces(self, request):
         """删除单元化命名空间
 
         :param request: Request instance for DeleteUnitNamespaces.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteUnitNamespacesRequest`
@@ -1400,15 +1400,15 @@
             model = models.DeleteUnitNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUnitRule(self, request):
         """删除单元化规则
 
         :param request: Request instance for DeleteUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteUnitRuleRequest`
@@ -1423,15 +1423,15 @@
             model = models.DeleteUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployContainerGroup(self, request):
         """部署容器应用-更新
 
         :param request: Request instance for DeployContainerGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeployContainerGroupRequest`
@@ -1446,15 +1446,15 @@
             model = models.DeployContainerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployGroup(self, request):
         """部署虚拟机部署组应用
 
         :param request: Request instance for DeployGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeployGroupRequest`
@@ -1469,15 +1469,15 @@
             model = models.DeployGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiDetail(self, request):
         """查询API详情
 
         :param request: Request instance for DescribeApiDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiDetailRequest`
@@ -1492,15 +1492,15 @@
             model = models.DescribeApiDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiGroup(self, request):
         """查询API分组
 
         :param request: Request instance for DescribeApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiGroupRequest`
@@ -1515,15 +1515,15 @@
             model = models.DescribeApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiGroups(self, request):
         """查询API 分组信息列表
 
         :param request: Request instance for DescribeApiGroups.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiGroupsRequest`
@@ -1538,15 +1538,15 @@
             model = models.DescribeApiGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiRateLimitRules(self, request):
         """查询API限流规则
 
         :param request: Request instance for DescribeApiRateLimitRules.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiRateLimitRulesRequest`
@@ -1561,15 +1561,15 @@
             model = models.DescribeApiRateLimitRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiUseDetail(self, request):
         """查询网关API监控明细数据
 
         :param request: Request instance for DescribeApiUseDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiUseDetailRequest`
@@ -1584,15 +1584,15 @@
             model = models.DescribeApiUseDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiVersions(self, request):
         """查询API 版本
 
         :param request: Request instance for DescribeApiVersions.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApiVersionsRequest`
@@ -1607,15 +1607,15 @@
             model = models.DescribeApiVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplication(self, request):
         """获取应用详情
 
         :param request: Request instance for DescribeApplication.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApplicationRequest`
@@ -1630,15 +1630,15 @@
             model = models.DescribeApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationAttribute(self, request):
         """获取应用列表其它字段，如实例数量信息等
 
         :param request: Request instance for DescribeApplicationAttribute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApplicationAttributeRequest`
@@ -1653,15 +1653,15 @@
             model = models.DescribeApplicationAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationBusinessLogConfig(self, request):
         """查询应用关联日志配置项信息
 
         :param request: Request instance for DescribeApplicationBusinessLogConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApplicationBusinessLogConfigRequest`
@@ -1676,15 +1676,15 @@
             model = models.DescribeApplicationBusinessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplications(self, request):
         """获取应用列表
 
         :param request: Request instance for DescribeApplications.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeApplicationsRequest`
@@ -1699,15 +1699,15 @@
             model = models.DescribeApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicResourceUsage(self, request):
         """TSF基本资源信息概览接口
 
         :param request: Request instance for DescribeBasicResourceUsage.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeBasicResourceUsageRequest`
@@ -1722,15 +1722,15 @@
             model = models.DescribeBasicResourceUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBusinessLogConfig(self, request):
         """查询业务日志配置项信息
 
         :param request: Request instance for DescribeBusinessLogConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeBusinessLogConfigRequest`
@@ -1745,15 +1745,15 @@
             model = models.DescribeBusinessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBusinessLogConfigs(self, request):
         """查询日志配置项列表
 
         :param request: Request instance for DescribeBusinessLogConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeBusinessLogConfigsRequest`
@@ -1768,15 +1768,15 @@
             model = models.DescribeBusinessLogConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterInstances(self, request):
         """查询集群实例
 
         :param request: Request instance for DescribeClusterInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeClusterInstancesRequest`
@@ -1791,15 +1791,15 @@
             model = models.DescribeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """获取集群列表
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeClustersRequest`
@@ -1814,15 +1814,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfig(self, request):
         """查询配置
 
         :param request: Request instance for DescribeConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigRequest`
@@ -1837,15 +1837,15 @@
             model = models.DescribeConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigReleaseLogs(self, request):
         """查询配置发布历史
 
         :param request: Request instance for DescribeConfigReleaseLogs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigReleaseLogsRequest`
@@ -1860,15 +1860,15 @@
             model = models.DescribeConfigReleaseLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigReleases(self, request):
         """查询配置发布信息
 
         :param request: Request instance for DescribeConfigReleases.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigReleasesRequest`
@@ -1883,15 +1883,15 @@
             model = models.DescribeConfigReleasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigSummary(self, request):
         """查询配置汇总列表
 
         :param request: Request instance for DescribeConfigSummary.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigSummaryRequest`
@@ -1906,15 +1906,15 @@
             model = models.DescribeConfigSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigTemplate(self, request):
         """导入配置
 
         :param request: Request instance for DescribeConfigTemplate.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigTemplateRequest`
@@ -1929,15 +1929,15 @@
             model = models.DescribeConfigTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigs(self, request):
         """查询配置项列表
 
         :param request: Request instance for DescribeConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeConfigsRequest`
@@ -1952,15 +1952,15 @@
             model = models.DescribeConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerEvents(self, request):
         """获取容器事件列表
 
         :param request: Request instance for DescribeContainerEvents.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerEventsRequest`
@@ -1975,15 +1975,15 @@
             model = models.DescribeContainerEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerGroupAttribute(self, request):
         """获取部署组其他字段-用于前端并发调用
 
         :param request: Request instance for DescribeContainerGroupAttribute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupAttributeRequest`
@@ -1998,15 +1998,15 @@
             model = models.DescribeContainerGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerGroupDeployInfo(self, request):
         """获取部署组详情
 
         :param request: Request instance for DescribeContainerGroupDeployInfo.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupDeployInfoRequest`
@@ -2021,15 +2021,15 @@
             model = models.DescribeContainerGroupDeployInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerGroupDetail(self, request):
         """容器部署组详情（已废弃，请使用  DescribeContainerGroupDeployInfo）
 
         :param request: Request instance for DescribeContainerGroupDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupDetailRequest`
@@ -2044,15 +2044,15 @@
             model = models.DescribeContainerGroupDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerGroups(self, request):
         """容器部署组列表
 
         :param request: Request instance for DescribeContainerGroups.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeContainerGroupsRequest`
@@ -2067,15 +2067,15 @@
             model = models.DescribeContainerGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCreateGatewayApiStatus(self, request):
         """查询一键导入API分组任务的状态
 
         :param request: Request instance for DescribeCreateGatewayApiStatus.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeCreateGatewayApiStatusRequest`
@@ -2090,15 +2090,15 @@
             model = models.DescribeCreateGatewayApiStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeliveryConfig(self, request):
         """获取单个投递项配置信息
 
         :param request: Request instance for DescribeDeliveryConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeDeliveryConfigRequest`
@@ -2113,15 +2113,15 @@
             model = models.DescribeDeliveryConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeliveryConfigByGroupId(self, request):
         """用部署组id获取绑定信息
 
         :param request: Request instance for DescribeDeliveryConfigByGroupId.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeDeliveryConfigByGroupIdRequest`
@@ -2136,15 +2136,15 @@
             model = models.DescribeDeliveryConfigByGroupIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeliveryConfigs(self, request):
         """获取多个投递项配置
 
         :param request: Request instance for DescribeDeliveryConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeDeliveryConfigsRequest`
@@ -2159,15 +2159,15 @@
             model = models.DescribeDeliveryConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDownloadInfo(self, request):
         """TSF上传的程序包存放在腾讯云对象存储（COS）中，通过该API可以获取从COS下载程序包需要的信息，包括包所在的桶、存储路径、鉴权信息等，之后使用COS API（或SDK）进行下载。
         COS相关文档请查阅：https://cloud.tencent.com/document/product/436
 
         :param request: Request instance for DescribeDownloadInfo.
@@ -2183,15 +2183,15 @@
             model = models.DescribeDownloadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnabledUnitRule(self, request):
         """查询生效的单元化规则
 
         :param request: Request instance for DescribeEnabledUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeEnabledUnitRuleRequest`
@@ -2206,15 +2206,15 @@
             model = models.DescribeEnabledUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileConfigReleases(self, request):
         """查询文件配置项发布信息
 
         :param request: Request instance for DescribeFileConfigReleases.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeFileConfigReleasesRequest`
@@ -2229,15 +2229,15 @@
             model = models.DescribeFileConfigReleasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileConfigs(self, request):
         """查询文件配置项列表
 
         :param request: Request instance for DescribeFileConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeFileConfigsRequest`
@@ -2252,15 +2252,15 @@
             model = models.DescribeFileConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowLastBatchState(self, request):
         """查询工作流最新一个批次的状态信息
 
         :param request: Request instance for DescribeFlowLastBatchState.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeFlowLastBatchStateRequest`
@@ -2275,15 +2275,15 @@
             model = models.DescribeFlowLastBatchStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayAllGroupApis(self, request):
         """查询网关所有分组下Api列表
 
         :param request: Request instance for DescribeGatewayAllGroupApis.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGatewayAllGroupApisRequest`
@@ -2298,15 +2298,15 @@
             model = models.DescribeGatewayAllGroupApisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayApis(self, request):
         """查询API分组下的Api列表信息
 
         :param request: Request instance for DescribeGatewayApis.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGatewayApisRequest`
@@ -2321,15 +2321,15 @@
             model = models.DescribeGatewayApisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGatewayMonitorOverview(self, request):
         """查询网关监控概览
 
         :param request: Request instance for DescribeGatewayMonitorOverview.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGatewayMonitorOverviewRequest`
@@ -2344,15 +2344,15 @@
             model = models.DescribeGatewayMonitorOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroup(self, request):
         """查询虚拟机部署组详情
 
         :param request: Request instance for DescribeGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupRequest`
@@ -2367,15 +2367,15 @@
             model = models.DescribeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupAttribute(self, request):
         """获取部署组其他属性
 
         :param request: Request instance for DescribeGroupAttribute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupAttributeRequest`
@@ -2390,15 +2390,15 @@
             model = models.DescribeGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupBindedGateways(self, request):
         """查询某个API分组已绑定的网关部署组信息列表
 
         :param request: Request instance for DescribeGroupBindedGateways.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupBindedGatewaysRequest`
@@ -2413,15 +2413,15 @@
             model = models.DescribeGroupBindedGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupBusinessLogConfigs(self, request):
         """查询分组管理日志配置列表
 
         :param request: Request instance for DescribeGroupBusinessLogConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupBusinessLogConfigsRequest`
@@ -2436,15 +2436,15 @@
             model = models.DescribeGroupBusinessLogConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupGateways(self, request):
         """查询某个网关绑定的API 分组信息列表
 
         :param request: Request instance for DescribeGroupGateways.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupGatewaysRequest`
@@ -2459,15 +2459,15 @@
             model = models.DescribeGroupGatewaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupInstances(self, request):
         """查询虚拟机部署组云主机列表
 
         :param request: Request instance for DescribeGroupInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupInstancesRequest`
@@ -2482,15 +2482,15 @@
             model = models.DescribeGroupInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupRelease(self, request):
         """查询部署组相关的发布信息
 
         :param request: Request instance for DescribeGroupRelease.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupReleaseRequest`
@@ -2505,15 +2505,15 @@
             model = models.DescribeGroupReleaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupUseDetail(self, request):
         """查询网关分组监控明细数据
 
         :param request: Request instance for DescribeGroupUseDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupUseDetailRequest`
@@ -2528,15 +2528,15 @@
             model = models.DescribeGroupUseDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroups(self, request):
         """获取虚拟机部署组列表
 
         :param request: Request instance for DescribeGroups.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupsRequest`
@@ -2551,15 +2551,15 @@
             model = models.DescribeGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupsWithPlugin(self, request):
         """查询某个插件下绑定或未绑定的API分组
 
         :param request: Request instance for DescribeGroupsWithPlugin.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeGroupsWithPluginRequest`
@@ -2574,15 +2574,15 @@
             model = models.DescribeGroupsWithPluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageRepository(self, request):
         """镜像仓库列表
 
         :param request: Request instance for DescribeImageRepository.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeImageRepositoryRequest`
@@ -2597,15 +2597,15 @@
             model = models.DescribeImageRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageTags(self, request):
         """镜像版本列表
 
         :param request: Request instance for DescribeImageTags.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeImageTagsRequest`
@@ -2620,15 +2620,15 @@
             model = models.DescribeImageTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInovcationIndicators(self, request):
         """废弃
 
         :param request: Request instance for DescribeInovcationIndicators.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInovcationIndicatorsRequest`
@@ -2643,15 +2643,15 @@
             model = models.DescribeInovcationIndicatorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """无
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInstancesRequest`
@@ -2666,15 +2666,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocationMetricDataCurve(self, request):
         """查询调用指标数据变化曲线
 
         :param request: Request instance for DescribeInvocationMetricDataCurve.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInvocationMetricDataCurveRequest`
@@ -2689,15 +2689,15 @@
             model = models.DescribeInvocationMetricDataCurveResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocationMetricDataDimension(self, request):
         """查询维度
 
         :param request: Request instance for DescribeInvocationMetricDataDimension.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInvocationMetricDataDimensionRequest`
@@ -2712,15 +2712,15 @@
             model = models.DescribeInvocationMetricDataDimensionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocationMetricDataPoint(self, request):
         """查询单值指标维度
 
         :param request: Request instance for DescribeInvocationMetricDataPoint.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInvocationMetricDataPointRequest`
@@ -2735,15 +2735,15 @@
             model = models.DescribeInvocationMetricDataPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInvocationMetricScatterPlot(self, request):
         """查询调用指标数据散点图
 
         :param request: Request instance for DescribeInvocationMetricScatterPlot.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeInvocationMetricScatterPlotRequest`
@@ -2758,15 +2758,15 @@
             model = models.DescribeInvocationMetricScatterPlotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJvmMonitor(self, request):
         """查询java实例jvm监控数据,返回数据可选
 
         :param request: Request instance for DescribeJvmMonitor.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeJvmMonitorRequest`
@@ -2781,15 +2781,15 @@
             model = models.DescribeJvmMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLaneRules(self, request):
         """查询泳道规则列表
 
         :param request: Request instance for DescribeLaneRules.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeLaneRulesRequest`
@@ -2804,15 +2804,15 @@
             model = models.DescribeLaneRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLanes(self, request):
         """查询泳道列表
 
         :param request: Request instance for DescribeLanes.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeLanesRequest`
@@ -2827,15 +2827,15 @@
             model = models.DescribeLanesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMicroservice(self, request):
         """查询微服务详情
 
         :param request: Request instance for DescribeMicroservice.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeMicroserviceRequest`
@@ -2850,15 +2850,15 @@
             model = models.DescribeMicroserviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMicroservices(self, request):
         """获取微服务列表
 
         :param request: Request instance for DescribeMicroservices.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeMicroservicesRequest`
@@ -2873,15 +2873,15 @@
             model = models.DescribeMicroservicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMsApiList(self, request):
         """查询服务API列表
 
         :param request: Request instance for DescribeMsApiList.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeMsApiListRequest`
@@ -2896,15 +2896,15 @@
             model = models.DescribeMsApiListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewInvocation(self, request):
         """服务调用监控统计概览
 
         :param request: Request instance for DescribeOverviewInvocation.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeOverviewInvocationRequest`
@@ -2919,15 +2919,15 @@
             model = models.DescribeOverviewInvocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePathRewrite(self, request):
         """查询路径重写
 
         :param request: Request instance for DescribePathRewrite.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePathRewriteRequest`
@@ -2942,15 +2942,15 @@
             model = models.DescribePathRewriteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePathRewrites(self, request):
         """查询路径重写列表
 
         :param request: Request instance for DescribePathRewrites.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePathRewritesRequest`
@@ -2965,15 +2965,15 @@
             model = models.DescribePathRewritesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePkgs(self, request):
         """无
 
         :param request: Request instance for DescribePkgs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePkgsRequest`
@@ -2988,15 +2988,15 @@
             model = models.DescribePkgsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePluginInstances(self, request):
         """分页查询网关分组/API绑定（或未绑定）的插件列表
 
         :param request: Request instance for DescribePluginInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePluginInstancesRequest`
@@ -3011,15 +3011,15 @@
             model = models.DescribePluginInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePodInstances(self, request):
         """获取部署组实例列表
 
         :param request: Request instance for DescribePodInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePodInstancesRequest`
@@ -3034,15 +3034,15 @@
             model = models.DescribePodInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrograms(self, request):
         """查询数据集列表
 
         :param request: Request instance for DescribePrograms.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeProgramsRequest`
@@ -3057,15 +3057,15 @@
             model = models.DescribeProgramsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicConfig(self, request):
         """查询公共配置（单条）
 
         :param request: Request instance for DescribePublicConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePublicConfigRequest`
@@ -3080,15 +3080,15 @@
             model = models.DescribePublicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicConfigReleaseLogs(self, request):
         """查询公共配置发布历史
 
         :param request: Request instance for DescribePublicConfigReleaseLogs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePublicConfigReleaseLogsRequest`
@@ -3103,15 +3103,15 @@
             model = models.DescribePublicConfigReleaseLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicConfigReleases(self, request):
         """查询公共配置发布信息
 
         :param request: Request instance for DescribePublicConfigReleases.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePublicConfigReleasesRequest`
@@ -3126,15 +3126,15 @@
             model = models.DescribePublicConfigReleasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicConfigSummary(self, request):
         """查询公共配置汇总列表
 
         :param request: Request instance for DescribePublicConfigSummary.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePublicConfigSummaryRequest`
@@ -3149,15 +3149,15 @@
             model = models.DescribePublicConfigSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicConfigs(self, request):
         """查询公共配置项列表
 
         :param request: Request instance for DescribePublicConfigs.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribePublicConfigsRequest`
@@ -3172,15 +3172,15 @@
             model = models.DescribePublicConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReleasedConfig(self, request):
         """查询group发布的配置
 
         :param request: Request instance for DescribeReleasedConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeReleasedConfigRequest`
@@ -3195,15 +3195,15 @@
             model = models.DescribeReleasedConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepositories(self, request):
         """查询仓库列表
 
         :param request: Request instance for DescribeRepositories.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeRepositoriesRequest`
@@ -3218,15 +3218,15 @@
             model = models.DescribeRepositoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRepository(self, request):
         """查询仓库信息
 
         :param request: Request instance for DescribeRepository.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeRepositoryRequest`
@@ -3241,15 +3241,15 @@
             model = models.DescribeRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceTaskStatus(self, request):
         """资源任务的执行状态描述接口
 
         :param request: Request instance for DescribeResourceTaskStatus.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeResourceTaskStatusRequest`
@@ -3264,15 +3264,15 @@
             model = models.DescribeResourceTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSimpleApplications(self, request):
         """查询简单应用列表
 
         :param request: Request instance for DescribeSimpleApplications.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeSimpleApplicationsRequest`
@@ -3287,15 +3287,15 @@
             model = models.DescribeSimpleApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSimpleClusters(self, request):
         """查询简单集群列表
 
         :param request: Request instance for DescribeSimpleClusters.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeSimpleClustersRequest`
@@ -3310,15 +3310,15 @@
             model = models.DescribeSimpleClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSimpleGroups(self, request):
         """查询简单部署组列表
 
         :param request: Request instance for DescribeSimpleGroups.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeSimpleGroupsRequest`
@@ -3333,15 +3333,15 @@
             model = models.DescribeSimpleGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSimpleNamespaces(self, request):
         """查询简单命名空间列表
 
         :param request: Request instance for DescribeSimpleNamespaces.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeSimpleNamespacesRequest`
@@ -3356,15 +3356,15 @@
             model = models.DescribeSimpleNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStatistics(self, request):
         """服务统计页面：接口和服务维度
 
         :param request: Request instance for DescribeStatistics.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeStatisticsRequest`
@@ -3379,15 +3379,15 @@
             model = models.DescribeStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """查询任务详情
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeTaskDetailRequest`
@@ -3402,15 +3402,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskLastStatus(self, request):
         """查询任务最近一次执行状态
 
         :param request: Request instance for DescribeTaskLastStatus.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeTaskLastStatusRequest`
@@ -3425,15 +3425,15 @@
             model = models.DescribeTaskLastStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskRecords(self, request):
         """翻页查询任务列表
 
         :param request: Request instance for DescribeTaskRecords.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeTaskRecordsRequest`
@@ -3448,15 +3448,15 @@
             model = models.DescribeTaskRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnitApiUseDetail(self, request):
         """查询网关API监控明细数据（仅单元化网关），非单元化网关使用DescribeApiUseDetail
 
         :param request: Request instance for DescribeUnitApiUseDetail.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUnitApiUseDetailRequest`
@@ -3471,15 +3471,15 @@
             model = models.DescribeUnitApiUseDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnitNamespaces(self, request):
         """查询单元化命名空间列表
 
         :param request: Request instance for DescribeUnitNamespaces.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUnitNamespacesRequest`
@@ -3494,15 +3494,15 @@
             model = models.DescribeUnitNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnitRule(self, request):
         """查询单元化规则详情
 
         :param request: Request instance for DescribeUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUnitRuleRequest`
@@ -3517,15 +3517,15 @@
             model = models.DescribeUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnitRules(self, request):
         """查询单元化规则列表
 
         :param request: Request instance for DescribeUnitRules.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUnitRulesRequest`
@@ -3540,15 +3540,15 @@
             model = models.DescribeUnitRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnitRulesV2(self, request):
         """查询单元化规则列表V2
 
         :param request: Request instance for DescribeUnitRulesV2.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUnitRulesV2Request`
@@ -3563,15 +3563,15 @@
             model = models.DescribeUnitRulesV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUploadInfo(self, request):
         """TSF会将软件包上传到腾讯云对象存储（COS）。调用此接口获取上传信息，如目标地域，桶，包Id，存储路径，鉴权信息等，之后请使用COS API（或SDK）进行上传。
         COS相关文档请查阅：https://cloud.tencent.com/document/product/436
 
         :param request: Request instance for DescribeUploadInfo.
@@ -3587,15 +3587,15 @@
             model = models.DescribeUploadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsableUnitNamespaces(self, request):
         """查询可用于被导入的命名空间列表
 
         :param request: Request instance for DescribeUsableUnitNamespaces.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DescribeUsableUnitNamespacesRequest`
@@ -3610,15 +3610,15 @@
             model = models.DescribeUsableUnitNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableTask(self, request):
         """停用任务
 
         :param request: Request instance for DisableTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisableTaskRequest`
@@ -3633,15 +3633,15 @@
             model = models.DisableTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableTaskFlow(self, request):
         """停用工作流
 
         :param request: Request instance for DisableTaskFlow.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisableTaskFlowRequest`
@@ -3656,15 +3656,15 @@
             model = models.DisableTaskFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableUnitRoute(self, request):
         """禁用单元化路由
 
         :param request: Request instance for DisableUnitRoute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisableUnitRouteRequest`
@@ -3679,15 +3679,15 @@
             model = models.DisableUnitRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableUnitRule(self, request):
         """禁用单元化规则
 
         :param request: Request instance for DisableUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisableUnitRuleRequest`
@@ -3702,15 +3702,15 @@
             model = models.DisableUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateBusinessLogConfig(self, request):
         """取消关联业务日志配置项和应用
 
         :param request: Request instance for DisassociateBusinessLogConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisassociateBusinessLogConfigRequest`
@@ -3725,15 +3725,15 @@
             model = models.DisassociateBusinessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateKafkaConfig(self, request):
         """取消关联投递信息和部署组
 
         :param request: Request instance for DisassociateKafkaConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DisassociateKafkaConfigRequest`
@@ -3748,15 +3748,15 @@
             model = models.DisassociateKafkaConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DraftApiGroup(self, request):
         """下线Api分组
 
         :param request: Request instance for DraftApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DraftApiGroupRequest`
@@ -3771,15 +3771,15 @@
             model = models.DraftApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableTask(self, request):
         """启用任务
 
         :param request: Request instance for EnableTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.EnableTaskRequest`
@@ -3794,15 +3794,15 @@
             model = models.EnableTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableTaskFlow(self, request):
         """启用工作流
 
         :param request: Request instance for EnableTaskFlow.
         :type request: :class:`tencentcloud.tsf.v20180326.models.EnableTaskFlowRequest`
@@ -3817,15 +3817,15 @@
             model = models.EnableTaskFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableUnitRoute(self, request):
         """启用单元化路由
 
         :param request: Request instance for EnableUnitRoute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.EnableUnitRouteRequest`
@@ -3840,15 +3840,15 @@
             model = models.EnableUnitRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableUnitRule(self, request):
         """启用单元化规则
 
         :param request: Request instance for EnableUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.EnableUnitRuleRequest`
@@ -3863,15 +3863,15 @@
             model = models.EnableUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteTask(self, request):
         """手动执行一次任务。
 
         :param request: Request instance for ExecuteTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ExecuteTaskRequest`
@@ -3886,15 +3886,15 @@
             model = models.ExecuteTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteTaskFlow(self, request):
         """执行一次工作流
 
         :param request: Request instance for ExecuteTaskFlow.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ExecuteTaskFlowRequest`
@@ -3909,15 +3909,15 @@
             model = models.ExecuteTaskFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExpandGroup(self, request):
         """虚拟机部署组添加实例
 
         :param request: Request instance for ExpandGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ExpandGroupRequest`
@@ -3932,15 +3932,15 @@
             model = models.ExpandGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplication(self, request):
         """修改应用
 
         :param request: Request instance for ModifyApplication.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyApplicationRequest`
@@ -3955,15 +3955,15 @@
             model = models.ModifyApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCluster(self, request):
         """修改集群信息
 
         :param request: Request instance for ModifyCluster.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyClusterRequest`
@@ -3978,15 +3978,15 @@
             model = models.ModifyClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyContainerGroup(self, request):
         """修改容器部署组
 
         :param request: Request instance for ModifyContainerGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyContainerGroupRequest`
@@ -4001,15 +4001,15 @@
             model = models.ModifyContainerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyContainerReplicas(self, request):
         """修改容器部署组实例数
 
         :param request: Request instance for ModifyContainerReplicas.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyContainerReplicasRequest`
@@ -4024,15 +4024,15 @@
             model = models.ModifyContainerReplicasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGroup(self, request):
         """更新部署组信息
 
         :param request: Request instance for ModifyGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyGroupRequest`
@@ -4047,15 +4047,15 @@
             model = models.ModifyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLane(self, request):
         """更新泳道信息
 
         :param request: Request instance for ModifyLane.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyLaneRequest`
@@ -4070,15 +4070,15 @@
             model = models.ModifyLaneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLaneRule(self, request):
         """更新泳道规则
 
         :param request: Request instance for ModifyLaneRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyLaneRuleRequest`
@@ -4093,15 +4093,15 @@
             model = models.ModifyLaneRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMicroservice(self, request):
         """修改微服务详情
 
         :param request: Request instance for ModifyMicroservice.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyMicroserviceRequest`
@@ -4116,15 +4116,15 @@
             model = models.ModifyMicroserviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNamespace(self, request):
         """修改命名空间
 
         :param request: Request instance for ModifyNamespace.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyNamespaceRequest`
@@ -4139,15 +4139,15 @@
             model = models.ModifyNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPathRewrite(self, request):
         """修改路径重写
 
         :param request: Request instance for ModifyPathRewrite.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyPathRewriteRequest`
@@ -4162,15 +4162,15 @@
             model = models.ModifyPathRewriteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTask(self, request):
         """修改任务
 
         :param request: Request instance for ModifyTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ModifyTaskRequest`
@@ -4185,15 +4185,15 @@
             model = models.ModifyTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUploadInfo(self, request):
         """调用该接口和COS的上传接口后，需要调用此接口更新TSF中保存的程序包状态。
         调用此接口完成后，才标志上传包流程结束。
 
         :param request: Request instance for ModifyUploadInfo.
@@ -4209,15 +4209,15 @@
             model = models.ModifyUploadInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OperateApplicationTcrBinding(self, request):
         """绑定解绑tcr仓库
 
         :param request: Request instance for OperateApplicationTcrBinding.
         :type request: :class:`tencentcloud.tsf.v20180326.models.OperateApplicationTcrBindingRequest`
@@ -4232,15 +4232,15 @@
             model = models.OperateApplicationTcrBindingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReassociateBusinessLogConfig(self, request):
         """重关联业务日志配置
 
         :param request: Request instance for ReassociateBusinessLogConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReassociateBusinessLogConfigRequest`
@@ -4255,15 +4255,15 @@
             model = models.ReassociateBusinessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RedoTask(self, request):
         """重新执行任务
 
         :param request: Request instance for RedoTask.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RedoTaskRequest`
@@ -4278,15 +4278,15 @@
             model = models.RedoTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RedoTaskBatch(self, request):
         """重新执行任务批次
 
         :param request: Request instance for RedoTaskBatch.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RedoTaskBatchRequest`
@@ -4301,15 +4301,15 @@
             model = models.RedoTaskBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RedoTaskExecute(self, request):
         """重新执行在某个节点上执行任务。
 
         :param request: Request instance for RedoTaskExecute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RedoTaskExecuteRequest`
@@ -4324,15 +4324,15 @@
             model = models.RedoTaskExecuteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RedoTaskFlowBatch(self, request):
         """重新执行工作流批次
 
         :param request: Request instance for RedoTaskFlowBatch.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RedoTaskFlowBatchRequest`
@@ -4347,15 +4347,15 @@
             model = models.RedoTaskFlowBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseApiGroup(self, request):
         """发布Api分组
 
         :param request: Request instance for ReleaseApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReleaseApiGroupRequest`
@@ -4370,15 +4370,15 @@
             model = models.ReleaseApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseConfig(self, request):
         """发布配置
 
         :param request: Request instance for ReleaseConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReleaseConfigRequest`
@@ -4393,15 +4393,15 @@
             model = models.ReleaseConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseConfigWithDetailResp(self, request):
         """发布配置,并且返回配置 ID
 
         :param request: Request instance for ReleaseConfigWithDetailResp.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReleaseConfigWithDetailRespRequest`
@@ -4416,15 +4416,15 @@
             model = models.ReleaseConfigWithDetailRespResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseFileConfig(self, request):
         """发布文件配置
 
         :param request: Request instance for ReleaseFileConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReleaseFileConfigRequest`
@@ -4439,15 +4439,15 @@
             model = models.ReleaseFileConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleasePublicConfig(self, request):
         """发布公共配置
 
         :param request: Request instance for ReleasePublicConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ReleasePublicConfigRequest`
@@ -4462,15 +4462,15 @@
             model = models.ReleasePublicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveInstances(self, request):
         """从 TSF 集群中批量移除云主机节点
 
         :param request: Request instance for RemoveInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RemoveInstancesRequest`
@@ -4485,15 +4485,15 @@
             model = models.RemoveInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevocationConfig(self, request):
         """撤回已发布的配置
 
         :param request: Request instance for RevocationConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RevocationConfigRequest`
@@ -4508,15 +4508,15 @@
             model = models.RevocationConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevocationPublicConfig(self, request):
         """撤回已发布的公共配置
 
         :param request: Request instance for RevocationPublicConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RevocationPublicConfigRequest`
@@ -4531,15 +4531,15 @@
             model = models.RevocationPublicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeFileConfig(self, request):
         """撤回已发布的文件配置
 
         :param request: Request instance for RevokeFileConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RevokeFileConfigRequest`
@@ -4554,15 +4554,15 @@
             model = models.RevokeFileConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackConfig(self, request):
         """回滚配置
 
         :param request: Request instance for RollbackConfig.
         :type request: :class:`tencentcloud.tsf.v20180326.models.RollbackConfigRequest`
@@ -4577,15 +4577,15 @@
             model = models.RollbackConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchBusinessLog(self, request):
         """业务日志搜索
 
         :param request: Request instance for SearchBusinessLog.
         :type request: :class:`tencentcloud.tsf.v20180326.models.SearchBusinessLogRequest`
@@ -4600,15 +4600,15 @@
             model = models.SearchBusinessLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchStdoutLog(self, request):
         """标准输出日志搜索
 
         :param request: Request instance for SearchStdoutLog.
         :type request: :class:`tencentcloud.tsf.v20180326.models.SearchStdoutLogRequest`
@@ -4623,15 +4623,15 @@
             model = models.SearchStdoutLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ShrinkGroup(self, request):
         """下线部署组所有机器实例
 
         :param request: Request instance for ShrinkGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ShrinkGroupRequest`
@@ -4646,15 +4646,15 @@
             model = models.ShrinkGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ShrinkInstances(self, request):
         """虚拟机部署组下线实例
 
         :param request: Request instance for ShrinkInstances.
         :type request: :class:`tencentcloud.tsf.v20180326.models.ShrinkInstancesRequest`
@@ -4669,15 +4669,15 @@
             model = models.ShrinkInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartContainerGroup(self, request):
         """启动容器部署组
 
         :param request: Request instance for StartContainerGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StartContainerGroupRequest`
@@ -4692,15 +4692,15 @@
             model = models.StartContainerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartGroup(self, request):
         """启动分组
 
         :param request: Request instance for StartGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StartGroupRequest`
@@ -4715,15 +4715,15 @@
             model = models.StartGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopContainerGroup(self, request):
         """停止容器部署组
 
         :param request: Request instance for StopContainerGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StopContainerGroupRequest`
@@ -4738,15 +4738,15 @@
             model = models.StopContainerGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopGroup(self, request):
         """停止虚拟机部署组
 
         :param request: Request instance for StopGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StopGroupRequest`
@@ -4761,15 +4761,15 @@
             model = models.StopGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopTaskBatch(self, request):
         """停止执行中的任务批次， 非运行中的任务不可调用。
 
         :param request: Request instance for StopTaskBatch.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StopTaskBatchRequest`
@@ -4784,15 +4784,15 @@
             model = models.StopTaskBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopTaskExecute(self, request):
         """停止正在某个节点上执行的任务
 
         :param request: Request instance for StopTaskExecute.
         :type request: :class:`tencentcloud.tsf.v20180326.models.StopTaskExecuteRequest`
@@ -4807,15 +4807,15 @@
             model = models.StopTaskExecuteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateTaskFlowBatch(self, request):
         """停止一个工作流批次
 
         :param request: Request instance for TerminateTaskFlowBatch.
         :type request: :class:`tencentcloud.tsf.v20180326.models.TerminateTaskFlowBatchRequest`
@@ -4830,15 +4830,15 @@
             model = models.TerminateTaskFlowBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindApiGroup(self, request):
         """API分组批量与网关解绑
 
         :param request: Request instance for UnbindApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UnbindApiGroupRequest`
@@ -4853,15 +4853,15 @@
             model = models.UnbindApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiGroup(self, request):
         """更新Api分组
 
         :param request: Request instance for UpdateApiGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateApiGroupRequest`
@@ -4876,15 +4876,15 @@
             model = models.UpdateApiGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiRateLimitRule(self, request):
         """更新API限流规则
 
         :param request: Request instance for UpdateApiRateLimitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateApiRateLimitRuleRequest`
@@ -4899,15 +4899,15 @@
             model = models.UpdateApiRateLimitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiRateLimitRules(self, request):
         """批量更新API限流规则
 
         :param request: Request instance for UpdateApiRateLimitRules.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateApiRateLimitRulesRequest`
@@ -4922,15 +4922,15 @@
             model = models.UpdateApiRateLimitRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiTimeouts(self, request):
         """批量更新API超时
 
         :param request: Request instance for UpdateApiTimeouts.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateApiTimeoutsRequest`
@@ -4945,15 +4945,15 @@
             model = models.UpdateApiTimeoutsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateConfigTemplate(self, request):
         """更新参数模板
 
         :param request: Request instance for UpdateConfigTemplate.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateConfigTemplateRequest`
@@ -4968,15 +4968,15 @@
             model = models.UpdateConfigTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGatewayApi(self, request):
         """更新API
 
         :param request: Request instance for UpdateGatewayApi.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateGatewayApiRequest`
@@ -4991,15 +4991,15 @@
             model = models.UpdateGatewayApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateHealthCheckSettings(self, request):
         """更新健康检查配置
 
         :param request: Request instance for UpdateHealthCheckSettings.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateHealthCheckSettingsRequest`
@@ -5014,15 +5014,15 @@
             model = models.UpdateHealthCheckSettingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRepository(self, request):
         """更新仓库信息
 
         :param request: Request instance for UpdateRepository.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateRepositoryRequest`
@@ -5037,15 +5037,15 @@
             model = models.UpdateRepositoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateUnitRule(self, request):
         """更新单元化规则
 
         :param request: Request instance for UpdateUnitRule.
         :type request: :class:`tencentcloud.tsf.v20180326.models.UpdateUnitRuleRequest`
@@ -5060,8 +5060,8 @@
             model = models.UpdateUnitRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.938/tencentcloud/tsf/v20180326/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.938/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/README.rst` & `tencentcloud-sdk-python-tsf-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.937/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.938/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

