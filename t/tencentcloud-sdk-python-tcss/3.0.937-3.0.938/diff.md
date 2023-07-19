# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.937.tar", last modified: Tue Jul 18 00:31:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.938.tar", last modified: Wed Jul 19 00:49:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.937.tar` & `tencentcloud-sdk-python-tcss-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   317082 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1689506 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:31:56.000000 tencentcloud-sdk-python-tcss-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   318406 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1689506 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:49:21.000000 tencentcloud-sdk-python-tcss-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.938/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/setup.py` & `tencentcloud-sdk-python-tcss-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddAndPublishNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddAndPublishNetworkFirewallPolicyYamlDetail(self, request):
         """容器网络创建Yaml网络策略并发布任务
 
         :param request: Request instance for AddAndPublishNetworkFirewallPolicyYamlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddAndPublishNetworkFirewallPolicyYamlDetailRequest`
@@ -65,15 +65,15 @@
             model = models.AddAndPublishNetworkFirewallPolicyYamlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddAssetImageRegistryRegistryDetail(self, request):
         """新增单个镜像仓库详细信息
 
         :param request: Request instance for AddAssetImageRegistryRegistryDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddAssetImageRegistryRegistryDetailRequest`
@@ -88,15 +88,15 @@
             model = models.AddAssetImageRegistryRegistryDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddComplianceAssetPolicySetToWhitelist(self, request):
         """新增安全合规忽略(资产+检测项列表)列表，不显示指定的检查项包含的资产内容
         参考的AddCompliancePolicyItemToWhitelist，除输入字段外，其它应该是一致的，如果有不同可能是定义的不对
 
         :param request: Request instance for AddComplianceAssetPolicySetToWhitelist.
@@ -112,15 +112,15 @@
             model = models.AddComplianceAssetPolicySetToWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddCompliancePolicyAssetSetToWhitelist(self, request):
         """新增安全合规忽略(检测项+资产)列表，不显示指定的检查项包含的资产内容
         参考的AddCompliancePolicyItemToWhitelist，除输入字段外，其它应该是一致的，如果有不同可能是定义的不对
 
         :param request: Request instance for AddCompliancePolicyAssetSetToWhitelist.
@@ -136,15 +136,15 @@
             model = models.AddCompliancePolicyAssetSetToWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddCompliancePolicyItemToWhitelist(self, request):
         """将指定的检测项添加到白名单中，不显示未通过结果。
 
         :param request: Request instance for AddCompliancePolicyItemToWhitelist.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddCompliancePolicyItemToWhitelistRequest`
@@ -159,15 +159,15 @@
             model = models.AddCompliancePolicyItemToWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditAbnormalProcessRule(self, request):
         """添加编辑运行时异常进程策略
 
         :param request: Request instance for AddEditAbnormalProcessRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditAbnormalProcessRuleRequest`
@@ -182,15 +182,15 @@
             model = models.AddEditAbnormalProcessRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditAccessControlRule(self, request):
         """添加编辑运行时访问控制策略
 
         :param request: Request instance for AddEditAccessControlRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditAccessControlRuleRequest`
@@ -205,15 +205,15 @@
             model = models.AddEditAccessControlRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditImageAutoAuthorizedRule(self, request):
         """新增或编辑本地镜像自动授权规则
 
         :param request: Request instance for AddEditImageAutoAuthorizedRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditImageAutoAuthorizedRuleRequest`
@@ -228,15 +228,15 @@
             model = models.AddEditImageAutoAuthorizedRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditReverseShellWhiteList(self, request):
         """添加编辑运行时反弹shell白名单
 
         :param request: Request instance for AddEditReverseShellWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditReverseShellWhiteListRequest`
@@ -251,15 +251,15 @@
             model = models.AddEditReverseShellWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditRiskSyscallWhiteList(self, request):
         """添加编辑运行时高危系统调用白名单
 
         :param request: Request instance for AddEditRiskSyscallWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditRiskSyscallWhiteListRequest`
@@ -274,15 +274,15 @@
             model = models.AddEditRiskSyscallWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEditWarningRules(self, request):
         """添加编辑告警策略
 
         :param request: Request instance for AddEditWarningRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEditWarningRulesRequest`
@@ -297,15 +297,15 @@
             model = models.AddEditWarningRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddEscapeWhiteList(self, request):
         """新增逃逸白名单
 
         :param request: Request instance for AddEscapeWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddEscapeWhiteListRequest`
@@ -320,15 +320,15 @@
             model = models.AddEscapeWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddIgnoreVul(self, request):
         """新增漏洞扫描忽略漏洞
 
         :param request: Request instance for AddIgnoreVul.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddIgnoreVulRequest`
@@ -343,15 +343,15 @@
             model = models.AddIgnoreVulResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddNetworkFirewallPolicyDetail(self, request):
         """容器网络创建网络策略添加任务
 
         :param request: Request instance for AddNetworkFirewallPolicyDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddNetworkFirewallPolicyDetailRequest`
@@ -366,15 +366,15 @@
             model = models.AddNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddNetworkFirewallPolicyYamlDetail(self, request):
         """容器网络创建Yaml网络策略添加任务
 
         :param request: Request instance for AddNetworkFirewallPolicyYamlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.AddNetworkFirewallPolicyYamlDetailRequest`
@@ -389,15 +389,15 @@
             model = models.AddNetworkFirewallPolicyYamlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckNetworkFirewallPolicyYaml(self, request):
         """容器网络创建检查Yaml网络策略任务
 
         :param request: Request instance for CheckNetworkFirewallPolicyYaml.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CheckNetworkFirewallPolicyYamlRequest`
@@ -412,15 +412,15 @@
             model = models.CheckNetworkFirewallPolicyYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckRepeatAssetImageRegistry(self, request):
         """检查单个镜像仓库名是否重复
 
         :param request: Request instance for CheckRepeatAssetImageRegistry.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CheckRepeatAssetImageRegistryRequest`
@@ -435,15 +435,15 @@
             model = models.CheckRepeatAssetImageRegistryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ConfirmNetworkFirewallPolicy(self, request):
         """容器网络创建网络策略确认任务
 
         :param request: Request instance for ConfirmNetworkFirewallPolicy.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ConfirmNetworkFirewallPolicyRequest`
@@ -458,15 +458,15 @@
             model = models.ConfirmNetworkFirewallPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAbnormalProcessRulesExportJob(self, request):
         """创建异常进程规则导出任务
 
         :param request: Request instance for CreateAbnormalProcessRulesExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAbnormalProcessRulesExportJobRequest`
@@ -481,15 +481,15 @@
             model = models.CreateAbnormalProcessRulesExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccessControlsRuleExportJob(self, request):
         """创建文件篡改规则导出任务
 
         :param request: Request instance for CreateAccessControlsRuleExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAccessControlsRuleExportJobRequest`
@@ -504,15 +504,15 @@
             model = models.CreateAccessControlsRuleExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetImageRegistryScanTask(self, request):
         """镜像仓库创建镜像扫描任务
 
         :param request: Request instance for CreateAssetImageRegistryScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAssetImageRegistryScanTaskRequest`
@@ -527,15 +527,15 @@
             model = models.CreateAssetImageRegistryScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetImageRegistryScanTaskOneKey(self, request):
         """镜像仓库创建镜像一键扫描任务
 
         :param request: Request instance for CreateAssetImageRegistryScanTaskOneKey.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAssetImageRegistryScanTaskOneKeyRequest`
@@ -550,15 +550,15 @@
             model = models.CreateAssetImageRegistryScanTaskOneKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetImageScanSetting(self, request):
         """添加容器安全镜像扫描设置
 
         :param request: Request instance for CreateAssetImageScanSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAssetImageScanSettingRequest`
@@ -573,15 +573,15 @@
             model = models.CreateAssetImageScanSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetImageScanTask(self, request):
         """容器安全创建镜像扫描任务
 
         :param request: Request instance for CreateAssetImageScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAssetImageScanTaskRequest`
@@ -596,15 +596,15 @@
             model = models.CreateAssetImageScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetImageVirusExportJob(self, request):
         """创建本地镜像木马列表导出任务
 
         :param request: Request instance for CreateAssetImageVirusExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateAssetImageVirusExportJobRequest`
@@ -619,15 +619,15 @@
             model = models.CreateAssetImageVirusExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCheckComponent(self, request):
         """安装检查组件，创建防护容器
 
         :param request: Request instance for CreateCheckComponent.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateCheckComponentRequest`
@@ -642,15 +642,15 @@
             model = models.CreateCheckComponentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterCheckTask(self, request):
         """创建集群检查任务，用户检查用户的集群相关风险项
 
         :param request: Request instance for CreateClusterCheckTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateClusterCheckTaskRequest`
@@ -665,15 +665,15 @@
             model = models.CreateClusterCheckTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateComplianceTask(self, request):
         """创建合规检查任务，在资产级别触发重新检测时使用。
 
         :param request: Request instance for CreateComplianceTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateComplianceTaskRequest`
@@ -688,15 +688,15 @@
             model = models.CreateComplianceTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateComponentExportJob(self, request):
         """查询本地镜像组件列表导出
 
         :param request: Request instance for CreateComponentExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateComponentExportJobRequest`
@@ -711,15 +711,15 @@
             model = models.CreateComponentExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDefenceVulExportJob(self, request):
         """创建支持防御的漏洞导出任务
 
         :param request: Request instance for CreateDefenceVulExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateDefenceVulExportJobRequest`
@@ -734,15 +734,15 @@
             model = models.CreateDefenceVulExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEmergencyVulExportJob(self, request):
         """创建应急漏洞导出任务
 
         :param request: Request instance for CreateEmergencyVulExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateEmergencyVulExportJobRequest`
@@ -757,15 +757,15 @@
             model = models.CreateEmergencyVulExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEscapeEventsExportJob(self, request):
         """创建逃逸事件导出异步任务
 
         :param request: Request instance for CreateEscapeEventsExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateEscapeEventsExportJobRequest`
@@ -780,15 +780,15 @@
             model = models.CreateEscapeEventsExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEscapeWhiteListExportJob(self, request):
         """创建逃逸白名单导出任务
 
         :param request: Request instance for CreateEscapeWhiteListExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateEscapeWhiteListExportJobRequest`
@@ -803,15 +803,15 @@
             model = models.CreateEscapeWhiteListExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateExportComplianceStatusListJob(self, request):
         """创建一个导出安全合规信息的任务
 
         :param request: Request instance for CreateExportComplianceStatusListJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateExportComplianceStatusListJobRequest`
@@ -826,15 +826,15 @@
             model = models.CreateExportComplianceStatusListJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHostExportJob(self, request):
         """创建主机列表导出任务
 
         :param request: Request instance for CreateHostExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateHostExportJobRequest`
@@ -849,15 +849,15 @@
             model = models.CreateHostExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImageExportJob(self, request):
         """创建镜像导出任务
 
         :param request: Request instance for CreateImageExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateImageExportJobRequest`
@@ -872,15 +872,15 @@
             model = models.CreateImageExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateK8sApiAbnormalEventExportJob(self, request):
         """创建k8s api异常事件导出任务
 
         :param request: Request instance for CreateK8sApiAbnormalEventExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateK8sApiAbnormalEventExportJobRequest`
@@ -895,15 +895,15 @@
             model = models.CreateK8sApiAbnormalEventExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateK8sApiAbnormalRuleExportJob(self, request):
         """创建k8sApi异常规则导出任务
 
         :param request: Request instance for CreateK8sApiAbnormalRuleExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateK8sApiAbnormalRuleExportJobRequest`
