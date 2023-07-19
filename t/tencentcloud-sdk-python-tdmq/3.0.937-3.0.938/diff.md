# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.937.tar", last modified: Tue Jul 18 00:32:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.938.tar", last modified: Wed Jul 19 00:49:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.937.tar` & `tencentcloud-sdk-python-tdmq-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94149 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   591001 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:32:16.000000 tencentcloud-sdk-python-tdmq-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94553 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   591001 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:49:53.000000 tencentcloud-sdk-python-tdmq-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AcknowledgeMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClearCmqQueue(self, request):
         """清空cmq消息队列中的消息
 
         :param request: Request instance for ClearCmqQueue.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ClearCmqQueueRequest`
@@ -65,15 +65,15 @@
             model = models.ClearCmqQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClearCmqSubscriptionFilterTags(self, request):
         """清空订阅者消息标签
 
         :param request: Request instance for ClearCmqSubscriptionFilterTags.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ClearCmqSubscriptionFilterTagsRequest`
@@ -88,15 +88,15 @@
             model = models.ClearCmqSubscriptionFilterTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """创建用户的集群
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateClusterRequest`
@@ -111,15 +111,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCmqQueue(self, request):
         """创建cmq队列接口
 
         :param request: Request instance for CreateCmqQueue.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateCmqQueueRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCmqQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCmqSubscribe(self, request):
         """创建cmq订阅接口
 
         :param request: Request instance for CreateCmqSubscribe.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateCmqSubscribeRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCmqSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCmqTopic(self, request):
         """创建cmq主题
 
         :param request: Request instance for CreateCmqTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateCmqTopicRequest`
@@ -180,15 +180,15 @@
             model = models.CreateCmqTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEnvironment(self, request):
         """用于在用户账户下创建消息队列 Tdmq 命名空间
 
         :param request: Request instance for CreateEnvironment.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateEnvironmentRequest`
@@ -203,15 +203,15 @@
             model = models.CreateEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEnvironmentRole(self, request):
         """创建环境角色授权
 
         :param request: Request instance for CreateEnvironmentRole.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateEnvironmentRoleRequest`
@@ -226,15 +226,15 @@
             model = models.CreateEnvironmentRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRabbitMQUser(self, request):
         """创建RabbitMQ的用户
 
         :param request: Request instance for CreateRabbitMQUser.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRabbitMQUserRequest`
@@ -249,15 +249,15 @@
             model = models.CreateRabbitMQUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRabbitMQVipInstance(self, request):
         """创建RabbitMQ专享版实例
 
         :param request: Request instance for CreateRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRabbitMQVipInstanceRequest`
@@ -272,15 +272,15 @@
             model = models.CreateRabbitMQVipInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRabbitMQVirtualHost(self, request):
         """创建RabbitMQ的vhost
 
         :param request: Request instance for CreateRabbitMQVirtualHost.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRabbitMQVirtualHostRequest`
@@ -295,15 +295,15 @@
             model = models.CreateRabbitMQVirtualHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRocketMQCluster(self, request):
         """此接口用于创建一个RocketMQ集群
 
         :param request: Request instance for CreateRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQClusterRequest`
@@ -318,15 +318,15 @@
             model = models.CreateRocketMQClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRocketMQGroup(self, request):
         """创建RocketMQ消费组
 
         :param request: Request instance for CreateRocketMQGroup.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQGroupRequest`
@@ -341,15 +341,15 @@
             model = models.CreateRocketMQGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRocketMQNamespace(self, request):
         """创建RocketMQ命名空间
 
         :param request: Request instance for CreateRocketMQNamespace.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQNamespaceRequest`
@@ -364,15 +364,15 @@
             model = models.CreateRocketMQNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRocketMQTopic(self, request):
         """创建RocketMQ主题
 
         :param request: Request instance for CreateRocketMQTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQTopicRequest`
@@ -387,15 +387,15 @@
             model = models.CreateRocketMQTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRole(self, request):
         """创建角色
 
         :param request: Request instance for CreateRole.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRoleRequest`
@@ -410,15 +410,15 @@
             model = models.CreateRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSubscription(self, request):
         """创建一个主题的订阅关系
 
         :param request: Request instance for CreateSubscription.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateSubscriptionRequest`
