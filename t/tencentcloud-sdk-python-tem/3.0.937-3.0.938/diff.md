# Comparing `tmp/tencentcloud-sdk-python-tem-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tem-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.937.tar", last modified: Tue Jul 18 00:32:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.938.tar", last modified: Wed Jul 19 00:50:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tem-3.0.937.tar` & `tencentcloud-sdk-python-tem-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16604 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45873 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   379283 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/__init__.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15756 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   117434 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:32:28.000000 tencentcloud-sdk-python-tem-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16604 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46073 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   379283 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   117434 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:50:09.000000 tencentcloud-sdk-python-tem-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tem-3.0.937/setup.py` & `tencentcloud-sdk-python-tem-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/tem_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationAutoscaler(self, request):
         """创建弹性伸缩策略组合
 
         :param request: Request instance for CreateApplicationAutoscaler.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateApplicationAutoscalerRequest`
@@ -65,15 +65,15 @@
             model = models.CreateApplicationAutoscalerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationService(self, request):
         """新增访问方式
 
         :param request: Request instance for CreateApplicationService.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateApplicationServiceRequest`
@@ -88,15 +88,15 @@
             model = models.CreateApplicationServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigData(self, request):
         """创建配置
 
         :param request: Request instance for CreateConfigData.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateConfigDataRequest`
@@ -111,15 +111,15 @@
             model = models.CreateConfigDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCosToken(self, request):
         """生成Cos临时秘钥
 
         :param request: Request instance for CreateCosToken.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateCosTokenRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCosTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEnvironment(self, request):
         """创建环境
 
         :param request: Request instance for CreateEnvironment.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateEnvironmentRequest`
@@ -157,15 +157,15 @@
             model = models.CreateEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLogConfig(self, request):
         """创建日志收集配置
 
         :param request: Request instance for CreateLogConfig.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateLogConfigRequest`
@@ -180,15 +180,15 @@
             model = models.CreateLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResource(self, request):
         """绑定云资源
 
         :param request: Request instance for CreateResource.
         :type request: :class:`tencentcloud.tem.v20210701.models.CreateResourceRequest`
@@ -203,15 +203,15 @@
             model = models.CreateResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplication(self, request):
         """服务删除
           - 停止当前运行服务
           - 删除服务相关资源
           - 删除服务
@@ -229,15 +229,15 @@
             model = models.DeleteApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplicationAutoscaler(self, request):
         """删除应用弹性策略组合
 
         :param request: Request instance for DeleteApplicationAutoscaler.
         :type request: :class:`tencentcloud.tem.v20210701.models.DeleteApplicationAutoscalerRequest`
@@ -252,15 +252,15 @@
             model = models.DeleteApplicationAutoscalerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplicationService(self, request):
         """删除一条访问方式
 
         :param request: Request instance for DeleteApplicationService.
         :type request: :class:`tencentcloud.tem.v20210701.models.DeleteApplicationServiceRequest`
@@ -275,15 +275,15 @@
             model = models.DeleteApplicationServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIngress(self, request):
         """删除 Ingress 规则
 
         :param request: Request instance for DeleteIngress.
         :type request: :class:`tencentcloud.tem.v20210701.models.DeleteIngressRequest`
@@ -298,15 +298,15 @@
             model = models.DeleteIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployApplication(self, request):
         """应用部署
 
         :param request: Request instance for DeployApplication.
         :type request: :class:`tencentcloud.tem.v20210701.models.DeployApplicationRequest`
@@ -321,15 +321,15 @@
             model = models.DeployApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationAutoscalerList(self, request):
         """获取应用弹性策略组合
 
         :param request: Request instance for DescribeApplicationAutoscalerList.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationAutoscalerListRequest`
@@ -344,15 +344,15 @@
             model = models.DescribeApplicationAutoscalerListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationInfo(self, request):
         """服务基本信息查看
 
         :param request: Request instance for DescribeApplicationInfo.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationInfoRequest`
@@ -367,15 +367,15 @@
             model = models.DescribeApplicationInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationPods(self, request):
         """获取应用实例列表
 
         :param request: Request instance for DescribeApplicationPods.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationPodsRequest`
