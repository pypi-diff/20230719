# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.937.tar", last modified: Tue Jul 18 00:32:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.938.tar", last modified: Wed Jul 19 00:50:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.937.tar` & `tencentcloud-sdk-python-teo-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60328 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    23798 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   605318 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60588 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    23798 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605318 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:15.000000 tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-teo-3.0.937/setup.py` & `tencentcloud-sdk-python-teo-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/teo_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindZoneToPlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckCnameStatus(self, request):
         """校验域名 CNAME 状态
 
         :param request: Request instance for CheckCnameStatus.
         :type request: :class:`tencentcloud.teo.v20220901.models.CheckCnameStatusRequest`
@@ -65,15 +65,15 @@
             model = models.CheckCnameStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccelerationDomain(self, request):
         """创建加速域名
 
         :param request: Request instance for CreateAccelerationDomain.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateAccelerationDomainRequest`
@@ -88,15 +88,15 @@
             model = models.CreateAccelerationDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAliasDomain(self, request):
         """创建别称域名。
 
         :param request: Request instance for CreateAliasDomain.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateAliasDomainRequest`
@@ -111,15 +111,15 @@
             model = models.CreateAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationProxy(self, request):
         """创建应用代理
 
         :param request: Request instance for CreateApplicationProxy.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyRequest`
@@ -134,15 +134,15 @@
             model = models.CreateApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationProxyRule(self, request):
         """创建应用代理规则
 
         :param request: Request instance for CreateApplicationProxyRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateApplicationProxyRuleRequest`
@@ -157,15 +157,15 @@
             model = models.CreateApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOriginGroup(self, request):
         """创建源站组
 
         :param request: Request instance for CreateOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateOriginGroupRequest`
@@ -180,15 +180,15 @@
             model = models.CreateOriginGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePlanForZone(self, request):
         """为未购买套餐的站点购买套餐
 
         :param request: Request instance for CreatePlanForZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreatePlanForZoneRequest`
@@ -203,15 +203,15 @@
             model = models.CreatePlanForZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrefetchTask(self, request):
         """创建预热任务
 
         :param request: Request instance for CreatePrefetchTask.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreatePrefetchTaskRequest`
@@ -226,15 +226,15 @@
             model = models.CreatePrefetchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePurgeTask(self, request):
         """当源站资源更新，但节点缓存 TTL 未过期时，用户仍会访问到旧的资源，此时可以通过该接口实现节点资源更新。触发更新的方法有以下两种：<li>直接删除：不做任何校验，直接删除节点缓存，用户请求时触发回源拉取；</li><li>标记过期：将节点资源置为过期，用户请求时触发回源校验，即发送带有 If-None-Match 和 If-Modified-Since 头部的 HTTP 条件请求。若源站响应 200，则节点会回源拉取新的资源并更新缓存；若源站响应 304，则节点不会更新缓存；</li>
 
         清除缓存任务详情请查看[清除缓存](https://cloud.tencent.com/document/product/1552/70759)。</li>
 
@@ -251,15 +251,15 @@
             model = models.CreatePurgeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRule(self, request):
         """规则引擎创建规则。
 
         :param request: Request instance for CreateRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateRuleRequest`
@@ -274,15 +274,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityIPGroup(self, request):
         """创建安全 IP 组
 
         :param request: Request instance for CreateSecurityIPGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateSecurityIPGroupRequest`
@@ -297,15 +297,15 @@
             model = models.CreateSecurityIPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateZone(self, request):
         """用于用户接入新的站点。
 
         :param request: Request instance for CreateZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.CreateZoneRequest`
@@ -320,15 +320,15 @@
             model = models.CreateZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccelerationDomains(self, request):
         """批量删除加速域名
 
         :param request: Request instance for DeleteAccelerationDomains.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteAccelerationDomainsRequest`
@@ -343,15 +343,15 @@
             model = models.DeleteAccelerationDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAliasDomain(self, request):
         """删除别称域名。
 
         :param request: Request instance for DeleteAliasDomain.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteAliasDomainRequest`
@@ -366,15 +366,15 @@
             model = models.DeleteAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplicationProxy(self, request):
         """删除应用代理
 
         :param request: Request instance for DeleteApplicationProxy.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyRequest`
@@ -389,15 +389,15 @@
             model = models.DeleteApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplicationProxyRule(self, request):
         """删除应用代理规则
 
         :param request: Request instance for DeleteApplicationProxyRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteApplicationProxyRuleRequest`
