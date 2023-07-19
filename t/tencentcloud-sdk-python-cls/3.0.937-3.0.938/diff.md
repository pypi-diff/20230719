# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.937.tar", last modified: Tue Jul 18 00:20:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.938.tar", last modified: Wed Jul 19 00:24:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.937.tar` & `tencentcloud-sdk-python-cls-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    77073 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9048 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   461117 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:20:46.000000 tencentcloud-sdk-python-cls-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    78273 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   468744 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:24:52.000000 tencentcloud-sdk-python-cls-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.937/setup.py` & `tencentcloud-sdk-python-cls-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddMachineGroupInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyConfigToMachineGroup(self, request):
         """应用采集配置到指定机器组
 
         :param request: Request instance for ApplyConfigToMachineGroup.
         :type request: :class:`tencentcloud.cls.v20201016.models.ApplyConfigToMachineGroupRequest`
@@ -65,15 +65,15 @@
             model = models.ApplyConfigToMachineGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckRechargeKafkaServer(self, request):
         """本接口用于校验Kafka服务集群是否可以正常访问
 
         :param request: Request instance for CheckRechargeKafkaServer.
         :type request: :class:`tencentcloud.cls.v20201016.models.CheckRechargeKafkaServerRequest`
@@ -88,15 +88,15 @@
             model = models.CheckRechargeKafkaServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseKafkaConsumer(self, request):
         """关闭Kafka协议消费
 
         :param request: Request instance for CloseKafkaConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.CloseKafkaConsumerRequest`
@@ -111,15 +111,15 @@
             model = models.CloseKafkaConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlarm(self, request):
         """本接口用于创建告警策略。
 
         :param request: Request instance for CreateAlarm.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateAlarmRequest`
@@ -134,15 +134,15 @@
             model = models.CreateAlarmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlarmNotice(self, request):
         """该接口用于创建通知渠道组。
 
         :param request: Request instance for CreateAlarmNotice.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateAlarmNoticeRequest`
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
 
 
     def CreateConfig(self, request):
         """创建采集规则配置
 
         :param request: Request instance for CreateConfig.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateConfigRequest`
@@ -180,15 +180,15 @@
             model = models.CreateConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigExtra(self, request):
         """本接口用于创建特殊采集配置任务，特殊采集配置应用于自建K8S环境的采集Agent
 
         :param request: Request instance for CreateConfigExtra.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateConfigExtraRequest`
@@ -203,15 +203,15 @@
             model = models.CreateConfigExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConsumer(self, request):
         """本接口用于创建投递任务
 
         :param request: Request instance for CreateConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateConsumerRequest`
@@ -226,15 +226,15 @@
             model = models.CreateConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCosRecharge(self, request):
         """本接口用于创建cos导入任务
 
         :param request: Request instance for CreateCosRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateCosRechargeRequest`
@@ -249,15 +249,15 @@
             model = models.CreateCosRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDataTransform(self, request):
         """本接口用于创建数据加工任务。
 
         :param request: Request instance for CreateDataTransform.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateDataTransformRequest`
@@ -272,15 +272,15 @@
             model = models.CreateDataTransformResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateExport(self, request):
         """本接口仅创建下载任务，任务返回的下载地址，请用户调用DescribeExports查看任务列表。其中有下载地址CosPath参数。参考文档https://cloud.tencent.com/document/product/614/56449
 
         :param request: Request instance for CreateExport.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateExportRequest`
@@ -295,15 +295,15 @@
             model = models.CreateExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIndex(self, request):
         """本接口用于创建索引
 
         :param request: Request instance for CreateIndex.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateIndexRequest`
@@ -318,15 +318,15 @@
             model = models.CreateIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKafkaRecharge(self, request):
         """本接口用于创建Kafka数据订阅任务
 
         :param request: Request instance for CreateKafkaRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateKafkaRechargeRequest`
@@ -341,15 +341,15 @@
             model = models.CreateKafkaRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLogset(self, request):
         """本接口用于创建日志集，返回新创建的日志集的 ID。
 
         :param request: Request instance for CreateLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateLogsetRequest`
