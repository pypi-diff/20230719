# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.937.tar", last modified: Tue Jul 18 00:16:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.938.tar", last modified: Wed Jul 19 00:20:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.937.tar` & `tencentcloud-sdk-python-antiddos-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88167 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   502349 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88539 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   502349 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:20:46.000000 tencentcloud-sdk-python-antiddos-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AssociateDDoSEipAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateDDoSEipLoadBalancer(self, request):
         """本接口 (AssociateDDoSEipLoadBalancer) 用于将高防弹性公网IP绑定到负载均衡指定内网 IP 上。
 
         :param request: Request instance for AssociateDDoSEipLoadBalancer.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.AssociateDDoSEipLoadBalancerRequest`
@@ -65,15 +65,15 @@
             model = models.AssociateDDoSEipLoadBalancerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBlackWhiteIpList(self, request):
         """添加DDoS防护的IP黑白名单
 
         :param request: Request instance for CreateBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateBlackWhiteIpListRequest`
@@ -88,15 +88,15 @@
             model = models.CreateBlackWhiteIpListResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateBoundIPRequest`
@@ -111,15 +111,15 @@
             model = models.CreateBoundIPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCCPrecisionPolicy(self, request):
         """新增CC精准防护策略
 
         :param request: Request instance for CreateCCPrecisionPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateCCPrecisionPolicyRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCCPrecisionPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCCReqLimitPolicy(self, request):
         """新增CC频率限制策略
 
         :param request: Request instance for CreateCCReqLimitPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateCCReqLimitPolicyRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCCReqLimitPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCcBlackWhiteIpList(self, request):
         """新建CC四层黑白名单
 
         :param request: Request instance for CreateCcBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateCcBlackWhiteIpListRequest`
@@ -180,15 +180,15 @@
             model = models.CreateCcBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCcGeoIPBlockConfig(self, request):
         """新建cc防护的地域封禁配置
 
         :param request: Request instance for CreateCcGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateCcGeoIPBlockConfigRequest`
@@ -203,15 +203,15 @@
             model = models.CreateCcGeoIPBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSAI(self, request):
         """设置DDoS防护的AI防护开关
 
         :param request: Request instance for CreateDDoSAI.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDDoSAIRequest`
@@ -226,15 +226,15 @@
             model = models.CreateDDoSAIResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSBlackWhiteIpList(self, request):
         """添加DDoS防护的IP网段黑白名单
 
         :param request: Request instance for CreateDDoSBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDDoSBlackWhiteIpListRequest`
@@ -249,15 +249,15 @@
             model = models.CreateDDoSBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSConnectLimit(self, request):
         """配置DDoS连接抑制选项
 
         :param request: Request instance for CreateDDoSConnectLimit.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDDoSConnectLimitRequest`
@@ -272,15 +272,15 @@
             model = models.CreateDDoSConnectLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSGeoIPBlockConfig(self, request):
         """添加DDoS防护的区域封禁配置
 
         :param request: Request instance for CreateDDoSGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDDoSGeoIPBlockConfigRequest`
@@ -295,15 +295,15 @@
             model = models.CreateDDoSGeoIPBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDDoSSpeedLimitConfig(self, request):
         """添加DDoS防护的访问限速配置
 
         :param request: Request instance for CreateDDoSSpeedLimitConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDDoSSpeedLimitConfigRequest`
@@ -318,15 +318,15 @@
             model = models.CreateDDoSSpeedLimitConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDefaultAlarmThreshold(self, request):
         """设置单IP默认告警阈值配置
 
         :param request: Request instance for CreateDefaultAlarmThreshold.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateDefaultAlarmThresholdRequest`
@@ -341,15 +341,15 @@
             model = models.CreateDefaultAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIPAlarmThresholdConfig(self, request):
         """设置单IP告警阈值配置
 
         :param request: Request instance for CreateIPAlarmThresholdConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateIPAlarmThresholdConfigRequest`
@@ -364,15 +364,15 @@
             model = models.CreateIPAlarmThresholdConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateL7RuleCerts(self, request):
         """批量配置L7转发规则的证书供SSL测调用
 
         :param request: Request instance for CreateL7RuleCerts.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateL7RuleCertsRequest`
@@ -387,15 +387,15 @@
             model = models.CreateL7RuleCertsResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateNewL7RulesRequest`
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
 
 
     def CreatePacketFilterConfig(self, request):
         """添加DDoS防护的特征过滤规则
 
         :param request: Request instance for CreatePacketFilterConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreatePacketFilterConfigRequest`
@@ -433,15 +433,15 @@
             model = models.CreatePacketFilterConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePortAclConfig(self, request):
         """添加DDoS防护的端口acl策略
 
         :param request: Request instance for CreatePortAclConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreatePortAclConfigRequest`
@@ -456,15 +456,15 @@
             model = models.CreatePortAclConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePortAclConfigList(self, request):
         """批量添加DDoS防护的端口acl策略
 
         :param request: Request instance for CreatePortAclConfigList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreatePortAclConfigListRequest`
@@ -479,15 +479,15 @@
             model = models.CreatePortAclConfigListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProtocolBlockConfig(self, request):
         """设置DDoS防护的协议封禁配置
 
         :param request: Request instance for CreateProtocolBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateProtocolBlockConfigRequest`
@@ -502,15 +502,15 @@
             model = models.CreateProtocolBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSchedulingDomain(self, request):
         """创建一个域名，可用于在封堵时调度切换IP
 
         :param request: Request instance for CreateSchedulingDomain.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateSchedulingDomainRequest`
@@ -525,15 +525,15 @@
             model = models.CreateSchedulingDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWaterPrintConfig(self, request):
         """添加DDoS防护的水印防护配置
 
         :param request: Request instance for CreateWaterPrintConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateWaterPrintConfigRequest`
@@ -548,15 +548,15 @@
             model = models.CreateWaterPrintConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWaterPrintKey(self, request):
         """添加DDoS防护的水印防护密钥
 
         :param request: Request instance for CreateWaterPrintKey.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.CreateWaterPrintKeyRequest`
@@ -571,15 +571,15 @@
             model = models.CreateWaterPrintKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCLevelPolicy(self, request):
         """删除CC分级策略
 
         :param request: Request instance for DeleteCCLevelPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCCLevelPolicyRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteCCLevelPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCPrecisionPolicy(self, request):
         """删除CC精准防护策略
 
         :param request: Request instance for DeleteCCPrecisionPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCCPrecisionPolicyRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteCCPrecisionPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCRequestLimitPolicy(self, request):
         """删除CC频率限制策略
 
         :param request: Request instance for DeleteCCRequestLimitPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCCRequestLimitPolicyRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteCCRequestLimitPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCCThresholdPolicy(self, request):
         """删除CC清洗阈值策略
 
         :param request: Request instance for DeleteCCThresholdPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCCThresholdPolicyRequest`
@@ -663,15 +663,15 @@
             model = models.DeleteCCThresholdPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCcBlackWhiteIpList(self, request):
         """删除CC四层黑白名单
 
         :param request: Request instance for DeleteCcBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCcBlackWhiteIpListRequest`
@@ -686,15 +686,15 @@
             model = models.DeleteCcBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCcGeoIPBlockConfig(self, request):
         """删除CC防护的区域封禁配置
 
         :param request: Request instance for DeleteCcGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteCcGeoIPBlockConfigRequest`
@@ -709,15 +709,15 @@
             model = models.DeleteCcGeoIPBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDDoSBlackWhiteIpList(self, request):
         """删除DDoS防护的IP网段黑白名单
 
         :param request: Request instance for DeleteDDoSBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteDDoSBlackWhiteIpListRequest`
@@ -732,15 +732,15 @@
             model = models.DeleteDDoSBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDDoSGeoIPBlockConfig(self, request):
         """删除DDoS防护的区域封禁配置
 
         :param request: Request instance for DeleteDDoSGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteDDoSGeoIPBlockConfigRequest`
@@ -755,15 +755,15 @@
             model = models.DeleteDDoSGeoIPBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDDoSSpeedLimitConfig(self, request):
         """删除DDoS防护的访问限速配置
 
         :param request: Request instance for DeleteDDoSSpeedLimitConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteDDoSSpeedLimitConfigRequest`
@@ -778,15 +778,15 @@
             model = models.DeleteDDoSSpeedLimitConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePacketFilterConfig(self, request):
         """删除DDoS防护的特征过滤规则
 
         :param request: Request instance for DeletePacketFilterConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeletePacketFilterConfigRequest`
@@ -801,15 +801,15 @@
             model = models.DeletePacketFilterConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePortAclConfig(self, request):
         """删除DDoS防护的端口acl策略
 
         :param request: Request instance for DeletePortAclConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeletePortAclConfigRequest`
@@ -824,15 +824,15 @@
             model = models.DeletePortAclConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWaterPrintConfig(self, request):
         """删除DDoS防护的水印防护配置
 
         :param request: Request instance for DeleteWaterPrintConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteWaterPrintConfigRequest`
@@ -847,15 +847,15 @@
             model = models.DeleteWaterPrintConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWaterPrintKey(self, request):
         """删除DDoS防护的水印防护密钥
 
         :param request: Request instance for DeleteWaterPrintKey.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DeleteWaterPrintKeyRequest`
@@ -870,15 +870,15 @@
             model = models.DeleteWaterPrintKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicDeviceStatus(self, request):
         """获取基础防护攻击状态
 
         :param request: Request instance for DescribeBasicDeviceStatus.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBasicDeviceStatusRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeBasicDeviceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBgpBizTrend(self, request):
         """获取高防包流量折线图
 
         :param request: Request instance for DescribeBgpBizTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBgpBizTrendRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeBgpBizTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBizHttpStatus(self, request):
         """获取业务流量状态码统计列表
 
         :param request: Request instance for DescribeBizHttpStatus.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizHttpStatusRequest`
@@ -939,15 +939,15 @@
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBizTrendRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeBizTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBlackWhiteIpList(self, request):
         """获取DDoS防护的IP黑白名单
 
         :param request: Request instance for DescribeBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeBlackWhiteIpListRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCLevelList(self, request):
         """获取边界防护CC防护等级列表
 
         :param request: Request instance for DescribeCCLevelList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCLevelListRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeCCLevelListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCLevelPolicy(self, request):
         """获取CC分级策略
 
         :param request: Request instance for DescribeCCLevelPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCLevelPolicyRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeCCLevelPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCPrecisionPlyList(self, request):
         """获取CC精准防护列表
 
         :param request: Request instance for DescribeCCPrecisionPlyList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCPrecisionPlyListRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeCCPrecisionPlyListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCReqLimitPolicyList(self, request):
         """获取CC频率限制策略列表
 
         :param request: Request instance for DescribeCCReqLimitPolicyList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCReqLimitPolicyListRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeCCReqLimitPolicyListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCThresholdList(self, request):
         """获取CC清洗阈值列表
 
         :param request: Request instance for DescribeCCThresholdList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCThresholdListRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeCCThresholdListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCCTrend(self, request):
         """获取CC攻击指标数据，包括总请求峰值(QPS)和攻击请求(QPS)以及总请求次数和攻击请求次数
 
         :param request: Request instance for DescribeCCTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCCTrendRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeCCTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcBlackWhiteIpList(self, request):
         """获取CC四层黑白名单列表
 
         :param request: Request instance for DescribeCcBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCcBlackWhiteIpListRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeCcBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcGeoIPBlockConfigList(self, request):
         """获取CC防护的区域封禁配置列表
 
         :param request: Request instance for DescribeCcGeoIPBlockConfigList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeCcGeoIPBlockConfigListRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeCcGeoIPBlockConfigListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSBlackWhiteIpList(self, request):
         """获取DDoS防护的IP网段黑白名单
 
         :param request: Request instance for DescribeDDoSBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeDDoSBlackWhiteIpListRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeDDoSBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDDoSConnectLimitList(self, request):
         """获取DDoS连接抑制配置列表
 
         :param request: Request instance for DescribeDDoSConnectLimitList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeDDoSConnectLimitListRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeDDoSConnectLimitListResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeDDoSTrendRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeDDoSTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDefaultAlarmThreshold(self, request):
         """获取单IP默认告警阈值配置
 
         :param request: Request instance for DescribeDefaultAlarmThreshold.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeDefaultAlarmThresholdRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeDefaultAlarmThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeL7RulesBySSLCertId(self, request):
         """查询与证书ID对于域名匹配的七层规则
 
         :param request: Request instance for DescribeL7RulesBySSLCertId.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeL7RulesBySSLCertIdRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeL7RulesBySSLCertIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListBGPIPInstances(self, request):
         """获取高防IP资产实例列表
 
         :param request: Request instance for DescribeListBGPIPInstances.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListBGPIPInstancesRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeListBGPIPInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListBGPInstances(self, request):
         """获取高防包资产实例列表
 
         :param request: Request instance for DescribeListBGPInstances.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListBGPInstancesRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeListBGPInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListBlackWhiteIpList(self, request):
         """获取DDoS防护的IP黑白名单列表
 
         :param request: Request instance for DescribeListBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListBlackWhiteIpListRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeListBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListDDoSAI(self, request):
         """获取DDoS防护的AI防护开关列表
 
         :param request: Request instance for DescribeListDDoSAI.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListDDoSAIRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeListDDoSAIResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListDDoSGeoIPBlockConfig(self, request):
         """获取DDoS防护的区域封禁配置列表
 
         :param request: Request instance for DescribeListDDoSGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListDDoSGeoIPBlockConfigRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeListDDoSGeoIPBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListDDoSSpeedLimitConfig(self, request):
         """获取DDoS防护的访问限速配置列表
 
         :param request: Request instance for DescribeListDDoSSpeedLimitConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListDDoSSpeedLimitConfigRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeListDDoSSpeedLimitConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListIPAlarmConfig(self, request):
         """获取单IP告警阈值配置列表
 
         :param request: Request instance for DescribeListIPAlarmConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListIPAlarmConfigRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeListIPAlarmConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListListener(self, request):
         """获取转发监听器列表
 
         :param request: Request instance for DescribeListListener.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListListenerRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeListListenerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListPacketFilterConfig(self, request):
         """获取DDoS防护的特征过滤规则列表
 
         :param request: Request instance for DescribeListPacketFilterConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListPacketFilterConfigRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeListPacketFilterConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListPortAclList(self, request):
         """获取DDoS防护的端口acl策略列表
 
         :param request: Request instance for DescribeListPortAclList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListPortAclListRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeListPortAclListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListProtectThresholdConfig(self, request):
         """获取防护阈值配置列表，包括DDoS的AI、等级、CC阈值开关等
 
         :param request: Request instance for DescribeListProtectThresholdConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListProtectThresholdConfigRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeListProtectThresholdConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListProtocolBlockConfig(self, request):
         """获取DDoS防护的协议封禁配置列表
 
         :param request: Request instance for DescribeListProtocolBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListProtocolBlockConfigRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeListProtocolBlockConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListSchedulingDomain(self, request):
         """获取智能调度域名列表
 
         :param request: Request instance for DescribeListSchedulingDomain.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListSchedulingDomainRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeListSchedulingDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeListWaterPrintConfig(self, request):
         """获取DDoS防护的水印防护配置列表
 
         :param request: Request instance for DescribeListWaterPrintConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeListWaterPrintConfigRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeListWaterPrintConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewL7Rules(self, request):
         """高防IP获取7层规则
 
         :param request: Request instance for DescribeNewL7Rules.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeNewL7RulesRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribeNewL7RulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewL7RulesErrHealth(self, request):
         """获取L7转发规则健康检查异常结果列表
 
         :param request: Request instance for DescribeNewL7RulesErrHealth.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeNewL7RulesErrHealthRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeNewL7RulesErrHealthResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewAttackTrend(self, request):
         """拉取防护概览攻击趋势
 
         :param request: Request instance for DescribeOverviewAttackTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeOverviewAttackTrendRequest`
@@ -1675,15 +1675,15 @@
             model = models.DescribeOverviewAttackTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewCCTrend(self, request):
         """获取防护概览总请求峰值(QPS)和攻击请求(QPS)以及总请求次数和攻击请求次数
 
         :param request: Request instance for DescribeOverviewCCTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeOverviewCCTrendRequest`
@@ -1698,15 +1698,15 @@
             model = models.DescribeOverviewCCTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewDDoSEventList(self, request):
         """获取防护概览的ddos攻击事件
 
         :param request: Request instance for DescribeOverviewDDoSEventList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeOverviewDDoSEventListRequest`
@@ -1721,15 +1721,15 @@
             model = models.DescribeOverviewDDoSEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewDDoSTrend(self, request):
         """获取防护概览DDoS攻击流量带宽和攻击包速率数据
 
         :param request: Request instance for DescribeOverviewDDoSTrend.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeOverviewDDoSTrendRequest`
@@ -1744,15 +1744,15 @@
             model = models.DescribeOverviewDDoSTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOverviewIndex(self, request):
         """拉取防护概览指标
 
         :param request: Request instance for DescribeOverviewIndex.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribeOverviewIndexRequest`
@@ -1767,15 +1767,15 @@
             model = models.DescribeOverviewIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePendingRiskInfo(self, request):
         """查询账号维度待处理风险信息，包括是否为付费用户，查询攻击中、封堵中、过期资源数量等
 
         :param request: Request instance for DescribePendingRiskInfo.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DescribePendingRiskInfoRequest`
@@ -1790,15 +1790,15 @@
             model = models.DescribePendingRiskInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateDDoSEipAddress(self, request):
         """本接口 (DisassociateDDoSEipAddress) 用于解绑高防弹性公网IP。
 
         :param request: Request instance for DisassociateDDoSEipAddress.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.DisassociateDDoSEipAddressRequest`
@@ -1813,15 +1813,15 @@
             model = models.DisassociateDDoSEipAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCLevelPolicy(self, request):
         """修改CC防护等级
 
         :param request: Request instance for ModifyCCLevelPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyCCLevelPolicyRequest`
@@ -1836,15 +1836,15 @@
             model = models.ModifyCCLevelPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCPrecisionPolicy(self, request):
         """修改CC精准防护策略
 
         :param request: Request instance for ModifyCCPrecisionPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyCCPrecisionPolicyRequest`
@@ -1859,15 +1859,15 @@
             model = models.ModifyCCPrecisionPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCReqLimitPolicy(self, request):
         """修改CC频率限制策略
 
         :param request: Request instance for ModifyCCReqLimitPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyCCReqLimitPolicyRequest`
@@ -1882,15 +1882,15 @@
             model = models.ModifyCCReqLimitPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCCThresholdPolicy(self, request):
         """修改CC清洗阈值
 
         :param request: Request instance for ModifyCCThresholdPolicy.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyCCThresholdPolicyRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifyCCThresholdPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCcBlackWhiteIpList(self, request):
         """修改CC四层黑白名单
 
         :param request: Request instance for ModifyCcBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyCcBlackWhiteIpListRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyCcBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSBlackWhiteIpList(self, request):
         """修改DDoS黑白名单列表
 
         :param request: Request instance for ModifyDDoSBlackWhiteIpList.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDDoSBlackWhiteIpListRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyDDoSBlackWhiteIpListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSGeoIPBlockConfig(self, request):
         """修改DDoS防护的区域封禁配置
 
         :param request: Request instance for ModifyDDoSGeoIPBlockConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDDoSGeoIPBlockConfigRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyDDoSGeoIPBlockConfigResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDDoSLevelRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyDDoSLevelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDDoSSpeedLimitConfig(self, request):
         """修改DDoS防护的访问限速配置
 
         :param request: Request instance for ModifyDDoSSpeedLimitConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDDoSSpeedLimitConfigRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyDDoSSpeedLimitConfigResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDDoSThresholdRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyDDoSThresholdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainUsrName(self, request):
         """修改智能解析域名名称
 
         :param request: Request instance for ModifyDomainUsrName.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyDomainUsrNameRequest`
@@ -2066,15 +2066,15 @@
             model = models.ModifyDomainUsrNameResponse()
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
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyNewDomainRulesRequest`
@@ -2089,15 +2089,15 @@
             model = models.ModifyNewDomainRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPacketFilterConfig(self, request):
         """修改DDoS防护的特征过滤规则
 
         :param request: Request instance for ModifyPacketFilterConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyPacketFilterConfigRequest`
@@ -2112,15 +2112,15 @@
             model = models.ModifyPacketFilterConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPortAclConfig(self, request):
         """修改DDoS防护的端口acl策略
 
         :param request: Request instance for ModifyPortAclConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.ModifyPortAclConfigRequest`
@@ -2135,15 +2135,15 @@
             model = models.ModifyPortAclConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchWaterPrintConfig(self, request):
         """开启或关闭DDoS防护的水印防护配置
 
         :param request: Request instance for SwitchWaterPrintConfig.
         :type request: :class:`tencentcloud.antiddos.v20200309.models.SwitchWaterPrintConfigRequest`
@@ -2158,8 +2158,8 @@
             model = models.SwitchWaterPrintConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud/antiddos/v20200309/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.938/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.937/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.938/README.rst`

 * *Files identical despite different names*