@@ -412,15 +412,15 @@
             model = models.DeleteApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteOriginGroup(self, request):
         """删除源站组
 
         :param request: Request instance for DeleteOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteOriginGroupRequest`
@@ -435,15 +435,15 @@
             model = models.DeleteOriginGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRules(self, request):
         """批量删除规则引擎规则。
 
         :param request: Request instance for DeleteRules.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteRulesRequest`
@@ -458,15 +458,15 @@
             model = models.DeleteRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityIPGroup(self, request):
         """删除指定 IP 组，如果有规则引用了 IP 组情况，则不允许删除。
 
         :param request: Request instance for DeleteSecurityIPGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteSecurityIPGroupRequest`
@@ -481,15 +481,15 @@
             model = models.DeleteSecurityIPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteZone(self, request):
         """删除站点。
 
         :param request: Request instance for DeleteZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.DeleteZoneRequest`
@@ -504,15 +504,15 @@
             model = models.DeleteZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccelerationDomains(self, request):
         """查询加速域名列表，支持搜索、分页、排序、过滤。
 
         :param request: Request instance for DescribeAccelerationDomains.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAccelerationDomainsRequest`
@@ -527,15 +527,15 @@
             model = models.DescribeAccelerationDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAliasDomains(self, request):
         """查询别称域名信息列表。
 
         :param request: Request instance for DescribeAliasDomains.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAliasDomainsRequest`
@@ -550,15 +550,15 @@
             model = models.DescribeAliasDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationProxies(self, request):
         """查询应用代理列表。
 
         :param request: Request instance for DescribeApplicationProxies.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeApplicationProxiesRequest`
@@ -573,15 +573,15 @@
             model = models.DescribeApplicationProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailablePlans(self, request):
         """查询当前账户可用套餐信息列表
 
         :param request: Request instance for DescribeAvailablePlans.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeAvailablePlansRequest`
@@ -596,15 +596,15 @@
             model = models.DescribeAvailablePlansResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContentQuota(self, request):
         """查询内容管理接口配额
 
         :param request: Request instance for DescribeContentQuota.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeContentQuotaRequest`
@@ -619,15 +619,15 @@
             model = models.DescribeContentQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAttackData(self, request):
         """本接口（DescribeDDoSAttackData）用于查询DDoS攻击时序数据。
 
         :param request: Request instance for DescribeDDoSAttackData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackDataRequest`
@@ -642,15 +642,15 @@
             model = models.DescribeDDoSAttackDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAttackEvent(self, request):
         """本接口（DescribeDDoSAttackEvent）用于查询DDoS攻击事件列表。
 
         :param request: Request instance for DescribeDDoSAttackEvent.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackEventRequest`
@@ -665,15 +665,15 @@
             model = models.DescribeDDoSAttackEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSAttackTopData(self, request):
         """本接口（DescribeDDoSAttackTopData）用于查询DDoS攻击Top数据。
 
         :param request: Request instance for DescribeDDoSAttackTopData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDDoSAttackTopDataRequest`
@@ -688,15 +688,15 @@
             model = models.DescribeDDoSAttackTopDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDefaultCertificates(self, request):
         """查询默认证书列表
 
         :param request: Request instance for DescribeDefaultCertificates.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeDefaultCertificatesRequest`
@@ -711,15 +711,15 @@
             model = models.DescribeDefaultCertificatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostsSetting(self, request):
         """用于查询域名配置信息
 
         :param request: Request instance for DescribeHostsSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeHostsSettingRequest`
@@ -734,15 +734,15 @@
             model = models.DescribeHostsSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIdentifications(self, request):
         """查询站点的验证信息。
 
         :param request: Request instance for DescribeIdentifications.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeIdentificationsRequest`
@@ -757,15 +757,15 @@
             model = models.DescribeIdentificationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOriginGroup(self, request):
         """获取源站组列表
 
         :param request: Request instance for DescribeOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOriginGroupRequest`
@@ -780,15 +780,15 @@
             model = models.DescribeOriginGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOriginProtection(self, request):
         """查询源站防护信息
 
         :param request: Request instance for DescribeOriginProtection.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOriginProtectionRequest`
@@ -803,15 +803,15 @@
             model = models.DescribeOriginProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewL7Data(self, request):
         """本接口（DescribeOverviewL7Data）用于查询七层监控类时序流量数据。
 
         :param request: Request instance for DescribeOverviewL7Data.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeOverviewL7DataRequest`
