# Comparing `tmp/tencentcloud-sdk-python-gaap-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-gaap-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gaap-3.0.937.tar", last modified: Tue Jul 18 00:24:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gaap-3.0.938.tar", last modified: Wed Jul 19 00:39:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gaap-3.0.937.tar` & `tencentcloud-sdk-python-gaap-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11791 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   101202 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/gaap_client.py
--rw-r--r--   0 root         (0) root         (0)   515457 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:24:18.000000 tencentcloud-sdk-python-gaap-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11791 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   101614 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/gaap_client.py
+-rw-r--r--   0 root         (0) root         (0)   515457 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:39:35.000000 tencentcloud-sdk-python-gaap-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/setup.py` & `tencentcloud-sdk-python-gaap-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/errorcodes.py` & `tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/gaap_client.py` & `tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/gaap_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BanAndRecoverProxy(self, request):
         """本接口（BanAndRecoverProxy）用于联通封禁解封GAAP跨境通道实例，支持按照客户UIN维度下发请求。被封禁的实例带宽上限将会被限制到0Mbps，无法正常处理客户端和源站之间的请求。
 
         :param request: Request instance for BanAndRecoverProxy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.BanAndRecoverProxyRequest`
@@ -65,15 +65,15 @@
             model = models.BanAndRecoverProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindListenerRealServers(self, request):
         """本接口（BindListenerRealServers）用于TCP/UDP监听器绑定解绑源站。
         注意：本接口会解绑之前绑定的源站，绑定本次调用所选择的源站。例如：原来绑定的源站为A，B，C，本次调用的选择绑定的源站为C，D，E，那么调用后所绑定的源站为C，D，E。
 
         :param request: Request instance for BindListenerRealServers.
@@ -89,15 +89,15 @@
             model = models.BindListenerRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindRuleRealServers(self, request):
         """该接口用于7层监听器的转发规则绑定源站。注意：本接口会解绑之前绑定的源站，绑定本次调用所选择的源站。
 
         :param request: Request instance for BindRuleRealServers.
         :type request: :class:`tencentcloud.gaap.v20180529.models.BindRuleRealServersRequest`
@@ -112,15 +112,15 @@
             model = models.BindRuleRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckProxyCreate(self, request):
         """本接口(CheckProxyCreate)用于查询能否创建指定配置的加速通道。
 
         :param request: Request instance for CheckProxyCreate.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CheckProxyCreateRequest`
@@ -135,15 +135,15 @@
             model = models.CheckProxyCreateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseProxies(self, request):
         """本接口（CloseProxies）用于关闭通道。通道关闭后，不再产生流量，但每天仍然收取通道基础配置费用。
 
         :param request: Request instance for CloseProxies.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CloseProxiesRequest`
@@ -158,15 +158,15 @@
             model = models.CloseProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseProxyGroup(self, request):
         """本接口（CloseProxyGroup）用于关闭通道组。通道组关闭后，不再产生流量，但每天仍然收取通道基础配置费用。
 
         :param request: Request instance for CloseProxyGroup.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CloseProxyGroupRequest`
@@ -181,15 +181,15 @@
             model = models.CloseProxyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseSecurityPolicy(self, request):
         """关闭安全策略
 
         :param request: Request instance for CloseSecurityPolicy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CloseSecurityPolicyRequest`
@@ -204,15 +204,15 @@
             model = models.CloseSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCertificate(self, request):
         """本接口（CreateCertificate）用于创建Gaap相关证书和配置文件，包括基础认证配置文件，客户端CA证书，服务器SSL证书，Gaap SSL证书以及源站CA证书。
 
         :param request: Request instance for CreateCertificate.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateCertificateRequest`
@@ -227,15 +227,15 @@
             model = models.CreateCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomHeader(self, request):
         """本接口（CreateCustomHeader）用于创建HTTP/HTTPS监听器的自定义header，客户端请求通过访问该监听器时，会将监听器中配置的header信息发送到源站。
 
         :param request: Request instance for CreateCustomHeader.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateCustomHeaderRequest`
@@ -250,15 +250,15 @@
             model = models.CreateCustomHeaderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomain(self, request):
         """本接口（CreateDomain）用于创建HTTP/HTTPS监听器的访问域名，客户端请求通过访问该域名来请求后端业务。
         该接口仅支持version3.0的通道。
 
         :param request: Request instance for CreateDomain.
