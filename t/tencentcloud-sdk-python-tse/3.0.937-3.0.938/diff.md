# Comparing `tmp/tencentcloud-sdk-python-tse-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tse-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tse-3.0.937.tar", last modified: Tue Jul 18 00:34:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tse-3.0.938.tar", last modified: Wed Jul 19 00:52:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tse-3.0.937.tar` & `tencentcloud-sdk-python-tse-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/
--rw-r--r--   0 root         (0) root         (0)    31417 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/tse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4625 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   210902 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:18.000000 tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/
+-rw-r--r--   0 root         (0) root         (0)    32536 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/tse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   216107 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:52:53.000000 tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tse-3.0.937/setup.py` & `tencentcloud-sdk-python-tse-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tse-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tse-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/tse_client.py` & `tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/tse_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCloudNativeAPIGatewayCanaryRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudNativeAPIGatewayRoute(self, request):
         """创建云原生网关路由
 
         :param request: Request instance for CreateCloudNativeAPIGatewayRoute.
         :type request: :class:`tencentcloud.tse.v20201207.models.CreateCloudNativeAPIGatewayRouteRequest`
@@ -65,15 +65,15 @@
             model = models.CreateCloudNativeAPIGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudNativeAPIGatewayRouteRateLimit(self, request):
         """创建云原生网关限流插件(路由)
 
         :param request: Request instance for CreateCloudNativeAPIGatewayRouteRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.CreateCloudNativeAPIGatewayRouteRateLimitRequest`
@@ -88,15 +88,15 @@
             model = models.CreateCloudNativeAPIGatewayRouteRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudNativeAPIGatewayService(self, request):
         """创建云原生网关服务
 
         :param request: Request instance for CreateCloudNativeAPIGatewayService.
         :type request: :class:`tencentcloud.tse.v20201207.models.CreateCloudNativeAPIGatewayServiceRequest`
@@ -111,15 +111,15 @@
             model = models.CreateCloudNativeAPIGatewayServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudNativeAPIGatewayServiceRateLimit(self, request):
         """创建云原生网关限流插件(服务)
 
         :param request: Request instance for CreateCloudNativeAPIGatewayServiceRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.CreateCloudNativeAPIGatewayServiceRateLimitRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCloudNativeAPIGatewayServiceRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEngine(self, request):
         """创建引擎实例
 
         :param request: Request instance for CreateEngine.
         :type request: :class:`tencentcloud.tse.v20201207.models.CreateEngineRequest`
@@ -157,15 +157,15 @@
             model = models.CreateEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudNativeAPIGatewayCanaryRule(self, request):
         """删除云原生网关的灰度规则
 
         :param request: Request instance for DeleteCloudNativeAPIGatewayCanaryRule.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteCloudNativeAPIGatewayCanaryRuleRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteCloudNativeAPIGatewayCanaryRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudNativeAPIGatewayRoute(self, request):
         """删除云原生网关路由
 
         :param request: Request instance for DeleteCloudNativeAPIGatewayRoute.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteCloudNativeAPIGatewayRouteRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteCloudNativeAPIGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudNativeAPIGatewayRouteRateLimit(self, request):
         """删除云原生网关的限流插件(路由)
 
         :param request: Request instance for DeleteCloudNativeAPIGatewayRouteRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteCloudNativeAPIGatewayRouteRateLimitRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteCloudNativeAPIGatewayRouteRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudNativeAPIGatewayService(self, request):
         """删除云原生网关服务
 
         :param request: Request instance for DeleteCloudNativeAPIGatewayService.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteCloudNativeAPIGatewayServiceRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteCloudNativeAPIGatewayServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCloudNativeAPIGatewayServiceRateLimit(self, request):
         """删除云原生网关的限流插件(服务)
 
         :param request: Request instance for DeleteCloudNativeAPIGatewayServiceRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteCloudNativeAPIGatewayServiceRateLimitRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteCloudNativeAPIGatewayServiceRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEngine(self, request):
         """删除引擎实例
 
         :param request: Request instance for DeleteEngine.
         :type request: :class:`tencentcloud.tse.v20201207.models.DeleteEngineRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayCanaryRules(self, request):
         """查询云原生网关灰度规则列表
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayCanaryRules.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayCanaryRulesRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeCloudNativeAPIGatewayCanaryRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayNodes(self, request):
         """获取云原生网关节点列表
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayNodes.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayNodesRequest`
@@ -341,15 +341,38 @@
             model = models.DescribeCloudNativeAPIGatewayNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeCloudNativeAPIGatewayPorts(self, request):
+        """获取云原生API网关实例端口信息
+
+        :param request: Request instance for DescribeCloudNativeAPIGatewayPorts.
+        :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayPortsRequest`
+        :rtype: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayPortsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCloudNativeAPIGatewayPorts", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCloudNativeAPIGatewayPortsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayRouteRateLimit(self, request):
         """查询云原生网关的限流插件(路由)
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayRouteRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayRouteRateLimitRequest`
@@ -364,15 +387,15 @@
             model = models.DescribeCloudNativeAPIGatewayRouteRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayRoutes(self, request):
         """查询云原生网关路由列表
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayRoutes.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayRoutesRequest`
@@ -387,15 +410,15 @@
             model = models.DescribeCloudNativeAPIGatewayRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayServiceRateLimit(self, request):
         """查询云原生网关的限流插件(服务)
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayServiceRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayServiceRateLimitRequest`
@@ -410,15 +433,15 @@
             model = models.DescribeCloudNativeAPIGatewayServiceRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudNativeAPIGatewayServices(self, request):
         """查询云原生网关服务列表
 
         :param request: Request instance for DescribeCloudNativeAPIGatewayServices.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeCloudNativeAPIGatewayServicesRequest`
@@ -433,15 +456,15 @@
             model = models.DescribeCloudNativeAPIGatewayServicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNacosReplicas(self, request):
         """查询Nacos类型引擎实例副本信息
 
         :param request: Request instance for DescribeNacosReplicas.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeNacosReplicasRequest`
@@ -456,15 +479,15 @@
             model = models.DescribeNacosReplicasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNacosServerInterfaces(self, request):
         """查询nacos服务接口列表
 
         :param request: Request instance for DescribeNacosServerInterfaces.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeNacosServerInterfacesRequest`
@@ -479,15 +502,15 @@
             model = models.DescribeNacosServerInterfacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOneCloudNativeAPIGatewayService(self, request):
         """获取云原生网关服务详情
 
         :param request: Request instance for DescribeOneCloudNativeAPIGatewayService.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeOneCloudNativeAPIGatewayServiceRequest`
@@ -502,15 +525,15 @@
             model = models.DescribeOneCloudNativeAPIGatewayServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSREInstanceAccessAddress(self, request):
         """查询引擎实例访问地址
 
         :param request: Request instance for DescribeSREInstanceAccessAddress.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeSREInstanceAccessAddressRequest`
@@ -525,15 +548,15 @@
             model = models.DescribeSREInstanceAccessAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSREInstances(self, request):
         """用于查询引擎实例列表
 
         :param request: Request instance for DescribeSREInstances.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeSREInstancesRequest`
@@ -548,15 +571,15 @@
             model = models.DescribeSREInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZookeeperReplicas(self, request):
         """查询Zookeeper类型注册引擎实例副本信息
 
         :param request: Request instance for DescribeZookeeperReplicas.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeZookeeperReplicasRequest`
@@ -571,15 +594,15 @@
             model = models.DescribeZookeeperReplicasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZookeeperServerInterfaces(self, request):
         """查询zookeeper服务接口列表
 
         :param request: Request instance for DescribeZookeeperServerInterfaces.
         :type request: :class:`tencentcloud.tse.v20201207.models.DescribeZookeeperServerInterfacesRequest`
@@ -594,15 +617,15 @@
             model = models.DescribeZookeeperServerInterfacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudNativeAPIGatewayCanaryRule(self, request):
         """修改云原生网关的灰度规则
 
         :param request: Request instance for ModifyCloudNativeAPIGatewayCanaryRule.
         :type request: :class:`tencentcloud.tse.v20201207.models.ModifyCloudNativeAPIGatewayCanaryRuleRequest`
@@ -617,15 +640,15 @@
             model = models.ModifyCloudNativeAPIGatewayCanaryRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudNativeAPIGatewayRoute(self, request):
         """修改云原生网关路由
 
         :param request: Request instance for ModifyCloudNativeAPIGatewayRoute.
         :type request: :class:`tencentcloud.tse.v20201207.models.ModifyCloudNativeAPIGatewayRouteRequest`
@@ -640,15 +663,15 @@
             model = models.ModifyCloudNativeAPIGatewayRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudNativeAPIGatewayRouteRateLimit(self, request):
         """修改云原生网关限流插件(路由)
 
         :param request: Request instance for ModifyCloudNativeAPIGatewayRouteRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.ModifyCloudNativeAPIGatewayRouteRateLimitRequest`
@@ -663,15 +686,15 @@
             model = models.ModifyCloudNativeAPIGatewayRouteRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudNativeAPIGatewayService(self, request):
         """修改云原生网关服务
 
         :param request: Request instance for ModifyCloudNativeAPIGatewayService.
         :type request: :class:`tencentcloud.tse.v20201207.models.ModifyCloudNativeAPIGatewayServiceRequest`
