# Comparing `tmp/tencentcloud-sdk-python-eb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-eb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eb-3.0.937.tar", last modified: Tue Jul 18 00:23:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eb-3.0.938.tar", last modified: Wed Jul 19 00:38:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eb-3.0.937.tar` & `tencentcloud-sdk-python-eb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/
--rw-r--r--   0 root         (0) root         (0)    24672 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/eb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14675 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   140384 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:09.000000 tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/
+-rw-r--r--   0 root         (0) root         (0)    24784 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/eb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14675 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   140384 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:22.000000 tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-eb-3.0.937/setup.py` & `tencentcloud-sdk-python-eb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/eb_client.py` & `tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/eb_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CheckRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckTransformation(self, request):
         """用于在ETL配置页面, 测试规则和数据.
 
         :param request: Request instance for CheckTransformation.
         :type request: :class:`tencentcloud.eb.v20210416.models.CheckTransformationRequest`
@@ -65,15 +65,15 @@
             model = models.CheckTransformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConnection(self, request):
         """创建事件连接器
 
         :param request: Request instance for CreateConnection.
         :type request: :class:`tencentcloud.eb.v20210416.models.CreateConnectionRequest`
@@ -88,15 +88,15 @@
             model = models.CreateConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEventBus(self, request):
         """用于创建事件集
 
         :param request: Request instance for CreateEventBus.
         :type request: :class:`tencentcloud.eb.v20210416.models.CreateEventBusRequest`
@@ -111,15 +111,15 @@
             model = models.CreateEventBusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRule(self, request):
         """创建事件规则
 
         :param request: Request instance for CreateRule.
         :type request: :class:`tencentcloud.eb.v20210416.models.CreateRuleRequest`
@@ -134,15 +134,15 @@
             model = models.CreateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTarget(self, request):
         """创建事件目标
 
         :param request: Request instance for CreateTarget.
         :type request: :class:`tencentcloud.eb.v20210416.models.CreateTargetRequest`
@@ -157,15 +157,15 @@
             model = models.CreateTargetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTransformation(self, request):
         """用于创建转换器
 
         :param request: Request instance for CreateTransformation.
         :type request: :class:`tencentcloud.eb.v20210416.models.CreateTransformationRequest`
@@ -180,15 +180,15 @@
             model = models.CreateTransformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConnection(self, request):
         """删除事件连接器
 
         :param request: Request instance for DeleteConnection.
         :type request: :class:`tencentcloud.eb.v20210416.models.DeleteConnectionRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEventBus(self, request):
         """删除事件集
 
         :param request: Request instance for DeleteEventBus.
         :type request: :class:`tencentcloud.eb.v20210416.models.DeleteEventBusRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteEventBusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRule(self, request):
         """删除事件规则
 
         :param request: Request instance for DeleteRule.
         :type request: :class:`tencentcloud.eb.v20210416.models.DeleteRuleRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTarget(self, request):
         """删除事件目标
 
         :param request: Request instance for DeleteTarget.
         :type request: :class:`tencentcloud.eb.v20210416.models.DeleteTargetRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteTargetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTransformation(self, request):
         """用于删除转换器
 
         :param request: Request instance for DeleteTransformation.
         :type request: :class:`tencentcloud.eb.v20210416.models.DeleteTransformationRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteTransformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogTagValue(self, request):
         """查询日志索引维度值
 
         :param request: Request instance for DescribeLogTagValue.
         :type request: :class:`tencentcloud.eb.v20210416.models.DescribeLogTagValueRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeLogTagValueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEventBus(self, request):
         """获取事件集详情
 
         :param request: Request instance for GetEventBus.
         :type request: :class:`tencentcloud.eb.v20210416.models.GetEventBusRequest`
@@ -341,15 +341,15 @@
             model = models.GetEventBusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRule(self, request):
         """获取事件规则详情
 
         :param request: Request instance for GetRule.
         :type request: :class:`tencentcloud.eb.v20210416.models.GetRuleRequest`