@@ -274,15 +274,15 @@
             model = models.CreateDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomainErrorPageInfo(self, request):
         """定制域名指定错误码的错误响应
 
         :param request: Request instance for CreateDomainErrorPageInfo.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateDomainErrorPageInfoRequest`
@@ -297,15 +297,15 @@
             model = models.CreateDomainErrorPageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFirstLinkSession(self, request):
         """本接口（CreateFirstLinkSession）用于创建接入段加速会话，创建有可能成功，也可能失败，需要通过返回码来进行判断。
 
         :param request: Request instance for CreateFirstLinkSession.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateFirstLinkSessionRequest`
@@ -320,15 +320,15 @@
             model = models.CreateFirstLinkSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGlobalDomain(self, request):
         """用来创建统一域名
 
         :param request: Request instance for CreateGlobalDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateGlobalDomainRequest`
@@ -343,15 +343,15 @@
             model = models.CreateGlobalDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGlobalDomainDns(self, request):
         """创建域名解析记录
 
         :param request: Request instance for CreateGlobalDomainDns.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateGlobalDomainDnsRequest`
@@ -366,15 +366,15 @@
             model = models.CreateGlobalDomainDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHTTPListener(self, request):
         """该接口（CreateHTTPListener）用于在通道实例下创建HTTP协议类型的监听器。
 
         :param request: Request instance for CreateHTTPListener.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateHTTPListenerRequest`
@@ -389,15 +389,15 @@
             model = models.CreateHTTPListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHTTPSListener(self, request):
         """该接口（CreateHTTPSListener）用于在通道实例下创建HTTPS协议类型的监听器。
 
         :param request: Request instance for CreateHTTPSListener.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateHTTPSListenerRequest`
@@ -412,15 +412,15 @@
             model = models.CreateHTTPSListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxy(self, request):
         """本接口（CreateProxy）用于创建/复制一个指定配置的加速通道。当复制通道时，需要设置新通道的基本配置参数，并设置ClonedProxyId来指定被复制的通道。
 
         :param request: Request instance for CreateProxy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateProxyRequest`
@@ -435,15 +435,15 @@
             model = models.CreateProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxyGroup(self, request):
         """本接口（CreateProxyGroup）用于创建通道组。
 
         :param request: Request instance for CreateProxyGroup.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateProxyGroupRequest`
@@ -458,15 +458,15 @@
             model = models.CreateProxyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxyGroupDomain(self, request):
         """本接口（CreateProxyGroupDomain）用于创建通道组域名，并开启域名解析。
 
         :param request: Request instance for CreateProxyGroupDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateProxyGroupDomainRequest`
@@ -481,15 +481,15 @@
             model = models.CreateProxyGroupDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRule(self, request):
         """该接口（CreateRule）用于创建HTTP/HTTPS监听器转发规则。
 
         :param request: Request instance for CreateRule.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateRuleRequest`
@@ -504,15 +504,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityPolicy(self, request):
         """创建安全策略
 
         :param request: Request instance for CreateSecurityPolicy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateSecurityPolicyRequest`
@@ -527,15 +527,15 @@
             model = models.CreateSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecurityRules(self, request):
         """添加安全策略规则
 
         :param request: Request instance for CreateSecurityRules.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateSecurityRulesRequest`
@@ -550,15 +550,15 @@
             model = models.CreateSecurityRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTCPListeners(self, request):
         """该接口（CreateTCPListeners）用于批量创建单通道或者通道组的TCP协议类型的监听器。
 
         :param request: Request instance for CreateTCPListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateTCPListenersRequest`
@@ -573,15 +573,15 @@
             model = models.CreateTCPListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUDPListeners(self, request):
         """该接口（CreateUDPListeners）用于批量创建单通道或者通道组的UDP协议类型的监听器。
 
         :param request: Request instance for CreateUDPListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.CreateUDPListenersRequest`
@@ -596,15 +596,15 @@
             model = models.CreateUDPListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCertificate(self, request):
         """本接口（DeleteCertificate）用于删除证书。
 
         :param request: Request instance for DeleteCertificate.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteCertificateRequest`