@@ -364,15 +364,15 @@
             model = models.CreateLogsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMachineGroup(self, request):
         """创建机器组
 
         :param request: Request instance for CreateMachineGroup.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateMachineGroupRequest`
@@ -387,15 +387,38 @@
             model = models.CreateMachineGroupResponse()
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
+    def CreateScheduledSql(self, request):
+        """本接口用于创建ScheduledSql任务
+
+        :param request: Request instance for CreateScheduledSql.
+        :type request: :class:`tencentcloud.cls.v20201016.models.CreateScheduledSqlRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.CreateScheduledSqlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateScheduledSql", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateScheduledSqlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateShipper(self, request):
         """新建投递到COS的任务，【！！！注意】使用此接口，需要检查是否配置了投递COS的角色和权限。如果没有配置，请参考文档投递权限查看和配置https://cloud.tencent.com/document/product/614/71623。
 
         :param request: Request instance for CreateShipper.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateShipperRequest`
@@ -410,15 +433,15 @@
             model = models.CreateShipperResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopic(self, request):
         """本接口用于创建日志主题。
 
         :param request: Request instance for CreateTopic.
         :type request: :class:`tencentcloud.cls.v20201016.models.CreateTopicRequest`
@@ -433,15 +456,15 @@
             model = models.CreateTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlarm(self, request):
         """本接口用于删除告警策略。
 
         :param request: Request instance for DeleteAlarm.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteAlarmRequest`
@@ -456,15 +479,15 @@
             model = models.DeleteAlarmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlarmNotice(self, request):
         """该接口用于删除通知渠道组
 
         :param request: Request instance for DeleteAlarmNotice.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteAlarmNoticeRequest`
@@ -479,15 +502,15 @@
             model = models.DeleteAlarmNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfig(self, request):
         """删除采集规则配置
 
         :param request: Request instance for DeleteConfig.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteConfigRequest`
@@ -502,15 +525,15 @@
             model = models.DeleteConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfigExtra(self, request):
         """本接口用于删除特殊采集规则配置，特殊采集配置应用于自建K8S环境的采集Agent
 
         :param request: Request instance for DeleteConfigExtra.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteConfigExtraRequest`
@@ -525,15 +548,15 @@
             model = models.DeleteConfigExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfigFromMachineGroup(self, request):
         """删除应用到机器组的采集配置
 
         :param request: Request instance for DeleteConfigFromMachineGroup.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteConfigFromMachineGroupRequest`
@@ -548,15 +571,15 @@
             model = models.DeleteConfigFromMachineGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConsumer(self, request):
         """本接口用于删除投递配置
 
         :param request: Request instance for DeleteConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteConsumerRequest`
@@ -571,15 +594,15 @@
             model = models.DeleteConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDataTransform(self, request):
         """本接口用于删除数据加工任务
 
         :param request: Request instance for DeleteDataTransform.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteDataTransformRequest`
@@ -594,15 +617,15 @@
             model = models.DeleteDataTransformResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteExport(self, request):
         """本接口用于删除日志下载任务
 
         :param request: Request instance for DeleteExport.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteExportRequest`
@@ -617,15 +640,15 @@
             model = models.DeleteExportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIndex(self, request):
         """本接口用于删除日志主题的索引配置，删除索引配置后将无法检索和查询采集到的日志。
 
         :param request: Request instance for DeleteIndex.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteIndexRequest`
@@ -640,15 +663,15 @@
             model = models.DeleteIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteKafkaRecharge(self, request):
         """本接口用于删除Kafka数据订阅任务
 
         :param request: Request instance for DeleteKafkaRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteKafkaRechargeRequest`
@@ -663,15 +686,15 @@
             model = models.DeleteKafkaRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLogset(self, request):
         """本接口用于删除日志集。
 
         :param request: Request instance for DeleteLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteLogsetRequest`
