# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.937.tar", last modified: Tue Jul 18 00:16:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.938.tar", last modified: Wed Jul 19 00:21:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.937.tar` & `tencentcloud-sdk-python-apigateway-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21433 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   648251 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    96105 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-18 00:16:57.000000 tencentcloud-sdk-python-apigateway-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21433 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   648251 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    96493 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-19 00:21:05.000000 tencentcloud-sdk-python-apigateway-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AttachPluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindApiApp(self, request):
         """本接口（BindApiApp）用于绑定应用到API。
 
         :param request: Request instance for BindApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.BindApiAppRequest`
@@ -65,15 +65,15 @@
             model = models.BindApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindEnvironment(self, request):
         """本接口（BindEnvironment）用于绑定使用计划到服务或API。
         用户在发布服务到某个环境中后，如果 API 需要鉴权，还需要绑定使用计划才能进行调用，此接口用户将使用计划绑定到特定环境。
         目前支持绑定使用计划到API，但是同一个服务不能同时存在绑定到服务的使用计划和绑定到API的使用计划，所以对已经绑定过服务级别使用计划的环境，请先使用 服务级别使用计划降级 接口进行降级操作。
 
@@ -90,15 +90,15 @@
             model = models.BindEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindIPStrategy(self, request):
         """本接口（BindIPStrategy）用于API绑定IP策略。
 
         :param request: Request instance for BindIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.BindIPStrategyRequest`
@@ -113,15 +113,15 @@
             model = models.BindIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindSecretIds(self, request):
         """本接口（BindSecretIds）用于为使用计划绑定密钥。
         将密钥绑定到某个使用计划，并将此使用计划绑定到某个服务发布的环境上，调用者方可使用此密钥调用这个服务中的 API，可使用本接口为使用计划绑定密钥。
 
         :param request: Request instance for BindSecretIds.
@@ -137,15 +137,15 @@
             model = models.BindSecretIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindSubDomain(self, request):
         """本接口（BindSubDomain）用于绑定自定义域名到服务。
         API 网关中每个服务都会提供一个默认的域名供用户调用，但当用户想使用自己的已有域名时，也可以将自定义域名绑定到此服务，在做好备案、与默认域名的 CNAME 后，可直接调用自定义域名。
 
         :param request: Request instance for BindSubDomain.
@@ -161,15 +161,15 @@
             model = models.BindSubDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BuildAPIDoc(self, request):
         """构建 API 文档
 
         :param request: Request instance for BuildAPIDoc.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.BuildAPIDocRequest`
@@ -184,15 +184,15 @@
             model = models.BuildAPIDocResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAPIDoc(self, request):
         """创建 API 文档
 
         :param request: Request instance for CreateAPIDoc.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateAPIDocRequest`
@@ -207,15 +207,15 @@
             model = models.CreateAPIDocResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApi(self, request):
         """本接口（CreateApi）用于创建 API 接口，创建 API 前，用户需要先创建服务，每个 API 都有自己归属的服务。
 
         :param request: Request instance for CreateApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateApiRequest`
@@ -230,15 +230,15 @@
             model = models.CreateApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApiApp(self, request):
         """本接口（CreateApiApp）用于创建应用。
 
         :param request: Request instance for CreateApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateApiAppRequest`
@@ -253,15 +253,15 @@
             model = models.CreateApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApiKey(self, request):
         """本接口（CreateApiKey）用于创建一对新的 API 密钥。
 
         :param request: Request instance for CreateApiKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateApiKeyRequest`
@@ -276,15 +276,15 @@
             model = models.CreateApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIPStrategy(self, request):
         """本接口（CreateIPStrategy）用于创建服务IP策略。
 
         :param request: Request instance for CreateIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateIPStrategyRequest`
@@ -299,15 +299,15 @@
             model = models.CreateIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePlugin(self, request):
         """创建API网关插件。
 
         :param request: Request instance for CreatePlugin.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreatePluginRequest`
@@ -322,15 +322,15 @@
             model = models.CreatePluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateService(self, request):
         """本接口（CreateService）用于创建服务。
         API 网关使用的最大单元为服务，每个服务中可创建多个 API 接口。每个服务有一个默认域名供客户调用，用户也可绑定自定义域名到此服务中。
 
         :param request: Request instance for CreateService.
@@ -346,15 +346,15 @@
             model = models.CreateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUpstream(self, request):
         """用于创建后端通道
 
         :param request: Request instance for CreateUpstream.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.CreateUpstreamRequest`