@@ -619,15 +619,15 @@
             model = models.DeleteCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomain(self, request):
         """本接口（DeleteDomain）仅适用于7层监听器，用于删除该监听器下对应域名及域名下的所有规则，所有已绑定源站的规则将自动解绑。
 
         :param request: Request instance for DeleteDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteDomainRequest`
@@ -642,15 +642,15 @@
             model = models.DeleteDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomainErrorPageInfo(self, request):
         """删除域名的定制错误
 
         :param request: Request instance for DeleteDomainErrorPageInfo.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteDomainErrorPageInfoRequest`
@@ -665,15 +665,15 @@
             model = models.DeleteDomainErrorPageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFirstLinkSession(self, request):
         """本接口（DeleteFirstLinkSession）用于删除接入段加速会话，删除加速会话后会停止加速。
 
         :param request: Request instance for DeleteFirstLinkSession.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteFirstLinkSessionRequest`
@@ -688,15 +688,15 @@
             model = models.DeleteFirstLinkSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGlobalDomain(self, request):
         """删除统一域名
 
         :param request: Request instance for DeleteGlobalDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteGlobalDomainRequest`
@@ -711,15 +711,15 @@
             model = models.DeleteGlobalDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGlobalDomainDns(self, request):
         """删除域名的某条解析记录
 
         :param request: Request instance for DeleteGlobalDomainDns.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteGlobalDomainDnsRequest`
@@ -734,15 +734,15 @@
             model = models.DeleteGlobalDomainDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteListeners(self, request):
         """该接口（DeleteListeners）用于批量删除通道或通道组的监听器，包括4/7层监听器。
 
         :param request: Request instance for DeleteListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteListenersRequest`
@@ -757,15 +757,15 @@
             model = models.DeleteListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteProxyGroup(self, request):
         """本接口（DeleteProxyGroup）用于删除通道组。
 
         :param request: Request instance for DeleteProxyGroup.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteProxyGroupRequest`
@@ -780,15 +780,15 @@
             model = models.DeleteProxyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRule(self, request):
         """该接口（DeleteRule）用于删除HTTP/HTTPS监听器的转发规则。
 
         :param request: Request instance for DeleteRule.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteRuleRequest`
@@ -803,15 +803,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityPolicy(self, request):
         """删除安全策略
 
         :param request: Request instance for DeleteSecurityPolicy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteSecurityPolicyRequest`
@@ -826,15 +826,15 @@
             model = models.DeleteSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecurityRules(self, request):
         """删除安全策略规则
 
         :param request: Request instance for DeleteSecurityRules.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DeleteSecurityRulesRequest`
@@ -849,15 +849,15 @@
             model = models.DeleteSecurityRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessRegions(self, request):
         """本接口（DescribeAccessRegions）用于查询加速区域，即客户端接入区域。
 
         :param request: Request instance for DescribeAccessRegions.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeAccessRegionsRequest`
@@ -872,15 +872,15 @@
             model = models.DescribeAccessRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessRegionsByDestRegion(self, request):
         """本接口（DescribeAccessRegionsByDestRegion）根据源站区域查询可用的加速区域列表。
 
         :param request: Request instance for DescribeAccessRegionsByDestRegion.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeAccessRegionsByDestRegionRequest`
@@ -895,15 +895,15 @@
             model = models.DescribeAccessRegionsByDestRegionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuthSignature(self, request):
         """为了防止在下单、询价、后付费开通等过程中确保来源合法以及订单参数没有被篡改过，各个业务方使用下单、询价等场景需调用计费签名接口获取签名，获取签名的请求需带上签名以验证身份，本接口可以获取计费签名。
 
         :param request: Request instance for DescribeAuthSignature.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeAuthSignatureRequest`
@@ -918,15 +918,15 @@
             model = models.DescribeAuthSignatureResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBlackHeader(self, request):
         """本接口（DescribeBlackHeader）用于查询禁用的自定义header 名称
 
         :param request: Request instance for DescribeBlackHeader.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeBlackHeaderRequest`
@@ -941,15 +941,15 @@
             model = models.DescribeBlackHeaderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificateDetail(self, request):
         """本接口（DescribeCertificateDetail）用于查询证书详情，包括证书ID，证书名字，证书类型，证书内容以及密钥等信息。
 
         :param request: Request instance for DescribeCertificateDetail.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeCertificateDetailRequest`