@@ -433,15 +433,15 @@
             model = models.CreateSubscriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTopic(self, request):
         """新增指定分区、类型的消息主题
 
         :param request: Request instance for CreateTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateTopicRequest`
@@ -456,15 +456,15 @@
             model = models.CreateTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """删除集群
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteClusterRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCmqQueue(self, request):
         """删除cmq队列
 
         :param request: Request instance for DeleteCmqQueue.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteCmqQueueRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteCmqQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCmqSubscribe(self, request):
         """删除cmq订阅
 
         :param request: Request instance for DeleteCmqSubscribe.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteCmqSubscribeRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteCmqSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCmqTopic(self, request):
         """删除cmq主题
 
         :param request: Request instance for DeleteCmqTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteCmqTopicRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteCmqTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEnvironmentRoles(self, request):
         """删除环境角色授权。
 
         :param request: Request instance for DeleteEnvironmentRoles.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteEnvironmentRolesRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteEnvironmentRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEnvironments(self, request):
         """批量删除租户下的命名空间
 
         :param request: Request instance for DeleteEnvironments.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteEnvironmentsRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRabbitMQUser(self, request):
         """删除RabbitMQ的用户
 
         :param request: Request instance for DeleteRabbitMQUser.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQUserRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteRabbitMQUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRabbitMQVipInstance(self, request):
         """删除RabbitMQ专享版实例
 
         :param request: Request instance for DeleteRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVipInstanceRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteRabbitMQVipInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRabbitMQVirtualHost(self, request):
         """删除RabbitMQ的vhost
 
         :param request: Request instance for DeleteRabbitMQVirtualHost.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVirtualHostRequest`
@@ -663,15 +663,15 @@
             model = models.DeleteRabbitMQVirtualHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRocketMQCluster(self, request):
         """删除RocketMQ集群
 
         :param request: Request instance for DeleteRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQClusterRequest`
@@ -686,15 +686,15 @@
             model = models.DeleteRocketMQClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRocketMQGroup(self, request):
         """删除RocketMQ消费组
 
         :param request: Request instance for DeleteRocketMQGroup.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQGroupRequest`
@@ -709,15 +709,15 @@
             model = models.DeleteRocketMQGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRocketMQNamespace(self, request):
         """删除RocketMQ命名空间
 
         :param request: Request instance for DeleteRocketMQNamespace.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQNamespaceRequest`
@@ -732,15 +732,15 @@
             model = models.DeleteRocketMQNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRocketMQTopic(self, request):
         """删除RocketMQ主题
 
         :param request: Request instance for DeleteRocketMQTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQTopicRequest`
@@ -755,15 +755,15 @@
             model = models.DeleteRocketMQTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRoles(self, request):
         """删除角色，支持批量。
 
         :param request: Request instance for DeleteRoles.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRolesRequest`
@@ -778,15 +778,15 @@
             model = models.DeleteRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSubscriptions(self, request):
         """删除订阅关系
 
         :param request: Request instance for DeleteSubscriptions.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteSubscriptionsRequest`
@@ -801,15 +801,15 @@
             model = models.DeleteSubscriptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTopics(self, request):
         """批量删除topics
 
         :param request: Request instance for DeleteTopics.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteTopicsRequest`
