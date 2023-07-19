# Comparing `tmp/tencentcloud-sdk-python-bmlb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-bmlb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.937.tar", last modified: Tue Jul 18 00:18:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.938.tar", last modified: Wed Jul 19 00:22:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bmlb-3.0.937.tar` & `tencentcloud-sdk-python-bmlb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/
--rw-r--r--   0 root         (0) root         (0)    47086 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/bmlb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   327109 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:18:11.000000 tencentcloud-sdk-python-bmlb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    47282 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/bmlb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   327109 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:22:17.000000 tencentcloud-sdk-python-bmlb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/setup.py` & `tencentcloud-sdk-python-bmlb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/bmlb_client.py` & `tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/bmlb_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindL4BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindL7Backends(self, request):
         """绑定黑石物理服务器或半托管服务器到七层转发路径。
 
         :param request: Request instance for BindL7Backends.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.BindL7BackendsRequest`
@@ -65,15 +65,15 @@
             model = models.BindL7BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindTrafficMirrorListeners(self, request):
         """绑定黑石服务器七层监听器到流量镜像实例。
 
         :param request: Request instance for BindTrafficMirrorListeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.BindTrafficMirrorListenersRequest`
@@ -88,15 +88,15 @@
             model = models.BindTrafficMirrorListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindTrafficMirrorReceivers(self, request):
         """绑定黑石物理服务器成为流量镜像接收机。
 
         :param request: Request instance for BindTrafficMirrorReceivers.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.BindTrafficMirrorReceiversRequest`
@@ -111,15 +111,15 @@
             model = models.BindTrafficMirrorReceiversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL4Listeners(self, request):
         """创建黑石四层负载均衡监听器功能。黑石负载均衡四层监听器提供了转发用户请求的具体规则，包括端口、协议、会话保持、健康检查等参数。
 
         :param request: Request instance for CreateL4Listeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.CreateL4ListenersRequest`
@@ -134,15 +134,15 @@
             model = models.CreateL4ListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7Listeners(self, request):
         """创建黑石负载均衡七层监听器功能。负载均衡七层监听器提供了转发用户请求的具体规则，包括端口、协议等参数。
 
         :param request: Request instance for CreateL7Listeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.CreateL7ListenersRequest`
@@ -157,15 +157,15 @@
             model = models.CreateL7ListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7Rules(self, request):
         """创建黑石负载均衡七层转发规则。
 
         :param request: Request instance for CreateL7Rules.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.CreateL7RulesRequest`