@@ -686,15 +709,15 @@
             model = models.DeleteLogsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMachineGroup(self, request):
         """删除机器组
 
         :param request: Request instance for DeleteMachineGroup.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteMachineGroupRequest`
@@ -709,15 +732,15 @@
             model = models.DeleteMachineGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMachineGroupInfo(self, request):
         """用于删除机器组信息
 
         :param request: Request instance for DeleteMachineGroupInfo.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteMachineGroupInfoRequest`
@@ -732,15 +755,15 @@
             model = models.DeleteMachineGroupInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteShipper(self, request):
         """删除投递COS任务
 
         :param request: Request instance for DeleteShipper.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteShipperRequest`
@@ -755,15 +778,15 @@
             model = models.DeleteShipperResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopic(self, request):
         """本接口用于删除日志主题。
 
         :param request: Request instance for DeleteTopic.
         :type request: :class:`tencentcloud.cls.v20201016.models.DeleteTopicRequest`
@@ -778,15 +801,15 @@
             model = models.DeleteTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarmNotices(self, request):
         """该接口用于获取通知渠道组列表
 
         :param request: Request instance for DescribeAlarmNotices.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeAlarmNoticesRequest`
@@ -801,15 +824,15 @@
             model = models.DescribeAlarmNoticesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlarms(self, request):
         """本接口用于获取告警策略列表。
 
         :param request: Request instance for DescribeAlarms.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeAlarmsRequest`
@@ -824,15 +847,15 @@
             model = models.DescribeAlarmsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlertRecordHistory(self, request):
         """获取告警历史，例如今天未恢复的告警
 
         :param request: Request instance for DescribeAlertRecordHistory.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeAlertRecordHistoryRequest`
@@ -847,15 +870,15 @@
             model = models.DescribeAlertRecordHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigExtras(self, request):
         """本接口用于获取特殊采集配置，特殊采集配置应用于自建K8S环境的采集Agent
 
         :param request: Request instance for DescribeConfigExtras.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeConfigExtrasRequest`
@@ -870,15 +893,15 @@
             model = models.DescribeConfigExtrasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigMachineGroups(self, request):
         """获取采集规则配置所绑定的机器组
 
         :param request: Request instance for DescribeConfigMachineGroups.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeConfigMachineGroupsRequest`
@@ -893,15 +916,15 @@
             model = models.DescribeConfigMachineGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigs(self, request):
         """获取采集规则配置
 
         :param request: Request instance for DescribeConfigs.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeConfigsRequest`
@@ -916,15 +939,15 @@
             model = models.DescribeConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConsumer(self, request):
         """本接口用于获取投递配置
 
         :param request: Request instance for DescribeConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeConsumerRequest`
@@ -939,15 +962,15 @@
             model = models.DescribeConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCosRecharges(self, request):
         """本接口用于获取cos导入配置
 
         :param request: Request instance for DescribeCosRecharges.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeCosRechargesRequest`
@@ -962,15 +985,15 @@
             model = models.DescribeCosRechargesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDataTransformInfo(self, request):
         """本接口用于获取数据加工任务列表基本信息
 
         :param request: Request instance for DescribeDataTransformInfo.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeDataTransformInfoRequest`
@@ -985,15 +1008,15 @@
             model = models.DescribeDataTransformInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExports(self, request):
         """本接口用于获取日志下载任务列表
 
         :param request: Request instance for DescribeExports.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeExportsRequest`
@@ -1008,15 +1031,15 @@
             model = models.DescribeExportsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIndex(self, request):
         """本接口用于获取索引配置信息
 
         :param request: Request instance for DescribeIndex.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeIndexRequest`