@@ -390,15 +390,15 @@
             model = models.DescribeApplicationPodsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationServiceList(self, request):
         """查询应用访问方式列表
 
         :param request: Request instance for DescribeApplicationServiceList.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationServiceListRequest`
@@ -413,15 +413,15 @@
             model = models.DescribeApplicationServiceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplications(self, request):
         """获取运行服务列表
 
         :param request: Request instance for DescribeApplications.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationsRequest`
@@ -436,15 +436,15 @@
             model = models.DescribeApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationsStatus(self, request):
         """单环境下所有应用状态查看
 
         :param request: Request instance for DescribeApplicationsStatus.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeApplicationsStatusRequest`
@@ -459,15 +459,15 @@
             model = models.DescribeApplicationsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigData(self, request):
         """查询配置详情
 
         :param request: Request instance for DescribeConfigData.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeConfigDataRequest`
@@ -482,15 +482,15 @@
             model = models.DescribeConfigDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigDataList(self, request):
         """查询配置列表
 
         :param request: Request instance for DescribeConfigDataList.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeConfigDataListRequest`
@@ -505,15 +505,15 @@
             model = models.DescribeConfigDataListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDeployApplicationDetail(self, request):
         """获取分批发布详情
 
         :param request: Request instance for DescribeDeployApplicationDetail.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeDeployApplicationDetailRequest`
@@ -528,15 +528,15 @@
             model = models.DescribeDeployApplicationDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironment(self, request):
         """获取环境基础信息
 
         :param request: Request instance for DescribeEnvironment.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeEnvironmentRequest`
@@ -551,15 +551,15 @@
             model = models.DescribeEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironmentStatus(self, request):
         """获取环境状态
 
         :param request: Request instance for DescribeEnvironmentStatus.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeEnvironmentStatusRequest`
@@ -574,15 +574,15 @@
             model = models.DescribeEnvironmentStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironments(self, request):
         """获取环境列表
 
         :param request: Request instance for DescribeEnvironments.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeEnvironmentsRequest`
@@ -597,15 +597,15 @@
             model = models.DescribeEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIngress(self, request):
         """查询 Ingress 规则
 
         :param request: Request instance for DescribeIngress.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeIngressRequest`
@@ -620,15 +620,15 @@
             model = models.DescribeIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIngresses(self, request):
         """查询 Ingress 规则列表
 
         :param request: Request instance for DescribeIngresses.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeIngressesRequest`
@@ -643,15 +643,15 @@
             model = models.DescribeIngressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogConfig(self, request):
         """查询日志收集配置详情
 
         :param request: Request instance for DescribeLogConfig.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeLogConfigRequest`
@@ -666,15 +666,15 @@
             model = models.DescribeLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePagedLogConfigList(self, request):
         """查询分页的日志收集配置列表
 
         :param request: Request instance for DescribePagedLogConfigList.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribePagedLogConfigListRequest`
@@ -689,15 +689,15 @@
             model = models.DescribePagedLogConfigListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRelatedIngresses(self, request):
         """查询应用关联的 Ingress 规则列表
 
         :param request: Request instance for DescribeRelatedIngresses.
         :type request: :class:`tencentcloud.tem.v20210701.models.DescribeRelatedIngressesRequest`
@@ -712,15 +712,15 @@
             model = models.DescribeRelatedIngressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyConfigData(self, request):
         """销毁配置
 
         :param request: Request instance for DestroyConfigData.
         :type request: :class:`tencentcloud.tem.v20210701.models.DestroyConfigDataRequest`
@@ -735,15 +735,15 @@
             model = models.DestroyConfigDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyEnvironment(self, request):
         """销毁环境
 
         :param request: Request instance for DestroyEnvironment.
         :type request: :class:`tencentcloud.tem.v20210701.models.DestroyEnvironmentRequest`
@@ -758,15 +758,15 @@
             model = models.DestroyEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyLogConfig(self, request):
         """销毁日志收集配置
 
         :param request: Request instance for DestroyLogConfig.
         :type request: :class:`tencentcloud.tem.v20210701.models.DestroyLogConfigRequest`
@@ -781,15 +781,15 @@
             model = models.DestroyLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableApplicationAutoscaler(self, request):
         """关闭应用弹性策略组合
 
         :param request: Request instance for DisableApplicationAutoscaler.
         :type request: :class:`tencentcloud.tem.v20210701.models.DisableApplicationAutoscalerRequest`