@@ -369,15 +369,15 @@
             model = models.CreateUpstreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUsagePlan(self, request):
         """本接口（CreateUsagePlan）用于创建使用计划。
         用户在使用 API 网关时，需要创建使用计划并将其绑定到服务的环境中使用。
 
         :param request: Request instance for CreateUsagePlan.
@@ -393,15 +393,15 @@
             model = models.CreateUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAPIDoc(self, request):
         """删除 API 文档
 
         :param request: Request instance for DeleteAPIDoc.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteAPIDocRequest`
@@ -416,15 +416,15 @@
             model = models.DeleteAPIDocResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApi(self, request):
         """本接口（DeleteApi）用于删除已经创建的API。
 
         :param request: Request instance for DeleteApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteApiRequest`
@@ -439,15 +439,15 @@
             model = models.DeleteApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApiApp(self, request):
         """本接口（DeleteApiApp）用于删除已经创建的应用。
 
         :param request: Request instance for DeleteApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteApiAppRequest`
@@ -462,15 +462,15 @@
             model = models.DeleteApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApiKey(self, request):
         """本接口（DeleteApiKey）用于删除一对 API 密钥。
 
         :param request: Request instance for DeleteApiKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteApiKeyRequest`
@@ -485,15 +485,15 @@
             model = models.DeleteApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIPStrategy(self, request):
         """本接口（DeleteIPStrategy）用于删除服务IP策略。
 
         :param request: Request instance for DeleteIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteIPStrategyRequest`
@@ -508,15 +508,15 @@
             model = models.DeleteIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePlugin(self, request):
         """删除API网关插件
 
         :param request: Request instance for DeletePlugin.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeletePluginRequest`
@@ -531,15 +531,15 @@
             model = models.DeletePluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteService(self, request):
         """本接口（DeleteService）用于删除 API 网关中某个服务。
 
         :param request: Request instance for DeleteService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteServiceRequest`
@@ -554,15 +554,15 @@
             model = models.DeleteServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceSubDomainMapping(self, request):
         """本接口（DeleteServiceSubDomainMapping）用于删除服务中某个环境的自定义域名映射。
         当用户使用自定义域名，并使用了自定义映射时，可使用此接口。但需注意，若删除了所有环境的映射时，调用此 API 均会返回失败。
 
         :param request: Request instance for DeleteServiceSubDomainMapping.
@@ -578,15 +578,15 @@
             model = models.DeleteServiceSubDomainMappingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUpstream(self, request):
         """删除后端通道，需要注意有API绑定时，不允许删除
 
         :param request: Request instance for DeleteUpstream.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteUpstreamRequest`
@@ -601,15 +601,15 @@
             model = models.DeleteUpstreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUsagePlan(self, request):
         """本接口（DeleteUsagePlan）用于删除使用计划。
 
         :param request: Request instance for DeleteUsagePlan.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DeleteUsagePlanRequest`
@@ -624,15 +624,15 @@
             model = models.DeleteUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DemoteServiceUsagePlan(self, request):
         """本接口（DemoteServiceUsagePlan）用于将某个服务在某个环境的使用计划，降级到API上。
         如果服务内没有API不允许进行此操作。
         如果当前环境没有发布，不允许进行此操作。
 
@@ -649,15 +649,15 @@
             model = models.DemoteServiceUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAPIDocDetail(self, request):
         """查询 API 文档详情
 
         :param request: Request instance for DescribeAPIDocDetail.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeAPIDocDetailRequest`
@@ -672,15 +672,15 @@
             model = models.DescribeAPIDocDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAPIDocs(self, request):
         """查询 API 文档列表
 
         :param request: Request instance for DescribeAPIDocs.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeAPIDocsRequest`
@@ -695,15 +695,15 @@
             model = models.DescribeAPIDocsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllPluginApis(self, request):
         """展示插件相关的API列表，包括已绑定的和未绑定的API信息。
 
         :param request: Request instance for DescribeAllPluginApis.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeAllPluginApisRequest`