@@ -964,15 +964,15 @@
             model = models.DescribeCertificateDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertificates(self, request):
         """本接口（DescribeCertificates）用来查询可以使用的证书列表。
 
         :param request: Request instance for DescribeCertificates.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeCertificatesRequest`
@@ -987,15 +987,15 @@
             model = models.DescribeCertificatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCountryAreaMapping(self, request):
         """本接口（DescribeCountryAreaMapping）用于获取国家地区编码映射表。
 
         :param request: Request instance for DescribeCountryAreaMapping.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeCountryAreaMappingRequest`
@@ -1010,15 +1010,15 @@
             model = models.DescribeCountryAreaMappingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCrossBorderProxies(self, request):
         """本接口（DescribeCrossBorderProxies）用于查询跨境通道实例列表。
 
         :param request: Request instance for DescribeCrossBorderProxies.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeCrossBorderProxiesRequest`
@@ -1033,15 +1033,15 @@
             model = models.DescribeCrossBorderProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomHeader(self, request):
         """本接口（DescribeCustomHeader）用于自定义header列表
 
         :param request: Request instance for DescribeCustomHeader.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeCustomHeaderRequest`
@@ -1056,15 +1056,15 @@
             model = models.DescribeCustomHeaderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDestRegions(self, request):
         """本接口（DescribeDestRegions）用于查询源站区域，即源站服务器所在区域。
 
         :param request: Request instance for DescribeDestRegions.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeDestRegionsRequest`
@@ -1079,15 +1079,15 @@
             model = models.DescribeDestRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainErrorPageInfo(self, request):
         """查询目前定制域名的错误响应
 
         :param request: Request instance for DescribeDomainErrorPageInfo.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeDomainErrorPageInfoRequest`
@@ -1102,15 +1102,15 @@
             model = models.DescribeDomainErrorPageInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainErrorPageInfoByIds(self, request):
         """根据定制错误ID查询错误响应
 
         :param request: Request instance for DescribeDomainErrorPageInfoByIds.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeDomainErrorPageInfoByIdsRequest`
@@ -1125,15 +1125,15 @@
             model = models.DescribeDomainErrorPageInfoByIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirstLinkSession(self, request):
         """本接口（DescribeFirstLinkSession）用于查询接入段加速会话状态，包括会话状态，生效时长，加速套餐等信息。
 
         :param request: Request instance for DescribeFirstLinkSession.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeFirstLinkSessionRequest`
@@ -1148,15 +1148,15 @@
             model = models.DescribeFirstLinkSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGlobalDomainDns(self, request):
         """查询域名解析列表
 
         :param request: Request instance for DescribeGlobalDomainDns.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeGlobalDomainDnsRequest`
@@ -1171,15 +1171,15 @@
             model = models.DescribeGlobalDomainDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGlobalDomains(self, request):
         """查询域名列表
 
         :param request: Request instance for DescribeGlobalDomains.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeGlobalDomainsRequest`
@@ -1194,15 +1194,15 @@
             model = models.DescribeGlobalDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupAndStatisticsProxy(self, request):
         """该接口为内部接口，用于查询可以获取统计数据的通道组和通道信息
 
         :param request: Request instance for DescribeGroupAndStatisticsProxy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeGroupAndStatisticsProxyRequest`
@@ -1217,15 +1217,15 @@
             model = models.DescribeGroupAndStatisticsProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupDomainConfig(self, request):
         """本接口（DescribeGroupDomainConfig）用于获取通道组域名解析配置详情。
 
         :param request: Request instance for DescribeGroupDomainConfig.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeGroupDomainConfigRequest`
@@ -1240,15 +1240,15 @@
             model = models.DescribeGroupDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHTTPListeners(self, request):
         """该接口（DescribeHTTPListeners）用来查询HTTP监听器信息。
 
         :param request: Request instance for DescribeHTTPListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeHTTPListenersRequest`
@@ -1263,15 +1263,15 @@
             model = models.DescribeHTTPListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHTTPSListeners(self, request):
         """本接口（DescribeHTTPSListeners）用来查询HTTPS监听器信息。
 
         :param request: Request instance for DescribeHTTPSListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeHTTPSListenersRequest`
@@ -1286,15 +1286,15 @@
             model = models.DescribeHTTPSListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListenerRealServers(self, request):
         """该接口（DescribeListenerRealServers）用于查询TCP/UDP监听器源站列表，包括该监听器已经绑定的源站列表以及可以绑定的源站列表。
 
         :param request: Request instance for DescribeListenerRealServers.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeListenerRealServersRequest`
@@ -1309,15 +1309,15 @@
             model = models.DescribeListenerRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListenerStatistics(self, request):
         """该接口用于查询监听器统计数据，包括出入带宽，出入包量，并发数据。支持300秒, 3600秒和86400秒的细粒度，取值为细粒度范围内最大值。
 
         :param request: Request instance for DescribeListenerStatistics.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeListenerStatisticsRequest`
@@ -1332,15 +1332,15 @@
             model = models.DescribeListenerStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxies(self, request):
         """本接口（DescribeProxies）用于查询通道实例列表。
 
         :param request: Request instance for DescribeProxies.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxiesRequest`
@@ -1355,15 +1355,15 @@
             model = models.DescribeProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxiesStatus(self, request):
         """本接口（DescribeProxiesStatus）用于查询通道状态列表。
 
         :param request: Request instance for DescribeProxiesStatus.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxiesStatusRequest`
@@ -1378,15 +1378,15 @@
             model = models.DescribeProxiesStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyAndStatisticsListeners(self, request):
         """该接口为内部接口，用于查询可以获取统计数据的通道和监听器信息
 
         :param request: Request instance for DescribeProxyAndStatisticsListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyAndStatisticsListenersRequest`
@@ -1401,15 +1401,15 @@
             model = models.DescribeProxyAndStatisticsListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyDetail(self, request):
         """本接口（DescribeProxyDetail）用于查询通道详情。
 
         :param request: Request instance for DescribeProxyDetail.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyDetailRequest`
@@ -1424,15 +1424,15 @@
             model = models.DescribeProxyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyGroupDetails(self, request):
         """本接口（DescribeProxyGroupDetails）用于查询通道组详情。
 
         :param request: Request instance for DescribeProxyGroupDetails.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyGroupDetailsRequest`
@@ -1447,15 +1447,15 @@
             model = models.DescribeProxyGroupDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyGroupList(self, request):
         """本接口（DescribeProxyGroupList）用于拉取通道组列表及各通道组基本信息。
 
         :param request: Request instance for DescribeProxyGroupList.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyGroupListRequest`
@@ -1470,15 +1470,15 @@
             model = models.DescribeProxyGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyGroupStatistics(self, request):
         """该接口用于查询监听器统计数据，包括出入带宽，出入包量，并发数据。支持300, 3600和86400的细粒度，取值为细粒度范围内最大值。
 
         :param request: Request instance for DescribeProxyGroupStatistics.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyGroupStatisticsRequest`
@@ -1493,15 +1493,15 @@
             model = models.DescribeProxyGroupStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyStatistics(self, request):
         """该接口用于查询监听器统计数据，包括出入带宽，出入包量，并发，丢包和时延数据。支持300, 3600和86400的细粒度，取值为细粒度范围内最大值。
 
         :param request: Request instance for DescribeProxyStatistics.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeProxyStatisticsRequest`
