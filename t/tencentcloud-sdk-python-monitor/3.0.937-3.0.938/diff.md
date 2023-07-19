# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.937.tar", last modified: Tue Jul 18 00:27:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.938.tar", last modified: Wed Jul 19 00:42:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.937.tar` & `tencentcloud-sdk-python-monitor-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10348 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   145047 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)   867907 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:27:33.000000 tencentcloud-sdk-python-monitor-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144242 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)   863968 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:42:56.000000 tencentcloud-sdk-python-monitor-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.938/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/setup.py` & `tencentcloud-sdk-python-monitor-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindPrometheusManagedGrafanaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindingPolicyObject(self, request):
         """将告警策略绑定到特定对象
 
         :param request: Request instance for BindingPolicyObject.
         :type request: :class:`tencentcloud.monitor.v20180724.models.BindingPolicyObjectRequest`
@@ -65,15 +65,15 @@
             model = models.BindingPolicyObjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindingPolicyTag(self, request):
         """策略绑定标签
 
         :param request: Request instance for BindingPolicyTag.
         :type request: :class:`tencentcloud.monitor.v20180724.models.BindingPolicyTagRequest`
@@ -88,15 +88,15 @@
             model = models.BindingPolicyTagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckIsPrometheusNewUser(self, request):
         """判断用户是否为云原生监控新用户，即在任何地域下均未创建过监控实例的用户
 
         :param request: Request instance for CheckIsPrometheusNewUser.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CheckIsPrometheusNewUserRequest`
@@ -111,15 +111,15 @@
             model = models.CheckIsPrometheusNewUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CleanGrafanaInstance(self, request):
         """强制销毁 Grafana 实例
 
         :param request: Request instance for CleanGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CleanGrafanaInstanceRequest`
@@ -134,15 +134,15 @@
             model = models.CleanGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlarmNotice(self, request):
         """创建通知模板
 
         :param request: Request instance for CreateAlarmNotice.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateAlarmNoticeRequest`