@@ -718,15 +718,15 @@
             model = models.DescribeAllPluginApisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApi(self, request):
         """本接口（DescribeApi）用于查询用户 API 网关的 API 接口的详细信息。​
 
         :param request: Request instance for DescribeApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiRequest`
@@ -741,15 +741,15 @@
             model = models.DescribeApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiApp(self, request):
         """本接口（DescribeApiApp）用于根据应用ID搜索应用。
 
         :param request: Request instance for DescribeApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiAppRequest`
@@ -764,15 +764,15 @@
             model = models.DescribeApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiAppBindApisStatus(self, request):
         """本接口（DescribeApiAppBindApisStatus）查询应用绑定的Api列表。
 
         :param request: Request instance for DescribeApiAppBindApisStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiAppBindApisStatusRequest`
@@ -787,15 +787,15 @@
             model = models.DescribeApiAppBindApisStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiAppsStatus(self, request):
         """本接口（DescribeApiAppsStatus）查询应用列表。
 
         :param request: Request instance for DescribeApiAppsStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiAppsStatusRequest`
@@ -810,15 +810,15 @@
             model = models.DescribeApiAppsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiBindApiAppsStatus(self, request):
         """本接口（DescribeApiBindApiAppsStatus）查询Api绑定的应用列表。
 
         :param request: Request instance for DescribeApiBindApiAppsStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiBindApiAppsStatusRequest`
@@ -833,15 +833,15 @@
             model = models.DescribeApiBindApiAppsStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiEnvironmentStrategy(self, request):
         """本接口（DescribeApiEnvironmentStrategy）用于展示API绑定的限流策略。
 
         :param request: Request instance for DescribeApiEnvironmentStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiEnvironmentStrategyRequest`
@@ -856,15 +856,15 @@
             model = models.DescribeApiEnvironmentStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiForApiApp(self, request):
         """本接口（DescribeApiForApiApp）用于应用使用者查询部署于 API 网关的 API 接口的详细信息。​
 
         :param request: Request instance for DescribeApiForApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApiForApiAppRequest`
@@ -879,15 +879,15 @@
             model = models.DescribeApiForApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiKey(self, request):
         """本接口（DescribeApiKey）用于查询密钥详情。
         用户在创建密钥后，可用此接口查询一个 API 密钥的详情，该接口会显示密钥 Key。
 
         :param request: Request instance for DescribeApiKey.
@@ -903,15 +903,15 @@
             model = models.DescribeApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiKeysStatus(self, request):
         """本接口（DescribeApiKeysStatus）用于查询密钥列表。
         当用户创建了多个密钥对时，可使用本接口查询一个或多个 API 密钥信息。
 
         :param request: Request instance for DescribeApiKeysStatus.
@@ -927,15 +927,15 @@
             model = models.DescribeApiKeysStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApiUsagePlan(self, request):
         """本接口（DescribeApiUsagePlan）用于查询服务中 API 使用计划详情。
         服务若需要鉴权限流生效，则需要绑定使用计划到此服务中，本接口用于查询绑定到一个服务及其中 API 的所有使用计划。
 
         :param request: Request instance for DescribeApiUsagePlan.
@@ -951,15 +951,15 @@
             model = models.DescribeApiUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApisStatus(self, request):
         """本接口（DescribeApisStatus）用于查看一个服务下的某个 API 或所有 API 列表及其相关信息。
 
         :param request: Request instance for DescribeApisStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeApisStatusRequest`
@@ -974,15 +974,15 @@
             model = models.DescribeApisStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExclusiveInstanceDetail(self, request):
         """本接口（DescribeExclusiveInstanceDetail）用于查询独享实例详情信息。
 
         :param request: Request instance for DescribeExclusiveInstanceDetail.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstanceDetailRequest`
@@ -997,15 +997,15 @@
             model = models.DescribeExclusiveInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExclusiveInstances(self, request):
         """本接口（DescribeExclusiveInstances）用于查询独享实例列表信息。
 
         :param request: Request instance for DescribeExclusiveInstances.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstancesRequest`