@@ -804,15 +804,15 @@
             model = models.DisableApplicationAutoscalerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableApplicationAutoscaler(self, request):
         """启用应用弹性策略组合
 
         :param request: Request instance for EnableApplicationAutoscaler.
         :type request: :class:`tencentcloud.tem.v20210701.models.EnableApplicationAutoscalerRequest`
@@ -827,15 +827,15 @@
             model = models.EnableApplicationAutoscalerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateApplicationPackageDownloadUrl(self, request):
         """生成应用程序包预签名下载链接
 
         :param request: Request instance for GenerateApplicationPackageDownloadUrl.
         :type request: :class:`tencentcloud.tem.v20210701.models.GenerateApplicationPackageDownloadUrlRequest`
@@ -850,15 +850,15 @@
             model = models.GenerateApplicationPackageDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationAutoscaler(self, request):
         """修改弹性伸缩策略组合
 
         :param request: Request instance for ModifyApplicationAutoscaler.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyApplicationAutoscalerRequest`
@@ -873,15 +873,15 @@
             model = models.ModifyApplicationAutoscalerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationInfo(self, request):
         """修改应用基本信息
 
         :param request: Request instance for ModifyApplicationInfo.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyApplicationInfoRequest`
@@ -896,15 +896,15 @@
             model = models.ModifyApplicationInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationReplicas(self, request):
         """修改应用实例数量
 
         :param request: Request instance for ModifyApplicationReplicas.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyApplicationReplicasRequest`
@@ -919,15 +919,15 @@
             model = models.ModifyApplicationReplicasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationService(self, request):
         """修改服务访问方式列表
 
         :param request: Request instance for ModifyApplicationService.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyApplicationServiceRequest`
@@ -942,15 +942,15 @@
             model = models.ModifyApplicationServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConfigData(self, request):
         """编辑配置
 
         :param request: Request instance for ModifyConfigData.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyConfigDataRequest`
@@ -965,15 +965,15 @@
             model = models.ModifyConfigDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEnvironment(self, request):
         """编辑环境
 
         :param request: Request instance for ModifyEnvironment.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyEnvironmentRequest`
@@ -988,15 +988,15 @@
             model = models.ModifyEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIngress(self, request):
         """创建或者更新 Ingress 规则
 
         :param request: Request instance for ModifyIngress.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyIngressRequest`
@@ -1011,15 +1011,15 @@
             model = models.ModifyIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLogConfig(self, request):
         """编辑日志收集配置
 
         :param request: Request instance for ModifyLogConfig.
         :type request: :class:`tencentcloud.tem.v20210701.models.ModifyLogConfigRequest`
@@ -1034,15 +1034,15 @@
             model = models.ModifyLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartApplication(self, request):
         """服务重启
 
         :param request: Request instance for RestartApplication.
         :type request: :class:`tencentcloud.tem.v20210701.models.RestartApplicationRequest`
@@ -1057,15 +1057,15 @@
             model = models.RestartApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartApplicationPod(self, request):
         """重启应用实例
 
         :param request: Request instance for RestartApplicationPod.
         :type request: :class:`tencentcloud.tem.v20210701.models.RestartApplicationPodRequest`
@@ -1080,15 +1080,15 @@
             model = models.RestartApplicationPodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeDeployApplication(self, request):
         """开始下一批次发布
 
         :param request: Request instance for ResumeDeployApplication.
         :type request: :class:`tencentcloud.tem.v20210701.models.ResumeDeployApplicationRequest`
@@ -1103,15 +1103,15 @@
             model = models.ResumeDeployApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevertDeployApplication(self, request):
         """回滚分批发布
 
         :param request: Request instance for RevertDeployApplication.
         :type request: :class:`tencentcloud.tem.v20210701.models.RevertDeployApplicationRequest`
@@ -1126,15 +1126,15 @@
             model = models.RevertDeployApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollingUpdateApplicationByVersion(self, request):
         """更新应用部署版本
 
         :param request: Request instance for RollingUpdateApplicationByVersion.
         :type request: :class:`tencentcloud.tem.v20210701.models.RollingUpdateApplicationByVersionRequest`
@@ -1149,15 +1149,15 @@
             model = models.RollingUpdateApplicationByVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopApplication(self, request):
         """服务停止
 
         :param request: Request instance for StopApplication.
         :type request: :class:`tencentcloud.tem.v20210701.models.StopApplicationRequest`