@@ -1516,15 +1516,15 @@
             model = models.DescribeProxyStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealServerStatistics(self, request):
         """该接口（DescribeRealServerStatistics）用于查询源站健康检查结果的统计数据。源站状态展示位为1：正常或者0：异常。查询的源站需要在监听器或者规则上进行了绑定，查询时需指定绑定的监听器或者规则ID。该接口支持1分钟细粒度的源站状态统计数据展示。
 
         :param request: Request instance for DescribeRealServerStatistics.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRealServerStatisticsRequest`
@@ -1539,15 +1539,15 @@
             model = models.DescribeRealServerStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealServers(self, request):
         """本接口（DescribeRealServers）用于查询源站信息，可以根据项目名查询所有的源站信息，此外支持指定IP或者域名的源站模糊查询。
 
         :param request: Request instance for DescribeRealServers.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRealServersRequest`
@@ -1562,15 +1562,15 @@
             model = models.DescribeRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealServersStatus(self, request):
         """本接口（DescribeRealServersStatus）用于查询源站是否已被规则或者监听器绑定
 
         :param request: Request instance for DescribeRealServersStatus.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRealServersStatusRequest`
@@ -1585,15 +1585,15 @@
             model = models.DescribeRealServersStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegionAndPrice(self, request):
         """该接口（DescribeRegionAndPrice）用于获取源站区域和带宽梯度价格
 
         :param request: Request instance for DescribeRegionAndPrice.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRegionAndPriceRequest`
@@ -1608,15 +1608,15 @@
             model = models.DescribeRegionAndPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcesByTag(self, request):
         """本接口（DescribeResourcesByTag）用于根据标签来查询对应的资源信息，包括通道，通道组和源站。
 
         :param request: Request instance for DescribeResourcesByTag.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeResourcesByTagRequest`
@@ -1631,15 +1631,15 @@
             model = models.DescribeResourcesByTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleRealServers(self, request):
         """本接口（DescribeRuleRealServers）用于查询转发规则相关的源站信息， 包括该规则可绑定的源站信息和已绑定的源站信息。
 
         :param request: Request instance for DescribeRuleRealServers.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRuleRealServersRequest`
@@ -1654,15 +1654,15 @@
             model = models.DescribeRuleRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRules(self, request):
         """本接口（DescribeRules）用于查询监听器下的所有规则信息，包括规则域名，路径以及该规则下所绑定的源站列表。当通道版本为3.0时，该接口会返回该域名对应的高级认证配置信息。
 
         :param request: Request instance for DescribeRules.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRulesRequest`
@@ -1677,15 +1677,15 @@
             model = models.DescribeRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRulesByRuleIds(self, request):
         """本接口（DescribeRulesByRuleIds）用于根据规则ID拉取规则信息列表。支持一个或者多个规则信息的拉取。一次最多支持10个规则信息的拉取。
 
         :param request: Request instance for DescribeRulesByRuleIds.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeRulesByRuleIdsRequest`
@@ -1700,15 +1700,15 @@
             model = models.DescribeRulesByRuleIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityPolicyDetail(self, request):
         """获取安全策略详情
 
         :param request: Request instance for DescribeSecurityPolicyDetail.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeSecurityPolicyDetailRequest`
@@ -1723,15 +1723,15 @@
             model = models.DescribeSecurityPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityRules(self, request):
         """本接口（DescribeSecurityRules）用于根据安全规则ID查询安全规则详情列表。支持一个或多个安全规则的查询。一次最多支持20个安全规则的查询。
 
         :param request: Request instance for DescribeSecurityRules.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeSecurityRulesRequest`
@@ -1746,15 +1746,15 @@
             model = models.DescribeSecurityRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTCPListeners(self, request):
         """该接口（DescribeTCPListeners）用于查询单通道或者通道组下的TCP监听器信息。
 
         :param request: Request instance for DescribeTCPListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeTCPListenersRequest`
@@ -1769,15 +1769,15 @@
             model = models.DescribeTCPListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUDPListeners(self, request):
         """该接口（DescribeUDPListeners）用于查询单通道或者通道组下的UDP监听器信息
 
         :param request: Request instance for DescribeUDPListeners.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DescribeUDPListenersRequest`
@@ -1792,15 +1792,15 @@
             model = models.DescribeUDPListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyProxies(self, request):
         """本接口（DestroyProxies）用于销毁。通道销毁后，不再产生任何费用。
 
         :param request: Request instance for DestroyProxies.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DestroyProxiesRequest`
@@ -1815,15 +1815,15 @@
             model = models.DestroyProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableGlobalDomain(self, request):
         """暂停域名解析
 
         :param request: Request instance for DisableGlobalDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.DisableGlobalDomainRequest`
@@ -1838,15 +1838,15 @@
             model = models.DisableGlobalDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableGlobalDomain(self, request):
         """开启域名解析
 
         :param request: Request instance for EnableGlobalDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.EnableGlobalDomainRequest`