@@ -1020,15 +1020,15 @@
             model = models.DescribeExclusiveInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExclusiveInstancesStatus(self, request):
         """查询专享实例列表（新）
 
         :param request: Request instance for DescribeExclusiveInstancesStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeExclusiveInstancesStatusRequest`
@@ -1043,15 +1043,15 @@
             model = models.DescribeExclusiveInstancesStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIPStrategy(self, request):
         """本接口（DescribeIPStrategy）用于查询IP策略详情。
 
         :param request: Request instance for DescribeIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeIPStrategyRequest`
@@ -1066,15 +1066,15 @@
             model = models.DescribeIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIPStrategyApisStatus(self, request):
         """本接口（DescribeIPStrategyApisStatus）用于查询IP策略可以绑定的API列表。即服务下所有API和该策略已绑定API的差集。
 
         :param request: Request instance for DescribeIPStrategyApisStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeIPStrategyApisStatusRequest`
@@ -1089,15 +1089,15 @@
             model = models.DescribeIPStrategyApisStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIPStrategysStatus(self, request):
         """本接口（DescribeIPStrategysStatus）用于查询服务IP策略列表，因为接口名拼写错误，已不推荐使用，请优先使用DescribeIPStrategiesStatus接口。
 
         :param request: Request instance for DescribeIPStrategysStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeIPStrategysStatusRequest`
@@ -1112,15 +1112,15 @@
             model = models.DescribeIPStrategysStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogSearch(self, request):
         """本接口DescribeLogSearch用于搜索日志
 
         :param request: Request instance for DescribeLogSearch.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeLogSearchRequest`
@@ -1135,15 +1135,15 @@
             model = models.DescribeLogSearchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlugin(self, request):
         """展示插件详情，支持按照插件ID进行。
 
         :param request: Request instance for DescribePlugin.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribePluginRequest`
@@ -1158,15 +1158,15 @@
             model = models.DescribePluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePluginApis(self, request):
         """查询指定插件下绑定的API信息
 
         :param request: Request instance for DescribePluginApis.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribePluginApisRequest`
@@ -1181,15 +1181,15 @@
             model = models.DescribePluginApisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlugins(self, request):
         """展示插件列表和详情，支持分页，支持按照插件类型查询，支持按照插件ID批量查询，支持按照插件名称查询。
 
         :param request: Request instance for DescribePlugins.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribePluginsRequest`
@@ -1204,15 +1204,15 @@
             model = models.DescribePluginsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePluginsByApi(self, request):
         """展示API上已绑定的插件列表。
 
         :param request: Request instance for DescribePluginsByApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribePluginsByApiRequest`
@@ -1227,15 +1227,15 @@
             model = models.DescribePluginsByApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeService(self, request):
         """本接口（DescribeService）用于查询一个服务的详细信息、包括服务的描述、域名、协议、创建时间、发布情况等信息。
 
         :param request: Request instance for DescribeService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeServiceRequest`
@@ -1250,15 +1250,15 @@
             model = models.DescribeServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceEnvironmentList(self, request):
         """本接口（DescribeServiceEnvironmentList）用于查询一个服务的环境列表，可查询到此服务下所有环境及其状态。
 
         :param request: Request instance for DescribeServiceEnvironmentList.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeServiceEnvironmentListRequest`
@@ -1273,15 +1273,15 @@
             model = models.DescribeServiceEnvironmentListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceEnvironmentReleaseHistory(self, request):
         """本接口（DescribeServiceEnvironmentReleaseHistory）用于查询服务环境的发布历史。
         用户在创建好服务后需要发布到某个环境中才能进行使用，本接口用于查询一个服务某个环境的发布记录。
 
         :param request: Request instance for DescribeServiceEnvironmentReleaseHistory.
@@ -1297,15 +1297,15 @@
             model = models.DescribeServiceEnvironmentReleaseHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceEnvironmentStrategy(self, request):
         """本接口（DescribeServiceEnvironmentStrategy）用于展示服务限流策略。
 
         :param request: Request instance for DescribeServiceEnvironmentStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeServiceEnvironmentStrategyRequest`
@@ -1320,15 +1320,15 @@
             model = models.DescribeServiceEnvironmentStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceForApiApp(self, request):
         """本接口（DescribeServiceForApiApp）用于应用使用者查询一个服务的详细信息、包括服务的描述、域名、协议等信息。
 
         :param request: Request instance for DescribeServiceForApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeServiceForApiAppRequest`
@@ -1343,15 +1343,15 @@
             model = models.DescribeServiceForApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceReleaseVersion(self, request):
         """本接口（DescribeServiceReleaseVersion）查询一个服务下面所有已经发布的版本列表。
         用户在发布服务时，常有多个版本发布，可使用本接口查询已发布的版本。
 
         :param request: Request instance for DescribeServiceReleaseVersion.
@@ -1367,15 +1367,15 @@
             model = models.DescribeServiceReleaseVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceSubDomainMappings(self, request):
         """本接口（DescribeServiceSubDomainMappings）用于查询自定义域名的路径映射。
         API 网关可绑定自定义域名到服务，并且可以对自定义域名的路径进行映射，可自定义不同的路径映射到服务中的三个环境，本接口用于查询绑定服务的自定义域名的路径映射列表。
 
         :param request: Request instance for DescribeServiceSubDomainMappings.
@@ -1391,15 +1391,15 @@
             model = models.DescribeServiceSubDomainMappingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceSubDomains(self, request):
         """本接口（DescribeServiceSubDomains）用于查询自定义域名列表。
         API 网关可绑定自定义域名到服务，用于服务调用。此接口用于查询用户绑定在服务的自定义域名列表。
 
         :param request: Request instance for DescribeServiceSubDomains.
@@ -1415,15 +1415,15 @@
             model = models.DescribeServiceSubDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceUsagePlan(self, request):
         """本接口（DescribeServiceUsagePlan）用于查询服务使用计划详情。
         服务若需要鉴权限流生效，则需要绑定使用计划到此服务中，本接口用于查询绑定到一个服务的所有使用计划。
 
         :param request: Request instance for DescribeServiceUsagePlan.
@@ -1439,15 +1439,15 @@
             model = models.DescribeServiceUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServicesStatus(self, request):
         """本接口（DescribeServicesStatus）用于搜索查询某一个服务或多个服务的列表，并返回服务相关的域名、时间等信息。
 
         :param request: Request instance for DescribeServicesStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeServicesStatusRequest`
@@ -1462,15 +1462,15 @@
             model = models.DescribeServicesStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUpstreamBindApis(self, request):
         """查询后端通道所绑定的API列表
 
         :param request: Request instance for DescribeUpstreamBindApis.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeUpstreamBindApisRequest`
@@ -1485,15 +1485,15 @@
             model = models.DescribeUpstreamBindApisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUpstreams(self, request):
         """查询后端通道列表详情
 
         :param request: Request instance for DescribeUpstreams.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeUpstreamsRequest`
@@ -1508,15 +1508,15 @@
             model = models.DescribeUpstreamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsagePlan(self, request):
         """本接口（DescribeUsagePlan）用于查询一个使用计划的详细信息，包括名称、QPS、创建时间绑定的环境等。
 
         :param request: Request instance for DescribeUsagePlan.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeUsagePlanRequest`
@@ -1531,15 +1531,15 @@
             model = models.DescribeUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsagePlanEnvironments(self, request):
         """本接口（DescribeUsagePlanEnvironments）用于查询使用计划绑定的环境列表。
         用户在绑定了某个使用计划到环境后，可使用本接口查询这个使用计划绑定的所有服务的环境。
 
         :param request: Request instance for DescribeUsagePlanEnvironments.
@@ -1555,15 +1555,15 @@
             model = models.DescribeUsagePlanEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsagePlanSecretIds(self, request):
         """本接口（DescribeUsagePlanSecretIds）用于查询使用计划绑定的密钥列表。
         在 API 网关中，一个使用计划可绑定多个密钥对，可使用本接口查询使用计划绑定的密钥列表。
 
         :param request: Request instance for DescribeUsagePlanSecretIds.
@@ -1579,15 +1579,15 @@
             model = models.DescribeUsagePlanSecretIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsagePlansStatus(self, request):
         """本接口（DescribeUsagePlanStatus）用于查询使用计划的列表。
 
         :param request: Request instance for DescribeUsagePlansStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeUsagePlansStatusRequest`
@@ -1602,15 +1602,15 @@
             model = models.DescribeUsagePlansStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachPlugin(self, request):
         """解除插件与API绑定
 
         :param request: Request instance for DetachPlugin.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DetachPluginRequest`
@@ -1625,15 +1625,15 @@
             model = models.DetachPluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableApiKey(self, request):
         """本接口（DisableApiKey）用于禁用一对 API 密钥。
 
         :param request: Request instance for DisableApiKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DisableApiKeyRequest`
@@ -1648,15 +1648,15 @@
             model = models.DisableApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableApiKey(self, request):
         """本接口（EnableApiKey）用于启动一对被禁用的 API 密钥。
 
         :param request: Request instance for EnableApiKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.EnableApiKeyRequest`
@@ -1671,15 +1671,15 @@
             model = models.EnableApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GenerateApiDocument(self, request):
         """接口已废弃
 
         本接口（GenerateApiDocument）用于自动生成 API 文档和 SDK，一个服务的一个环境生成一份文档和 SDK。
 
@@ -1696,15 +1696,15 @@
             model = models.GenerateApiDocumentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportOpenApi(self, request):
         """本接口（ImportOpenApi）用于将OpenAPI规范定义的API导入到API网关。
 
         :param request: Request instance for ImportOpenApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ImportOpenApiRequest`
@@ -1719,15 +1719,15 @@
             model = models.ImportOpenApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAPIDoc(self, request):
         """修改 API 文档
 
         :param request: Request instance for ModifyAPIDoc.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyAPIDocRequest`
@@ -1742,15 +1742,15 @@
             model = models.ModifyAPIDocResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApi(self, request):
         """本接口（ModifyApi）用于修改 API 接口，可调用此接口对已经配置的 API 接口进行编辑修改。修改后的 API 需要重新发布 API 所在的服务到对应环境方能生效。
 
         :param request: Request instance for ModifyApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyApiRequest`
@@ -1765,15 +1765,15 @@
             model = models.ModifyApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApiApp(self, request):
         """本接口（ModifyApiApp）用于修改已经创建的应用。
 
         :param request: Request instance for ModifyApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyApiAppRequest`
@@ -1788,15 +1788,15 @@
             model = models.ModifyApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApiEnvironmentStrategy(self, request):
         """本接口（ModifyApiEnvironmentStrategy）用于修改API限流策略
 
         :param request: Request instance for ModifyApiEnvironmentStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyApiEnvironmentStrategyRequest`
@@ -1811,15 +1811,15 @@
             model = models.ModifyApiEnvironmentStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApiIncrement(self, request):
         """提供增量更新API能力，主要是给程序调用（区别于ModifyApi，该接口是需要传入API的全量参数，对console使用较友好）
 
         :param request: Request instance for ModifyApiIncrement.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyApiIncrementRequest`
@@ -1834,15 +1834,15 @@
             model = models.ModifyApiIncrementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyExclusiveInstance(self, request):
         """本接口（ModifyExclusiveInstance）用于修改独享实例信息。​
 
         :param request: Request instance for ModifyExclusiveInstance.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyExclusiveInstanceRequest`
@@ -1857,15 +1857,15 @@
             model = models.ModifyExclusiveInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIPStrategy(self, request):
         """本接口（ModifyIPStrategy）用于修改服务IP策略。
 
         :param request: Request instance for ModifyIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyIPStrategyRequest`
@@ -1880,15 +1880,15 @@
             model = models.ModifyIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPlugin(self, request):
         """修改API网关插件。
 
         :param request: Request instance for ModifyPlugin.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyPluginRequest`
@@ -1903,15 +1903,15 @@
             model = models.ModifyPluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyService(self, request):
         """本接口（ModifyService）用于修改服务的相关信息。当服务创建后，服务的名称、描述和服务类型均可被修改。
 
         :param request: Request instance for ModifyService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyServiceRequest`
@@ -1926,15 +1926,15 @@
             model = models.ModifyServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyServiceEnvironmentStrategy(self, request):
         """本接口（ModifyServiceEnvironmentStrategy）用于修改服务限流策略
 
         :param request: Request instance for ModifyServiceEnvironmentStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyServiceEnvironmentStrategyRequest`
@@ -1949,15 +1949,15 @@
             model = models.ModifyServiceEnvironmentStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubDomain(self, request):
         """本接口（ModifySubDomain）用于修改服务的自定义域名设置中的路径映射，可以修改绑定自定义域名之前的路径映射规则。
 
         :param request: Request instance for ModifySubDomain.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifySubDomainRequest`
@@ -1972,15 +1972,15 @@
             model = models.ModifySubDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUpstream(self, request):
         """修改后端通道
 
         :param request: Request instance for ModifyUpstream.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyUpstreamRequest`
@@ -1995,15 +1995,15 @@
             model = models.ModifyUpstreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUsagePlan(self, request):
         """本接口（ModifyUsagePlan）用于修改使用计划的名称，描述及 QPS。
 
         :param request: Request instance for ModifyUsagePlan.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ModifyUsagePlanRequest`
@@ -2018,15 +2018,15 @@
             model = models.ModifyUsagePlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseService(self, request):
         """本接口（ReleaseService）用于发布服务。
         API 网关的服务创建后，需要发布到某个环境方生效后，使用者才能进行调用，此接口用于发布服务到环境，如 release 环境。
 
         :param request: Request instance for ReleaseService.
@@ -2042,15 +2042,15 @@
             model = models.ReleaseServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAPIDocPassword(self, request):
         """重置API文档密码
 
         :param request: Request instance for ResetAPIDocPassword.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ResetAPIDocPasswordRequest`
@@ -2065,15 +2065,15 @@
             model = models.ResetAPIDocPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindEnvironment(self, request):
         """本接口（UnBindEnvironment）用于将使用计划从特定环境解绑。
 
         :param request: Request instance for UnBindEnvironment.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UnBindEnvironmentRequest`
@@ -2088,15 +2088,15 @@
             model = models.UnBindEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindIPStrategy(self, request):
         """本接口（UnBindIPStrategy）用于服务解绑IP策略。
 
         :param request: Request instance for UnBindIPStrategy.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UnBindIPStrategyRequest`
@@ -2111,15 +2111,15 @@
             model = models.UnBindIPStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindSecretIds(self, request):
         """本接口（UnBindSecretIds）用于为使用计划解绑密钥。
 
         :param request: Request instance for UnBindSecretIds.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UnBindSecretIdsRequest`
@@ -2134,15 +2134,15 @@
             model = models.UnBindSecretIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindSubDomain(self, request):
         """本接口（UnBindSubDomain）用于解绑自定义域名。
         用户使用 API 网关绑定了自定义域名到服务中后，若想要解绑此自定义域名，可使用此接口。
 
         :param request: Request instance for UnBindSubDomain.
@@ -2158,15 +2158,15 @@
             model = models.UnBindSubDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnReleaseService(self, request):
         """本接口（UnReleaseService）用于下线服务。
         用户发布服务到某个环境后，此服务中的 API 方可被调用者进行调用，当用户需要将此服务从发布环境中下线时，可调用此 API。下线后的服务不可被调用。
 
         :param request: Request instance for UnReleaseService.
@@ -2182,15 +2182,15 @@
             model = models.UnReleaseServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindApiApp(self, request):
         """本接口（UnbindApiApp）用于解除应用和API绑定。
 
         :param request: Request instance for UnbindApiApp.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UnbindApiAppRequest`
@@ -2205,15 +2205,15 @@
             model = models.UnbindApiAppResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiAppKey(self, request):
         """本接口（UpdateApiAppKey）用于更新应用密钥。
 
         :param request: Request instance for UpdateApiAppKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UpdateApiAppKeyRequest`
@@ -2228,15 +2228,15 @@
             model = models.UpdateApiAppKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApiKey(self, request):
         """本接口（UpdateApiKey）用于更换用户已创建的一对 API 密钥。
 
         :param request: Request instance for UpdateApiKey.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UpdateApiKeyRequest`
@@ -2251,15 +2251,15 @@
             model = models.UpdateApiKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateService(self, request):
         """本接口（UpdateService）用于从服务已发布的环境中将运行版本切换到特定版本。用户在使用 API 网关创建服务并发布服务到某个环境后，如在开发过程产生多个版本需要切换，此时可调用本接口。
 
         :param request: Request instance for UpdateService.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.UpdateServiceRequest`
@@ -2274,8 +2274,8 @@
             model = models.UpdateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.938/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.937/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.938/README.rst`

 * *Files identical despite different names*