@@ -1031,15 +1054,15 @@
             model = models.DescribeIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKafkaRecharges(self, request):
         """本接口用于获取Kafka数据订阅任务
 
         :param request: Request instance for DescribeKafkaRecharges.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaRechargesRequest`
@@ -1054,15 +1077,15 @@
             model = models.DescribeKafkaRechargesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogContext(self, request):
         """本接口用于搜索日志上下文附近的内容
 
         :param request: Request instance for DescribeLogContext.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeLogContextRequest`
@@ -1077,15 +1100,15 @@
             model = models.DescribeLogContextResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogHistogram(self, request):
         """本接口用于构建日志数量直方图
 
         :param request: Request instance for DescribeLogHistogram.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeLogHistogramRequest`
@@ -1100,15 +1123,15 @@
             model = models.DescribeLogHistogramResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogsets(self, request):
         """本接口用于获取日志集信息列表。
 
         :param request: Request instance for DescribeLogsets.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeLogsetsRequest`
@@ -1123,15 +1146,15 @@
             model = models.DescribeLogsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachineGroupConfigs(self, request):
         """获取机器组绑定的采集规则配置
 
         :param request: Request instance for DescribeMachineGroupConfigs.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeMachineGroupConfigsRequest`
@@ -1146,15 +1169,15 @@
             model = models.DescribeMachineGroupConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachineGroups(self, request):
         """获取机器组信息列表
 
         :param request: Request instance for DescribeMachineGroups.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeMachineGroupsRequest`
@@ -1169,15 +1192,15 @@
             model = models.DescribeMachineGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachines(self, request):
         """获取制定机器组下的机器状态
 
         :param request: Request instance for DescribeMachines.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeMachinesRequest`
@@ -1192,15 +1215,15 @@
             model = models.DescribeMachinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePartitions(self, request):
         """本接口用于获取主题分区列表。
 
         :param request: Request instance for DescribePartitions.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribePartitionsRequest`
@@ -1215,15 +1238,15 @@
             model = models.DescribePartitionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShipperTasks(self, request):
         """获取投递任务列表
 
         :param request: Request instance for DescribeShipperTasks.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeShipperTasksRequest`
@@ -1238,15 +1261,15 @@
             model = models.DescribeShipperTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShippers(self, request):
         """获取投递到COS的任务配置信息
 
         :param request: Request instance for DescribeShippers.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeShippersRequest`
@@ -1261,15 +1284,15 @@
             model = models.DescribeShippersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopics(self, request):
         """本接口用于获取日志主题列表，支持分页
 
         :param request: Request instance for DescribeTopics.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeTopicsRequest`
@@ -1284,15 +1307,15 @@
             model = models.DescribeTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAlarmLog(self, request):
         """本接口用于获取告警任务历史
 
         :param request: Request instance for GetAlarmLog.
         :type request: :class:`tencentcloud.cls.v20201016.models.GetAlarmLogRequest`
@@ -1307,15 +1330,15 @@
             model = models.GetAlarmLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MergePartition(self, request):
         """本接口用于合并一个读写态的主题分区，合并时指定一个主题分区 ID，日志服务会自动合并范围右相邻的分区。
 
         :param request: Request instance for MergePartition.
         :type request: :class:`tencentcloud.cls.v20201016.models.MergePartitionRequest`
@@ -1330,15 +1353,15 @@
             model = models.MergePartitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarm(self, request):
         """本接口用于修改告警策略。需要至少修改一项有效内容。
 
         :param request: Request instance for ModifyAlarm.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyAlarmRequest`
@@ -1353,15 +1376,15 @@
             model = models.ModifyAlarmResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAlarmNotice(self, request):
         """该接口用于修改通知渠道组
 
         :param request: Request instance for ModifyAlarmNotice.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyAlarmNoticeRequest`
@@ -1376,15 +1399,15 @@
             model = models.ModifyAlarmNoticeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConfig(self, request):
         """修改采集规则配置
 
         :param request: Request instance for ModifyConfig.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyConfigRequest`
@@ -1399,15 +1422,15 @@
             model = models.ModifyConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConfigExtra(self, request):
         """本接口用于修改特殊采集配置任务，特殊采集配置应用于自建K8S环境的采集Agent
 
         :param request: Request instance for ModifyConfigExtra.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyConfigExtraRequest`
