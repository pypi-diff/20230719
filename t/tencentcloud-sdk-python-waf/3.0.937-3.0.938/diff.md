# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.937.tar", last modified: Tue Jul 18 00:35:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.938.tar", last modified: Wed Jul 19 00:53:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.937.tar` & `tencentcloud-sdk-python-waf-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47458 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   309127 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    47662 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   309127 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:51.000000 tencentcloud-sdk-python-waf-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.937/setup.py` & `tencentcloud-sdk-python-waf-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddCustomRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddCustomWhiteRule(self, request):
         """增加精准白名单规则
 
         :param request: Request instance for AddCustomWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.AddCustomWhiteRuleRequest`
@@ -65,15 +65,15 @@
             model = models.AddCustomWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddDomainWhiteRule(self, request):
         """增加域名规则白名单
 
         :param request: Request instance for AddDomainWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.AddDomainWhiteRuleRequest`
@@ -88,15 +88,15 @@
             model = models.AddDomainWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddSpartaProtection(self, request):
         """添加Spart防护域名
 
         :param request: Request instance for AddSpartaProtection.
         :type request: :class:`tencentcloud.waf.v20180125.models.AddSpartaProtectionRequest`
@@ -111,15 +111,15 @@
             model = models.AddSpartaProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccessExport(self, request):
         """本接口用于创建访问日志导出
 
         :param request: Request instance for CreateAccessExport.
         :type request: :class:`tencentcloud.waf.v20180125.models.CreateAccessExportRequest`
@@ -134,15 +134,15 @@
             model = models.CreateAccessExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHost(self, request):
         """clb-waf中添加防护的域名
 
         :param request: Request instance for CreateHost.
         :type request: :class:`tencentcloud.waf.v20180125.models.CreateHostRequest`
@@ -157,15 +157,15 @@
             model = models.CreateHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccessExport(self, request):
         """本接口用于删除访问日志导出
 
         :param request: Request instance for DeleteAccessExport.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteAccessExportRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteAccessExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAttackDownloadRecord(self, request):
         """删除攻击日志下载任务记录
 
         :param request: Request instance for DeleteAttackDownloadRecord.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteAttackDownloadRecordRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteAttackDownloadRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomWhiteRule(self, request):
         """删除精准白名单规则
 
         :param request: Request instance for DeleteCustomWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteCustomWhiteRuleRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteCustomWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomainWhiteRules(self, request):
         """删除域名规则白名单
 
         :param request: Request instance for DeleteDomainWhiteRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteDomainWhiteRulesRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteDomainWhiteRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDownloadRecord(self, request):
         """删除访问日志下载记录
 
         :param request: Request instance for DeleteDownloadRecord.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteDownloadRecordRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteDownloadRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIpAccessControl(self, request):
         """Waf IP黑白名单Delete接口
 
         :param request: Request instance for DeleteIpAccessControl.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteIpAccessControlRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteIpAccessControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSession(self, request):
         """删除CC攻击的session设置
 
         :param request: Request instance for DeleteSession.
         :type request: :class:`tencentcloud.waf.v20180125.models.DeleteSessionRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessExports(self, request):
         """本接口用于获取访问日志导出列表
 
         :param request: Request instance for DescribeAccessExports.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAccessExportsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeAccessExportsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessFastAnalysis(self, request):
         """本接口用于访问日志的快速分析
 
         :param request: Request instance for DescribeAccessFastAnalysis.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAccessFastAnalysisRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeAccessFastAnalysisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessIndex(self, request):
         """本接口用于获取访问日志索引配置信息
 
         :param request: Request instance for DescribeAccessIndex.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAccessIndexRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeAccessIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAttackOverview(self, request):
         """攻击总览
 
         :param request: Request instance for DescribeAttackOverview.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAttackOverviewRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeAttackOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoDenyIP(self, request):
         """描述WAF自动封禁IP详情,对齐自动封堵状态
 
         :param request: Request instance for DescribeAutoDenyIP.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAutoDenyIPRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeAutoDenyIPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCustomWhiteRule(self, request):
         """获取防护配置中的精准白名单策略列表
 
         :param request: Request instance for DescribeCustomWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeCustomWhiteRuleRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeCustomWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainDetailsSaas(self, request):
         """查询单个saas域名详情
 
         :param request: Request instance for DescribeDomainDetailsSaas.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeDomainDetailsSaasRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeDomainDetailsSaasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainWhiteRules(self, request):
         """获取域名的规则白名单
 
         :param request: Request instance for DescribeDomainWhiteRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeDomainWhiteRulesRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeDomainWhiteRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomains(self, request):
         """查询用户所有域名的详细信息
 
         :param request: Request instance for DescribeDomains.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeDomainsRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeDomainsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowTrend(self, request):
         """获取waf流量访问趋势
 
         :param request: Request instance for DescribeFlowTrend.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeFlowTrendRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeFlowTrendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """查询用户所有实例的详细信息
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeInstancesRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpAccessControl(self, request):
         """Waf ip黑白名单查询
 
         :param request: Request instance for DescribeIpAccessControl.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeIpAccessControlRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeIpAccessControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIpHitItems(self, request):
         """Waf  IP封堵状态查询
 
         :param request: Request instance for DescribeIpHitItems.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeIpHitItemsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeIpHitItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePeakPoints(self, request):
         """查询业务和攻击概要趋势
 
         :param request: Request instance for DescribePeakPoints.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribePeakPointsRequest`
@@ -640,15 +640,15 @@
             model = models.DescribePeakPointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePeakValue(self, request):
         """获取业务和攻击概览峰值
 
         :param request: Request instance for DescribePeakValue.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribePeakValueRequest`