@@ -824,15 +824,15 @@
             model = models.DeleteTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAMQPClusters(self, request):
         """获取amqp集群列表
 
         :param request: Request instance for DescribeAMQPClusters.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeAMQPClustersRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeAMQPClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllTenants(self, request):
         """获取某个租户的虚拟集群列表
 
         :param request: Request instance for DescribeAllTenants.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeAllTenantsRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeAllTenantsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBindClusters(self, request):
         """获取用户绑定的专享集群列表
 
         :param request: Request instance for DescribeBindClusters.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeBindClustersRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeBindClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBindVpcs(self, request):
         """获取租户VPC绑定关系
 
         :param request: Request instance for DescribeBindVpcs.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeBindVpcsRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeBindVpcsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterDetail(self, request):
         """获取集群的详细信息
 
         :param request: Request instance for DescribeClusterDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeClusterDetailRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeClusterDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """获取集群列表
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeClustersRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqDeadLetterSourceQueues(self, request):
         """枚举cmq死信队列源队列
 
         :param request: Request instance for DescribeCmqDeadLetterSourceQueues.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqDeadLetterSourceQueuesRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeCmqDeadLetterSourceQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqQueueDetail(self, request):
         """查询cmq队列详情
 
         :param request: Request instance for DescribeCmqQueueDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqQueueDetailRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeCmqQueueDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqQueues(self, request):
         """查询cmq全量队列
 
         :param request: Request instance for DescribeCmqQueues.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqQueuesRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeCmqQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqSubscriptionDetail(self, request):
         """查询cmq订阅详情
 
         :param request: Request instance for DescribeCmqSubscriptionDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqSubscriptionDetailRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeCmqSubscriptionDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqTopicDetail(self, request):
         """查询cmq主题详情
 
         :param request: Request instance for DescribeCmqTopicDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqTopicDetailRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeCmqTopicDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCmqTopics(self, request):
         """枚举cmq全量主题
 
         :param request: Request instance for DescribeCmqTopics.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeCmqTopicsRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeCmqTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironmentAttributes(self, request):
         """获取指定命名空间的属性
 
         :param request: Request instance for DescribeEnvironmentAttributes.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeEnvironmentAttributesRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeEnvironmentAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironmentRoles(self, request):
         """获取命名空间角色列表
 
         :param request: Request instance for DescribeEnvironmentRoles.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeEnvironmentRolesRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeEnvironmentRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironments(self, request):
         """获取租户下命名空间列表
 
         :param request: Request instance for DescribeEnvironments.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeEnvironmentsRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespaceBundlesOpt(self, request):
         """运营端获取命名空间bundle列表
 
         :param request: Request instance for DescribeNamespaceBundlesOpt.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeNamespaceBundlesOptRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeNamespaceBundlesOptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNodeHealthOpt(self, request):
         """运营端获节点健康状态
 
         :param request: Request instance for DescribeNodeHealthOpt.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeNodeHealthOptRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeNodeHealthOptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublisherSummary(self, request):
         """获取消息生产概览信息
 
         :param request: Request instance for DescribePublisherSummary.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePublisherSummaryRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribePublisherSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublishers(self, request):
         """获取生产者信息列表
 
         :param request: Request instance for DescribePublishers.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePublishersRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribePublishersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePulsarProInstanceDetail(self, request):
         """获取Pulsar专业版集群实例信息
 
         :param request: Request instance for DescribePulsarProInstanceDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstanceDetailRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribePulsarProInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePulsarProInstances(self, request):
         """查询用户已购的Pulsar专业版实例列表
 
         :param request: Request instance for DescribePulsarProInstances.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstancesRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribePulsarProInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQNodeList(self, request):
         """RabbitMQ专享版查询节点列表
 
         :param request: Request instance for DescribeRabbitMQNodeList.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQNodeListRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeRabbitMQNodeListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQUser(self, request):
         """查询RabbitMQ用户列表
 
         :param request: Request instance for DescribeRabbitMQUser.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQUserRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeRabbitMQUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQVipInstance(self, request):
         """获取单个RabbitMQ专享实例信息
 
         :param request: Request instance for DescribeRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVipInstanceRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeRabbitMQVipInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQVipInstances(self, request):
         """查询用户已购的RabbitMQ专享实例列表
 
         :param request: Request instance for DescribeRabbitMQVipInstances.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVipInstancesRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeRabbitMQVipInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQVirtualHost(self, request):
         """查询RabbitMQ vhost列表
 
         :param request: Request instance for DescribeRabbitMQVirtualHost.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeRabbitMQVirtualHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRabbitMQVirtualHostList(self, request):
         """RabbitMQ专享版查询虚拟主机列表
 
         :param request: Request instance for DescribeRabbitMQVirtualHostList.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQVirtualHostListRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeRabbitMQVirtualHostListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQCluster(self, request):
         """获取单个RocketMQ集群信息
 
         :param request: Request instance for DescribeRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQClusterRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeRocketMQClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQClusters(self, request):
         """获取RocketMQ集群列表
 
         :param request: Request instance for DescribeRocketMQClusters.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQClustersRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeRocketMQClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQGroups(self, request):
         """获取RocketMQ消费组列表
 
         :param request: Request instance for DescribeRocketMQGroups.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQGroupsRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeRocketMQGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQMsg(self, request):
         """rocketmq消息详情
 
         :param request: Request instance for DescribeRocketMQMsg.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQMsgRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeRocketMQMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQNamespaces(self, request):
         """获取RocketMQ命名空间列表
 
         :param request: Request instance for DescribeRocketMQNamespaces.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQNamespacesRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeRocketMQNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQTopics(self, request):
         """获取RocketMQ主题列表
 
         :param request: Request instance for DescribeRocketMQTopics.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQTopicsRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeRocketMQTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQVipInstanceDetail(self, request):
         """获取单个RocketMQ专享集群信息
 
         :param request: Request instance for DescribeRocketMQVipInstanceDetail.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQVipInstanceDetailRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeRocketMQVipInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRocketMQVipInstances(self, request):
         """查询用户已购的RocketMQ专享实例列表
 
         :param request: Request instance for DescribeRocketMQVipInstances.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRocketMQVipInstancesRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribeRocketMQVipInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRoles(self, request):
         """获取角色列表
 
         :param request: Request instance for DescribeRoles.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRolesRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeRolesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubscriptions(self, request):
         """查询指定环境和主题下的订阅者列表
 
         :param request: Request instance for DescribeSubscriptions.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeSubscriptionsRequest`
@@ -1675,15 +1675,15 @@
             model = models.DescribeSubscriptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopics(self, request):
         """获取环境下主题列表
 
         :param request: Request instance for DescribeTopics.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeTopicsRequest`
@@ -1698,15 +1698,15 @@
             model = models.DescribeTopicsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAMQPCluster(self, request):
         """更新Amqp集群信息
 
         :param request: Request instance for ModifyAMQPCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyAMQPClusterRequest`