@@ -918,15 +918,15 @@
             model = models.CreateK8sApiAbnormalRuleExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateK8sApiAbnormalRuleInfo(self, request):
         """创建k8sapi异常事件规则
 
         :param request: Request instance for CreateK8sApiAbnormalRuleInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateK8sApiAbnormalRuleInfoRequest`
@@ -941,15 +941,15 @@
             model = models.CreateK8sApiAbnormalRuleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkFirewallClusterRefresh(self, request):
         """容器网络集群下发刷新任务
 
         :param request: Request instance for CreateNetworkFirewallClusterRefresh.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateNetworkFirewallClusterRefreshRequest`
@@ -964,15 +964,15 @@
             model = models.CreateNetworkFirewallClusterRefreshResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkFirewallPolicyDiscover(self, request):
         """容器网络集群网络策略创建自动发现任务
 
         :param request: Request instance for CreateNetworkFirewallPolicyDiscover.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateNetworkFirewallPolicyDiscoverRequest`
@@ -987,15 +987,15 @@
             model = models.CreateNetworkFirewallPolicyDiscoverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkFirewallPublish(self, request):
         """容器网络创建网络策略发布任务
 
         :param request: Request instance for CreateNetworkFirewallPublish.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateNetworkFirewallPublishRequest`
@@ -1010,15 +1010,15 @@
             model = models.CreateNetworkFirewallPublishResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNetworkFirewallUndoPublish(self, request):
         """容器网络创建网络策略撤销任务
 
         :param request: Request instance for CreateNetworkFirewallUndoPublish.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateNetworkFirewallUndoPublishRequest`
@@ -1033,15 +1033,15 @@
             model = models.CreateNetworkFirewallUndoPublishResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrModifyPostPayCores(self, request):
         """CreateOrModifyPostPayCores  创建或者编辑弹性计费上限
 
         :param request: Request instance for CreateOrModifyPostPayCores.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateOrModifyPostPayCoresRequest`
@@ -1056,15 +1056,15 @@
             model = models.CreateOrModifyPostPayCoresResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProcessEventsExportJob(self, request):
         """创建异常进程事件导出异步任务
 
         :param request: Request instance for CreateProcessEventsExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateProcessEventsExportJobRequest`
@@ -1079,15 +1079,15 @@
             model = models.CreateProcessEventsExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRefreshTask(self, request):
         """下发刷新任务，会刷新资产信息
 
         :param request: Request instance for CreateRefreshTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateRefreshTaskRequest`
@@ -1102,15 +1102,15 @@
             model = models.CreateRefreshTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRiskDnsEventExportJob(self, request):
         """创建恶意请求事件导出任务
 
         :param request: Request instance for CreateRiskDnsEventExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateRiskDnsEventExportJobRequest`
@@ -1125,15 +1125,15 @@
             model = models.CreateRiskDnsEventExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSearchTemplate(self, request):
         """添加检索模板
 
         :param request: Request instance for CreateSearchTemplate.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateSearchTemplateRequest`
@@ -1148,15 +1148,15 @@
             model = models.CreateSearchTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSystemVulExportJob(self, request):
         """创建系统漏洞导出任务
 
         :param request: Request instance for CreateSystemVulExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateSystemVulExportJobRequest`
@@ -1171,15 +1171,15 @@
             model = models.CreateSystemVulExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVirusScanAgain(self, request):
         """运行时文件查杀重新检测
 
         :param request: Request instance for CreateVirusScanAgain.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVirusScanAgainRequest`
@@ -1194,15 +1194,15 @@
             model = models.CreateVirusScanAgainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVirusScanTask(self, request):
         """运行时文件查杀一键扫描
 
         :param request: Request instance for CreateVirusScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVirusScanTaskRequest`
@@ -1217,15 +1217,15 @@
             model = models.CreateVirusScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulContainerExportJob(self, request):
         """创建受漏洞影响的容器导出任务
 
         :param request: Request instance for CreateVulContainerExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulContainerExportJobRequest`
@@ -1240,15 +1240,15 @@
             model = models.CreateVulContainerExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulDefenceEventExportJob(self, request):
         """创建漏洞防御导出任务
 
         :param request: Request instance for CreateVulDefenceEventExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulDefenceEventExportJobRequest`
@@ -1263,15 +1263,15 @@
             model = models.CreateVulDefenceEventExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulDefenceHostExportJob(self, request):
         """创建漏洞防御主机导出任务
 
         :param request: Request instance for CreateVulDefenceHostExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulDefenceHostExportJobRequest`
@@ -1286,15 +1286,15 @@
             model = models.CreateVulDefenceHostExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulExportJob(self, request):
         """查询本地镜像漏洞列表导出
 
         :param request: Request instance for CreateVulExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulExportJobRequest`
@@ -1309,15 +1309,15 @@
             model = models.CreateVulExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulImageExportJob(self, request):
         """创建受漏洞影响的镜像导出任务
 
         :param request: Request instance for CreateVulImageExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulImageExportJobRequest`
@@ -1332,15 +1332,15 @@
             model = models.CreateVulImageExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVulScanTask(self, request):
         """创建漏洞扫描任务
 
         :param request: Request instance for CreateVulScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateVulScanTaskRequest`
@@ -1355,15 +1355,15 @@
             model = models.CreateVulScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWebVulExportJob(self, request):
         """创建web漏洞导出任务
 
         :param request: Request instance for CreateWebVulExportJob.
         :type request: :class:`tencentcloud.tcss.v20201101.models.CreateWebVulExportJobRequest`
@@ -1378,15 +1378,15 @@
             model = models.CreateWebVulExportJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAbnormalProcessRules(self, request):
         """删除运行异常进程策略
 
         :param request: Request instance for DeleteAbnormalProcessRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteAbnormalProcessRulesRequest`
@@ -1401,15 +1401,15 @@
             model = models.DeleteAbnormalProcessRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccessControlRules(self, request):
         """删除运行访问控制策略
 
         :param request: Request instance for DeleteAccessControlRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteAccessControlRulesRequest`
@@ -1424,15 +1424,15 @@
             model = models.DeleteAccessControlRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteComplianceAssetPolicySetFromWhitelist(self, request):
         """移除安全合规忽略(资产+检测项)列表，不显示指定的检查项包含的资产内容
         参考的AddCompliancePolicyAssetSetToWhitelist，除输入字段外，其它应该是一致的，如果有不同可能是定义的不对
 
         :param request: Request instance for DeleteComplianceAssetPolicySetFromWhitelist.
@@ -1448,15 +1448,15 @@
             model = models.DeleteComplianceAssetPolicySetFromWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCompliancePolicyAssetSetFromWhitelist(self, request):
         """新增安全合规忽略(检测项+资产)列表，不显示指定的检查项包含的资产内容
 
         :param request: Request instance for DeleteCompliancePolicyAssetSetFromWhitelist.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteCompliancePolicyAssetSetFromWhitelistRequest`
@@ -1471,15 +1471,15 @@
             model = models.DeleteCompliancePolicyAssetSetFromWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCompliancePolicyItemFromWhitelist(self, request):
         """从白名单中删除将指定的检测项。
 
         :param request: Request instance for DeleteCompliancePolicyItemFromWhitelist.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteCompliancePolicyItemFromWhitelistRequest`
@@ -1494,15 +1494,15 @@
             model = models.DeleteCompliancePolicyItemFromWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEscapeWhiteList(self, request):
         """删除逃逸白名单
 
         :param request: Request instance for DeleteEscapeWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteEscapeWhiteListRequest`
@@ -1517,15 +1517,15 @@
             model = models.DeleteEscapeWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIgnoreVul(self, request):
         """取消漏洞扫描忽略漏洞
 
         :param request: Request instance for DeleteIgnoreVul.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteIgnoreVulRequest`
@@ -1540,15 +1540,15 @@
             model = models.DeleteIgnoreVulResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteK8sApiAbnormalRule(self, request):
         """删除k8sapi异常事件规则
 
         :param request: Request instance for DeleteK8sApiAbnormalRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteK8sApiAbnormalRuleRequest`
@@ -1563,15 +1563,15 @@
             model = models.DeleteK8sApiAbnormalRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMachine(self, request):
         """卸载Agent客户端
 
         :param request: Request instance for DeleteMachine.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteMachineRequest`
@@ -1586,15 +1586,15 @@
             model = models.DeleteMachineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNetworkFirewallPolicyDetail(self, request):
         """容器网络创建网络策略删除任务
 
         :param request: Request instance for DeleteNetworkFirewallPolicyDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteNetworkFirewallPolicyDetailRequest`
@@ -1609,15 +1609,15 @@
             model = models.DeleteNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReverseShellEvents(self, request):
         """删除运行时反弹shell事件
 
         :param request: Request instance for DeleteReverseShellEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteReverseShellEventsRequest`
@@ -1632,15 +1632,15 @@
             model = models.DeleteReverseShellEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReverseShellWhiteLists(self, request):
         """删除运行时反弹shell白名单
 
         :param request: Request instance for DeleteReverseShellWhiteLists.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteReverseShellWhiteListsRequest`
@@ -1655,15 +1655,15 @@
             model = models.DeleteReverseShellWhiteListsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRiskSyscallEvents(self, request):
         """删除运行时高危系统调用事件
 
         :param request: Request instance for DeleteRiskSyscallEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteRiskSyscallEventsRequest`
@@ -1678,15 +1678,15 @@
             model = models.DeleteRiskSyscallEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRiskSyscallWhiteLists(self, request):
         """删除运行时高危系统调用白名单
 
         :param request: Request instance for DeleteRiskSyscallWhiteLists.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteRiskSyscallWhiteListsRequest`
@@ -1701,15 +1701,15 @@
             model = models.DeleteRiskSyscallWhiteListsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSearchTemplate(self, request):
         """删除检索模板
 
         :param request: Request instance for DeleteSearchTemplate.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DeleteSearchTemplateRequest`
@@ -1724,15 +1724,15 @@
             model = models.DeleteSearchTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeABTestConfig(self, request):
         """获取用户当前灰度配置
 
         :param request: Request instance for DescribeABTestConfig.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeABTestConfigRequest`
@@ -1747,15 +1747,15 @@
             model = models.DescribeABTestConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessDetail(self, request):
         """查询运行时异常进程事件详细信息
 
         :param request: Request instance for DescribeAbnormalProcessDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessDetailRequest`
@@ -1770,15 +1770,15 @@
             model = models.DescribeAbnormalProcessDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessEventTendency(self, request):
         """查询待处理异常进程事件趋势
 
         :param request: Request instance for DescribeAbnormalProcessEventTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessEventTendencyRequest`
@@ -1793,15 +1793,15 @@
             model = models.DescribeAbnormalProcessEventTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessEvents(self, request):
         """查询运行时异常进程事件列表信息
 
         :param request: Request instance for DescribeAbnormalProcessEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessEventsRequest`
@@ -1816,15 +1816,15 @@
             model = models.DescribeAbnormalProcessEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessEventsExport(self, request):
         """查询运行时异常进程事件列表信息导出
 
         :param request: Request instance for DescribeAbnormalProcessEventsExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessEventsExportRequest`
@@ -1839,15 +1839,15 @@
             model = models.DescribeAbnormalProcessEventsExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessLevelSummary(self, request):
         """统计异常进程各威胁等级待处理事件数
 
         :param request: Request instance for DescribeAbnormalProcessLevelSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessLevelSummaryRequest`
@@ -1862,15 +1862,15 @@
             model = models.DescribeAbnormalProcessLevelSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessRuleDetail(self, request):
         """查询运行时异常策略详细信息
 
         :param request: Request instance for DescribeAbnormalProcessRuleDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessRuleDetailRequest`