@@ -826,15 +826,15 @@
             model = models.DescribeOverviewL7DataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrefetchTasks(self, request):
         """查询预热任务状态
 
         :param request: Request instance for DescribePrefetchTasks.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribePrefetchTasksRequest`
@@ -849,15 +849,15 @@
             model = models.DescribePrefetchTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurgeTasks(self, request):
         """查询清除缓存历史记录
 
         :param request: Request instance for DescribePurgeTasks.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribePurgeTasksRequest`
@@ -872,15 +872,15 @@
             model = models.DescribePurgeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRules(self, request):
         """查询规则引擎规则。
 
         :param request: Request instance for DescribeRules.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeRulesRequest`
@@ -895,15 +895,15 @@
             model = models.DescribeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRulesSetting(self, request):
         """返回规则引擎可应用匹配请求的设置列表及其详细建议配置信息
 
         :param request: Request instance for DescribeRulesSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeRulesSettingRequest`
@@ -918,15 +918,15 @@
             model = models.DescribeRulesSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimingL4Data(self, request):
         """本接口（DescribeTimingL4Data）用于查询四层时序流量数据列表。
 
         :param request: Request instance for DescribeTimingL4Data.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL4DataRequest`
@@ -941,15 +941,15 @@
             model = models.DescribeTimingL4DataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimingL7AnalysisData(self, request):
         """本接口（DescribeTimingL7AnalysisData）查询七层数据分析类时序数据。
 
         :param request: Request instance for DescribeTimingL7AnalysisData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7AnalysisDataRequest`
@@ -964,15 +964,15 @@
             model = models.DescribeTimingL7AnalysisDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimingL7CacheData(self, request):
         """本接口（DescribeTimingL7CacheData）用于查询七层缓存分析时序类流量数据。
 
         :param request: Request instance for DescribeTimingL7CacheData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTimingL7CacheDataRequest`
@@ -987,15 +987,15 @@
             model = models.DescribeTimingL7CacheDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopL7AnalysisData(self, request):
         """本接口（DescribeTopL7AnalysisData）用于查询七层流量前topN的数据。
 
         :param request: Request instance for DescribeTopL7AnalysisData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7AnalysisDataRequest`
@@ -1010,15 +1010,15 @@
             model = models.DescribeTopL7AnalysisDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopL7CacheData(self, request):
         """本接口（DescribeTopL7CacheData）用于查询七层缓存分析topN流量数据。
 
         :param request: Request instance for DescribeTopL7CacheData.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeTopL7CacheDataRequest`
@@ -1033,15 +1033,15 @@
             model = models.DescribeTopL7CacheDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZoneSetting(self, request):
         """用于查询站点的所有配置信息。
 
         :param request: Request instance for DescribeZoneSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeZoneSettingRequest`
@@ -1056,15 +1056,15 @@
             model = models.DescribeZoneSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """用户查询用户站点信息列表，支持分页。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.teo.v20220901.models.DescribeZonesRequest`
@@ -1079,15 +1079,15 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadL4Logs(self, request):
         """本接口（DownloadL4Logs）用于下载四层离线日志。
 
         :param request: Request instance for DownloadL4Logs.
         :type request: :class:`tencentcloud.teo.v20220901.models.DownloadL4LogsRequest`
@@ -1102,15 +1102,15 @@
             model = models.DownloadL4LogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadL7Logs(self, request):
         """本接口（DownloadL7Logs）下载七层离线日志。
 
         :param request: Request instance for DownloadL7Logs.
         :type request: :class:`tencentcloud.teo.v20220901.models.DownloadL7LogsRequest`
@@ -1125,15 +1125,15 @@
             model = models.DownloadL7LogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IdentifyZone(self, request):
         """用于验证站点所有权。
 
         :param request: Request instance for IdentifyZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.IdentifyZoneRequest`
@@ -1148,15 +1148,15 @@
             model = models.IdentifyZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccelerationDomain(self, request):
         """修改加速域名信息
 
         :param request: Request instance for ModifyAccelerationDomain.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainRequest`
@@ -1171,15 +1171,15 @@
             model = models.ModifyAccelerationDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccelerationDomainStatuses(self, request):
         """批量修改加速域名状态
 
         :param request: Request instance for ModifyAccelerationDomainStatuses.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAccelerationDomainStatusesRequest`
@@ -1194,15 +1194,15 @@
             model = models.ModifyAccelerationDomainStatusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAliasDomain(self, request):
         """修改别称域名。
 
         :param request: Request instance for ModifyAliasDomain.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainRequest`