@@ -1721,15 +1721,15 @@
             model = models.ModifyAMQPClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCluster(self, request):
         """更新集群信息
 
         :param request: Request instance for ModifyCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyClusterRequest`
@@ -1744,15 +1744,15 @@
             model = models.ModifyClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCmqQueueAttribute(self, request):
         """修改cmq队列属性
 
         :param request: Request instance for ModifyCmqQueueAttribute.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyCmqQueueAttributeRequest`
@@ -1767,15 +1767,15 @@
             model = models.ModifyCmqQueueAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCmqSubscriptionAttribute(self, request):
         """修改cmq订阅属性
 
         :param request: Request instance for ModifyCmqSubscriptionAttribute.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyCmqSubscriptionAttributeRequest`
@@ -1790,15 +1790,15 @@
             model = models.ModifyCmqSubscriptionAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCmqTopicAttribute(self, request):
         """修改cmq主题属性
 
         :param request: Request instance for ModifyCmqTopicAttribute.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyCmqTopicAttributeRequest`
@@ -1813,15 +1813,15 @@
             model = models.ModifyCmqTopicAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEnvironmentAttributes(self, request):
         """修改指定命名空间的属性值
 
         :param request: Request instance for ModifyEnvironmentAttributes.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyEnvironmentAttributesRequest`
@@ -1836,15 +1836,15 @@
             model = models.ModifyEnvironmentAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEnvironmentRole(self, request):
         """修改环境角色授权。
 
         :param request: Request instance for ModifyEnvironmentRole.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyEnvironmentRoleRequest`
@@ -1859,15 +1859,15 @@
             model = models.ModifyEnvironmentRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRabbitMQUser(self, request):
         """修改RabbitMQ的用户
 
         :param request: Request instance for ModifyRabbitMQUser.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQUserRequest`
@@ -1882,15 +1882,15 @@
             model = models.ModifyRabbitMQUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRabbitMQVipInstance(self, request):
         """修改RabbitMQ专享版实例
 
         :param request: Request instance for ModifyRabbitMQVipInstance.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVipInstanceRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifyRabbitMQVipInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRabbitMQVirtualHost(self, request):
         """修改RabbitMQ的vhost
 
         :param request: Request instance for ModifyRabbitMQVirtualHost.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRabbitMQVirtualHostRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyRabbitMQVirtualHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRocketMQCluster(self, request):
         """更新RocketMQ集群信息
 
         :param request: Request instance for ModifyRocketMQCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQClusterRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyRocketMQClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRocketMQGroup(self, request):
         """更新RocketMQ消费组信息
 
         :param request: Request instance for ModifyRocketMQGroup.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQGroupRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyRocketMQGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRocketMQInstanceSpec(self, request):
         """本API用于修改RocketMQ专享实例配置，可以支持实例规格、节点数和存储的升配和实例规格的降配。本API发起订单并成功支付后进入实例配置变更的流程，可通过DescribeRocketMQVipInstances查询实例是否已变更完成。
 
         :param request: Request instance for ModifyRocketMQInstanceSpec.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQInstanceSpecRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyRocketMQInstanceSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRocketMQNamespace(self, request):
         """更新RocketMQ命名空间
 
         :param request: Request instance for ModifyRocketMQNamespace.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQNamespaceRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyRocketMQNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRocketMQTopic(self, request):
         """更新RocketMQ主题信息
 
         :param request: Request instance for ModifyRocketMQTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQTopicRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyRocketMQTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRole(self, request):
         """角色修改
 
         :param request: Request instance for ModifyRole.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRoleRequest`
@@ -2066,15 +2066,15 @@
             model = models.ModifyRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTopic(self, request):
         """修改主题备注和分区数
 
         :param request: Request instance for ModifyTopic.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyTopicRequest`
@@ -2089,15 +2089,15 @@
             model = models.ModifyTopicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishCmqMsg(self, request):
         """发送cmq主题消息
 
         :param request: Request instance for PublishCmqMsg.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.PublishCmqMsgRequest`