@@ -1885,15 +1885,15 @@
             model = models.DescribeAbnormalProcessRuleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessRules(self, request):
         """查询运行时异常进程策略列表信息
 
         :param request: Request instance for DescribeAbnormalProcessRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessRulesRequest`
@@ -1908,15 +1908,15 @@
             model = models.DescribeAbnormalProcessRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAbnormalProcessRulesExport(self, request):
         """查询运行时异常进程策略列表信息导出
 
         :param request: Request instance for DescribeAbnormalProcessRulesExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAbnormalProcessRulesExportRequest`
@@ -1931,15 +1931,15 @@
             model = models.DescribeAbnormalProcessRulesExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlDetail(self, request):
         """查询运行时访问控制事件的详细信息
 
         :param request: Request instance for DescribeAccessControlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlDetailRequest`
@@ -1954,15 +1954,15 @@
             model = models.DescribeAccessControlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlEvents(self, request):
         """查询运行时访问控制事件列表
 
         :param request: Request instance for DescribeAccessControlEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlEventsRequest`
@@ -1977,15 +1977,15 @@
             model = models.DescribeAccessControlEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlEventsExport(self, request):
         """查询运行时访问控制事件列表导出
 
         :param request: Request instance for DescribeAccessControlEventsExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlEventsExportRequest`
@@ -2000,15 +2000,15 @@
             model = models.DescribeAccessControlEventsExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlRuleDetail(self, request):
         """查询运行时访问控制策略详细信息
 
         :param request: Request instance for DescribeAccessControlRuleDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlRuleDetailRequest`
@@ -2023,15 +2023,15 @@
             model = models.DescribeAccessControlRuleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlRules(self, request):
         """查询运行访问控制策略列表信息
 
         :param request: Request instance for DescribeAccessControlRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlRulesRequest`
@@ -2046,15 +2046,15 @@
             model = models.DescribeAccessControlRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessControlRulesExport(self, request):
         """查询运行时访问控制策略列表导出
 
         :param request: Request instance for DescribeAccessControlRulesExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAccessControlRulesExportRequest`
@@ -2069,15 +2069,15 @@
             model = models.DescribeAccessControlRulesExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAffectedClusterCount(self, request):
         """获取受影响的集群数量，返回数量
 
         :param request: Request instance for DescribeAffectedClusterCount.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAffectedClusterCountRequest`
@@ -2092,15 +2092,15 @@
             model = models.DescribeAffectedClusterCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAffectedNodeList(self, request):
         """查询节点类型的影响范围，返回节点列表
 
         :param request: Request instance for DescribeAffectedNodeList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAffectedNodeListRequest`
@@ -2115,15 +2115,15 @@
             model = models.DescribeAffectedNodeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAffectedWorkloadList(self, request):
         """查询workload类型的影响范围，返回workload列表
 
         :param request: Request instance for DescribeAffectedWorkloadList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAffectedWorkloadListRequest`
@@ -2138,15 +2138,15 @@
             model = models.DescribeAffectedWorkloadListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentDaemonSetCmd(self, request):
         """查询平行容器安装命令
 
         :param request: Request instance for DescribeAgentDaemonSetCmd.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAgentDaemonSetCmdRequest`
@@ -2161,15 +2161,15 @@
             model = models.DescribeAgentDaemonSetCmdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAgentInstallCommand(self, request):
         """查询agent安装命令
 
         :param request: Request instance for DescribeAgentInstallCommand.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAgentInstallCommandRequest`
@@ -2184,15 +2184,15 @@
             model = models.DescribeAgentInstallCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetAppServiceList(self, request):
         """容器安全查询app服务列表
 
         :param request: Request instance for DescribeAssetAppServiceList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetAppServiceListRequest`
@@ -2207,15 +2207,15 @@
             model = models.DescribeAssetAppServiceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetClusterList(self, request):
         """查询集群列表
 
         :param request: Request instance for DescribeAssetClusterList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetClusterListRequest`
@@ -2230,15 +2230,15 @@
             model = models.DescribeAssetClusterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetComponentList(self, request):
         """容器安全搜索查询容器组件列表
 
         :param request: Request instance for DescribeAssetComponentList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetComponentListRequest`
@@ -2253,15 +2253,15 @@
             model = models.DescribeAssetComponentListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetContainerDetail(self, request):
         """查询容器详细信息
 
         :param request: Request instance for DescribeAssetContainerDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetContainerDetailRequest`
@@ -2276,15 +2276,15 @@
             model = models.DescribeAssetContainerDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetContainerList(self, request):
         """搜索查询容器列表
 
         :param request: Request instance for DescribeAssetContainerList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetContainerListRequest`
@@ -2299,15 +2299,15 @@
             model = models.DescribeAssetContainerListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetDBServiceList(self, request):
         """容器安全查询db服务列表
 
         :param request: Request instance for DescribeAssetDBServiceList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetDBServiceListRequest`
@@ -2322,15 +2322,15 @@
             model = models.DescribeAssetDBServiceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetHostDetail(self, request):
         """查询主机详细信息
 
         :param request: Request instance for DescribeAssetHostDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetHostDetailRequest`
@@ -2345,15 +2345,15 @@
             model = models.DescribeAssetHostDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetHostList(self, request):
         """容器安全搜索查询主机列表
 
         :param request: Request instance for DescribeAssetHostList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetHostListRequest`
@@ -2368,15 +2368,15 @@
             model = models.DescribeAssetHostListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageBindRuleInfo(self, request):
         """镜像绑定规则列表信息，包含运行时访问控制和异常进程公用
 
         :param request: Request instance for DescribeAssetImageBindRuleInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageBindRuleInfoRequest`
@@ -2391,15 +2391,15 @@
             model = models.DescribeAssetImageBindRuleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageDetail(self, request):
         """查询镜像详细信息
 
         :param request: Request instance for DescribeAssetImageDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageDetailRequest`
@@ -2414,15 +2414,15 @@
             model = models.DescribeAssetImageDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageHostList(self, request):
         """容器安全查询镜像关联主机
 
         :param request: Request instance for DescribeAssetImageHostList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageHostListRequest`
@@ -2437,15 +2437,15 @@
             model = models.DescribeAssetImageHostListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageList(self, request):
         """容器安全搜索查询镜像列表
 
         :param request: Request instance for DescribeAssetImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageListRequest`
@@ -2460,15 +2460,15 @@
             model = models.DescribeAssetImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageListExport(self, request):
         """容器安全搜索查询镜像列表导出
 
         :param request: Request instance for DescribeAssetImageListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageListExportRequest`
@@ -2483,15 +2483,15 @@
             model = models.DescribeAssetImageListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryAssetStatus(self, request):
         """查看镜像仓库资产更新进度状态
 
         :param request: Request instance for DescribeAssetImageRegistryAssetStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryAssetStatusRequest`
@@ -2506,15 +2506,15 @@
             model = models.DescribeAssetImageRegistryAssetStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryDetail(self, request):
         """镜像仓库镜像仓库列表详情
 
         :param request: Request instance for DescribeAssetImageRegistryDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryDetailRequest`
@@ -2529,15 +2529,15 @@
             model = models.DescribeAssetImageRegistryDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryList(self, request):
         """镜像仓库镜像仓库列表
 
         :param request: Request instance for DescribeAssetImageRegistryList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryListRequest`
@@ -2552,15 +2552,15 @@
             model = models.DescribeAssetImageRegistryListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryListExport(self, request):
         """镜像仓库镜像列表导出
 
         :param request: Request instance for DescribeAssetImageRegistryListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryListExportRequest`
@@ -2575,15 +2575,15 @@
             model = models.DescribeAssetImageRegistryListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryRegistryDetail(self, request):
         """查看单个镜像仓库详细信息
 
         :param request: Request instance for DescribeAssetImageRegistryRegistryDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryRegistryDetailRequest`
@@ -2598,15 +2598,15 @@
             model = models.DescribeAssetImageRegistryRegistryDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryRegistryList(self, request):
         """镜像仓库仓库列表
 
         :param request: Request instance for DescribeAssetImageRegistryRegistryList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryRegistryListRequest`
@@ -2621,15 +2621,15 @@
             model = models.DescribeAssetImageRegistryRegistryListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryRiskInfoList(self, request):
         """镜像仓库查询镜像高危行为列表
 
         :param request: Request instance for DescribeAssetImageRegistryRiskInfoList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryRiskInfoListRequest`
@@ -2644,15 +2644,15 @@
             model = models.DescribeAssetImageRegistryRiskInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryRiskListExport(self, request):
         """镜像仓库敏感信息列表导出
 
         :param request: Request instance for DescribeAssetImageRegistryRiskListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryRiskListExportRequest`
@@ -2667,15 +2667,15 @@
             model = models.DescribeAssetImageRegistryRiskListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryScanStatusOneKey(self, request):
         """镜像仓库查询一键镜像扫描状态
 
         :param request: Request instance for DescribeAssetImageRegistryScanStatusOneKey.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryScanStatusOneKeyRequest`
@@ -2690,15 +2690,15 @@
             model = models.DescribeAssetImageRegistryScanStatusOneKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistrySummary(self, request):
         """镜像仓库查询镜像统计信息
 
         :param request: Request instance for DescribeAssetImageRegistrySummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistrySummaryRequest`
@@ -2713,15 +2713,15 @@
             model = models.DescribeAssetImageRegistrySummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryVirusList(self, request):
         """镜像仓库查询木马病毒列表
 
         :param request: Request instance for DescribeAssetImageRegistryVirusList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryVirusListRequest`
@@ -2736,15 +2736,15 @@
             model = models.DescribeAssetImageRegistryVirusListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryVirusListExport(self, request):
         """镜像仓库木马信息列表导出
 
         :param request: Request instance for DescribeAssetImageRegistryVirusListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryVirusListExportRequest`
@@ -2759,15 +2759,15 @@
             model = models.DescribeAssetImageRegistryVirusListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryVulList(self, request):
         """镜像仓库查询镜像漏洞列表
 
         :param request: Request instance for DescribeAssetImageRegistryVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryVulListRequest`
@@ -2782,15 +2782,15 @@
             model = models.DescribeAssetImageRegistryVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRegistryVulListExport(self, request):
         """镜像仓库漏洞列表导出
 
         :param request: Request instance for DescribeAssetImageRegistryVulListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRegistryVulListExportRequest`
@@ -2805,15 +2805,15 @@
             model = models.DescribeAssetImageRegistryVulListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRiskList(self, request):
         """容器安全查询镜像风险列表
 
         :param request: Request instance for DescribeAssetImageRiskList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRiskListRequest`
@@ -2828,15 +2828,15 @@
             model = models.DescribeAssetImageRiskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageRiskListExport(self, request):
         """容器安全搜索查询镜像风险列表导出
 
         :param request: Request instance for DescribeAssetImageRiskListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageRiskListExportRequest`