@@ -1172,8 +1172,8 @@
             model = models.StopApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20210701/models.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/tem_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCosTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCosTokenV2(self, request):
         """生成Cos临时秘钥
 
         :param request: Request instance for CreateCosTokenV2.
         :type request: :class:`tencentcloud.tem.v20201221.models.CreateCosTokenV2Request`
@@ -65,15 +65,15 @@
             model = models.CreateCosTokenV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespace(self, request):
         """创建环境
 
         :param request: Request instance for CreateNamespace.
         :type request: :class:`tencentcloud.tem.v20201221.models.CreateNamespaceRequest`
@@ -88,15 +88,15 @@
             model = models.CreateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResource(self, request):
         """绑定云资源
 
         :param request: Request instance for CreateResource.
         :type request: :class:`tencentcloud.tem.v20201221.models.CreateResourceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateResourceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceV2(self, request):
         """创建服务
 
         :param request: Request instance for CreateServiceV2.
         :type request: :class:`tencentcloud.tem.v20201221.models.CreateServiceV2Request`
@@ -134,15 +134,15 @@
             model = models.CreateServiceV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIngress(self, request):
         """删除 Ingress 规则
 
         :param request: Request instance for DeleteIngress.
         :type request: :class:`tencentcloud.tem.v20201221.models.DeleteIngressRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeployServiceV2(self, request):
         """服务部署
 
         :param request: Request instance for DeployServiceV2.
         :type request: :class:`tencentcloud.tem.v20201221.models.DeployServiceV2Request`
@@ -180,15 +180,15 @@
             model = models.DeployServiceV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIngress(self, request):
         """查询 Ingress 规则
 
         :param request: Request instance for DescribeIngress.
         :type request: :class:`tencentcloud.tem.v20201221.models.DescribeIngressRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIngresses(self, request):
         """查询 Ingress 规则列表
 
         :param request: Request instance for DescribeIngresses.
         :type request: :class:`tencentcloud.tem.v20201221.models.DescribeIngressesRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeIngressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespaces(self, request):
         """获取租户环境列表
 
         :param request: Request instance for DescribeNamespaces.
         :type request: :class:`tencentcloud.tem.v20201221.models.DescribeNamespacesRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRelatedIngresses(self, request):
         """查询服务关联的 Ingress 规则列表
 
         :param request: Request instance for DescribeRelatedIngresses.
         :type request: :class:`tencentcloud.tem.v20201221.models.DescribeRelatedIngressesRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeRelatedIngressesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceRunPodListV2(self, request):
         """获取服务下面运行pod列表
 
         :param request: Request instance for DescribeServiceRunPodListV2.
         :type request: :class:`tencentcloud.tem.v20201221.models.DescribeServiceRunPodListV2Request`
@@ -295,15 +295,15 @@
             model = models.DescribeServiceRunPodListV2Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateDownloadUrl(self, request):
         """生成包预签名下载链接
 
         :param request: Request instance for GenerateDownloadUrl.
         :type request: :class:`tencentcloud.tem.v20201221.models.GenerateDownloadUrlRequest`
@@ -318,15 +318,15 @@
             model = models.GenerateDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIngress(self, request):
         """创建或者更新 Ingress 规则
 
         :param request: Request instance for ModifyIngress.
         :type request: :class:`tencentcloud.tem.v20201221.models.ModifyIngressRequest`
@@ -341,15 +341,15 @@
             model = models.ModifyIngressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNamespace(self, request):
         """编辑环境
 
         :param request: Request instance for ModifyNamespace.
         :type request: :class:`tencentcloud.tem.v20201221.models.ModifyNamespaceRequest`
@@ -364,15 +364,15 @@
             model = models.ModifyNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceInfo(self, request):
         """修改服务基本信息
 
         :param request: Request instance for ModifyServiceInfo.
         :type request: :class:`tencentcloud.tem.v20201221.models.ModifyServiceInfoRequest`
@@ -387,15 +387,15 @@
             model = models.ModifyServiceInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartServiceRunPod(self, request):
         """重启实例
 
         :param request: Request instance for RestartServiceRunPod.
         :type request: :class:`tencentcloud.tem.v20201221.models.RestartServiceRunPodRequest`
@@ -410,8 +410,8 @@
             model = models.RestartServiceRunPodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud/tem/v20201221/models.py` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud/tem/v20201221/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.937/tencentcloud_sdk_python_tem.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.938/tencentcloud_sdk_python_tem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.937/README.rst` & `tencentcloud-sdk-python-tem-3.0.938/README.rst`

 * *Files identical despite different names*