@@ -180,15 +180,15 @@
             model = models.CreateL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLoadBalancers(self, request):
         """用来创建黑石负载均衡。为了使用黑石负载均衡服务，您必须要创建一个或者多个负载均衡实例。通过成功调用该接口，会返回负载均衡实例的唯一ID。用户可以购买的黑石负载均衡实例类型分为：公网类型、内网类型。公网类型负载均衡对应一个BGP VIP，可用于快速访问公网负载均衡绑定的物理服务器；内网类型负载均衡对应一个腾讯云内部的VIP，不能通过Internet访问，可快速访问内网负载均衡绑定的物理服务器。
 
         :param request: Request instance for CreateLoadBalancers.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.CreateLoadBalancersRequest`
@@ -203,15 +203,15 @@
             model = models.CreateLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTrafficMirror(self, request):
         """创建流量镜像实例。
 
         :param request: Request instance for CreateTrafficMirror.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.CreateTrafficMirrorRequest`
@@ -226,15 +226,15 @@
             model = models.CreateTrafficMirrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteL7Domains(self, request):
         """删除黑石负载均衡七层转发域名。
 
         :param request: Request instance for DeleteL7Domains.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DeleteL7DomainsRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteL7DomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteL7Rules(self, request):
         """删除黑石负载均衡七层转发规则。
 
         :param request: Request instance for DeleteL7Rules.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DeleteL7RulesRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteListeners(self, request):
         """删除黑石负载均衡监听器。
 
         :param request: Request instance for DeleteListeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DeleteListenersRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLoadBalancer(self, request):
         """删除用户指定的黑石负载均衡实例。
 
         :param request: Request instance for DeleteLoadBalancer.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DeleteLoadBalancerRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteLoadBalancerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTrafficMirror(self, request):
         """删除已创建的黑石流量镜像实例，删除过程是异步执行的，因此需要使用查询任务接口获取删除的结果。
 
         :param request: Request instance for DeleteTrafficMirror.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DeleteTrafficMirrorRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteTrafficMirrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCertDetail(self, request):
         """获取黑石负载均衡证书详情。
 
         :param request: Request instance for DescribeCertDetail.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeCertDetailRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeCertDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDevicesBindInfo(self, request):
         """查询黑石物理机和虚机以及托管服务器绑定的黑石负载均衡详情。
 
         :param request: Request instance for DescribeDevicesBindInfo.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeDevicesBindInfoRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeDevicesBindInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL4Backends(self, request):
         """获取黑石负载均衡四层监听器绑定的主机列表。
 
         :param request: Request instance for DescribeL4Backends.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL4BackendsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeL4BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL4ListenerInfo(self, request):
         """查找绑定了某主机或者指定监听器名称的黑石负载均衡四层监听器。
 
         :param request: Request instance for DescribeL4ListenerInfo.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL4ListenerInfoRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeL4ListenerInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL4Listeners(self, request):
         """获取黑石负载均衡四层监听器。
 
         :param request: Request instance for DescribeL4Listeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL4ListenersRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeL4ListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7Backends(self, request):
         """获取黑石负载均衡七层监听器绑定的主机列表
 
         :param request: Request instance for DescribeL7Backends.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL7BackendsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeL7BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7ListenerInfo(self, request):
         """查找绑定了某主机或者有某转发域名黑石负载均衡七层监听器。
 
         :param request: Request instance for DescribeL7ListenerInfo.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL7ListenerInfoRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeL7ListenerInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7Listeners(self, request):
         """获取黑石负载均衡七层监听器列表信息。
 
         :param request: Request instance for DescribeL7Listeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL7ListenersRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeL7ListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7ListenersEx(self, request):
         """获取指定VPC下的7层监听器(支持模糊匹配)。
 
         :param request: Request instance for DescribeL7ListenersEx.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL7ListenersExRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeL7ListenersExResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7Rules(self, request):
         """获取黑石负载均衡七层转发规则。
 
         :param request: Request instance for DescribeL7Rules.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeL7RulesRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoadBalancerPortInfo(self, request):
         """获取黑石负载均衡端口相关信息。
 
         :param request: Request instance for DescribeLoadBalancerPortInfo.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeLoadBalancerPortInfoRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeLoadBalancerPortInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoadBalancerTaskResult(self, request):
         """查询负载均衡实例异步任务的执行情况。
 
         :param request: Request instance for DescribeLoadBalancerTaskResult.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeLoadBalancerTaskResultRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeLoadBalancerTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLoadBalancers(self, request):
         """获取黑石负载均衡实例列表
 
         :param request: Request instance for DescribeLoadBalancers.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeLoadBalancersRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeLoadBalancersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficMirrorListeners(self, request):
         """获取流量镜像的监听器列表信息。
 
         :param request: Request instance for DescribeTrafficMirrorListeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeTrafficMirrorListenersRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeTrafficMirrorListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficMirrorReceiverHealthStatus(self, request):
         """获取流量镜像接收机健康状态。
 
         :param request: Request instance for DescribeTrafficMirrorReceiverHealthStatus.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeTrafficMirrorReceiverHealthStatusRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeTrafficMirrorReceiverHealthStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficMirrorReceivers(self, request):
         """获取指定流量镜像实例的接收机信息。
 
         :param request: Request instance for DescribeTrafficMirrorReceivers.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeTrafficMirrorReceiversRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeTrafficMirrorReceiversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrafficMirrors(self, request):
         """获取流量镜像实例的列表信息。
 
         :param request: Request instance for DescribeTrafficMirrors.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.DescribeTrafficMirrorsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeTrafficMirrorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4BackendPort(self, request):
         """修改黑石负载均衡四层监听器后端实例端口。
 
         :param request: Request instance for ModifyL4BackendPort.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL4BackendPortRequest`
@@ -755,15 +755,15 @@
             model = models.ModifyL4BackendPortResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4BackendProbePort(self, request):
         """修改黑石负载均衡四层监听器后端探测端口。
 
         :param request: Request instance for ModifyL4BackendProbePort.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL4BackendProbePortRequest`
@@ -778,15 +778,15 @@
             model = models.ModifyL4BackendProbePortResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4BackendWeight(self, request):
         """修改黑石负载均衡四层监听器后端实例权重功能。
 
         :param request: Request instance for ModifyL4BackendWeight.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL4BackendWeightRequest`
@@ -801,15 +801,15 @@
             model = models.ModifyL4BackendWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL4Listener(self, request):
         """修改黑石负载均衡四层监听器。
 
         :param request: Request instance for ModifyL4Listener.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL4ListenerRequest`