@@ -2851,15 +2851,15 @@
             model = models.DescribeAssetImageRiskListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageScanSetting(self, request):
         """获取镜像扫描设置信息
 
         :param request: Request instance for DescribeAssetImageScanSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageScanSettingRequest`
@@ -2874,15 +2874,15 @@
             model = models.DescribeAssetImageScanSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageScanStatus(self, request):
         """容器安全查询镜像扫描状态
 
         :param request: Request instance for DescribeAssetImageScanStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageScanStatusRequest`
@@ -2897,15 +2897,15 @@
             model = models.DescribeAssetImageScanStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageScanTask(self, request):
         """查询正在一键扫描的镜像扫描taskid
 
         :param request: Request instance for DescribeAssetImageScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageScanTaskRequest`
@@ -2920,15 +2920,15 @@
             model = models.DescribeAssetImageScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageSimpleList(self, request):
         """容器安全搜索查询镜像简略信息列表
 
         :param request: Request instance for DescribeAssetImageSimpleList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageSimpleListRequest`
@@ -2943,15 +2943,15 @@
             model = models.DescribeAssetImageSimpleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageVirusList(self, request):
         """容器安全查询镜像病毒列表
 
         :param request: Request instance for DescribeAssetImageVirusList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageVirusListRequest`
@@ -2966,15 +2966,15 @@
             model = models.DescribeAssetImageVirusListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageVirusListExport(self, request):
         """容器安全搜索查询镜像木马列表导出
 
         :param request: Request instance for DescribeAssetImageVirusListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageVirusListExportRequest`
@@ -2989,15 +2989,15 @@
             model = models.DescribeAssetImageVirusListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageVulList(self, request):
         """容器安全查询镜像漏洞列表
 
         :param request: Request instance for DescribeAssetImageVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageVulListRequest`
@@ -3012,15 +3012,15 @@
             model = models.DescribeAssetImageVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetImageVulListExport(self, request):
         """容器安全搜索查询镜像漏洞列表导出
 
         :param request: Request instance for DescribeAssetImageVulListExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetImageVulListExportRequest`
@@ -3035,15 +3035,15 @@
             model = models.DescribeAssetImageVulListExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetPortList(self, request):
         """容器安全搜索查询端口占用列表
 
         :param request: Request instance for DescribeAssetPortList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetPortListRequest`
@@ -3058,15 +3058,15 @@
             model = models.DescribeAssetPortListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetProcessList(self, request):
         """容器安全搜索查询进程列表
 
         :param request: Request instance for DescribeAssetProcessList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetProcessListRequest`
@@ -3081,15 +3081,15 @@
             model = models.DescribeAssetProcessListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetSummary(self, request):
         """查询账户容器、镜像等统计信息
 
         :param request: Request instance for DescribeAssetSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetSummaryRequest`
@@ -3104,15 +3104,15 @@
             model = models.DescribeAssetSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetSyncLastTime(self, request):
         """查询资产同步最近时间
 
         :param request: Request instance for DescribeAssetSyncLastTime.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetSyncLastTimeRequest`
@@ -3127,15 +3127,15 @@
             model = models.DescribeAssetSyncLastTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetWebServiceList(self, request):
         """容器安全查询web服务列表
 
         :param request: Request instance for DescribeAssetWebServiceList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAssetWebServiceListRequest`
@@ -3150,15 +3150,15 @@
             model = models.DescribeAssetWebServiceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoAuthorizedRuleHost(self, request):
         """查询自动授权规则授权范围主机信息
 
         :param request: Request instance for DescribeAutoAuthorizedRuleHost.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeAutoAuthorizedRuleHostRequest`
@@ -3173,15 +3173,15 @@
             model = models.DescribeAutoAuthorizedRuleHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCheckItemList(self, request):
         """查询所有检查项接口，返回总数和检查项列表
 
         :param request: Request instance for DescribeCheckItemList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeCheckItemListRequest`
@@ -3196,15 +3196,15 @@
             model = models.DescribeCheckItemListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterDetail(self, request):
         """查询单个集群的详细信息
 
         :param request: Request instance for DescribeClusterDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeClusterDetailRequest`
@@ -3219,15 +3219,15 @@
             model = models.DescribeClusterDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterSummary(self, request):
         """查询用户集群资产总览
 
         :param request: Request instance for DescribeClusterSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeClusterSummaryRequest`
@@ -3242,15 +3242,15 @@
             model = models.DescribeClusterSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceAssetDetailInfo(self, request):
         """查询某个资产的详情
 
         :param request: Request instance for DescribeComplianceAssetDetailInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceAssetDetailInfoRequest`
@@ -3265,15 +3265,15 @@
             model = models.DescribeComplianceAssetDetailInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceAssetList(self, request):
         """查询某类资产的列表
 
         :param request: Request instance for DescribeComplianceAssetList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceAssetListRequest`
@@ -3288,15 +3288,15 @@
             model = models.DescribeComplianceAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceAssetPolicyItemList(self, request):
         """查询某资产下的检测项列表
 
         :param request: Request instance for DescribeComplianceAssetPolicyItemList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceAssetPolicyItemListRequest`
@@ -3311,15 +3311,15 @@
             model = models.DescribeComplianceAssetPolicyItemListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompliancePeriodTaskList(self, request):
         """查询合规检测的定时任务列表
 
         :param request: Request instance for DescribeCompliancePeriodTaskList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeCompliancePeriodTaskListRequest`
@@ -3334,15 +3334,15 @@
             model = models.DescribeCompliancePeriodTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompliancePolicyItemAffectedAssetList(self, request):
         """按照 检测项 → 资产 的两级层次展开的第二层级：资产层级。
 
         :param request: Request instance for DescribeCompliancePolicyItemAffectedAssetList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeCompliancePolicyItemAffectedAssetListRequest`
@@ -3357,15 +3357,15 @@
             model = models.DescribeCompliancePolicyItemAffectedAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCompliancePolicyItemAffectedSummary(self, request):
         """按照 检测项 → 资产 的两级层次展开的第一层级：检测项层级。
 
         :param request: Request instance for DescribeCompliancePolicyItemAffectedSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeCompliancePolicyItemAffectedSummaryRequest`
@@ -3380,15 +3380,15 @@
             model = models.DescribeCompliancePolicyItemAffectedSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceScanFailedAssetList(self, request):
         """按照 资产 → 检测项 二层结构展示的信息。这里查询第一层 资产的通过率汇总信息。
 
         :param request: Request instance for DescribeComplianceScanFailedAssetList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceScanFailedAssetListRequest`
@@ -3403,15 +3403,15 @@
             model = models.DescribeComplianceScanFailedAssetListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceTaskAssetSummary(self, request):
         """查询上次任务的资产通过率汇总信息
 
         :param request: Request instance for DescribeComplianceTaskAssetSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceTaskAssetSummaryRequest`
@@ -3426,15 +3426,15 @@
             model = models.DescribeComplianceTaskAssetSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceTaskPolicyItemSummaryList(self, request):
         """查询最近一次任务发现的检测项的汇总信息列表，按照 检测项 → 资产 的两级层次展开。
 
         :param request: Request instance for DescribeComplianceTaskPolicyItemSummaryList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceTaskPolicyItemSummaryListRequest`
@@ -3449,15 +3449,15 @@
             model = models.DescribeComplianceTaskPolicyItemSummaryListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeComplianceWhitelistItemList(self, request):
         """查询白名单列表
 
         :param request: Request instance for DescribeComplianceWhitelistItemList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeComplianceWhitelistItemListRequest`
@@ -3472,15 +3472,15 @@
             model = models.DescribeComplianceWhitelistItemListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerAssetSummary(self, request):
         """查询容器资产概览信息
 
         :param request: Request instance for DescribeContainerAssetSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeContainerAssetSummaryRequest`
@@ -3495,15 +3495,15 @@
             model = models.DescribeContainerAssetSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContainerSecEventSummary(self, request):
         """查询容器安全未处理事件信息
 
         :param request: Request instance for DescribeContainerSecEventSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeContainerSecEventSummaryRequest`
@@ -3518,15 +3518,15 @@
             model = models.DescribeContainerSecEventSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeESAggregations(self, request):
         """获取ES字段聚合结果
 
         :param request: Request instance for DescribeESAggregations.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeESAggregationsRequest`
@@ -3541,15 +3541,15 @@
             model = models.DescribeESAggregationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeESHits(self, request):
         """获取ES查询文档列表
 
         :param request: Request instance for DescribeESHits.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeESHitsRequest`
@@ -3564,15 +3564,15 @@
             model = models.DescribeESHitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEmergencyVulList(self, request):
         """查询应急漏洞列表
 
         :param request: Request instance for DescribeEmergencyVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEmergencyVulListRequest`
@@ -3587,15 +3587,15 @@
             model = models.DescribeEmergencyVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeEventDetail(self, request):
         """DescribeEscapeEventDetail  查询容器逃逸事件详情
 
         :param request: Request instance for DescribeEscapeEventDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeEventDetailRequest`
@@ -3610,15 +3610,15 @@
             model = models.DescribeEscapeEventDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeEventInfo(self, request):
         """DescribeEscapeEventInfo 查询容器逃逸事件列表
 
         :param request: Request instance for DescribeEscapeEventInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeEventInfoRequest`
@@ -3633,15 +3633,15 @@
             model = models.DescribeEscapeEventInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeEventTendency(self, request):
         """查询待处理逃逸事件趋势
 
         :param request: Request instance for DescribeEscapeEventTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeEventTendencyRequest`
@@ -3656,15 +3656,15 @@
             model = models.DescribeEscapeEventTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeEventTypeSummary(self, request):
         """统计容器逃逸各事件类型和待处理事件数
 
         :param request: Request instance for DescribeEscapeEventTypeSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeEventTypeSummaryRequest`
@@ -3679,15 +3679,15 @@
             model = models.DescribeEscapeEventTypeSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeEventsExport(self, request):
         """DescribeEscapeEventsExport  查询容器逃逸事件列表导出
 
         :param request: Request instance for DescribeEscapeEventsExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeEventsExportRequest`
@@ -3702,15 +3702,15 @@
             model = models.DescribeEscapeEventsExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeRuleInfo(self, request):
         """DescribeEscapeRuleInfo 查询容器逃逸扫描规则信息
 
         :param request: Request instance for DescribeEscapeRuleInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeRuleInfoRequest`
@@ -3725,15 +3725,15 @@
             model = models.DescribeEscapeRuleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeSafeState(self, request):
         """DescribeEscapeSafeState 查询容器逃逸安全状态
 
         :param request: Request instance for DescribeEscapeSafeState.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeSafeStateRequest`
@@ -3748,15 +3748,15 @@
             model = models.DescribeEscapeSafeStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEscapeWhiteList(self, request):
         """查询逃逸白名单
 
         :param request: Request instance for DescribeEscapeWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeEscapeWhiteListRequest`
@@ -3771,15 +3771,15 @@
             model = models.DescribeEscapeWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExportJobDownloadURL(self, request):
         """查询导出任务下载URL
 
         :param request: Request instance for DescribeExportJobDownloadURL.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeExportJobDownloadURLRequest`
@@ -3794,15 +3794,15 @@
             model = models.DescribeExportJobDownloadURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExportJobManageList(self, request):
         """查询导出任务管理列表
 
         :param request: Request instance for DescribeExportJobManageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeExportJobManageListRequest`