@@ -1861,15 +1861,15 @@
             model = models.EnableGlobalDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateProxy(self, request):
         """本接口（InquiryPriceCreateProxy）用于创建加速通道询价。
 
         :param request: Request instance for InquiryPriceCreateProxy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.InquiryPriceCreateProxyRequest`
@@ -1884,15 +1884,15 @@
             model = models.InquiryPriceCreateProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCertificate(self, request):
         """本接口（ModifyCertificate）用于修改监听器下的域名对应的证书。该接口仅适用于version3.0的通道。
 
         :param request: Request instance for ModifyCertificate.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyCertificateRequest`
@@ -1907,15 +1907,15 @@
             model = models.ModifyCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCertificateAttributes(self, request):
         """本接口（ModifyCertificateAttributes）用于修改证书，包括证书名字以及证书内容。
 
         :param request: Request instance for ModifyCertificateAttributes.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyCertificateAttributesRequest`
@@ -1930,15 +1930,15 @@
             model = models.ModifyCertificateAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomain(self, request):
         """本接口（ModifyDomain）用于监听器下的域名。当通道版本为3.0时，支持对该域名所对应的证书修改。
 
         :param request: Request instance for ModifyDomain.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyDomainRequest`
@@ -1953,15 +1953,15 @@
             model = models.ModifyDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGlobalDomainAttribute(self, request):
         """修改域名属性
 
         :param request: Request instance for ModifyGlobalDomainAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyGlobalDomainAttributeRequest`
@@ -1976,15 +1976,15 @@
             model = models.ModifyGlobalDomainAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGlobalDomainDns(self, request):
         """修改域名解析记录
 
         :param request: Request instance for ModifyGlobalDomainDns.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyGlobalDomainDnsRequest`
@@ -1999,15 +1999,15 @@
             model = models.ModifyGlobalDomainDnsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGroupDomainConfig(self, request):
         """本接口（ModifyGroupDomainConfig）用于配置通道组就近接入域名。
 
         :param request: Request instance for ModifyGroupDomainConfig.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyGroupDomainConfigRequest`
@@ -2022,15 +2022,15 @@
             model = models.ModifyGroupDomainConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHTTPListenerAttribute(self, request):
         """该接口（ModifyHTTPListenerAttribute）用于修改通道的HTTP监听器配置信息，目前仅支持修改监听器的名称。
         注意：通道组通道暂时不支持HTTP/HTTPS监听器。
 
         :param request: Request instance for ModifyHTTPListenerAttribute.
@@ -2046,15 +2046,15 @@
             model = models.ModifyHTTPListenerAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyHTTPSListenerAttribute(self, request):
         """该接口（ModifyHTTPSListenerAttribute）用于修改HTTPS监听器配置，当前不支持通道组和v1版本通道。
 
         :param request: Request instance for ModifyHTTPSListenerAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyHTTPSListenerAttributeRequest`
@@ -2069,15 +2069,15 @@
             model = models.ModifyHTTPSListenerAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxiesAttribute(self, request):
         """本接口（ModifyProxiesAttribute）用于修改实例的属性（目前只支持修改通道的名称）。
 
         :param request: Request instance for ModifyProxiesAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyProxiesAttributeRequest`
@@ -2092,15 +2092,15 @@
             model = models.ModifyProxiesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxiesProject(self, request):
         """本接口（ModifyProxiesProject）用于修改通道所属项目。
 
         :param request: Request instance for ModifyProxiesProject.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyProxiesProjectRequest`