@@ -663,15 +663,15 @@
             model = models.DescribePeakValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicyStatus(self, request):
         """获取防护状态以及生效的实例id
 
         :param request: Request instance for DescribePolicyStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribePolicyStatusRequest`
@@ -686,15 +686,15 @@
             model = models.DescribePolicyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuleLimit(self, request):
         """获取各个模块具体的规格限制
 
         :param request: Request instance for DescribeRuleLimit.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeRuleLimitRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeRuleLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserCdcClbWafRegions(self, request):
         """在CDC场景下，负载均衡型WAF的添加、编辑域名配置的时候，需要展示CDC负载均衡型WAF（cdc-clb-waf)支持的地域列表，通过DescribeUserCdcClbWafRegions既可以获得当前对客户已经开放的地域列表
 
         :param request: Request instance for DescribeUserCdcClbWafRegions.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeUserCdcClbWafRegionsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeUserCdcClbWafRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserClbWafRegions(self, request):
         """在负载均衡型WAF的添加、编辑域名配置的时候，需要展示负载均衡型WAF（clb-waf)支持的地域列表，通过DescribeUserClbWafRegions既可以获得当前对客户已经开放的地域列表
 
         :param request: Request instance for DescribeUserClbWafRegions.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeUserClbWafRegionsRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeUserClbWafRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVipInfo(self, request):
         """根据过滤条件查询VIP信息
 
         :param request: Request instance for DescribeVipInfo.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeVipInfoRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeVipInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWafAutoDenyRules(self, request):
         """返回ip惩罚规则详细信息
 
         :param request: Request instance for DescribeWafAutoDenyRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeWafAutoDenyRulesRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeWafAutoDenyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWafAutoDenyStatus(self, request):
         """描述WAF自动封禁模块详情
 
         :param request: Request instance for DescribeWafAutoDenyStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeWafAutoDenyStatusRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeWafAutoDenyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWafThreatenIntelligence(self, request):
         """描述WAF威胁情报封禁模块配置详情
 
         :param request: Request instance for DescribeWafThreatenIntelligence.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeWafThreatenIntelligenceRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeWafThreatenIntelligenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAttackDownloadRecords(self, request):
         """查询下载攻击日志任务记录列表
 
         :param request: Request instance for GetAttackDownloadRecords.
         :type request: :class:`tencentcloud.waf.v20180125.models.GetAttackDownloadRecordsRequest`
@@ -870,15 +870,15 @@
             model = models.GetAttackDownloadRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccessPeriod(self, request):
         """本接口用于修改访问日志保存期限及大字段是否存储
 
         :param request: Request instance for ModifyAccessPeriod.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyAccessPeriodRequest`
@@ -893,15 +893,15 @@
             model = models.ModifyAccessPeriodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAreaBanStatus(self, request):
         """修改防护域名的地域封禁状态
 
         :param request: Request instance for ModifyAreaBanStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyAreaBanStatusRequest`