@@ -3817,15 +3817,15 @@
             model = models.DescribeExportJobManageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExportJobResult(self, request):
         """查询导出任务的结果
 
         :param request: Request instance for DescribeExportJobResult.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeExportJobResultRequest`
@@ -3840,15 +3840,15 @@
             model = models.DescribeExportJobResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageAuthorizedInfo(self, request):
         """DescribeImageAuthorizedInfo  查询镜像授权信息
 
         :param request: Request instance for DescribeImageAuthorizedInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageAuthorizedInfoRequest`
@@ -3863,15 +3863,15 @@
             model = models.DescribeImageAuthorizedInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageAutoAuthorizedLogList(self, request):
         """查询镜像自动授权结果列表
 
         :param request: Request instance for DescribeImageAutoAuthorizedLogList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageAutoAuthorizedLogListRequest`
@@ -3886,15 +3886,15 @@
             model = models.DescribeImageAutoAuthorizedLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageAutoAuthorizedRule(self, request):
         """查询本地镜像自动授权规则
 
         :param request: Request instance for DescribeImageAutoAuthorizedRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageAutoAuthorizedRuleRequest`
@@ -3909,15 +3909,15 @@
             model = models.DescribeImageAutoAuthorizedRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageAutoAuthorizedTaskList(self, request):
         """查询镜像自动授权任务列表
 
         :param request: Request instance for DescribeImageAutoAuthorizedTaskList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageAutoAuthorizedTaskListRequest`
@@ -3932,15 +3932,15 @@
             model = models.DescribeImageAutoAuthorizedTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageComponentList(self, request):
         """查询本地镜像组件列表
 
         :param request: Request instance for DescribeImageComponentList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageComponentListRequest`
@@ -3955,15 +3955,15 @@
             model = models.DescribeImageComponentListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageRegistryNamespaceList(self, request):
         """查询用户镜像仓库下的项目名称列表
 
         :param request: Request instance for DescribeImageRegistryNamespaceList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageRegistryNamespaceListRequest`
@@ -3978,15 +3978,15 @@
             model = models.DescribeImageRegistryNamespaceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageRegistryTimingScanTask(self, request):
         """镜像仓库查看定时任务
 
         :param request: Request instance for DescribeImageRegistryTimingScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageRegistryTimingScanTaskRequest`
@@ -4001,15 +4001,15 @@
             model = models.DescribeImageRegistryTimingScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageRiskSummary(self, request):
         """查询本地镜像风险概览
 
         :param request: Request instance for DescribeImageRiskSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageRiskSummaryRequest`
@@ -4024,15 +4024,15 @@
             model = models.DescribeImageRiskSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageRiskTendency(self, request):
         """查询容器安全本地镜像风险趋势
 
         :param request: Request instance for DescribeImageRiskTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageRiskTendencyRequest`
@@ -4047,15 +4047,15 @@
             model = models.DescribeImageRiskTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageSimpleList(self, request):
         """DescribeImageSimpleList 查询全部镜像列表
 
         :param request: Request instance for DescribeImageSimpleList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeImageSimpleListRequest`
@@ -4070,15 +4070,15 @@
             model = models.DescribeImageSimpleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIndexList(self, request):
         """获取索引列表
 
         :param request: Request instance for DescribeIndexList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeIndexListRequest`
@@ -4093,15 +4093,15 @@
             model = models.DescribeIndexListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInspectionReport(self, request):
         """查询检查报告
 
         :param request: Request instance for DescribeInspectionReport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeInspectionReportRequest`
@@ -4116,15 +4116,15 @@
             model = models.DescribeInspectionReportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalEventInfo(self, request):
         """查询k8s api 异常事件详情
 
         :param request: Request instance for DescribeK8sApiAbnormalEventInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalEventInfoRequest`
@@ -4139,15 +4139,15 @@
             model = models.DescribeK8sApiAbnormalEventInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalEventList(self, request):
         """查询k8s api异常事件列表
 
         :param request: Request instance for DescribeK8sApiAbnormalEventList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalEventListRequest`
@@ -4162,15 +4162,15 @@
             model = models.DescribeK8sApiAbnormalEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalRuleInfo(self, request):
         """查询k8sapi异常请求规则详情
 
         :param request: Request instance for DescribeK8sApiAbnormalRuleInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalRuleInfoRequest`
@@ -4185,15 +4185,15 @@
             model = models.DescribeK8sApiAbnormalRuleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalRuleList(self, request):
         """查询k8sapi异常请求规则列表
 
         :param request: Request instance for DescribeK8sApiAbnormalRuleList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalRuleListRequest`
@@ -4208,15 +4208,15 @@
             model = models.DescribeK8sApiAbnormalRuleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalRuleScopeList(self, request):
         """查询k8sapi 异常规则中范围列表
 
         :param request: Request instance for DescribeK8sApiAbnormalRuleScopeList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalRuleScopeListRequest`
@@ -4231,15 +4231,15 @@
             model = models.DescribeK8sApiAbnormalRuleScopeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalSummary(self, request):
         """查询k8sapi异常事件统计
 
         :param request: Request instance for DescribeK8sApiAbnormalSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalSummaryRequest`
@@ -4254,15 +4254,15 @@
             model = models.DescribeK8sApiAbnormalSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeK8sApiAbnormalTendency(self, request):
         """查询k8sapi异常事件趋势
 
         :param request: Request instance for DescribeK8sApiAbnormalTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeK8sApiAbnormalTendencyRequest`
@@ -4277,15 +4277,15 @@
             model = models.DescribeK8sApiAbnormalTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogStorageStatistic(self, request):
         """获取日志检索容量使用统计
 
         :param request: Request instance for DescribeLogStorageStatistic.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeLogStorageStatisticRequest`
@@ -4300,15 +4300,15 @@
             model = models.DescribeLogStorageStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallAuditRecord(self, request):
         """查询集群策略审计列表
 
         :param request: Request instance for DescribeNetworkFirewallAuditRecord.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallAuditRecordRequest`
@@ -4323,15 +4323,15 @@
             model = models.DescribeNetworkFirewallAuditRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallClusterList(self, request):
         """查询集群策略列表
 
         :param request: Request instance for DescribeNetworkFirewallClusterList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallClusterListRequest`
@@ -4346,15 +4346,15 @@
             model = models.DescribeNetworkFirewallClusterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallClusterRefreshStatus(self, request):
         """容器网络查询资产任务进度
 
         :param request: Request instance for DescribeNetworkFirewallClusterRefreshStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallClusterRefreshStatusRequest`
@@ -4369,15 +4369,15 @@
             model = models.DescribeNetworkFirewallClusterRefreshStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallNamespaceLabelList(self, request):
         """查询集群网络空间标签列表
 
         :param request: Request instance for DescribeNetworkFirewallNamespaceLabelList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallNamespaceLabelListRequest`
@@ -4392,15 +4392,15 @@
             model = models.DescribeNetworkFirewallNamespaceLabelListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallNamespaceList(self, request):
         """查询集群网络空间列表
 
         :param request: Request instance for DescribeNetworkFirewallNamespaceList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallNamespaceListRequest`
@@ -4415,15 +4415,15 @@
             model = models.DescribeNetworkFirewallNamespaceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPodLabelsList(self, request):
         """查询集群网络pod标签
 
         :param request: Request instance for DescribeNetworkFirewallPodLabelsList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPodLabelsListRequest`
@@ -4438,15 +4438,15 @@
             model = models.DescribeNetworkFirewallPodLabelsListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPolicyDetail(self, request):
         """容器网络集群查看策略详情
 
         :param request: Request instance for DescribeNetworkFirewallPolicyDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPolicyDetailRequest`
@@ -4461,15 +4461,15 @@
             model = models.DescribeNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPolicyDiscover(self, request):
         """容器网络查询网络策略自动发现任务进度
 
         :param request: Request instance for DescribeNetworkFirewallPolicyDiscover.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPolicyDiscoverRequest`
@@ -4484,15 +4484,15 @@
             model = models.DescribeNetworkFirewallPolicyDiscoverResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPolicyList(self, request):
         """查询集群网络策略列表
 
         :param request: Request instance for DescribeNetworkFirewallPolicyList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPolicyListRequest`
@@ -4507,15 +4507,15 @@
             model = models.DescribeNetworkFirewallPolicyListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPolicyStatus(self, request):
         """容器网络查询网络策略策略执行状态
 
         :param request: Request instance for DescribeNetworkFirewallPolicyStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPolicyStatusRequest`
@@ -4530,15 +4530,15 @@
             model = models.DescribeNetworkFirewallPolicyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNetworkFirewallPolicyYamlDetail(self, request):
         """容器网络集群查看Yaml网络策略详情
 
         :param request: Request instance for DescribeNetworkFirewallPolicyYamlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNetworkFirewallPolicyYamlDetailRequest`
@@ -4553,15 +4553,15 @@
             model = models.DescribeNetworkFirewallPolicyYamlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNewestVul(self, request):
         """查询最新披露漏洞列表
 
         :param request: Request instance for DescribeNewestVul.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeNewestVulRequest`
@@ -4576,15 +4576,15 @@
             model = models.DescribeNewestVulResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePostPayDetail(self, request):
         """DescribePostPayDetail  查询后付费详情
 
         :param request: Request instance for DescribePostPayDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribePostPayDetailRequest`
@@ -4599,15 +4599,15 @@
             model = models.DescribePostPayDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProVersionInfo(self, request):
         """DescribeProVersionInfo  查询专业版需购买信息
 
         :param request: Request instance for DescribeProVersionInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeProVersionInfoRequest`
@@ -4622,15 +4622,15 @@
             model = models.DescribeProVersionInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePromotionActivity(self, request):
         """查询促销活动
 
         :param request: Request instance for DescribePromotionActivity.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribePromotionActivityRequest`
@@ -4645,15 +4645,15 @@
             model = models.DescribePromotionActivityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublicKey(self, request):
         """获取公钥
 
         :param request: Request instance for DescribePublicKey.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribePublicKeyRequest`
@@ -4668,15 +4668,15 @@
             model = models.DescribePublicKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePurchaseStateInfo(self, request):
         """DescribePurchaseStateInfo 查询容器安全服务已购买信息
 
         :param request: Request instance for DescribePurchaseStateInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribePurchaseStateInfoRequest`
@@ -4691,15 +4691,15 @@
             model = models.DescribePurchaseStateInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRefreshTask(self, request):
         """查询刷新任务
 
         :param request: Request instance for DescribeRefreshTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRefreshTaskRequest`
@@ -4714,15 +4714,15 @@
             model = models.DescribeRefreshTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellDetail(self, request):
         """查询运行时反弹shell事件详细信息
 
         :param request: Request instance for DescribeReverseShellDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeReverseShellDetailRequest`
@@ -4737,15 +4737,15 @@
             model = models.DescribeReverseShellDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellEvents(self, request):
         """查询运行时反弹shell事件列表信息
 
         :param request: Request instance for DescribeReverseShellEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeReverseShellEventsRequest`
@@ -4760,15 +4760,15 @@
             model = models.DescribeReverseShellEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellEventsExport(self, request):
         """查询运行时反弹shell事件列表信息导出
 
         :param request: Request instance for DescribeReverseShellEventsExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeReverseShellEventsExportRequest`
@@ -4783,15 +4783,15 @@
             model = models.DescribeReverseShellEventsExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellWhiteListDetail(self, request):
         """查询运行时反弹shell白名单详细信息
 
         :param request: Request instance for DescribeReverseShellWhiteListDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeReverseShellWhiteListDetailRequest`
@@ -4806,15 +4806,15 @@
             model = models.DescribeReverseShellWhiteListDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReverseShellWhiteLists(self, request):
         """查询运行时运行时反弹shell白名单列表信息
 
         :param request: Request instance for DescribeReverseShellWhiteLists.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeReverseShellWhiteListsRequest`
@@ -4829,15 +4829,15 @@
             model = models.DescribeReverseShellWhiteListsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskList(self, request):
         """查询最近一次任务发现的风险项的信息列表，支持根据特殊字段进行过滤
 
         :param request: Request instance for DescribeRiskList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskListRequest`