@@ -2115,15 +2115,15 @@
             model = models.ModifyProxiesProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxyConfiguration(self, request):
         """本接口（ModifyProxyConfiguration）用于修改通道的配置。根据当前业务的容量需求，扩容或缩容相关通道的配置。仅支持Scalarable为1的通道,Scalarable可通过接口DescribeProxies获取。
 
         :param request: Request instance for ModifyProxyConfiguration.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyProxyConfigurationRequest`
@@ -2138,15 +2138,15 @@
             model = models.ModifyProxyConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxyGroupAttribute(self, request):
         """本接口（ModifyProxyGroupAttribute）用于修改通道组属性，目前仅支持修改通道组名称。
 
         :param request: Request instance for ModifyProxyGroupAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyProxyGroupAttributeRequest`
@@ -2161,15 +2161,15 @@
             model = models.ModifyProxyGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRealServerName(self, request):
         """本接口（ModifyRealServerName）用于修改源站的名称
 
         :param request: Request instance for ModifyRealServerName.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyRealServerNameRequest`
@@ -2184,15 +2184,15 @@
             model = models.ModifyRealServerNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRuleAttribute(self, request):
         """本接口（ModifyRuleAttribute）用于修改转发规则的信息，包括健康检查的配置以及转发策略。
 
         :param request: Request instance for ModifyRuleAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyRuleAttributeRequest`
@@ -2207,15 +2207,15 @@
             model = models.ModifyRuleAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecurityRule(self, request):
         """修改安全策略规则名
 
         :param request: Request instance for ModifySecurityRule.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifySecurityRuleRequest`
@@ -2230,15 +2230,15 @@
             model = models.ModifySecurityRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTCPListenerAttribute(self, request):
         """本接口（ModifyTCPListenerAttribute）用于修改通道实例下TCP监听器配置，包括健康检查的配置，调度策略。
 
         :param request: Request instance for ModifyTCPListenerAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyTCPListenerAttributeRequest`
@@ -2253,15 +2253,15 @@
             model = models.ModifyTCPListenerAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyUDPListenerAttribute(self, request):
         """本接口（ModifyUDPListenerAttribute）用于修改通道实例下UDP监听器配置，包括监听器名称和调度策略的修改。
 
         :param request: Request instance for ModifyUDPListenerAttribute.
         :type request: :class:`tencentcloud.gaap.v20180529.models.ModifyUDPListenerAttributeRequest`
@@ -2276,15 +2276,15 @@
             model = models.ModifyUDPListenerAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenProxies(self, request):
         """该接口（OpenProxies）用于开启一条或者多条通道。
 
         :param request: Request instance for OpenProxies.
         :type request: :class:`tencentcloud.gaap.v20180529.models.OpenProxiesRequest`
@@ -2299,15 +2299,15 @@
             model = models.OpenProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenProxyGroup(self, request):
         """该接口（OpenProxyGroup）用于开启一条通道组中的所有通道
 
         :param request: Request instance for OpenProxyGroup.
         :type request: :class:`tencentcloud.gaap.v20180529.models.OpenProxyGroupRequest`
@@ -2322,15 +2322,15 @@
             model = models.OpenProxyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenSecurityPolicy(self, request):
         """开启安全策略
 
         :param request: Request instance for OpenSecurityPolicy.
         :type request: :class:`tencentcloud.gaap.v20180529.models.OpenSecurityPolicyRequest`
@@ -2345,15 +2345,15 @@
             model = models.OpenSecurityPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveRealServers(self, request):
         """删除已添加的源站(服务器)IP或域名
 
         :param request: Request instance for RemoveRealServers.
         :type request: :class:`tencentcloud.gaap.v20180529.models.RemoveRealServersRequest`
@@ -2368,15 +2368,15 @@
             model = models.RemoveRealServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAuthentication(self, request):
         """本接口（SetAuthentication）用于通道的高级认证配置，包括认证方式选择，以及各种认证方式对应的证书选择。仅支持Version3.0的通道。
 
         :param request: Request instance for SetAuthentication.
         :type request: :class:`tencentcloud.gaap.v20180529.models.SetAuthenticationRequest`
@@ -2391,8 +2391,8 @@
             model = models.SetAuthenticationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/gaap/v20180529/models.py` & `tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/gaap/v20180529/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gaap-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gaap-3.0.938/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gaap
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gaap SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-gaap-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gaap
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gaap SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.937/README.rst` & `tencentcloud-sdk-python-gaap-3.0.938/README.rst`

 * *Files identical despite different names*