@@ -157,15 +157,15 @@
             model = models.CreateAlarmNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlarmPolicy(self, request):
         """创建告警策略
 
         :param request: Request instance for CreateAlarmPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateAlarmPolicyRequest`
@@ -180,15 +180,15 @@
             model = models.CreateAlarmPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlertRule(self, request):
         """创建 Prometheus 告警规则。
 
         请注意，**告警对象和告警消息是 Prometheus Rule Annotations 的特殊字段，需要通过 annotations 来传递，对应的 Key 分别为summary/description**，，请参考 [Prometheus Rule更多配置请参考](https://prometheus.io/docs/prometheus/latest/configuration/alerting_rules/)。
 
@@ -205,15 +205,15 @@
             model = models.CreateAlertRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateExporterIntegration(self, request):
         """创建 exporter 集成
 
         :param request: Request instance for CreateExporterIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateExporterIntegrationRequest`
@@ -228,15 +228,15 @@
             model = models.CreateExporterIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGrafanaInstance(self, request):
         """本接口（CreateGrafanaInstance）用于创建 Grafana 包年包月实例，默认基础版、到期自动续费、不可使用代金券。
 
         :param request: Request instance for CreateGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateGrafanaInstanceRequest`
@@ -251,15 +251,15 @@
             model = models.CreateGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGrafanaIntegration(self, request):
         """创建 Grafana 集成配置
 
         :param request: Request instance for CreateGrafanaIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateGrafanaIntegrationRequest`
@@ -274,15 +274,15 @@
             model = models.CreateGrafanaIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGrafanaNotificationChannel(self, request):
         """创建 Grafana 告警通道
 
         :param request: Request instance for CreateGrafanaNotificationChannel.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateGrafanaNotificationChannelRequest`
@@ -297,15 +297,15 @@
             model = models.CreateGrafanaNotificationChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePolicyGroup(self, request):
         """增加策略组
 
         :param request: Request instance for CreatePolicyGroup.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePolicyGroupRequest`
@@ -320,15 +320,15 @@
             model = models.CreatePolicyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusAgent(self, request):
         """创建 Prometheus CVM Agent
 
         :param request: Request instance for CreatePrometheusAgent.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusAgentRequest`
@@ -343,15 +343,15 @@
             model = models.CreatePrometheusAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusAlertPolicy(self, request):
         """创建告警策略
 
         :param request: Request instance for CreatePrometheusAlertPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusAlertPolicyRequest`
@@ -366,15 +366,15 @@
             model = models.CreatePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusClusterAgent(self, request):
         """与腾讯云可观测融合的2.0实例关联集群
 
         :param request: Request instance for CreatePrometheusClusterAgent.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusClusterAgentRequest`
@@ -389,15 +389,15 @@
             model = models.CreatePrometheusClusterAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusConfig(self, request):
         """创建prometheus配置
 
         :param request: Request instance for CreatePrometheusConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusConfigRequest`
@@ -412,15 +412,15 @@
             model = models.CreatePrometheusConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusGlobalNotification(self, request):
         """创建全局告警通知渠道
 
         :param request: Request instance for CreatePrometheusGlobalNotification.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusGlobalNotificationRequest`
@@ -435,15 +435,15 @@
             model = models.CreatePrometheusGlobalNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusMultiTenantInstancePostPayMode(self, request):
         """创建按量 Prometheus 实例，根据用量收费实例
 
         :param request: Request instance for CreatePrometheusMultiTenantInstancePostPayMode.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusMultiTenantInstancePostPayModeRequest`
@@ -458,15 +458,15 @@
             model = models.CreatePrometheusMultiTenantInstancePostPayModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusRecordRuleYaml(self, request):
         """以Yaml的方式创建聚合规则
 
         :param request: Request instance for CreatePrometheusRecordRuleYaml.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusRecordRuleYamlRequest`
@@ -481,15 +481,15 @@
             model = models.CreatePrometheusRecordRuleYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusScrapeJob(self, request):
         """创建 Prometheus 抓取任务
 
         :param request: Request instance for CreatePrometheusScrapeJob.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusScrapeJobRequest`
@@ -504,15 +504,15 @@
             model = models.CreatePrometheusScrapeJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusTemp(self, request):
         """创建一个云原生Prometheus模板
 
         :param request: Request instance for CreatePrometheusTemp.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreatePrometheusTempRequest`
@@ -527,15 +527,15 @@
             model = models.CreatePrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecordingRule(self, request):
         """创建 Prometheus 的预聚合规则
 
         :param request: Request instance for CreateRecordingRule.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateRecordingRuleRequest`
@@ -550,15 +550,15 @@
             model = models.CreateRecordingRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSSOAccount(self, request):
         """Grafana实例授权其他腾讯云用户
 
         :param request: Request instance for CreateSSOAccount.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateSSOAccountRequest`
@@ -573,15 +573,15 @@
             model = models.CreateSSOAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceDiscovery(self, request):
         """在腾讯云容器服务下创建 Prometheus 服务发现。
         <p>注意：前提条件，已经通过 Prometheus 控制台集成了对应的腾讯云容器服务，具体请参考
         <a href="https://cloud.tencent.com/document/product/248/48859" target="_blank">Agent 安装</a>。</p>
 
@@ -598,15 +598,15 @@
             model = models.CreateServiceDiscoveryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlarmNotices(self, request):
         """删除告警通知模板
 
         :param request: Request instance for DeleteAlarmNotices.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteAlarmNoticesRequest`
@@ -621,15 +621,15 @@
             model = models.DeleteAlarmNoticesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlarmPolicy(self, request):
         """删除告警策略
 
         :param request: Request instance for DeleteAlarmPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteAlarmPolicyRequest`
@@ -644,15 +644,15 @@
             model = models.DeleteAlarmPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlertRules(self, request):
         """批量删除 Prometheus 报警规则
 
         :param request: Request instance for DeleteAlertRules.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteAlertRulesRequest`
@@ -667,15 +667,15 @@
             model = models.DeleteAlertRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteExporterIntegration(self, request):
         """删除 exporter 集成
 
         :param request: Request instance for DeleteExporterIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteExporterIntegrationRequest`
@@ -690,15 +690,15 @@
             model = models.DeleteExporterIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGrafanaInstance(self, request):
         """本接口（DeleteGrafanaInstance）用于 Grafana 包年包月实例的退费，调用后实例处于停服状态，不可使用，7天后自动销毁。
 
         :param request: Request instance for DeleteGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteGrafanaInstanceRequest`
@@ -713,15 +713,15 @@
             model = models.DeleteGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGrafanaIntegration(self, request):
         """删除 Grafana 集成配置
 
         :param request: Request instance for DeleteGrafanaIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteGrafanaIntegrationRequest`
@@ -736,15 +736,15 @@
             model = models.DeleteGrafanaIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGrafanaNotificationChannel(self, request):
         """删除 Grafana 告警通道
 
         :param request: Request instance for DeleteGrafanaNotificationChannel.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteGrafanaNotificationChannelRequest`
@@ -759,15 +759,15 @@
             model = models.DeleteGrafanaNotificationChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePolicyGroup(self, request):
         """删除告警策略组
 
         :param request: Request instance for DeletePolicyGroup.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePolicyGroupRequest`
@@ -782,15 +782,15 @@
             model = models.DeletePolicyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusAlertPolicy(self, request):
         """删除2.0实例告警策略
 
         :param request: Request instance for DeletePrometheusAlertPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusAlertPolicyRequest`
@@ -805,15 +805,15 @@
             model = models.DeletePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusClusterAgent(self, request):
         """解除TMP实例的集群关联
 
         :param request: Request instance for DeletePrometheusClusterAgent.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusClusterAgentRequest`
@@ -828,15 +828,15 @@
             model = models.DeletePrometheusClusterAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusConfig(self, request):
         """删除Prometheus配置，如果目标不存在，将返回成功
 
         :param request: Request instance for DeletePrometheusConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusConfigRequest`
@@ -851,15 +851,15 @@
             model = models.DeletePrometheusConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusRecordRuleYaml(self, request):
         """删除聚合实例
 
         :param request: Request instance for DeletePrometheusRecordRuleYaml.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusRecordRuleYamlRequest`
@@ -874,15 +874,15 @@
             model = models.DeletePrometheusRecordRuleYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusScrapeJobs(self, request):
         """删除 Prometheus 抓取任务
 
         :param request: Request instance for DeletePrometheusScrapeJobs.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusScrapeJobsRequest`
@@ -897,15 +897,15 @@
             model = models.DeletePrometheusScrapeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusTemp(self, request):
         """删除一个云原生Prometheus配置模板
 
         :param request: Request instance for DeletePrometheusTemp.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusTempRequest`
@@ -920,15 +920,15 @@
             model = models.DeletePrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusTempSync(self, request):
         """解除模板同步，这将会删除目标中该模板所生产的配置，针对V2版本实例
 
         :param request: Request instance for DeletePrometheusTempSync.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeletePrometheusTempSyncRequest`
@@ -943,15 +943,15 @@
             model = models.DeletePrometheusTempSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecordingRules(self, request):
         """批量删除 Prometheus 预聚合规则
 
         :param request: Request instance for DeleteRecordingRules.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteRecordingRulesRequest`
@@ -966,15 +966,15 @@
             model = models.DeleteRecordingRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSSOAccount(self, request):
         """Grafana可视化服务 删除授权用户
 
         :param request: Request instance for DeleteSSOAccount.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteSSOAccountRequest`
@@ -989,15 +989,15 @@
             model = models.DeleteSSOAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceDiscovery(self, request):
         """删除在腾讯云容器服务下创建的 Prometheus 服务发现。
         <p>注意：前提条件，已经通过 Prometheus 控制台集成了对应的腾讯云容器服务，具体请参考
         <a href="https://cloud.tencent.com/document/product/248/48859" target="_blank">Agent 安装</a>。</p>
 
@@ -1014,15 +1014,15 @@
             model = models.DeleteServiceDiscoveryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccidentEventList(self, request):
         """获取平台事件列表
 
         :param request: Request instance for DescribeAccidentEventList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAccidentEventListRequest`
@@ -1037,15 +1037,15 @@
             model = models.DescribeAccidentEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmEvents(self, request):
         """查询告警事件列表
 
         :param request: Request instance for DescribeAlarmEvents.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmEventsRequest`
@@ -1060,15 +1060,15 @@
             model = models.DescribeAlarmEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmHistories(self, request):
         """查询告警历史
 
         请注意，**如果使用子用户进行告警历史的查询，只能查询到被授权项目下的告警历史**，或不区分项目的产品的告警历史。如何对子账户授予项目的权限，请参考 [访问管理-项目与标签](https://cloud.tencent.com/document/product/598/32738)。
 
@@ -1085,15 +1085,15 @@
             model = models.DescribeAlarmHistoriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmMetrics(self, request):
         """查询告警指标列表
 
         :param request: Request instance for DescribeAlarmMetrics.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmMetricsRequest`
@@ -1108,15 +1108,15 @@
             model = models.DescribeAlarmMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmNotice(self, request):
         """查询单个通知模板的详情
 
         :param request: Request instance for DescribeAlarmNotice.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmNoticeRequest`
@@ -1131,15 +1131,15 @@
             model = models.DescribeAlarmNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmNoticeCallbacks(self, request):
         """获取告警通知模板所有回调URL
 
         :param request: Request instance for DescribeAlarmNoticeCallbacks.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmNoticeCallbacksRequest`
@@ -1154,15 +1154,15 @@
             model = models.DescribeAlarmNoticeCallbacksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmNotices(self, request):
         """查询通知模板列表
 
         :param request: Request instance for DescribeAlarmNotices.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmNoticesRequest`
@@ -1177,15 +1177,15 @@
             model = models.DescribeAlarmNoticesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmPolicies(self, request):
         """查询告警策略列表
 
         :param request: Request instance for DescribeAlarmPolicies.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmPoliciesRequest`
@@ -1200,15 +1200,15 @@
             model = models.DescribeAlarmPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmPolicy(self, request):
         """获取单个告警策略详情
 
         :param request: Request instance for DescribeAlarmPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlarmPolicyRequest`
@@ -1223,15 +1223,15 @@
             model = models.DescribeAlarmPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlertRules(self, request):
         """Prometheus 报警规则查询接口
 
         :param request: Request instance for DescribeAlertRules.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAlertRulesRequest`
@@ -1246,15 +1246,15 @@
             model = models.DescribeAlertRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllNamespaces(self, request):
         """查询所有名字空间
 
         :param request: Request instance for DescribeAllNamespaces.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeAllNamespacesRequest`
@@ -1269,15 +1269,15 @@
             model = models.DescribeAllNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBaseMetrics(self, request):
         """获取基础指标属性
 
         :param request: Request instance for DescribeBaseMetrics.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeBaseMetricsRequest`
@@ -1292,15 +1292,15 @@
             model = models.DescribeBaseMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBasicAlarmList(self, request):
         """获取基础告警列表
 
         :param request: Request instance for DescribeBasicAlarmList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeBasicAlarmListRequest`
@@ -1315,15 +1315,15 @@
             model = models.DescribeBasicAlarmListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBindingPolicyObjectList(self, request):
         """获取已绑定对象列表
 
         :param request: Request instance for DescribeBindingPolicyObjectList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeBindingPolicyObjectListRequest`
@@ -1338,15 +1338,15 @@
             model = models.DescribeBindingPolicyObjectListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterAgentCreatingProgress(self, request):
         """获取prom实例中集群详细的关联状态
 
         :param request: Request instance for DescribeClusterAgentCreatingProgress.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeClusterAgentCreatingProgressRequest`
@@ -1361,15 +1361,15 @@
             model = models.DescribeClusterAgentCreatingProgressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConditionsTemplateList(self, request):
         """获取条件模板列表
 
         :param request: Request instance for DescribeConditionsTemplateList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeConditionsTemplateListRequest`
@@ -1384,15 +1384,15 @@
             model = models.DescribeConditionsTemplateListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDNSConfig(self, request):
         """列出 Grafana DNS 配置
 
         :param request: Request instance for DescribeDNSConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeDNSConfigRequest`
@@ -1407,15 +1407,15 @@
             model = models.DescribeDNSConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExporterIntegrations(self, request):
         """查询 exporter 集成列表
 
         :param request: Request instance for DescribeExporterIntegrations.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeExporterIntegrationsRequest`
@@ -1430,15 +1430,15 @@
             model = models.DescribeExporterIntegrationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaChannels(self, request):
         """列出 Grafana 所有告警通道
 
         :param request: Request instance for DescribeGrafanaChannels.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaChannelsRequest`
@@ -1453,15 +1453,15 @@
             model = models.DescribeGrafanaChannelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaConfig(self, request):
         """列出 Grafana 的设置，即 grafana.ini 文件内容
 
         :param request: Request instance for DescribeGrafanaConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaConfigRequest`
@@ -1476,15 +1476,15 @@
             model = models.DescribeGrafanaConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaEnvironments(self, request):
         """列出 Grafana 环境变量
 
         :param request: Request instance for DescribeGrafanaEnvironments.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaEnvironmentsRequest`
@@ -1499,15 +1499,15 @@
             model = models.DescribeGrafanaEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaInstances(self, request):
         """列出用户所有的 Grafana 服务
 
         :param request: Request instance for DescribeGrafanaInstances.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaInstancesRequest`
@@ -1522,15 +1522,15 @@
             model = models.DescribeGrafanaInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaIntegrations(self, request):
         """列出 Grafana 已安装的集成
 
         :param request: Request instance for DescribeGrafanaIntegrations.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaIntegrationsRequest`
@@ -1545,15 +1545,15 @@
             model = models.DescribeGrafanaIntegrationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaNotificationChannels(self, request):
         """列出 Grafana 告警通道
 
         :param request: Request instance for DescribeGrafanaNotificationChannels.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaNotificationChannelsRequest`
@@ -1568,15 +1568,15 @@
             model = models.DescribeGrafanaNotificationChannelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGrafanaWhiteList(self, request):
         """列出 Grafana 白名单
 
         :param request: Request instance for DescribeGrafanaWhiteList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeGrafanaWhiteListRequest`
@@ -1591,15 +1591,15 @@
             model = models.DescribeGrafanaWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstalledPlugins(self, request):
         """列出实例已安装的插件
 
         :param request: Request instance for DescribeInstalledPlugins.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeInstalledPluginsRequest`
@@ -1614,15 +1614,15 @@
             model = models.DescribeInstalledPluginsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonitorTypes(self, request):
         """腾讯云可观测平台支持多种类型的监控，此接口列出支持的所有类型
 
         :param request: Request instance for DescribeMonitorTypes.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeMonitorTypesRequest`
@@ -1637,15 +1637,15 @@
             model = models.DescribeMonitorTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePluginOverviews(self, request):
         """列出可安装的所有 Grafana 插件
 
         :param request: Request instance for DescribePluginOverviews.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePluginOverviewsRequest`
@@ -1660,15 +1660,15 @@
             model = models.DescribePluginOverviewsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicyConditionList(self, request):
         """获取基础告警策略条件
 
         :param request: Request instance for DescribePolicyConditionList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePolicyConditionListRequest`
@@ -1683,15 +1683,15 @@
             model = models.DescribePolicyConditionListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicyGroupInfo(self, request):
         """获取基础策略组详情
 
         :param request: Request instance for DescribePolicyGroupInfo.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePolicyGroupInfoRequest`
@@ -1706,15 +1706,15 @@
             model = models.DescribePolicyGroupInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePolicyGroupList(self, request):
         """获取基础策略告警组列表
 
         :param request: Request instance for DescribePolicyGroupList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePolicyGroupListRequest`
@@ -1729,15 +1729,15 @@
             model = models.DescribePolicyGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductEventList(self, request):
         """分页获取产品事件的列表
 
         :param request: Request instance for DescribeProductEventList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeProductEventListRequest`
@@ -1752,15 +1752,15 @@
             model = models.DescribeProductEventListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductList(self, request):
         """查询腾讯云可观测平台云产品列表，支持云服务器CVM、云数据库、云消息队列、负载均衡、容器服务、专线等云产品。
 
         :param request: Request instance for DescribeProductList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeProductListRequest`
@@ -1775,15 +1775,15 @@
             model = models.DescribeProductListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusAgentInstances(self, request):
         """获取关联目标集群的实例列表
 
         :param request: Request instance for DescribePrometheusAgentInstances.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusAgentInstancesRequest`
@@ -1798,15 +1798,15 @@
             model = models.DescribePrometheusAgentInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusAgents(self, request):
         """列出 Prometheus CVM Agent
 
         :param request: Request instance for DescribePrometheusAgents.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusAgentsRequest`
@@ -1821,15 +1821,15 @@
             model = models.DescribePrometheusAgentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusAlertPolicy(self, request):
         """获取2.0实例告警策略列表
 
         :param request: Request instance for DescribePrometheusAlertPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusAlertPolicyRequest`
@@ -1844,15 +1844,15 @@
             model = models.DescribePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusClusterAgents(self, request):
         """获取TMP实例关联集群列表
 
         :param request: Request instance for DescribePrometheusClusterAgents.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusClusterAgentsRequest`
@@ -1867,15 +1867,15 @@
             model = models.DescribePrometheusClusterAgentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusConfig(self, request):
         """拉取Prometheus配置
 
         :param request: Request instance for DescribePrometheusConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusConfigRequest`
@@ -1890,15 +1890,15 @@
             model = models.DescribePrometheusConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusGlobalConfig(self, request):
         """获得实例级别抓取配置
 
         :param request: Request instance for DescribePrometheusGlobalConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusGlobalConfigRequest`
@@ -1913,15 +1913,15 @@
             model = models.DescribePrometheusGlobalConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusGlobalNotification(self, request):
         """查询全局告警通知渠道
 
         :param request: Request instance for DescribePrometheusGlobalNotification.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusGlobalNotificationRequest`
@@ -1936,15 +1936,15 @@
             model = models.DescribePrometheusGlobalNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstanceDetail(self, request):
         """获取TMP实例详情
 
         :param request: Request instance for DescribePrometheusInstanceDetail.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusInstanceDetailRequest`
@@ -1959,15 +1959,15 @@
             model = models.DescribePrometheusInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstanceInitStatus(self, request):
         """获取2.0实例初始化任务状态
 
         :param request: Request instance for DescribePrometheusInstanceInitStatus.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusInstanceInitStatusRequest`
@@ -1982,15 +1982,15 @@
             model = models.DescribePrometheusInstanceInitStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstanceUsage(self, request):
         """查询Prometheus按量实例用量
 
         :param request: Request instance for DescribePrometheusInstanceUsage.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusInstanceUsageRequest`
@@ -2005,15 +2005,15 @@
             model = models.DescribePrometheusInstanceUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstances(self, request):
         """本接口 (DescribePrometheusInstances) 用于查询一个或多个实例的详细信息。
         <ul>
         <li>可以根据实例ID、实例名称或者实例状态等信息来查询实例的详细信息</li>
         <li>如果参数为空，返回当前用户一定数量（Limit所指定的数量，默认为20）的实例。</li>
@@ -2032,15 +2032,15 @@
             model = models.DescribePrometheusInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstancesOverview(self, request):
         """获取与 Prometheus 监控融合实例列表
 
         :param request: Request instance for DescribePrometheusInstancesOverview.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusInstancesOverviewRequest`
@@ -2055,15 +2055,15 @@
             model = models.DescribePrometheusInstancesOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusRecordRuleYaml(self, request):
         """拉取Prometheus聚合规则yaml列表
 
         :param request: Request instance for DescribePrometheusRecordRuleYaml.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusRecordRuleYamlRequest`
@@ -2078,15 +2078,15 @@
             model = models.DescribePrometheusRecordRuleYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusRecordRules(self, request):
         """获取聚合规则列表，包含关联集群内crd资源创建的record rule
 
         :param request: Request instance for DescribePrometheusRecordRules.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusRecordRulesRequest`
@@ -2101,15 +2101,15 @@
             model = models.DescribePrometheusRecordRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusScrapeJobs(self, request):
         """列出 Prometheus 抓取任务
 
         :param request: Request instance for DescribePrometheusScrapeJobs.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusScrapeJobsRequest`
@@ -2124,15 +2124,15 @@
             model = models.DescribePrometheusScrapeJobsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTargetsTMP(self, request):
         """获取targets信息
 
         :param request: Request instance for DescribePrometheusTargetsTMP.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusTargetsTMPRequest`
@@ -2147,15 +2147,15 @@
             model = models.DescribePrometheusTargetsTMPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTemp(self, request):
         """拉取模板列表，默认模板将总是在最前面
 
         :param request: Request instance for DescribePrometheusTemp.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusTempRequest`
@@ -2170,15 +2170,15 @@
             model = models.DescribePrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTempSync(self, request):
         """获取模板关联实例信息，针对V2版本实例
 
         :param request: Request instance for DescribePrometheusTempSync.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusTempSyncRequest`
@@ -2193,15 +2193,15 @@
             model = models.DescribePrometheusTempSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusZones(self, request):
         """列出 Prometheus 服务可用区
 
         :param request: Request instance for DescribePrometheusZones.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribePrometheusZonesRequest`
@@ -2216,15 +2216,15 @@
             model = models.DescribePrometheusZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordingRules(self, request):
         """根据条件查询 Prometheus 预聚合规则
 
         :param request: Request instance for DescribeRecordingRules.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeRecordingRulesRequest`
@@ -2239,15 +2239,15 @@
             model = models.DescribeRecordingRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSSOAccount(self, request):
         """列出当前grafana实例的所有授权账号
 
         :param request: Request instance for DescribeSSOAccount.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeSSOAccountRequest`
@@ -2262,15 +2262,15 @@
             model = models.DescribeSSOAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceDiscovery(self, request):
         """列出在腾讯云容器服务下创建的 Prometheus 服务发现。
         <p>注意：前提条件，已经通过 Prometheus 控制台集成了对应的腾讯云容器服务，具体请参考
         <a href="https://cloud.tencent.com/document/product/248/48859" target="_blank">Agent 安装</a>。</p>
 
@@ -2287,15 +2287,15 @@
             model = models.DescribeServiceDiscoveryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStatisticData(self, request):
         """根据维度条件查询监控数据
 
         :param request: Request instance for DescribeStatisticData.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DescribeStatisticDataRequest`
@@ -2310,15 +2310,15 @@
             model = models.DescribeStatisticDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyPrometheusInstance(self, request):
         """彻底删除 Prometheus 实例相关数据，给定的实例必须先被 Terminate
 
         :param request: Request instance for DestroyPrometheusInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DestroyPrometheusInstanceRequest`
@@ -2333,15 +2333,15 @@
             model = models.DestroyPrometheusInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableGrafanaInternet(self, request):
         """设置 Grafana 公网访问
 
         :param request: Request instance for EnableGrafanaInternet.
         :type request: :class:`tencentcloud.monitor.v20180724.models.EnableGrafanaInternetRequest`
@@ -2356,15 +2356,15 @@
             model = models.EnableGrafanaInternetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableGrafanaSSO(self, request):
         """设置 Grafana 单点登录，使用腾讯云账号
 
         :param request: Request instance for EnableGrafanaSSO.
         :type request: :class:`tencentcloud.monitor.v20180724.models.EnableGrafanaSSORequest`
@@ -2379,15 +2379,15 @@
             model = models.EnableGrafanaSSOResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableSSOCamCheck(self, request):
         """SSO单点登录时，设置是否cam鉴权
 
         :param request: Request instance for EnableSSOCamCheck.
         :type request: :class:`tencentcloud.monitor.v20180724.models.EnableSSOCamCheckRequest`
@@ -2402,15 +2402,15 @@
             model = models.EnableSSOCamCheckResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetMonitorData(self, request):
         """获取云产品的监控数据。此接口不适用于拉取容器服务监控数据，如需拉取容器服务监控数据，请使用[根据维度条件查询监控数据](https://cloud.tencent.com/document/product/248/51845)接口。
         传入产品的命名空间、对象维度描述和监控指标即可获得相应的监控数据。
         接口调用限制：单请求最多可支持批量拉取10个实例的监控数据，单请求的数据点数限制为1440个。
         若您需要调用的指标、对象较多，可能存在因限频出现拉取失败的情况，建议尽量将请求按时间维度均摊。
@@ -2431,15 +2431,15 @@
             model = models.GetMonitorDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetPrometheusAgentManagementCommand(self, request):
         """获取 Prometheus Agent 管理相关的命令行
 
         :param request: Request instance for GetPrometheusAgentManagementCommand.
         :type request: :class:`tencentcloud.monitor.v20180724.models.GetPrometheusAgentManagementCommandRequest`
@@ -2454,15 +2454,15 @@
             model = models.GetPrometheusAgentManagementCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InstallPlugins(self, request):
         """安装 Grafana Plugin
 
         :param request: Request instance for InstallPlugins.
         :type request: :class:`tencentcloud.monitor.v20180724.models.InstallPluginsRequest`
@@ -2477,15 +2477,15 @@
             model = models.InstallPluginsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmNotice(self, request):
         """编辑告警通知模板
 
         :param request: Request instance for ModifyAlarmNotice.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmNoticeRequest`
@@ -2500,15 +2500,15 @@
             model = models.ModifyAlarmNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmPolicyCondition(self, request):
         """修改告警策略触发条件
 
         :param request: Request instance for ModifyAlarmPolicyCondition.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmPolicyConditionRequest`
@@ -2523,15 +2523,15 @@
             model = models.ModifyAlarmPolicyConditionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmPolicyInfo(self, request):
         """告警2.0编辑告警策略基本信息，包括策略名、备注
 
         :param request: Request instance for ModifyAlarmPolicyInfo.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmPolicyInfoRequest`
@@ -2546,15 +2546,15 @@
             model = models.ModifyAlarmPolicyInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmPolicyNotice(self, request):
         """修改告警策略绑定的告警通知模板
 
         :param request: Request instance for ModifyAlarmPolicyNotice.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmPolicyNoticeRequest`
@@ -2569,15 +2569,15 @@
             model = models.ModifyAlarmPolicyNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmPolicyStatus(self, request):
         """启停告警策略
 
         :param request: Request instance for ModifyAlarmPolicyStatus.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmPolicyStatusRequest`
@@ -2592,15 +2592,15 @@
             model = models.ModifyAlarmPolicyStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmPolicyTasks(self, request):
         """修改告警策略的触发任务，TriggerTasks字段放触发任务列表，TriggerTasks传空数组时，代表解绑该策略的所有触发任务。
 
         :param request: Request instance for ModifyAlarmPolicyTasks.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmPolicyTasksRequest`
@@ -2615,15 +2615,15 @@
             model = models.ModifyAlarmPolicyTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmReceivers(self, request):
         """修改告警接收人
 
         :param request: Request instance for ModifyAlarmReceivers.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyAlarmReceiversRequest`
@@ -2638,15 +2638,15 @@
             model = models.ModifyAlarmReceiversResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyGrafanaInstance(self, request):
         """修改 Grafana 实例属性
 
         :param request: Request instance for ModifyGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyGrafanaInstanceRequest`
@@ -2661,15 +2661,15 @@
             model = models.ModifyGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPolicyGroup(self, request):
         """更新策略组
 
         :param request: Request instance for ModifyPolicyGroup.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPolicyGroupRequest`
@@ -2684,15 +2684,15 @@
             model = models.ModifyPolicyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusAgentExternalLabels(self, request):
         """修改被关联集群的external labels
 
         :param request: Request instance for ModifyPrometheusAgentExternalLabels.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusAgentExternalLabelsRequest`
@@ -2707,15 +2707,15 @@
             model = models.ModifyPrometheusAgentExternalLabelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusAlertPolicy(self, request):
         """修改2.0实例告警策略
 
         :param request: Request instance for ModifyPrometheusAlertPolicy.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusAlertPolicyRequest`
@@ -2730,15 +2730,15 @@
             model = models.ModifyPrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusConfig(self, request):
         """修改prometheus配置，如果配置项不存在，则会新增
 
         :param request: Request instance for ModifyPrometheusConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusConfigRequest`
@@ -2753,15 +2753,15 @@
             model = models.ModifyPrometheusConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusGlobalNotification(self, request):
         """修改全局告警通知渠道
 
         :param request: Request instance for ModifyPrometheusGlobalNotification.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusGlobalNotificationRequest`
@@ -2776,15 +2776,15 @@
             model = models.ModifyPrometheusGlobalNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusInstanceAttributes(self, request):
         """修改 Prometheus 实例相关属性
 
         :param request: Request instance for ModifyPrometheusInstanceAttributes.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusInstanceAttributesRequest`
@@ -2799,15 +2799,15 @@
             model = models.ModifyPrometheusInstanceAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusRecordRuleYaml(self, request):
         """通过yaml的方式修改Prometheus聚合实例
 
         :param request: Request instance for ModifyPrometheusRecordRuleYaml.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusRecordRuleYamlRequest`
@@ -2822,15 +2822,15 @@
             model = models.ModifyPrometheusRecordRuleYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusTemp(self, request):
         """修改模板内容
 
         :param request: Request instance for ModifyPrometheusTemp.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ModifyPrometheusTempRequest`
@@ -2845,46 +2845,15 @@
             model = models.ModifyPrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def PutMonitorData(self, request):
-        """对应的功能控制台及后端服务已于2年前下线，剩余该API接口未下线。
-
-        默认接口请求频率限制：50次/秒。
-        默认单租户指标上限：100个。
-        单次上报最多 30 个指标/值对，请求返回错误时，请求中所有的指标/值均不会被保存。
-
-        上报的时间戳为期望保存的时间戳，建议构造整数分钟时刻的时间戳。
-        时间戳时间范围必须为当前时间到 300 秒前之间。
-        同一 IP 指标对的数据需按分钟先后顺序上报。
-
-        :param request: Request instance for PutMonitorData.
-        :type request: :class:`tencentcloud.monitor.v20180724.models.PutMonitorDataRequest`
-        :rtype: :class:`tencentcloud.monitor.v20180724.models.PutMonitorDataResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("PutMonitorData", params, headers=headers)
-            response = json.loads(body)
-            model = models.PutMonitorDataResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeGrafanaInstance(self, request):
         """本接口（ResumeGrafanaInstance）用于 Grafana 包年包月实例的停服续费，调用后按原版本续费一个月。仍在运行中的实例无法使用该接口进行续费。
 
         :param request: Request instance for ResumeGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ResumeGrafanaInstanceRequest`
@@ -2899,15 +2868,15 @@
             model = models.ResumeGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunPrometheusInstance(self, request):
         """初始化TMP实例，开启集成中心时调用
 
         :param request: Request instance for RunPrometheusInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.RunPrometheusInstanceRequest`
@@ -2922,15 +2891,15 @@
             model = models.RunPrometheusInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendCustomAlarmMsg(self, request):
         """发送自定义消息告警
 
         :param request: Request instance for SendCustomAlarmMsg.
         :type request: :class:`tencentcloud.monitor.v20180724.models.SendCustomAlarmMsgRequest`
@@ -2945,15 +2914,15 @@
             model = models.SendCustomAlarmMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetDefaultAlarmPolicy(self, request):
         """设置一个策略为该告警策略类型、该项目的默认告警策略。
         同一项目下相同的告警策略类型，就会被设置为非默认。
 
         :param request: Request instance for SetDefaultAlarmPolicy.
@@ -2969,15 +2938,15 @@
             model = models.SetDefaultAlarmPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncPrometheusTemp(self, request):
         """同步模板到实例或者集群，针对V2版本实例
 
         :param request: Request instance for SyncPrometheusTemp.
         :type request: :class:`tencentcloud.monitor.v20180724.models.SyncPrometheusTempRequest`
@@ -2992,15 +2961,15 @@
             model = models.SyncPrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminatePrometheusInstances(self, request):
         """销毁按量 Prometheus 实例
 
         :param request: Request instance for TerminatePrometheusInstances.
         :type request: :class:`tencentcloud.monitor.v20180724.models.TerminatePrometheusInstancesRequest`
@@ -3015,15 +2984,15 @@
             model = models.TerminatePrometheusInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindingAllPolicyObject(self, request):
         """删除全部的关联对象
 
         :param request: Request instance for UnBindingAllPolicyObject.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UnBindingAllPolicyObjectRequest`
@@ -3038,15 +3007,15 @@
             model = models.UnBindingAllPolicyObjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnBindingPolicyObject(self, request):
         """删除策略的关联对象
 
         :param request: Request instance for UnBindingPolicyObject.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UnBindingPolicyObjectRequest`
@@ -3061,15 +3030,15 @@
             model = models.UnBindingPolicyObjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindPrometheusManagedGrafana(self, request):
         """解除实例绑定的 Grafana 可视化实例
 
         :param request: Request instance for UnbindPrometheusManagedGrafana.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UnbindPrometheusManagedGrafanaRequest`
@@ -3084,15 +3053,15 @@
             model = models.UnbindPrometheusManagedGrafanaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UninstallGrafanaDashboard(self, request):
         """删除 Grafana Dashboard
 
         :param request: Request instance for UninstallGrafanaDashboard.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UninstallGrafanaDashboardRequest`
@@ -3107,15 +3076,15 @@
             model = models.UninstallGrafanaDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UninstallGrafanaPlugins(self, request):
         """删除已安装的插件
 
         :param request: Request instance for UninstallGrafanaPlugins.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UninstallGrafanaPluginsRequest`
@@ -3130,15 +3099,15 @@
             model = models.UninstallGrafanaPluginsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAlertRule(self, request):
         """更新 Prometheus 的报警规则。
 
         请注意，**告警对象和告警消息是 Prometheus Rule Annotations 的特殊字段，需要通过 annotations 来传递，对应的 Key 分别为summary/description**，，请参考 [Prometheus Rule更多配置请参考](https://prometheus.io/docs/prometheus/latest/configuration/alerting_rules/)。
 
@@ -3155,15 +3124,15 @@
             model = models.UpdateAlertRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAlertRuleState(self, request):
         """更新 Prometheus 报警策略状态
 
         :param request: Request instance for UpdateAlertRuleState.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateAlertRuleStateRequest`
@@ -3178,15 +3147,15 @@
             model = models.UpdateAlertRuleStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDNSConfig(self, request):
         """更新 Grafana 的 DNS 配置
 
         :param request: Request instance for UpdateDNSConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateDNSConfigRequest`
@@ -3201,15 +3170,15 @@
             model = models.UpdateDNSConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateExporterIntegration(self, request):
         """更新 exporter 集成配置
 
         :param request: Request instance for UpdateExporterIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateExporterIntegrationRequest`
@@ -3224,15 +3193,15 @@
             model = models.UpdateExporterIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGrafanaConfig(self, request):
         """更新 Grafana 配置
 
         :param request: Request instance for UpdateGrafanaConfig.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateGrafanaConfigRequest`
@@ -3247,15 +3216,15 @@
             model = models.UpdateGrafanaConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGrafanaEnvironments(self, request):
         """更新 Grafana 环境变量
 
         :param request: Request instance for UpdateGrafanaEnvironments.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateGrafanaEnvironmentsRequest`
@@ -3270,15 +3239,15 @@
             model = models.UpdateGrafanaEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGrafanaIntegration(self, request):
         """更新 Grafana 集成配置
 
         :param request: Request instance for UpdateGrafanaIntegration.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateGrafanaIntegrationRequest`
@@ -3293,15 +3262,15 @@
             model = models.UpdateGrafanaIntegrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGrafanaNotificationChannel(self, request):
         """更新 Grafana 告警通道
 
         :param request: Request instance for UpdateGrafanaNotificationChannel.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateGrafanaNotificationChannelRequest`
@@ -3316,15 +3285,15 @@
             model = models.UpdateGrafanaNotificationChannelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGrafanaWhiteList(self, request):
         """更新 Grafana 白名单
 
         :param request: Request instance for UpdateGrafanaWhiteList.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateGrafanaWhiteListRequest`
@@ -3339,15 +3308,15 @@
             model = models.UpdateGrafanaWhiteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePrometheusAgentStatus(self, request):
         """更新 Prometheus CVM Agent 状态
 
         :param request: Request instance for UpdatePrometheusAgentStatus.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdatePrometheusAgentStatusRequest`
@@ -3362,15 +3331,15 @@
             model = models.UpdatePrometheusAgentStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePrometheusScrapeJob(self, request):
         """更新 Prometheus 抓取任务
 
         :param request: Request instance for UpdatePrometheusScrapeJob.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdatePrometheusScrapeJobRequest`
@@ -3385,15 +3354,15 @@
             model = models.UpdatePrometheusScrapeJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRecordingRule(self, request):
         """更新 Prometheus 的预聚合规则
 
         :param request: Request instance for UpdateRecordingRule.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateRecordingRuleRequest`
@@ -3408,15 +3377,15 @@
             model = models.UpdateRecordingRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateSSOAccount(self, request):
         """更新已授权账号的备注、权限信息，会直接覆盖原有的信息，不传则不会更新。
 
         :param request: Request instance for UpdateSSOAccount.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpdateSSOAccountRequest`
@@ -3431,15 +3400,15 @@
             model = models.UpdateSSOAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateServiceDiscovery(self, request):
         """在腾讯云容器服务下更新 Prometheus 服务发现。
         <p>注意：前提条件，已经通过 Prometheus 控制台集成了对应的腾讯云容器服务，具体请参考
         <a href="https://cloud.tencent.com/document/product/248/48859" target="_blank">Agent 安装</a>。</p>
 
@@ -3456,15 +3425,15 @@
             model = models.UpdateServiceDiscoveryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeGrafanaDashboard(self, request):
         """升级 Grafana Dashboard
 
         :param request: Request instance for UpgradeGrafanaDashboard.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpgradeGrafanaDashboardRequest`
@@ -3479,15 +3448,15 @@
             model = models.UpgradeGrafanaDashboardResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeGrafanaInstance(self, request):
         """升级 Grafana 实例
 
         :param request: Request instance for UpgradeGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.UpgradeGrafanaInstanceRequest`
@@ -3502,8 +3471,8 @@
             model = models.UpgradeGrafanaInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -20585,59 +20585,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class MetricDatum(AbstractModel):
-    """指标名称和值的封装
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _MetricName: 指标名称
-        :type MetricName: str
-        :param _Value: 指标的值
-        :type Value: int
-        """
-        self._MetricName = None
-        self._Value = None
-
-    @property
-    def MetricName(self):
-        return self._MetricName
-
-    @MetricName.setter
-    def MetricName(self, MetricName):
-        self._MetricName = MetricName
-
-    @property
-    def Value(self):
-        return self._Value
-
-    @Value.setter
-    def Value(self, Value):
-        self._Value = Value
-
-
-    def _deserialize(self, params):
-        self._MetricName = params.get("MetricName")
-        self._Value = params.get("Value")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class MetricObjectMeaning(AbstractModel):
     """指标数据的解释
 
     """
 
     def __init__(self):
         r"""
@@ -26537,113 +26492,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class PutMonitorDataRequest(AbstractModel):
-    """PutMonitorData请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Metrics: 一组指标和数据
-        :type Metrics: list of MetricDatum
-        :param _AnnounceIp: 上报时自行指定的 IP
-        :type AnnounceIp: str
-        :param _AnnounceTimestamp: 上报时自行指定的时间戳
-        :type AnnounceTimestamp: int
-        :param _AnnounceInstance: 上报时自行指定的 IP 或 产品实例ID
-        :type AnnounceInstance: str
-        """
-        self._Metrics = None
-        self._AnnounceIp = None
-        self._AnnounceTimestamp = None
-        self._AnnounceInstance = None
-
-    @property
-    def Metrics(self):
-        return self._Metrics
-
-    @Metrics.setter
-    def Metrics(self, Metrics):
-        self._Metrics = Metrics
-
-    @property
-    def AnnounceIp(self):
-        return self._AnnounceIp
-
-    @AnnounceIp.setter
-    def AnnounceIp(self, AnnounceIp):
-        self._AnnounceIp = AnnounceIp
-
-    @property
-    def AnnounceTimestamp(self):
-        return self._AnnounceTimestamp
-
-    @AnnounceTimestamp.setter
-    def AnnounceTimestamp(self, AnnounceTimestamp):
-        self._AnnounceTimestamp = AnnounceTimestamp
-
-    @property
-    def AnnounceInstance(self):
-        return self._AnnounceInstance
-
-    @AnnounceInstance.setter
-    def AnnounceInstance(self, AnnounceInstance):
-        self._AnnounceInstance = AnnounceInstance
-
-
-    def _deserialize(self, params):
-        if params.get("Metrics") is not None:
-            self._Metrics = []
-            for item in params.get("Metrics"):
-                obj = MetricDatum()
-                obj._deserialize(item)
-                self._Metrics.append(obj)
-        self._AnnounceIp = params.get("AnnounceIp")
-        self._AnnounceTimestamp = params.get("AnnounceTimestamp")
-        self._AnnounceInstance = params.get("AnnounceInstance")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class PutMonitorDataResponse(AbstractModel):
-    """PutMonitorData返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
 class ReceiverInfo(AbstractModel):
     """接收人信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.937/README.rst` & `tencentcloud-sdk-python-monitor-3.0.938/README.rst`

 * *Files identical despite different names*