@@ -824,15 +824,15 @@
             model = models.ModifyL4ListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL7BackendPort(self, request):
         """修改黑石负载均衡七层转发路径后端实例端口。
 
         :param request: Request instance for ModifyL7BackendPort.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL7BackendPortRequest`
@@ -847,15 +847,15 @@
             model = models.ModifyL7BackendPortResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL7BackendWeight(self, request):
         """修改黑石负载均衡七层转发路径后端实例权重。
 
         :param request: Request instance for ModifyL7BackendWeight.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL7BackendWeightRequest`
@@ -870,15 +870,15 @@
             model = models.ModifyL7BackendWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL7Listener(self, request):
         """修改黑石负载均衡七层监听器。
 
         :param request: Request instance for ModifyL7Listener.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL7ListenerRequest`
@@ -893,15 +893,15 @@
             model = models.ModifyL7ListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyL7Locations(self, request):
         """修改黑石负载均衡七层转发路径。
 
         :param request: Request instance for ModifyL7Locations.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyL7LocationsRequest`
@@ -916,15 +916,15 @@
             model = models.ModifyL7LocationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoadBalancer(self, request):
         """根据输入参数来修改黑石负载均衡实例的基本配置信息。可能的信息包括负载均衡实例的名称，域名前缀。
 
         :param request: Request instance for ModifyLoadBalancer.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyLoadBalancerRequest`
@@ -939,15 +939,15 @@
             model = models.ModifyLoadBalancerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLoadBalancerChargeMode(self, request):
         """更改黑石负载均衡的计费方式
 
         :param request: Request instance for ModifyLoadBalancerChargeMode.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ModifyLoadBalancerChargeModeRequest`
@@ -962,15 +962,15 @@
             model = models.ModifyLoadBalancerChargeModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReplaceCert(self, request):
         """更新黑石负载均衡证书。
 
         :param request: Request instance for ReplaceCert.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.ReplaceCertRequest`
@@ -985,15 +985,15 @@
             model = models.ReplaceCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTrafficMirrorAlias(self, request):
         """设置流量镜像的别名。
 
         :param request: Request instance for SetTrafficMirrorAlias.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.SetTrafficMirrorAliasRequest`
@@ -1008,15 +1008,15 @@
             model = models.SetTrafficMirrorAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTrafficMirrorHealthSwitch(self, request):
         """设置流量镜像的健康检查参数。
 
         :param request: Request instance for SetTrafficMirrorHealthSwitch.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.SetTrafficMirrorHealthSwitchRequest`
@@ -1031,15 +1031,15 @@
             model = models.SetTrafficMirrorHealthSwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindL4Backends(self, request):
         """解绑黑石负载均衡四层监听器物理服务器。
 
         :param request: Request instance for UnbindL4Backends.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.UnbindL4BackendsRequest`
@@ -1054,15 +1054,15 @@
             model = models.UnbindL4BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindL7Backends(self, request):
         """解绑黑石物理服务器或者托管服务器到七层转发路径功能。
 
         :param request: Request instance for UnbindL7Backends.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.UnbindL7BackendsRequest`
@@ -1077,15 +1077,15 @@
             model = models.UnbindL7BackendsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindTrafficMirrorListeners(self, request):
         """解绑流量镜像监听器。
 
         :param request: Request instance for UnbindTrafficMirrorListeners.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.UnbindTrafficMirrorListenersRequest`
@@ -1100,15 +1100,15 @@
             model = models.UnbindTrafficMirrorListenersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindTrafficMirrorReceivers(self, request):
         """从流量镜像实例上解绑流量镜像接收机。
 
         :param request: Request instance for UnbindTrafficMirrorReceivers.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.UnbindTrafficMirrorReceiversRequest`
@@ -1123,15 +1123,15 @@
             model = models.UnbindTrafficMirrorReceiversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadCert(self, request):
         """创建黑石负载均衡证书。
 
         :param request: Request instance for UploadCert.
         :type request: :class:`tencentcloud.bmlb.v20180625.models.UploadCertRequest`
@@ -1146,8 +1146,8 @@
             model = models.UploadCertResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/errorcodes.py` & `tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/tencentcloud/bmlb/v20180625/models.py` & `tencentcloud-sdk-python-bmlb-3.0.938/tencentcloud/bmlb/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.937/README.rst` & `tencentcloud-sdk-python-bmlb-3.0.938/README.rst`

 * *Files identical despite different names*