@@ -4852,15 +4852,15 @@
             model = models.DescribeRiskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallDetail(self, request):
         """查询高危系统调用事件详细信息
 
         :param request: Request instance for DescribeRiskSyscallDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallDetailRequest`
@@ -4875,15 +4875,15 @@
             model = models.DescribeRiskSyscallDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallEvents(self, request):
         """查询运行时运行时高危系统调用列表信息
 
         :param request: Request instance for DescribeRiskSyscallEvents.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallEventsRequest`
@@ -4898,15 +4898,15 @@
             model = models.DescribeRiskSyscallEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallEventsExport(self, request):
         """运行时高危系统调用列表导出
 
         :param request: Request instance for DescribeRiskSyscallEventsExport.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallEventsExportRequest`
@@ -4921,15 +4921,15 @@
             model = models.DescribeRiskSyscallEventsExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallNames(self, request):
         """查询运行时高危系统调用系统名称列表
 
         :param request: Request instance for DescribeRiskSyscallNames.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallNamesRequest`
@@ -4944,15 +4944,15 @@
             model = models.DescribeRiskSyscallNamesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallWhiteListDetail(self, request):
         """查询运行时高危系统调用白名单详细信息
 
         :param request: Request instance for DescribeRiskSyscallWhiteListDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallWhiteListDetailRequest`
@@ -4967,15 +4967,15 @@
             model = models.DescribeRiskSyscallWhiteListDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRiskSyscallWhiteLists(self, request):
         """查询运行时高危系统调用白名单列表信息
 
         :param request: Request instance for DescribeRiskSyscallWhiteLists.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeRiskSyscallWhiteListsRequest`
@@ -4990,15 +4990,15 @@
             model = models.DescribeRiskSyscallWhiteListsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScanIgnoreVulList(self, request):
         """查询扫描忽略的漏洞列表
 
         :param request: Request instance for DescribeScanIgnoreVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeScanIgnoreVulListRequest`
@@ -5013,15 +5013,15 @@
             model = models.DescribeScanIgnoreVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSearchExportList(self, request):
         """导出ES查询文档列表
 
         :param request: Request instance for DescribeSearchExportList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSearchExportListRequest`
@@ -5036,15 +5036,15 @@
             model = models.DescribeSearchExportListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSearchLogs(self, request):
         """获取历史搜索记录
 
         :param request: Request instance for DescribeSearchLogs.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSearchLogsRequest`
@@ -5059,15 +5059,15 @@
             model = models.DescribeSearchLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSearchTemplates(self, request):
         """获取快速检索列表
 
         :param request: Request instance for DescribeSearchTemplates.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSearchTemplatesRequest`
@@ -5082,15 +5082,15 @@
             model = models.DescribeSearchTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecEventsTendency(self, request):
         """查询容器运行时安全事件趋势
 
         :param request: Request instance for DescribeSecEventsTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecEventsTendencyRequest`
@@ -5105,15 +5105,15 @@
             model = models.DescribeSecEventsTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogAlertMsg(self, request):
         """查询安全日志告警信息
 
         :param request: Request instance for DescribeSecLogAlertMsg.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogAlertMsgRequest`
@@ -5128,15 +5128,15 @@
             model = models.DescribeSecLogAlertMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogCleanSettingInfo(self, request):
         """查询安全日志清理设置详情
 
         :param request: Request instance for DescribeSecLogCleanSettingInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogCleanSettingInfoRequest`
@@ -5151,15 +5151,15 @@
             model = models.DescribeSecLogCleanSettingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogDeliveryClsOptions(self, request):
         """查询安全日志投递cls可选项
 
         :param request: Request instance for DescribeSecLogDeliveryClsOptions.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogDeliveryClsOptionsRequest`
@@ -5174,15 +5174,15 @@
             model = models.DescribeSecLogDeliveryClsOptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogDeliveryClsSetting(self, request):
         """查询安全日志投递Cls配置
 
         :param request: Request instance for DescribeSecLogDeliveryClsSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogDeliveryClsSettingRequest`
@@ -5197,15 +5197,15 @@
             model = models.DescribeSecLogDeliveryClsSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogDeliveryKafkaOptions(self, request):
         """查询安全日志投递kafka可选项
 
         :param request: Request instance for DescribeSecLogDeliveryKafkaOptions.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogDeliveryKafkaOptionsRequest`
@@ -5220,15 +5220,15 @@
             model = models.DescribeSecLogDeliveryKafkaOptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogDeliveryKafkaSetting(self, request):
         """查询安全日志投递kafka配置
 
         :param request: Request instance for DescribeSecLogDeliveryKafkaSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogDeliveryKafkaSettingRequest`
@@ -5243,15 +5243,15 @@
             model = models.DescribeSecLogDeliveryKafkaSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogJoinObjectList(self, request):
         """查询安全日志接入对象列表
 
         :param request: Request instance for DescribeSecLogJoinObjectList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogJoinObjectListRequest`
@@ -5266,15 +5266,15 @@
             model = models.DescribeSecLogJoinObjectListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogJoinTypeList(self, request):
         """查询安全日志接入列表
 
         :param request: Request instance for DescribeSecLogJoinTypeList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogJoinTypeListRequest`
@@ -5289,15 +5289,15 @@
             model = models.DescribeSecLogJoinTypeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogKafkaUIN(self, request):
         """查询安全日志KafkaUIN
 
         :param request: Request instance for DescribeSecLogKafkaUIN.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogKafkaUINRequest`
@@ -5312,15 +5312,15 @@
             model = models.DescribeSecLogKafkaUINResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecLogVasInfo(self, request):
         """查询安全日志商品信息
 
         :param request: Request instance for DescribeSecLogVasInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSecLogVasInfoRequest`
@@ -5335,15 +5335,15 @@
             model = models.DescribeSecLogVasInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSupportDefenceVul(self, request):
         """查询支持防御的漏洞列表
 
         :param request: Request instance for DescribeSupportDefenceVul.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSupportDefenceVulRequest`
@@ -5358,15 +5358,15 @@
             model = models.DescribeSupportDefenceVulResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSystemVulList(self, request):
         """查询系统漏洞列表
 
         :param request: Request instance for DescribeSystemVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeSystemVulListRequest`
@@ -5381,15 +5381,15 @@
             model = models.DescribeSystemVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskResultSummary(self, request):
         """查询检查结果总览，返回受影响的节点数量，返回7天的数据，总共7个
 
         :param request: Request instance for DescribeTaskResultSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeTaskResultSummaryRequest`
@@ -5404,15 +5404,15 @@
             model = models.DescribeTaskResultSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTcssSummary(self, request):
         """查询容器安全概览信息
 
         :param request: Request instance for DescribeTcssSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeTcssSummaryRequest`
@@ -5427,15 +5427,15 @@
             model = models.DescribeTcssSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnauthorizedCoresTendency(self, request):
         """查询当天未授权核数趋势
 
         :param request: Request instance for DescribeUnauthorizedCoresTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeUnauthorizedCoresTendencyRequest`
@@ -5450,15 +5450,15 @@
             model = models.DescribeUnauthorizedCoresTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUnfinishRefreshTask(self, request):
         """查询未完成的刷新资产任务信息
 
         :param request: Request instance for DescribeUnfinishRefreshTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeUnfinishRefreshTaskRequest`
@@ -5473,15 +5473,15 @@
             model = models.DescribeUnfinishRefreshTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserCluster(self, request):
         """安全概览和集群安全页进入调用该接口，查询用户集群相关信息。
 
         :param request: Request instance for DescribeUserCluster.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeUserClusterRequest`
@@ -5496,15 +5496,15 @@
             model = models.DescribeUserClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeValueAddedSrvInfo(self, request):
         """DescribeValueAddedSrvInfo查询增值服务需购买信息
 
         :param request: Request instance for DescribeValueAddedSrvInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeValueAddedSrvInfoRequest`
@@ -5519,15 +5519,15 @@
             model = models.DescribeValueAddedSrvInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusAutoIsolateSampleDetail(self, request):
         """查询木马自动隔离样本详情
 
         :param request: Request instance for DescribeVirusAutoIsolateSampleDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusAutoIsolateSampleDetailRequest`
@@ -5542,15 +5542,15 @@
             model = models.DescribeVirusAutoIsolateSampleDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusAutoIsolateSampleDownloadURL(self, request):
         """查询木马自动隔离样本下载链接
 
         :param request: Request instance for DescribeVirusAutoIsolateSampleDownloadURL.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusAutoIsolateSampleDownloadURLRequest`
@@ -5565,15 +5565,15 @@
             model = models.DescribeVirusAutoIsolateSampleDownloadURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusAutoIsolateSampleList(self, request):
         """查询木马自动隔离样本列表
 
         :param request: Request instance for DescribeVirusAutoIsolateSampleList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusAutoIsolateSampleListRequest`
@@ -5588,15 +5588,15 @@
             model = models.DescribeVirusAutoIsolateSampleListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusAutoIsolateSetting(self, request):
         """查询木马自动隔离设置
 
         :param request: Request instance for DescribeVirusAutoIsolateSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusAutoIsolateSettingRequest`
@@ -5611,15 +5611,15 @@
             model = models.DescribeVirusAutoIsolateSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusDetail(self, request):
         """运行时查询木马文件信息
 
         :param request: Request instance for DescribeVirusDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusDetailRequest`
@@ -5634,15 +5634,15 @@
             model = models.DescribeVirusDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusEventTendency(self, request):
         """查询木马事件趋势
 
         :param request: Request instance for DescribeVirusEventTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusEventTendencyRequest`
@@ -5657,15 +5657,15 @@
             model = models.DescribeVirusEventTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusList(self, request):
         """查询运行时文件查杀事件列表
 
         :param request: Request instance for DescribeVirusList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusListRequest`
@@ -5680,15 +5680,15 @@
             model = models.DescribeVirusListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusManualScanEstimateTimeout(self, request):
         """查询木马一键检测预估超时时间
 
         :param request: Request instance for DescribeVirusManualScanEstimateTimeout.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusManualScanEstimateTimeoutRequest`
@@ -5703,15 +5703,15 @@
             model = models.DescribeVirusManualScanEstimateTimeoutResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusMonitorSetting(self, request):
         """运行时查询文件查杀实时监控设置
 
         :param request: Request instance for DescribeVirusMonitorSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusMonitorSettingRequest`
@@ -5726,15 +5726,15 @@
             model = models.DescribeVirusMonitorSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusSampleDownloadUrl(self, request):
         """查询木马样本下载url
 
         :param request: Request instance for DescribeVirusSampleDownloadUrl.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusSampleDownloadUrlRequest`
@@ -5749,15 +5749,15 @@
             model = models.DescribeVirusSampleDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusScanSetting(self, request):
         """运行时查询文件查杀设置
 
         :param request: Request instance for DescribeVirusScanSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusScanSettingRequest`
@@ -5772,15 +5772,15 @@
             model = models.DescribeVirusScanSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusScanTaskStatus(self, request):
         """运行时查询文件查杀任务状态
 
         :param request: Request instance for DescribeVirusScanTaskStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusScanTaskStatusRequest`
@@ -5795,15 +5795,15 @@
             model = models.DescribeVirusScanTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusScanTimeoutSetting(self, request):
         """运行时文件扫描超时设置查询
 
         :param request: Request instance for DescribeVirusScanTimeoutSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusScanTimeoutSettingRequest`
@@ -5818,15 +5818,15 @@
             model = models.DescribeVirusScanTimeoutSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusSummary(self, request):
         """运行时查询木马概览信息
 
         :param request: Request instance for DescribeVirusSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusSummaryRequest`
@@ -5841,15 +5841,15 @@
             model = models.DescribeVirusSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVirusTaskList(self, request):
         """运行时查询文件查杀任务列表
 
         :param request: Request instance for DescribeVirusTaskList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVirusTaskListRequest`
@@ -5864,15 +5864,15 @@
             model = models.DescribeVirusTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulContainerList(self, request):
         """查询受漏洞的容器列表
 
         :param request: Request instance for DescribeVulContainerList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulContainerListRequest`
@@ -5887,15 +5887,15 @@
             model = models.DescribeVulContainerListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefenceEvent(self, request):
         """查询漏洞防御事件列表
 
         :param request: Request instance for DescribeVulDefenceEvent.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefenceEventRequest`
@@ -5910,15 +5910,15 @@
             model = models.DescribeVulDefenceEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefenceEventDetail(self, request):
         """查询漏洞防御事件详情
 
         :param request: Request instance for DescribeVulDefenceEventDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefenceEventDetailRequest`
@@ -5933,15 +5933,15 @@
             model = models.DescribeVulDefenceEventDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefenceEventTendency(self, request):
         """查询漏洞防御攻击事件趋势
 
         :param request: Request instance for DescribeVulDefenceEventTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefenceEventTendencyRequest`
@@ -5956,15 +5956,15 @@
             model = models.DescribeVulDefenceEventTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefenceHost(self, request):
         """查询漏洞防御的主机列表
 
         :param request: Request instance for DescribeVulDefenceHost.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefenceHostRequest`
@@ -5979,15 +5979,15 @@
             model = models.DescribeVulDefenceHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefencePlugin(self, request):
         """查询漏洞防御插件列表
 
         :param request: Request instance for DescribeVulDefencePlugin.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefencePluginRequest`
@@ -6002,15 +6002,15 @@
             model = models.DescribeVulDefencePluginResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDefenceSetting(self, request):
         """查询漏洞防御设置信息
 
         :param request: Request instance for DescribeVulDefenceSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDefenceSettingRequest`
@@ -6025,15 +6025,15 @@
             model = models.DescribeVulDefenceSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulDetail(self, request):
         """查询漏洞详情
 
         :param request: Request instance for DescribeVulDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulDetailRequest`
@@ -6048,15 +6048,15 @@
             model = models.DescribeVulDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulIgnoreLocalImageList(self, request):
         """查询漏洞扫描忽略的本地镜像列表
 
         :param request: Request instance for DescribeVulIgnoreLocalImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulIgnoreLocalImageListRequest`
@@ -6071,15 +6071,15 @@
             model = models.DescribeVulIgnoreLocalImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulIgnoreRegistryImageList(self, request):
         """查询漏洞扫描忽略的仓库镜像列表
 
         :param request: Request instance for DescribeVulIgnoreRegistryImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulIgnoreRegistryImageListRequest`
@@ -6094,15 +6094,15 @@
             model = models.DescribeVulIgnoreRegistryImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulImageList(self, request):
         """查询漏洞影响的镜像列表
 
         :param request: Request instance for DescribeVulImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulImageListRequest`
@@ -6117,15 +6117,15 @@
             model = models.DescribeVulImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulImageSummary(self, request):
         """查询漏洞镜像统计
 
         :param request: Request instance for DescribeVulImageSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulImageSummaryRequest`
@@ -6140,15 +6140,15 @@
             model = models.DescribeVulImageSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulLevelImageSummary(self, request):
         """查询应急漏洞各威胁等级统计镜像数
 
         :param request: Request instance for DescribeVulLevelImageSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulLevelImageSummaryRequest`
@@ -6163,15 +6163,15 @@
             model = models.DescribeVulLevelImageSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulLevelSummary(self, request):
         """查询漏洞各威胁等级统计数
 
         :param request: Request instance for DescribeVulLevelSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulLevelSummaryRequest`
@@ -6186,15 +6186,15 @@
             model = models.DescribeVulLevelSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulRegistryImageList(self, request):
         """查询漏洞影响的仓库镜像列表
 
         :param request: Request instance for DescribeVulRegistryImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulRegistryImageListRequest`
@@ -6209,15 +6209,15 @@
             model = models.DescribeVulRegistryImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulScanAuthorizedImageSummary(self, request):
         """统计漏洞扫描页已授权和未扫描镜像数
 
         :param request: Request instance for DescribeVulScanAuthorizedImageSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulScanAuthorizedImageSummaryRequest`
@@ -6232,15 +6232,15 @@
             model = models.DescribeVulScanAuthorizedImageSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulScanInfo(self, request):
         """查询漏洞扫描任务信息
 
         :param request: Request instance for DescribeVulScanInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulScanInfoRequest`
@@ -6255,15 +6255,15 @@
             model = models.DescribeVulScanInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulScanLocalImageList(self, request):
         """查询漏洞扫描任务的本地镜像列表
 
         :param request: Request instance for DescribeVulScanLocalImageList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulScanLocalImageListRequest`
@@ -6278,15 +6278,15 @@
             model = models.DescribeVulScanLocalImageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulSummary(self, request):
         """查询漏洞风险统计概览
 
         :param request: Request instance for DescribeVulSummary.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulSummaryRequest`
@@ -6301,15 +6301,15 @@
             model = models.DescribeVulSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulTendency(self, request):
         """查询本地镜像、仓库镜像中严重&高危的漏洞趋势
 
         :param request: Request instance for DescribeVulTendency.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulTendencyRequest`
@@ -6324,15 +6324,15 @@
             model = models.DescribeVulTendencyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVulTopRanking(self, request):
         """查询漏洞Top排名列表
 
         :param request: Request instance for DescribeVulTopRanking.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeVulTopRankingRequest`
@@ -6347,15 +6347,15 @@
             model = models.DescribeVulTopRankingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWarningRules(self, request):
         """获取告警策略列表
 
         :param request: Request instance for DescribeWarningRules.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeWarningRulesRequest`
@@ -6370,15 +6370,15 @@
             model = models.DescribeWarningRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWebVulList(self, request):
         """查询web应用漏洞列表
 
         :param request: Request instance for DescribeWebVulList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.DescribeWebVulListRequest`
@@ -6393,15 +6393,15 @@
             model = models.DescribeWebVulListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportVirusList(self, request):
         """运行时文件查杀事件列表导出
 
         :param request: Request instance for ExportVirusList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ExportVirusListRequest`
@@ -6416,15 +6416,15 @@
             model = models.ExportVirusListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InitializeUserComplianceEnvironment(self, request):
         """为客户初始化合规基线的使用环境，创建必要的数据和选项。
 
         :param request: Request instance for InitializeUserComplianceEnvironment.
         :type request: :class:`tencentcloud.tcss.v20201101.models.InitializeUserComplianceEnvironmentRequest`
@@ -6439,15 +6439,15 @@
             model = models.InitializeUserComplianceEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAbnormalProcessRuleStatus(self, request):
         """修改运行时异常进程策略的开启关闭状态
 
         :param request: Request instance for ModifyAbnormalProcessRuleStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAbnormalProcessRuleStatusRequest`
@@ -6462,15 +6462,15 @@
             model = models.ModifyAbnormalProcessRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAbnormalProcessStatus(self, request):
         """修改异常进程事件的状态信息
 
         :param request: Request instance for ModifyAbnormalProcessStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAbnormalProcessStatusRequest`
@@ -6485,15 +6485,15 @@
             model = models.ModifyAbnormalProcessStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccessControlRuleStatus(self, request):
         """修改运行时访问控制策略的状态，启用或者禁用
 
         :param request: Request instance for ModifyAccessControlRuleStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAccessControlRuleStatusRequest`
@@ -6508,15 +6508,15 @@
             model = models.ModifyAccessControlRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccessControlStatus(self, request):
         """修改运行时访问控制事件状态信息
 
         :param request: Request instance for ModifyAccessControlStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAccessControlStatusRequest`
@@ -6531,15 +6531,15 @@
             model = models.ModifyAccessControlStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAsset(self, request):
         """容器安全主机资产刷新
 
         :param request: Request instance for ModifyAsset.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAssetRequest`
@@ -6554,15 +6554,15 @@
             model = models.ModifyAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAssetImageRegistryScanStop(self, request):
         """镜像仓库停止镜像扫描任务
 
         :param request: Request instance for ModifyAssetImageRegistryScanStop.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAssetImageRegistryScanStopRequest`
@@ -6577,15 +6577,15 @@
             model = models.ModifyAssetImageRegistryScanStopResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAssetImageRegistryScanStopOneKey(self, request):
         """镜像仓库停止镜像一键扫描任务
 
         :param request: Request instance for ModifyAssetImageRegistryScanStopOneKey.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAssetImageRegistryScanStopOneKeyRequest`
@@ -6600,15 +6600,15 @@
             model = models.ModifyAssetImageRegistryScanStopOneKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAssetImageScanStop(self, request):
         """容器安全停止镜像扫描
 
         :param request: Request instance for ModifyAssetImageScanStop.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyAssetImageScanStopRequest`
@@ -6623,15 +6623,15 @@
             model = models.ModifyAssetImageScanStopResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCompliancePeriodTask(self, request):
         """修改定时任务的设置，包括检测周期、开启/禁用合规基准。
 
         :param request: Request instance for ModifyCompliancePeriodTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyCompliancePeriodTaskRequest`
@@ -6646,15 +6646,15 @@
             model = models.ModifyCompliancePeriodTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyContainerNetStatus(self, request):
         """隔离容器网络状态
 
         :param request: Request instance for ModifyContainerNetStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyContainerNetStatusRequest`
@@ -6669,15 +6669,15 @@
             model = models.ModifyContainerNetStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEscapeEventStatus(self, request):
         """ModifyEscapeEventStatus  修改容器逃逸扫描事件状态
 
         :param request: Request instance for ModifyEscapeEventStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyEscapeEventStatusRequest`
@@ -6692,15 +6692,15 @@
             model = models.ModifyEscapeEventStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEscapeRule(self, request):
         """ModifyEscapeRule  修改容器逃逸扫描规则信息
 
         :param request: Request instance for ModifyEscapeRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyEscapeRuleRequest`
@@ -6715,15 +6715,15 @@
             model = models.ModifyEscapeRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEscapeWhiteList(self, request):
         """修改逃逸白名单
 
         :param request: Request instance for ModifyEscapeWhiteList.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyEscapeWhiteListRequest`
@@ -6738,15 +6738,15 @@
             model = models.ModifyEscapeWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImageAuthorized(self, request):
         """批量授权镜像扫描V2.0
 
         :param request: Request instance for ModifyImageAuthorized.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyImageAuthorizedRequest`
@@ -6761,15 +6761,15 @@
             model = models.ModifyImageAuthorizedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyK8sApiAbnormalEventStatus(self, request):
         """修改k8sapi异常事件状态
 
         :param request: Request instance for ModifyK8sApiAbnormalEventStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyK8sApiAbnormalEventStatusRequest`
@@ -6784,15 +6784,15 @@
             model = models.ModifyK8sApiAbnormalEventStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyK8sApiAbnormalRuleInfo(self, request):
         """修改k8sapi异常规则信息
 
         :param request: Request instance for ModifyK8sApiAbnormalRuleInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyK8sApiAbnormalRuleInfoRequest`