@@ -686,15 +709,15 @@
             model = models.ModifyCloudNativeAPIGatewayServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCloudNativeAPIGatewayServiceRateLimit(self, request):
         """修改云原生网关限流插件(服务)
 
         :param request: Request instance for ModifyCloudNativeAPIGatewayServiceRateLimit.
         :type request: :class:`tencentcloud.tse.v20201207.models.ModifyCloudNativeAPIGatewayServiceRateLimitRequest`
@@ -709,15 +732,15 @@
             model = models.ModifyCloudNativeAPIGatewayServiceRateLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEngineInternetAccess(self, request):
         """修改引擎公网访问配置
 
         :param request: Request instance for UpdateEngineInternetAccess.
         :type request: :class:`tencentcloud.tse.v20201207.models.UpdateEngineInternetAccessRequest`
@@ -732,8 +755,8 @@
             model = models.UpdateEngineInternetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/errorcodes.py` & `tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tse-3.0.937/tencentcloud/tse/v20201207/models.py` & `tencentcloud-sdk-python-tse-3.0.938/tencentcloud/tse/v20201207/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2484,14 +2484,87 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeCloudNativeAPIGatewayPortsRequest(AbstractModel):
+    """DescribeCloudNativeAPIGatewayPorts请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _GatewayId: 云原生API网关实例ID
+        :type GatewayId: str
+        """
+        self._GatewayId = None
+
+    @property
+    def GatewayId(self):
+        return self._GatewayId
+
+    @GatewayId.setter
+    def GatewayId(self, GatewayId):
+        self._GatewayId = GatewayId
+
+
+    def _deserialize(self, params):
+        self._GatewayId = params.get("GatewayId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeCloudNativeAPIGatewayPortsResponse(AbstractModel):
+    """DescribeCloudNativeAPIGatewayPorts返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Result: 云原生API网关实例协议端口列表响应结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: :class:`tencentcloud.tse.v20201207.models.DescribeGatewayInstancePortResult`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Result = None
+        self._RequestId = None
+
+    @property
+    def Result(self):
+        return self._Result
+
+    @Result.setter
+    def Result(self, Result):
+        self._Result = Result
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self._Result = DescribeGatewayInstancePortResult()
+            self._Result._deserialize(params.get("Result"))
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeCloudNativeAPIGatewayRouteRateLimitRequest(AbstractModel):
     """DescribeCloudNativeAPIGatewayRouteRateLimit请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2905,14 +2978,66 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self._Result = KongServices()
             self._Result._deserialize(params.get("Result"))
         self._RequestId = params.get("RequestId")
 
 
+class DescribeGatewayInstancePortResult(AbstractModel):
+    """获取云原生API网关实例协议端口列表响应结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _GatewayId: 云原生API网关ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayId: str
+        :param _GatewayInstancePortList: 网关实例协议端口列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayInstancePortList: list of GatewayInstanceSchemeAndPorts
+        """
+        self._GatewayId = None
+        self._GatewayInstancePortList = None
+
+    @property
+    def GatewayId(self):
+        return self._GatewayId
+
+    @GatewayId.setter
+    def GatewayId(self, GatewayId):
+        self._GatewayId = GatewayId
+
+    @property
+    def GatewayInstancePortList(self):
+        return self._GatewayInstancePortList
+
+    @GatewayInstancePortList.setter
+    def GatewayInstancePortList(self, GatewayInstancePortList):
+        self._GatewayInstancePortList = GatewayInstancePortList
+
+
+    def _deserialize(self, params):
+        self._GatewayId = params.get("GatewayId")
+        if params.get("GatewayInstancePortList") is not None:
+            self._GatewayInstancePortList = []
+            for item in params.get("GatewayInstancePortList"):
+                obj = GatewayInstanceSchemeAndPorts()
+                obj._deserialize(item)
+                self._GatewayInstancePortList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeInstanceRegionInfo(AbstractModel):
     """实例地域信息描述
 
     """
 
     def __init__(self):
         r"""
@@ -4420,14 +4545,61 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GatewayInstanceSchemeAndPorts(AbstractModel):
+    """网关实例协议端口列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Scheme: 端口协议，可选HTTP、HTTPS、TCP和UDP
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Scheme: str
+        :param _PortList: 端口列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PortList: list of int non-negative
+        """
+        self._Scheme = None
+        self._PortList = None
+
+    @property
+    def Scheme(self):
+        return self._Scheme
+
+    @Scheme.setter
+    def Scheme(self, Scheme):
+        self._Scheme = Scheme
+
+    @property
+    def PortList(self):
+        return self._PortList
+
+    @PortList.setter
+    def PortList(self, PortList):
+        self._PortList = PortList
+
+
+    def _deserialize(self, params):
+        self._Scheme = params.get("Scheme")
+        self._PortList = params.get("PortList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class InstanceTagInfo(AbstractModel):
     """引擎实例的标签信息
 
     """
```

### Comparing `tencentcloud-sdk-python-tse-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tse-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tse-3.0.937/README.rst` & `tencentcloud-sdk-python-tse-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tse-3.0.937/tencentcloud_sdk_python_tse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tse-3.0.938/tencentcloud_sdk_python_tse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