@@ -364,15 +364,15 @@
             model = models.GetRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTransformation(self, request):
         """用于获取转换器详情
 
         :param request: Request instance for GetTransformation.
         :type request: :class:`tencentcloud.eb.v20210416.models.GetTransformationRequest`
@@ -387,15 +387,15 @@
             model = models.GetTransformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListConnections(self, request):
         """获取事件连接器列表
 
         :param request: Request instance for ListConnections.
         :type request: :class:`tencentcloud.eb.v20210416.models.ListConnectionsRequest`
@@ -410,15 +410,15 @@
             model = models.ListConnectionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEventBuses(self, request):
         """获取事件集列表
 
         :param request: Request instance for ListEventBuses.
         :type request: :class:`tencentcloud.eb.v20210416.models.ListEventBusesRequest`
@@ -433,15 +433,15 @@
             model = models.ListEventBusesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListRules(self, request):
         """获取事件规则列表
 
         :param request: Request instance for ListRules.
         :type request: :class:`tencentcloud.eb.v20210416.models.ListRulesRequest`
@@ -456,15 +456,15 @@
             model = models.ListRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListTargets(self, request):
         """获取事件目标列表
 
         :param request: Request instance for ListTargets.
         :type request: :class:`tencentcloud.eb.v20210416.models.ListTargetsRequest`
@@ -479,15 +479,15 @@
             model = models.ListTargetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PublishEvent(self, request):
         """（已废弃）用于Event事件投递
 
         :param request: Request instance for PublishEvent.
         :type request: :class:`tencentcloud.eb.v20210416.models.PublishEventRequest`
@@ -502,15 +502,15 @@
             model = models.PublishEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutEvents(self, request):
         """用于Event事件投递
 
         :param request: Request instance for PutEvents.
         :type request: :class:`tencentcloud.eb.v20210416.models.PutEventsRequest`
@@ -525,15 +525,15 @@
             model = models.PutEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchLog(self, request):
         """日志检索
 
         :param request: Request instance for SearchLog.
         :type request: :class:`tencentcloud.eb.v20210416.models.SearchLogRequest`
@@ -548,15 +548,15 @@
             model = models.SearchLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateConnection(self, request):
         """更新事件连接器
 
         :param request: Request instance for UpdateConnection.
         :type request: :class:`tencentcloud.eb.v20210416.models.UpdateConnectionRequest`
@@ -571,15 +571,15 @@
             model = models.UpdateConnectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEventBus(self, request):
         """更新事件集
 
         :param request: Request instance for UpdateEventBus.
         :type request: :class:`tencentcloud.eb.v20210416.models.UpdateEventBusRequest`
@@ -594,15 +594,15 @@
             model = models.UpdateEventBusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRule(self, request):
         """更新事件规则
 
         :param request: Request instance for UpdateRule.
         :type request: :class:`tencentcloud.eb.v20210416.models.UpdateRuleRequest`
@@ -617,15 +617,15 @@
             model = models.UpdateRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTarget(self, request):
         """更新事件目标
 
         :param request: Request instance for UpdateTarget.
         :type request: :class:`tencentcloud.eb.v20210416.models.UpdateTargetRequest`
@@ -640,15 +640,15 @@
             model = models.UpdateTargetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTransformation(self, request):
         """用于更新转换器
 
         :param request: Request instance for UpdateTransformation.
         :type request: :class:`tencentcloud.eb.v20210416.models.UpdateTransformationRequest`
@@ -663,8 +663,8 @@
             model = models.UpdateTransformationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/errorcodes.py` & `tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eb-3.0.937/tencentcloud/eb/v20210416/models.py` & `tencentcloud-sdk-python-eb-3.0.938/tencentcloud/eb/v20210416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-eb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eb-3.0.937/README.rst` & `tencentcloud-sdk-python-eb-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eb-3.0.937/tencentcloud_sdk_python_eb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eb-3.0.938/tencentcloud_sdk_python_eb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