@@ -6807,15 +6807,15 @@
             model = models.ModifyK8sApiAbnormalRuleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyK8sApiAbnormalRuleStatus(self, request):
         """修改k8sapi异常事件规则状态
 
         :param request: Request instance for ModifyK8sApiAbnormalRuleStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyK8sApiAbnormalRuleStatusRequest`
@@ -6830,15 +6830,15 @@
             model = models.ModifyK8sApiAbnormalRuleStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyReverseShellStatus(self, request):
         """修改反弹shell事件的状态信息
 
         :param request: Request instance for ModifyReverseShellStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyReverseShellStatusRequest`
@@ -6853,15 +6853,15 @@
             model = models.ModifyReverseShellStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRiskSyscallStatus(self, request):
         """修改高危系统调用事件的状态信息
 
         :param request: Request instance for ModifyRiskSyscallStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyRiskSyscallStatusRequest`
@@ -6876,15 +6876,15 @@
             model = models.ModifyRiskSyscallStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogCleanSettingInfo(self, request):
         """修改安全日志清理设置信息
 
         :param request: Request instance for ModifySecLogCleanSettingInfo.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogCleanSettingInfoRequest`
@@ -6899,15 +6899,15 @@
             model = models.ModifySecLogCleanSettingInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogDeliveryClsSetting(self, request):
         """更新安全日志-日志投递cls配置
 
         :param request: Request instance for ModifySecLogDeliveryClsSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogDeliveryClsSettingRequest`
@@ -6922,15 +6922,15 @@
             model = models.ModifySecLogDeliveryClsSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogDeliveryKafkaSetting(self, request):
         """更新安全日志投递kafka设置
 
         :param request: Request instance for ModifySecLogDeliveryKafkaSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogDeliveryKafkaSettingRequest`
@@ -6945,15 +6945,15 @@
             model = models.ModifySecLogDeliveryKafkaSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogJoinObjects(self, request):
         """修改安全日志接入对象
 
         :param request: Request instance for ModifySecLogJoinObjects.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogJoinObjectsRequest`
@@ -6968,15 +6968,15 @@
             model = models.ModifySecLogJoinObjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogJoinState(self, request):
         """修改安全日志接入状态
 
         :param request: Request instance for ModifySecLogJoinState.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogJoinStateRequest`
@@ -6991,15 +6991,15 @@
             model = models.ModifySecLogJoinStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecLogKafkaUIN(self, request):
         """修改安全日志kafkaUIN
 
         :param request: Request instance for ModifySecLogKafkaUIN.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifySecLogKafkaUINRequest`
@@ -7014,15 +7014,15 @@
             model = models.ModifySecLogKafkaUINResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusAutoIsolateExampleSwitch(self, request):
         """修改木马自动隔离样本开关
 
         :param request: Request instance for ModifyVirusAutoIsolateExampleSwitch.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusAutoIsolateExampleSwitchRequest`
@@ -7037,15 +7037,15 @@
             model = models.ModifyVirusAutoIsolateExampleSwitchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusAutoIsolateSetting(self, request):
         """修改木马自动隔离设置
 
         :param request: Request instance for ModifyVirusAutoIsolateSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusAutoIsolateSettingRequest`
@@ -7060,15 +7060,15 @@
             model = models.ModifyVirusAutoIsolateSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusFileStatus(self, request):
         """运行时更新木马文件事件状态
 
         :param request: Request instance for ModifyVirusFileStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusFileStatusRequest`
@@ -7083,15 +7083,15 @@
             model = models.ModifyVirusFileStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusMonitorSetting(self, request):
         """运行时更新文件查杀实时监控设置
 
         :param request: Request instance for ModifyVirusMonitorSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusMonitorSettingRequest`
@@ -7106,15 +7106,15 @@
             model = models.ModifyVirusMonitorSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusScanSetting(self, request):
         """运行时更新文件查杀设置
 
         :param request: Request instance for ModifyVirusScanSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusScanSettingRequest`
@@ -7129,15 +7129,15 @@
             model = models.ModifyVirusScanSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVirusScanTimeoutSetting(self, request):
         """运行时文件扫描超时设置
 
         :param request: Request instance for ModifyVirusScanTimeoutSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVirusScanTimeoutSettingRequest`
@@ -7152,15 +7152,15 @@
             model = models.ModifyVirusScanTimeoutSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVulDefenceEventStatus(self, request):
         """修改漏洞防御事件状态
 
         :param request: Request instance for ModifyVulDefenceEventStatus.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVulDefenceEventStatusRequest`
@@ -7175,15 +7175,15 @@
             model = models.ModifyVulDefenceEventStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVulDefenceSetting(self, request):
         """编辑漏洞防御设置
 
         :param request: Request instance for ModifyVulDefenceSetting.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ModifyVulDefenceSettingRequest`
@@ -7198,15 +7198,15 @@
             model = models.ModifyVulDefenceSettingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenTcssTrial(self, request):
         """开通容器安全服务试用
 
         :param request: Request instance for OpenTcssTrial.
         :type request: :class:`tencentcloud.tcss.v20201101.models.OpenTcssTrialRequest`
@@ -7221,15 +7221,15 @@
             model = models.OpenTcssTrialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveAssetImageRegistryRegistryDetail(self, request):
         """删除单个镜像仓库详细信息
 
         :param request: Request instance for RemoveAssetImageRegistryRegistryDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.RemoveAssetImageRegistryRegistryDetailRequest`
@@ -7244,15 +7244,15 @@
             model = models.RemoveAssetImageRegistryRegistryDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewImageAuthorizeState(self, request):
         """RenewImageAuthorizeState   授权镜像扫描
 
         :param request: Request instance for RenewImageAuthorizeState.
         :type request: :class:`tencentcloud.tcss.v20201101.models.RenewImageAuthorizeStateRequest`
@@ -7267,15 +7267,15 @@
             model = models.RenewImageAuthorizeStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetSecLogTopicConfig(self, request):
         """重置安全日志主题设置
 
         :param request: Request instance for ResetSecLogTopicConfig.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ResetSecLogTopicConfigRequest`
@@ -7290,15 +7290,15 @@
             model = models.ResetSecLogTopicConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanComplianceAssets(self, request):
         """重新检测选定的资产
 
         :param request: Request instance for ScanComplianceAssets.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ScanComplianceAssetsRequest`
@@ -7313,15 +7313,15 @@
             model = models.ScanComplianceAssetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanComplianceAssetsByPolicyItem(self, request):
         """用指定的检测项重新检测选定的资产，返回创建的合规检查任务的ID。
 
         :param request: Request instance for ScanComplianceAssetsByPolicyItem.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ScanComplianceAssetsByPolicyItemRequest`
@@ -7336,15 +7336,15 @@
             model = models.ScanComplianceAssetsByPolicyItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanCompliancePolicyItems(self, request):
         """重新检测选的检测项下的所有资产，返回创建的合规检查任务的ID。
 
         :param request: Request instance for ScanCompliancePolicyItems.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ScanCompliancePolicyItemsRequest`
@@ -7359,15 +7359,15 @@
             model = models.ScanCompliancePolicyItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanComplianceScanFailedAssets(self, request):
         """重新检测选定的检测失败的资产下的所有失败的检测项，返回创建的合规检查任务的ID。
 
         :param request: Request instance for ScanComplianceScanFailedAssets.
         :type request: :class:`tencentcloud.tcss.v20201101.models.ScanComplianceScanFailedAssetsRequest`
@@ -7382,15 +7382,15 @@
             model = models.ScanComplianceScanFailedAssetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetCheckMode(self, request):
         """设置检测模式和自动检查
 
         :param request: Request instance for SetCheckMode.
         :type request: :class:`tencentcloud.tcss.v20201101.models.SetCheckModeRequest`
@@ -7405,15 +7405,15 @@
             model = models.SetCheckModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopVirusScanTask(self, request):
         """运行时停止木马查杀任务
 
         :param request: Request instance for StopVirusScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.StopVirusScanTaskRequest`
@@ -7428,15 +7428,15 @@
             model = models.StopVirusScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopVulScanTask(self, request):
         """停止漏洞扫描任务
 
         :param request: Request instance for StopVulScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.StopVulScanTaskRequest`
@@ -7451,15 +7451,15 @@
             model = models.StopVulScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchImageAutoAuthorizedRule(self, request):
         """编辑本地镜像自动授权开关
 
         :param request: Request instance for SwitchImageAutoAuthorizedRule.
         :type request: :class:`tencentcloud.tcss.v20201101.models.SwitchImageAutoAuthorizedRuleRequest`
@@ -7474,15 +7474,15 @@
             model = models.SwitchImageAutoAuthorizedRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncAssetImageRegistryAsset(self, request):
         """镜像仓库资产刷新
 
         :param request: Request instance for SyncAssetImageRegistryAsset.
         :type request: :class:`tencentcloud.tcss.v20201101.models.SyncAssetImageRegistryAssetRequest`
@@ -7497,15 +7497,15 @@
             model = models.SyncAssetImageRegistryAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAndPublishNetworkFirewallPolicyDetail(self, request):
         """容器网络创建网络策略更新并发布任务
 
         :param request: Request instance for UpdateAndPublishNetworkFirewallPolicyDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateAndPublishNetworkFirewallPolicyDetailRequest`
@@ -7520,15 +7520,15 @@
             model = models.UpdateAndPublishNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAndPublishNetworkFirewallPolicyYamlDetail(self, request):
         """容器网络更新Yaml网络策略并发布任务
 
         :param request: Request instance for UpdateAndPublishNetworkFirewallPolicyYamlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateAndPublishNetworkFirewallPolicyYamlDetailRequest`
@@ -7543,15 +7543,15 @@
             model = models.UpdateAndPublishNetworkFirewallPolicyYamlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAssetImageRegistryRegistryDetail(self, request):
         """更新单个镜像仓库详细信息
 
         :param request: Request instance for UpdateAssetImageRegistryRegistryDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateAssetImageRegistryRegistryDetailRequest`
@@ -7566,15 +7566,15 @@
             model = models.UpdateAssetImageRegistryRegistryDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateImageRegistryTimingScanTask(self, request):
         """镜像仓库更新定时任务
 
         :param request: Request instance for UpdateImageRegistryTimingScanTask.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateImageRegistryTimingScanTaskRequest`
@@ -7589,15 +7589,15 @@
             model = models.UpdateImageRegistryTimingScanTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateNetworkFirewallPolicyDetail(self, request):
         """容器网络创建网络策略更新任务
 
         :param request: Request instance for UpdateNetworkFirewallPolicyDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateNetworkFirewallPolicyDetailRequest`
@@ -7612,15 +7612,15 @@
             model = models.UpdateNetworkFirewallPolicyDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateNetworkFirewallPolicyYamlDetail(self, request):
         """容器网络更新Yaml网络策略任务
 
         :param request: Request instance for UpdateNetworkFirewallPolicyYamlDetail.
         :type request: :class:`tencentcloud.tcss.v20201101.models.UpdateNetworkFirewallPolicyYamlDetailRequest`
@@ -7635,8 +7635,8 @@
             model = models.UpdateNetworkFirewallPolicyYamlDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/tcss/v20201101/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.937/README.rst` & `tencentcloud-sdk-python-tcss-3.0.938/README.rst`

 * *Files identical despite different names*