@@ -1217,15 +1217,15 @@
             model = models.ModifyAliasDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAliasDomainStatus(self, request):
         """修改别称域名状态。
 
         :param request: Request instance for ModifyAliasDomainStatus.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyAliasDomainStatusRequest`
@@ -1240,15 +1240,15 @@
             model = models.ModifyAliasDomainStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationProxy(self, request):
         """修改应用代理
 
         :param request: Request instance for ModifyApplicationProxy.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRequest`
@@ -1263,15 +1263,15 @@
             model = models.ModifyApplicationProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationProxyRule(self, request):
         """修改应用代理规则
 
         :param request: Request instance for ModifyApplicationProxyRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleRequest`
@@ -1286,15 +1286,15 @@
             model = models.ModifyApplicationProxyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationProxyRuleStatus(self, request):
         """修改应用代理规则的状态
 
         :param request: Request instance for ModifyApplicationProxyRuleStatus.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyRuleStatusRequest`
@@ -1309,15 +1309,15 @@
             model = models.ModifyApplicationProxyRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationProxyStatus(self, request):
         """修改应用代理的状态
 
         :param request: Request instance for ModifyApplicationProxyStatus.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyApplicationProxyStatusRequest`
@@ -1332,15 +1332,15 @@
             model = models.ModifyApplicationProxyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHostsCertificate(self, request):
         """用于修改域名证书
 
         :param request: Request instance for ModifyHostsCertificate.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyHostsCertificateRequest`
@@ -1355,15 +1355,15 @@
             model = models.ModifyHostsCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyOriginGroup(self, request):
         """修改源站组
 
         :param request: Request instance for ModifyOriginGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyOriginGroupRequest`
@@ -1378,15 +1378,15 @@
             model = models.ModifyOriginGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRule(self, request):
         """修改规则引擎规则。
 
         :param request: Request instance for ModifyRule.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyRuleRequest`
@@ -1401,15 +1401,15 @@
             model = models.ModifyRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityIPGroup(self, request):
         """修改安全 IP 组。
 
         :param request: Request instance for ModifySecurityIPGroup.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityIPGroupRequest`
@@ -1424,15 +1424,15 @@
             model = models.ModifySecurityIPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityPolicy(self, request):
         """修改Web&Bot安全配置。
 
         :param request: Request instance for ModifySecurityPolicy.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifySecurityPolicyRequest`
@@ -1447,15 +1447,15 @@
             model = models.ModifySecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyZone(self, request):
         """修改站点信息。
 
         :param request: Request instance for ModifyZone.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneRequest`
@@ -1470,15 +1470,15 @@
             model = models.ModifyZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyZoneSetting(self, request):
         """用于修改站点配置
 
         :param request: Request instance for ModifyZoneSetting.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneSettingRequest`
@@ -1493,15 +1493,15 @@
             model = models.ModifyZoneSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyZoneStatus(self, request):
         """用于开启，关闭站点。
 
         :param request: Request instance for ModifyZoneStatus.
         :type request: :class:`tencentcloud.teo.v20220901.models.ModifyZoneStatusRequest`
@@ -1516,8 +1516,8 @@
             model = models.ModifyZoneStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/teo_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreatePrefetchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePurgeTask(self, request):
         """创建清除缓存任务
 
         :param request: Request instance for CreatePurgeTask.
         :type request: :class:`tencentcloud.teo.v20220106.models.CreatePurgeTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CreatePurgeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrefetchTasks(self, request):
         """查询预热任务状态
 
         :param request: Request instance for DescribePrefetchTasks.
         :type request: :class:`tencentcloud.teo.v20220106.models.DescribePrefetchTasksRequest`
@@ -88,15 +88,15 @@
             model = models.DescribePrefetchTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurgeTasks(self, request):
         """查询清除缓存历史记录
 
         :param request: Request instance for DescribePurgeTasks.
         :type request: :class:`tencentcloud.teo.v20220106.models.DescribePurgeTasksRequest`
@@ -111,15 +111,15 @@
             model = models.DescribePurgeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """用户查询用户站点信息列表，支持分页
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.teo.v20220106.models.DescribeZonesRequest`
@@ -134,8 +134,8 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.937/README.rst` & `tencentcloud-sdk-python-teo-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.938/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