@@ -916,15 +916,15 @@
             model = models.ModifyAreaBanStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomRuleStatus(self, request):
         """开启或禁用访问控制（自定义策略）
 
         :param request: Request instance for ModifyCustomRuleStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyCustomRuleStatusRequest`
@@ -939,15 +939,15 @@
             model = models.ModifyCustomRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomWhiteRule(self, request):
         """编辑精准白名单
 
         :param request: Request instance for ModifyCustomWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyCustomWhiteRuleRequest`
@@ -962,15 +962,15 @@
             model = models.ModifyCustomWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainWhiteRule(self, request):
         """更改某一条规则
 
         :param request: Request instance for ModifyDomainWhiteRule.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyDomainWhiteRuleRequest`
@@ -985,15 +985,15 @@
             model = models.ModifyDomainWhiteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySpartaProtection(self, request):
         """修改域名配置
 
         :param request: Request instance for ModifySpartaProtection.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifySpartaProtectionRequest`
@@ -1008,15 +1008,15 @@
             model = models.ModifySpartaProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWafAutoDenyRules(self, request):
         """修改ip惩罚规则
 
         :param request: Request instance for ModifyWafAutoDenyRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyWafAutoDenyRulesRequest`
@@ -1031,15 +1031,15 @@
             model = models.ModifyWafAutoDenyRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWafAutoDenyStatus(self, request):
         """配置WAF自动封禁模块状态
 
         :param request: Request instance for ModifyWafAutoDenyStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyWafAutoDenyStatusRequest`
@@ -1054,15 +1054,15 @@
             model = models.ModifyWafAutoDenyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWafThreatenIntelligence(self, request):
         """配置WAF威胁情报封禁模块详情
 
         :param request: Request instance for ModifyWafThreatenIntelligence.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyWafThreatenIntelligenceRequest`
@@ -1077,15 +1077,15 @@
             model = models.ModifyWafThreatenIntelligenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PostAttackDownloadTask(self, request):
         """创建搜索下载攻击日志任务，使用CLS新版本的搜索下载getlog接口
 
         :param request: Request instance for PostAttackDownloadTask.
         :type request: :class:`tencentcloud.waf.v20180125.models.PostAttackDownloadTaskRequest`
@@ -1100,15 +1100,15 @@
             model = models.PostAttackDownloadTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchAccessLog(self, request):
         """本接口用于搜索WAF访问日志
 
         :param request: Request instance for SearchAccessLog.
         :type request: :class:`tencentcloud.waf.v20180125.models.SearchAccessLogRequest`
@@ -1123,15 +1123,15 @@
             model = models.SearchAccessLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchAttackLog(self, request):
         """新版本CLS接口存在参数变化，query改成了query_string支持lucence语法接口搜索查询。
 
         :param request: Request instance for SearchAttackLog.
         :type request: :class:`tencentcloud.waf.v20180125.models.SearchAttackLogRequest`
@@ -1146,15 +1146,15 @@
             model = models.SearchAttackLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchDomainRules(self, request):
         """切换域名的规则开关
 
         :param request: Request instance for SwitchDomainRules.
         :type request: :class:`tencentcloud.waf.v20180125.models.SwitchDomainRulesRequest`
@@ -1169,15 +1169,15 @@
             model = models.SwitchDomainRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpsertIpAccessControl(self, request):
         """Waf IP黑白名单Upsert接口
 
         :param request: Request instance for UpsertIpAccessControl.
         :type request: :class:`tencentcloud.waf.v20180125.models.UpsertIpAccessControlRequest`
@@ -1192,8 +1192,8 @@
             model = models.UpsertIpAccessControlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.938/tencentcloud/waf/v20180125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.938/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.937/README.rst` & `tencentcloud-sdk-python-waf-3.0.938/README.rst`

 * *Files identical despite different names*