@@ -2112,15 +2112,15 @@
             model = models.PublishCmqMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReceiveMessage(self, request):
         """当前 ReceiveMessage 接口只支持 Partitioned 类型的 Topic。该接口用于接收发送到指定 Partitioned Topic 中的消息，当 Partitioned Topic 中没有消息但还去尝试调用该接口时，会抛出 ReceiveTimeout 的异常。
 
         如何使用 BatchReceivePolicy：
 
@@ -2154,15 +2154,15 @@
             model = models.ReceiveMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetMsgSubOffsetByTimestamp(self, request):
         """根据时间戳进行消息回溯，精确到毫秒
 
         :param request: Request instance for ResetMsgSubOffsetByTimestamp.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ResetMsgSubOffsetByTimestampRequest`
@@ -2177,15 +2177,15 @@
             model = models.ResetMsgSubOffsetByTimestampResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetRocketMQConsumerOffSet(self, request):
         """重置指定Group的消费位点到指定时间戳
 
         :param request: Request instance for ResetRocketMQConsumerOffSet.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ResetRocketMQConsumerOffSetRequest`
@@ -2200,15 +2200,15 @@
             model = models.ResetRocketMQConsumerOffSetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RewindCmqQueue(self, request):
         """回溯cmq队列
 
         :param request: Request instance for RewindCmqQueue.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.RewindCmqQueueRequest`
@@ -2223,15 +2223,15 @@
             model = models.RewindCmqQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendBatchMessages(self, request):
         """批量发送消息
 
         注意：TDMQ 批量发送消息的接口是在 TDMQ-HTTP 的服务侧将消息打包为一个 Batch，然后将该 Batch 在服务内部当作一次 TCP 请求发送出去。所以在使用过程中，用户还是按照单条消息发送的逻辑，每一条消息是一个独立的 HTTP 的请求，在 TDMQ-HTTP 的服务内部，会将多个 HTTP 的请求聚合为一个 Batch 发送到服务端。即，批量发送消息在使用上与发送单条消息是一致的，batch 的聚合是在 TDMQ-HTTP 的服务内部完成的。
 
@@ -2248,15 +2248,15 @@
             model = models.SendBatchMessagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendCmqMsg(self, request):
         """发送cmq消息
 
         :param request: Request instance for SendCmqMsg.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.SendCmqMsgRequest`
@@ -2271,15 +2271,15 @@
             model = models.SendCmqMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendMessages(self, request):
         """发送单条消息
         不支持持久topic
 
         :param request: Request instance for SendMessages.
@@ -2295,15 +2295,15 @@
             model = models.SendMessagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendMsg(self, request):
         """此接口仅用于测试发生消息，不能作为现网正式生产使用
 
         :param request: Request instance for SendMsg.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.SendMsgRequest`
@@ -2318,15 +2318,15 @@
             model = models.SendMsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SendRocketMQMessage(self, request):
         """发送RocketMQ消息
 
         :param request: Request instance for SendRocketMQMessage.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.SendRocketMQMessageRequest`
@@ -2341,15 +2341,15 @@
             model = models.SendRocketMQMessageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindCmqDeadLetter(self, request):
         """解绑cmq死信队列
 
         :param request: Request instance for UnbindCmqDeadLetter.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.UnbindCmqDeadLetterRequest`
@@ -2364,8 +2364,8 @@
             model = models.UnbindCmqDeadLetterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/tdmq/v20200217/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.937/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.938/README.rst`

 * *Files identical despite different names*