@@ -1422,15 +1445,15 @@
             model = models.ModifyConfigExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConsumer(self, request):
         """本接口用于修改投递任务
 
         :param request: Request instance for ModifyConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyConsumerRequest`
@@ -1445,15 +1468,15 @@
             model = models.ModifyConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCosRecharge(self, request):
         """本接口用于修改cos导入任务
 
         :param request: Request instance for ModifyCosRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyCosRechargeRequest`
@@ -1468,15 +1491,15 @@
             model = models.ModifyCosRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDataTransform(self, request):
         """本接口用于修改数据加工任务
 
         :param request: Request instance for ModifyDataTransform.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyDataTransformRequest`
@@ -1491,15 +1514,15 @@
             model = models.ModifyDataTransformResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIndex(self, request):
         """本接口用于修改索引配置，该接口除受默认接口请求频率限制外，针对单个日志主题，并发数不能超过1，即同一时间同一个日志主题只能有一个正在执行的索引配置修改操作。
 
         :param request: Request instance for ModifyIndex.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyIndexRequest`
@@ -1514,15 +1537,15 @@
             model = models.ModifyIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyKafkaRecharge(self, request):
         """本接口用于修改Kafka数据订阅任务
 
         :param request: Request instance for ModifyKafkaRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaRechargeRequest`
@@ -1537,15 +1560,15 @@
             model = models.ModifyKafkaRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLogset(self, request):
         """本接口用于修改日志集信息
 
         :param request: Request instance for ModifyLogset.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyLogsetRequest`
@@ -1560,15 +1583,15 @@
             model = models.ModifyLogsetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMachineGroup(self, request):
         """修改机器组
 
         :param request: Request instance for ModifyMachineGroup.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyMachineGroupRequest`
@@ -1583,15 +1606,15 @@
             model = models.ModifyMachineGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyShipper(self, request):
         """修改现有的投递规则，客户如果使用此接口，需要自行处理CLS对指定bucket的写权限。
 
         :param request: Request instance for ModifyShipper.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyShipperRequest`
@@ -1606,15 +1629,15 @@
             model = models.ModifyShipperResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopic(self, request):
         """本接口用于修改日志主题。
 
         :param request: Request instance for ModifyTopic.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyTopicRequest`
@@ -1629,15 +1652,15 @@
             model = models.ModifyTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenKafkaConsumer(self, request):
         """打开Kafka协议消费功能
 
         :param request: Request instance for OpenKafkaConsumer.
         :type request: :class:`tencentcloud.cls.v20201016.models.OpenKafkaConsumerRequest`
@@ -1652,15 +1675,15 @@
             model = models.OpenKafkaConsumerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PreviewKafkaRecharge(self, request):
         """本接口用于预览Kafka数据订阅任务客户日志信息
 
         :param request: Request instance for PreviewKafkaRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.PreviewKafkaRechargeRequest`
@@ -1675,15 +1698,15 @@
             model = models.PreviewKafkaRechargeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryShipperTask(self, request):
         """重试失败的投递任务
 
         :param request: Request instance for RetryShipperTask.
         :type request: :class:`tencentcloud.cls.v20201016.models.RetryShipperTaskRequest`
@@ -1698,15 +1721,15 @@
             model = models.RetryShipperTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchLog(self, request):
         """本接口用于检索分析日志, 该接口除受默认接口请求频率限制外，针对单个日志主题，查询并发数不能超过15。
 
         :param request: Request instance for SearchLog.
         :type request: :class:`tencentcloud.cls.v20201016.models.SearchLogRequest`
@@ -1721,15 +1744,15 @@
             model = models.SearchLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SplitPartition(self, request):
         """本接口用于分裂主题分区
 
         :param request: Request instance for SplitPartition.
         :type request: :class:`tencentcloud.cls.v20201016.models.SplitPartitionRequest`
@@ -1744,15 +1767,15 @@
             model = models.SplitPartitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UploadLog(self, request, body):
         """## 提示
         为了保障您日志数据的可靠性以及更高效地使用日志服务，建议您使用CLS优化后的接口[上传结构化日志](https://cloud.tencent.com/document/product/614/16873)。
 
         同时我们给此接口专门优化定制了多个语言版本的SDK供您选择，SDK提供统一的异步发送、资源控制、自动重试、优雅关闭、感知上报等功能，使上报日志功能更完善，详情请参考[SDK采集](https://cloud.tencent.com/document/product/614/67157)。
@@ -1920,8 +1943,8 @@
             model = models.UploadLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.937/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.938/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4528,14 +4528,230 @@
 
 
     def _deserialize(self, params):
         self._GroupId = params.get("GroupId")
         self._RequestId = params.get("RequestId")
 
 
+class CreateScheduledSqlRequest(AbstractModel):
+    """CreateScheduledSql请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _SrcTopicId: 源日志主题
+        :type SrcTopicId: str
+        :param _Name: 任务名称
+        :type Name: str
+        :param _EnableFlag: 任务启动状态.  1正常开启,  2关闭
+        :type EnableFlag: int
+        :param _DstResource: 加工任务目的topic_id以及别名
+        :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
+        :param _ScheduledSqlContent: ScheduledSQL语句
+        :type ScheduledSqlContent: str
+        :param _ProcessStartTime: 调度开始时间,Unix时间戳，单位ms
+        :type ProcessStartTime: int
+        :param _ProcessType: 调度类型，1:持续运行 2:指定调度结束时间
+        :type ProcessType: int
+        :param _ProcessPeriod: 调度周期(分钟)
+        :type ProcessPeriod: int
+        :param _ProcessTimeWindow: 调度时间窗口
+        :type ProcessTimeWindow: str
+        :param _ProcessDelay: 执行延迟(秒)
+        :type ProcessDelay: int
+        :param _SrcTopicRegion: 源topicId的地域信息
+        :type SrcTopicRegion: str
+        :param _ProcessEndTime: 调度结束时间，当ProcessType=2时为必传字段, Unix时间戳，单位ms
+        :type ProcessEndTime: int
+        :param _SyntaxRule: 语法规则。 默认值为0。0：Lucene语法，1：CQL语法  
+        :type SyntaxRule: int
+        """
+        self._SrcTopicId = None
+        self._Name = None
+        self._EnableFlag = None
+        self._DstResource = None
+        self._ScheduledSqlContent = None
+        self._ProcessStartTime = None
+        self._ProcessType = None
+        self._ProcessPeriod = None
+        self._ProcessTimeWindow = None
+        self._ProcessDelay = None
+        self._SrcTopicRegion = None
+        self._ProcessEndTime = None
+        self._SyntaxRule = None
+
+    @property
+    def SrcTopicId(self):
+        return self._SrcTopicId
+
+    @SrcTopicId.setter
+    def SrcTopicId(self, SrcTopicId):
+        self._SrcTopicId = SrcTopicId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def EnableFlag(self):
+        return self._EnableFlag
+
+    @EnableFlag.setter
+    def EnableFlag(self, EnableFlag):
+        self._EnableFlag = EnableFlag
+
+    @property
+    def DstResource(self):
+        return self._DstResource
+
+    @DstResource.setter
+    def DstResource(self, DstResource):
+        self._DstResource = DstResource
+
+    @property
+    def ScheduledSqlContent(self):
+        return self._ScheduledSqlContent
+
+    @ScheduledSqlContent.setter
+    def ScheduledSqlContent(self, ScheduledSqlContent):
+        self._ScheduledSqlContent = ScheduledSqlContent
+
+    @property
+    def ProcessStartTime(self):
+        return self._ProcessStartTime
+
+    @ProcessStartTime.setter
+    def ProcessStartTime(self, ProcessStartTime):
+        self._ProcessStartTime = ProcessStartTime
+
+    @property
+    def ProcessType(self):
+        return self._ProcessType
+
+    @ProcessType.setter
+    def ProcessType(self, ProcessType):
+        self._ProcessType = ProcessType
+
+    @property
+    def ProcessPeriod(self):
+        return self._ProcessPeriod
+
+    @ProcessPeriod.setter
+    def ProcessPeriod(self, ProcessPeriod):
+        self._ProcessPeriod = ProcessPeriod
+
+    @property
+    def ProcessTimeWindow(self):
+        return self._ProcessTimeWindow
+
+    @ProcessTimeWindow.setter
+    def ProcessTimeWindow(self, ProcessTimeWindow):
+        self._ProcessTimeWindow = ProcessTimeWindow
+
+    @property
+    def ProcessDelay(self):
+        return self._ProcessDelay
+
+    @ProcessDelay.setter
+    def ProcessDelay(self, ProcessDelay):
+        self._ProcessDelay = ProcessDelay
+
+    @property
+    def SrcTopicRegion(self):
+        return self._SrcTopicRegion
+
+    @SrcTopicRegion.setter
+    def SrcTopicRegion(self, SrcTopicRegion):
+        self._SrcTopicRegion = SrcTopicRegion
+
+    @property
+    def ProcessEndTime(self):
+        return self._ProcessEndTime
+
+    @ProcessEndTime.setter
+    def ProcessEndTime(self, ProcessEndTime):
+        self._ProcessEndTime = ProcessEndTime
+
+    @property
+    def SyntaxRule(self):
+        return self._SyntaxRule
+
+    @SyntaxRule.setter
+    def SyntaxRule(self, SyntaxRule):
+        self._SyntaxRule = SyntaxRule
+
+
+    def _deserialize(self, params):
+        self._SrcTopicId = params.get("SrcTopicId")
+        self._Name = params.get("Name")
+        self._EnableFlag = params.get("EnableFlag")
+        if params.get("DstResource") is not None:
+            self._DstResource = ScheduledSqlResouceInfo()
+            self._DstResource._deserialize(params.get("DstResource"))
+        self._ScheduledSqlContent = params.get("ScheduledSqlContent")
+        self._ProcessStartTime = params.get("ProcessStartTime")
+        self._ProcessType = params.get("ProcessType")
+        self._ProcessPeriod = params.get("ProcessPeriod")
+        self._ProcessTimeWindow = params.get("ProcessTimeWindow")
+        self._ProcessDelay = params.get("ProcessDelay")
+        self._SrcTopicRegion = params.get("SrcTopicRegion")
+        self._ProcessEndTime = params.get("ProcessEndTime")
+        self._SyntaxRule = params.get("SyntaxRule")
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
+class CreateScheduledSqlResponse(AbstractModel):
+    """CreateScheduledSql返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务id
+        :type TaskId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TaskId = None
+        self._RequestId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
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
+        self._TaskId = params.get("TaskId")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateShipperRequest(AbstractModel):
     """CreateShipper请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14665,14 +14881,59 @@
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
+class ScheduledSqlResouceInfo(AbstractModel):
+    """ScheduledSql的资源信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TopicId: 目标主题id
+        :type TopicId: str
+        :param _Region: topic的地域信息
+        :type Region: str
+        """
+        self._TopicId = None
+        self._Region = None
+
+    @property
+    def TopicId(self):
+        return self._TopicId
+
+    @TopicId.setter
+    def TopicId(self, TopicId):
+        self._TopicId = TopicId
+
+    @property
+    def Region(self):
+        return self._Region
+
+    @Region.setter
+    def Region(self, Region):
+        self._Region = Region
+
+
+    def _deserialize(self, params):
+        self._TopicId = params.get("TopicId")
+        self._Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SearchLogRequest(AbstractModel):
     """SearchLog请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-cls-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.937/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.938/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.937/README.rst` & `tencentcloud-sdk-python-cls-3.0.938/README.rst`

 * *Files identical despite different names*

