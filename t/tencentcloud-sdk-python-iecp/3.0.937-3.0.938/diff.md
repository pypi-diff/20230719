# Comparing `tmp/tencentcloud-sdk-python-iecp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-iecp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iecp-3.0.937.tar", last modified: Tue Jul 18 00:25:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iecp-3.0.938.tar", last modified: Wed Jul 19 00:40:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iecp-3.0.937.tar` & `tencentcloud-sdk-python-iecp-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93641 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/iecp_client.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   489786 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:25:25.000000 tencentcloud-sdk-python-iecp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94049 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/iecp_client.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   489786 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:40:46.000000 tencentcloud-sdk-python-iecp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/setup.py` & `tencentcloud-sdk-python-iecp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/iecp_client.py` & `tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/iecp_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ApplyMarketComponentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BuildMessageRoute(self, request):
         """建立消息路由
 
         :param request: Request instance for BuildMessageRoute.
         :type request: :class:`tencentcloud.iecp.v20210914.models.BuildMessageRouteRequest`
@@ -65,15 +65,15 @@
             model = models.BuildMessageRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApplicationVisualization(self, request):
         """创建可视化创建应用模板
 
         :param request: Request instance for CreateApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateApplicationVisualizationRequest`
@@ -88,15 +88,15 @@
             model = models.CreateApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConfigMap(self, request):
         """创建ConfigMap
 
         :param request: Request instance for CreateConfigMap.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateConfigMapRequest`
@@ -111,15 +111,15 @@
             model = models.CreateConfigMapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeNode(self, request):
         """创建边缘节点
 
         :param request: Request instance for CreateEdgeNode.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeNodeRequest`
@@ -134,15 +134,15 @@
             model = models.CreateEdgeNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeNodeBatch(self, request):
         """批量预注册节点
 
         :param request: Request instance for CreateEdgeNodeBatch.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeNodeBatchRequest`
@@ -157,15 +157,15 @@
             model = models.CreateEdgeNodeBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeNodeGroup(self, request):
         """创建边缘单元NodeGroup
 
         :param request: Request instance for CreateEdgeNodeGroup.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeNodeGroupRequest`
@@ -180,15 +180,15 @@
             model = models.CreateEdgeNodeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeNodeUnitTemplate(self, request):
         """创建边缘单元NodeUnit模板
 
         :param request: Request instance for CreateEdgeNodeUnitTemplate.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeNodeUnitTemplateRequest`
@@ -203,15 +203,15 @@
             model = models.CreateEdgeNodeUnitTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeUnitApplicationVisualization(self, request):
         """可视化创建应用
 
         :param request: Request instance for CreateEdgeUnitApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeUnitApplicationVisualizationRequest`
@@ -226,15 +226,15 @@
             model = models.CreateEdgeUnitApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeUnitApplicationYaml(self, request):
         """yaml方式创建应用
 
         :param request: Request instance for CreateEdgeUnitApplicationYaml.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeUnitApplicationYamlRequest`
@@ -249,15 +249,15 @@
             model = models.CreateEdgeUnitApplicationYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeUnitCloud(self, request):
         """创建边缘单元
 
         :param request: Request instance for CreateEdgeUnitCloud.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeUnitCloudRequest`
@@ -272,15 +272,15 @@
             model = models.CreateEdgeUnitCloudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeUnitDevices(self, request):
         """批量绑定设备到单元
 
         :param request: Request instance for CreateEdgeUnitDevices.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateEdgeUnitDevicesRequest`
@@ -295,15 +295,15 @@
             model = models.CreateEdgeUnitDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIotDevice(self, request):
         """创建子设备
 
         :param request: Request instance for CreateIotDevice.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateIotDeviceRequest`
@@ -318,15 +318,15 @@
             model = models.CreateIotDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMessageRoute(self, request):
         """创建消息路由
 
         :param request: Request instance for CreateMessageRoute.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateMessageRouteRequest`
@@ -341,15 +341,15 @@
             model = models.CreateMessageRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateNamespace(self, request):
         """创建命名空间
 
         :param request: Request instance for CreateNamespace.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateNamespaceRequest`
@@ -364,15 +364,15 @@
             model = models.CreateNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSecret(self, request):
         """创建Secret
 
         :param request: Request instance for CreateSecret.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateSecretRequest`
@@ -387,15 +387,15 @@
             model = models.CreateSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUpdateNodeUnit(self, request):
         """创建或更新边缘单元NodeUnit
 
         :param request: Request instance for CreateUpdateNodeUnit.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateUpdateNodeUnitRequest`
@@ -410,15 +410,15 @@
             model = models.CreateUpdateNodeUnitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateUserToken(self, request):
         """创建token
 
         :param request: Request instance for CreateUserToken.
         :type request: :class:`tencentcloud.iecp.v20210914.models.CreateUserTokenRequest`
@@ -433,15 +433,15 @@
             model = models.CreateUserTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteApplications(self, request):
         """删除应用模板
 
         :param request: Request instance for DeleteApplications.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteApplicationsRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteConfigMap(self, request):
         """删除ConfigMap
 
         :param request: Request instance for DeleteConfigMap.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteConfigMapRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteConfigMapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeNodeGroup(self, request):
         """删除边缘单元NodeGroup
 
         :param request: Request instance for DeleteEdgeNodeGroup.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeNodeGroupRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteEdgeNodeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeNodeUnitTemplates(self, request):
         """删除边缘单元NodeUnit模板
 
         :param request: Request instance for DeleteEdgeNodeUnitTemplates.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeNodeUnitTemplatesRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteEdgeNodeUnitTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeNodes(self, request):
         """批量删除边缘节点
 
         :param request: Request instance for DeleteEdgeNodes.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeNodesRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteEdgeNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeUnitApplications(self, request):
         """删除应用列表
 
         :param request: Request instance for DeleteEdgeUnitApplications.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeUnitApplicationsRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteEdgeUnitApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeUnitCloud(self, request):
         """删除边缘单元
 
         :param request: Request instance for DeleteEdgeUnitCloud.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeUnitCloudRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteEdgeUnitCloudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeUnitDeployGridItem(self, request):
         """重新部署边缘单元指定Grid下应用
 
         :param request: Request instance for DeleteEdgeUnitDeployGridItem.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeUnitDeployGridItemRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteEdgeUnitDeployGridItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeUnitDevices(self, request):
         """批量解绑单元设备
 
         :param request: Request instance for DeleteEdgeUnitDevices.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeUnitDevicesRequest`
@@ -640,15 +640,15 @@
             model = models.DeleteEdgeUnitDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeUnitPod(self, request):
         """删除指定pod
 
         :param request: Request instance for DeleteEdgeUnitPod.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteEdgeUnitPodRequest`
@@ -663,15 +663,15 @@
             model = models.DeleteEdgeUnitPodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIotDevice(self, request):
         """删除设备
 
         :param request: Request instance for DeleteIotDevice.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteIotDeviceRequest`
@@ -686,15 +686,15 @@
             model = models.DeleteIotDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIotDeviceBatch(self, request):
         """批量删除设备
 
         :param request: Request instance for DeleteIotDeviceBatch.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteIotDeviceBatchRequest`
@@ -709,15 +709,15 @@
             model = models.DeleteIotDeviceBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMessageRoute(self, request):
         """删除消息路由
 
         :param request: Request instance for DeleteMessageRoute.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteMessageRouteRequest`
@@ -732,15 +732,15 @@
             model = models.DeleteMessageRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNamespace(self, request):
         """删除命名空间
 
         :param request: Request instance for DeleteNamespace.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteNamespaceRequest`
@@ -755,15 +755,15 @@
             model = models.DeleteNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNodeUnit(self, request):
         """删除边缘单元NodeUnit
 
         :param request: Request instance for DeleteNodeUnit.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteNodeUnitRequest`
@@ -778,15 +778,15 @@
             model = models.DeleteNodeUnitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSecret(self, request):
         """删除Secret
 
         :param request: Request instance for DeleteSecret.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DeleteSecretRequest`
@@ -801,15 +801,15 @@
             model = models.DeleteSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationVisualization(self, request):
         """获取应用模板可视化配置信息
 
         :param request: Request instance for DescribeApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeApplicationVisualizationRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationYaml(self, request):
         """查询应用模板Yaml
 
         :param request: Request instance for DescribeApplicationYaml.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeApplicationYamlRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeApplicationYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplicationYamlError(self, request):
         """检查应用模板的Yaml配置
 
         :param request: Request instance for DescribeApplicationYamlError.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeApplicationYamlErrorRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeApplicationYamlErrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplications(self, request):
         """获取应用模板列表
 
         :param request: Request instance for DescribeApplications.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeApplicationsRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigMap(self, request):
         """获取ConfigMap详情
 
         :param request: Request instance for DescribeConfigMap.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeConfigMapRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeConfigMapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigMapYamlError(self, request):
         """校验ConfigMap的Yaml语法
 
         :param request: Request instance for DescribeConfigMapYamlError.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeConfigMapYamlErrorRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeConfigMapYamlErrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConfigMaps(self, request):
         """获取ConfigMap列表
 
         :param request: Request instance for DescribeConfigMaps.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeConfigMapsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeConfigMapsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDracoEdgeNodeInstaller(self, request):
         """自动获取Draco设备的安装包
 
         :param request: Request instance for DescribeDracoEdgeNodeInstaller.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeDracoEdgeNodeInstallerRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDracoEdgeNodeInstallerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeAgentNodeInstaller(self, request):
         """获取节点安装信息
 
         :param request: Request instance for DescribeEdgeAgentNodeInstaller.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeAgentNodeInstallerRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeEdgeAgentNodeInstallerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeDefaultVpc(self, request):
         """获取边缘集群默认VPC信息
 
         :param request: Request instance for DescribeEdgeDefaultVpc.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeDefaultVpcRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeEdgeDefaultVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeNode(self, request):
         """获取边缘节点信息
 
         :param request: Request instance for DescribeEdgeNode.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeNodeRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeEdgeNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeNodePodContainers(self, request):
         """查询节点Pod内的容器列表
 
         :param request: Request instance for DescribeEdgeNodePodContainers.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeNodePodContainersRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeEdgeNodePodContainersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeNodePods(self, request):
         """查询节点Pod列表
 
         :param request: Request instance for DescribeEdgeNodePods.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeNodePodsRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeEdgeNodePodsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeNodeRemarkList(self, request):
         """获取节点备注信息列表
 
         :param request: Request instance for DescribeEdgeNodeRemarkList.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeNodeRemarkListRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeEdgeNodeRemarkListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeNodes(self, request):
         """查询边缘节点列表
 
         :param request: Request instance for DescribeEdgeNodes.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeNodesRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeEdgeNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeOperationLogs(self, request):
         """查询边缘操作日志
 
         :param request: Request instance for DescribeEdgeOperationLogs.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeOperationLogsRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeEdgeOperationLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgePod(self, request):
         """查询边缘单元Pod
 
         :param request: Request instance for DescribeEdgePod.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgePodRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeEdgePodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeSnNodes(self, request):
         """查询预注册节点列表
 
         :param request: Request instance for DescribeEdgeSnNodes.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeSnNodesRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeEdgeSnNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationEvents(self, request):
         """获取应用事件列表
 
         :param request: Request instance for DescribeEdgeUnitApplicationEvents.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationEventsRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeEdgeUnitApplicationEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationLogs(self, request):
         """获取应用日志
 
         :param request: Request instance for DescribeEdgeUnitApplicationLogs.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationLogsRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeEdgeUnitApplicationLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationPodContainers(self, request):
         """获取应用容器状态
 
         :param request: Request instance for DescribeEdgeUnitApplicationPodContainers.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationPodContainersRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeEdgeUnitApplicationPodContainersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationPods(self, request):
         """获取应用下Pod状态
 
         :param request: Request instance for DescribeEdgeUnitApplicationPods.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationPodsRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeEdgeUnitApplicationPodsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationVisualization(self, request):
         """获取单元可视化配置信息
 
         :param request: Request instance for DescribeEdgeUnitApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationVisualizationRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeEdgeUnitApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationYaml(self, request):
         """获取应用的Yaml配置
 
         :param request: Request instance for DescribeEdgeUnitApplicationYaml.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationYamlRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeEdgeUnitApplicationYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplicationYamlError(self, request):
         """检查单元应用的Yaml配置
 
         :param request: Request instance for DescribeEdgeUnitApplicationYamlError.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationYamlErrorRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeEdgeUnitApplicationYamlErrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitApplications(self, request):
         """获取单元下应用列表
 
         :param request: Request instance for DescribeEdgeUnitApplications.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitApplicationsRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeEdgeUnitApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitCloud(self, request):
         """查询边缘集群详情
 
         :param request: Request instance for DescribeEdgeUnitCloud.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitCloudRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeEdgeUnitCloudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitDeployGrid(self, request):
         """查询边缘单元Grid列表
 
         :param request: Request instance for DescribeEdgeUnitDeployGrid.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitDeployGridRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeEdgeUnitDeployGridResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitDeployGridItem(self, request):
         """查询边缘单元指定Grid下的部署应用列表
 
         :param request: Request instance for DescribeEdgeUnitDeployGridItem.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitDeployGridItemRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeEdgeUnitDeployGridItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitDeployGridItemYaml(self, request):
         """查询指定Grid下应用的Yaml
 
         :param request: Request instance for DescribeEdgeUnitDeployGridItemYaml.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitDeployGridItemYamlRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeEdgeUnitDeployGridItemYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitExtra(self, request):
         """查询边缘单元额外信息
 
         :param request: Request instance for DescribeEdgeUnitExtra.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitExtraRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeEdgeUnitExtraResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitGridEvents(self, request):
         """查询边缘单元Grid事件列表
 
         :param request: Request instance for DescribeEdgeUnitGridEvents.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitGridEventsRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeEdgeUnitGridEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitGridPods(self, request):
         """查询边缘单元Grid的Pod列表
 
         :param request: Request instance for DescribeEdgeUnitGridPods.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitGridPodsRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeEdgeUnitGridPodsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitMonitorStatus(self, request):
         """查询边缘集群监控状态
 
         :param request: Request instance for DescribeEdgeUnitMonitorStatus.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitMonitorStatusRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeEdgeUnitMonitorStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitNodeGroup(self, request):
         """查询边缘集群NodeGroup
 
         :param request: Request instance for DescribeEdgeUnitNodeGroup.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitNodeGroupRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeEdgeUnitNodeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitNodeUnitTemplates(self, request):
         """查询边缘单元EdgeUnit模板列表
 
         :param request: Request instance for DescribeEdgeUnitNodeUnitTemplates.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitNodeUnitTemplatesRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribeEdgeUnitNodeUnitTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeUnitsCloud(self, request):
         """查询边缘单元列表
 
         :param request: Request instance for DescribeEdgeUnitsCloud.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeEdgeUnitsCloudRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeEdgeUnitsCloudResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIotDevice(self, request):
         """获取设备信息
 
         :param request: Request instance for DescribeIotDevice.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeIotDeviceRequest`
@@ -1675,15 +1675,15 @@
             model = models.DescribeIotDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIotDevices(self, request):
         """获取设备列表信息
 
         :param request: Request instance for DescribeIotDevices.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeIotDevicesRequest`
@@ -1698,15 +1698,15 @@
             model = models.DescribeIotDevicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMessageRouteList(self, request):
         """获取消息路由列表
 
         :param request: Request instance for DescribeMessageRouteList.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeMessageRouteListRequest`
@@ -1721,15 +1721,15 @@
             model = models.DescribeMessageRouteListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMonitorMetrics(self, request):
         """查询边缘单元监控数据
 
         :param request: Request instance for DescribeMonitorMetrics.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeMonitorMetricsRequest`
@@ -1744,15 +1744,15 @@
             model = models.DescribeMonitorMetricsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespace(self, request):
         """获取命名空间
 
         :param request: Request instance for DescribeNamespace.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeNamespaceRequest`
@@ -1767,15 +1767,15 @@
             model = models.DescribeNamespaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespaceResources(self, request):
         """获取命名空间下的资源信息
 
         :param request: Request instance for DescribeNamespaceResources.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeNamespaceResourcesRequest`
@@ -1790,15 +1790,15 @@
             model = models.DescribeNamespaceResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNamespaces(self, request):
         """获取命名空间列表信息
 
         :param request: Request instance for DescribeNamespaces.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeNamespacesRequest`
@@ -1813,15 +1813,15 @@
             model = models.DescribeNamespacesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNodeUnit(self, request):
         """查询边缘单元NodeUnit列表
 
         :param request: Request instance for DescribeNodeUnit.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeNodeUnitRequest`
@@ -1836,15 +1836,15 @@
             model = models.DescribeNodeUnitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNodeUnitTemplateOnNodeGroup(self, request):
         """查询指定NodeGroup下NodeUnit模板列表
 
         :param request: Request instance for DescribeNodeUnitTemplateOnNodeGroup.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeNodeUnitTemplateOnNodeGroupRequest`
@@ -1859,15 +1859,15 @@
             model = models.DescribeNodeUnitTemplateOnNodeGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecret(self, request):
         """获取Secret详情
 
         :param request: Request instance for DescribeSecret.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeSecretRequest`
@@ -1882,15 +1882,15 @@
             model = models.DescribeSecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecretYamlError(self, request):
         """校验Secret的Yaml语法
 
         :param request: Request instance for DescribeSecretYamlError.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeSecretYamlErrorRequest`
@@ -1905,15 +1905,15 @@
             model = models.DescribeSecretYamlErrorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecrets(self, request):
         """获取Secrets列表
 
         :param request: Request instance for DescribeSecrets.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeSecretsRequest`
@@ -1928,15 +1928,15 @@
             model = models.DescribeSecretsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeYeheResourceLimit(self, request):
         """查询用户的资源限制
 
         :param request: Request instance for DescribeYeheResourceLimit.
         :type request: :class:`tencentcloud.iecp.v20210914.models.DescribeYeheResourceLimitRequest`
@@ -1951,15 +1951,15 @@
             model = models.DescribeYeheResourceLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetMarketComponent(self, request):
         """获取组件市场的组件信息
 
         :param request: Request instance for GetMarketComponent.
         :type request: :class:`tencentcloud.iecp.v20210914.models.GetMarketComponentRequest`
@@ -1974,15 +1974,15 @@
             model = models.GetMarketComponentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetMarketComponentList(self, request):
         """获取组件市场组件列表
 
         :param request: Request instance for GetMarketComponentList.
         :type request: :class:`tencentcloud.iecp.v20210914.models.GetMarketComponentListRequest`
@@ -1997,15 +1997,15 @@
             model = models.GetMarketComponentListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationBasicInfo(self, request):
         """修改应用模板基本信息
 
         :param request: Request instance for ModifyApplicationBasicInfo.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyApplicationBasicInfoRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyApplicationBasicInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApplicationVisualization(self, request):
         """修改应用模板配置
 
         :param request: Request instance for ModifyApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyApplicationVisualizationRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConfigMap(self, request):
         """修改ConfigMap
 
         :param request: Request instance for ModifyConfigMap.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyConfigMapRequest`
@@ -2066,15 +2066,15 @@
             model = models.ModifyConfigMapResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeDracoNode(self, request):
         """编辑draco设备信息
 
         :param request: Request instance for ModifyEdgeDracoNode.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeDracoNodeRequest`
@@ -2089,15 +2089,15 @@
             model = models.ModifyEdgeDracoNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeNodeLabels(self, request):
         """编辑边缘节点标签
 
         :param request: Request instance for ModifyEdgeNodeLabels.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeNodeLabelsRequest`
@@ -2112,15 +2112,15 @@
             model = models.ModifyEdgeNodeLabelsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnit(self, request):
         """修改边缘集群
 
         :param request: Request instance for ModifyEdgeUnit.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitRequest`
@@ -2135,15 +2135,15 @@
             model = models.ModifyEdgeUnitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnitApplicationBasicInfo(self, request):
         """修改单元应用基本信息
 
         :param request: Request instance for ModifyEdgeUnitApplicationBasicInfo.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitApplicationBasicInfoRequest`
@@ -2158,15 +2158,15 @@
             model = models.ModifyEdgeUnitApplicationBasicInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnitApplicationVisualization(self, request):
         """可视化修改应用配置
 
         :param request: Request instance for ModifyEdgeUnitApplicationVisualization.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitApplicationVisualizationRequest`
@@ -2181,15 +2181,15 @@
             model = models.ModifyEdgeUnitApplicationVisualizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnitApplicationYaml(self, request):
         """Yaml方式修改应用配置
 
         :param request: Request instance for ModifyEdgeUnitApplicationYaml.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitApplicationYamlRequest`
@@ -2204,15 +2204,15 @@
             model = models.ModifyEdgeUnitApplicationYamlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnitCloudApi(self, request):
         """更新边缘单元信息
 
         :param request: Request instance for ModifyEdgeUnitCloudApi.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitCloudApiRequest`
@@ -2227,15 +2227,15 @@
             model = models.ModifyEdgeUnitCloudApiResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEdgeUnitDeployGridItem(self, request):
         """修改边缘单元Grid部署应用副本数
 
         :param request: Request instance for ModifyEdgeUnitDeployGridItem.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyEdgeUnitDeployGridItemRequest`
@@ -2250,15 +2250,15 @@
             model = models.ModifyEdgeUnitDeployGridItemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIotDevice(self, request):
         """修改设备信息
 
         :param request: Request instance for ModifyIotDevice.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyIotDeviceRequest`
@@ -2273,15 +2273,15 @@
             model = models.ModifyIotDeviceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNodeUnitTemplate(self, request):
         """修改边缘单元NodeUnit模板
 
         :param request: Request instance for ModifyNodeUnitTemplate.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifyNodeUnitTemplateRequest`
@@ -2296,15 +2296,15 @@
             model = models.ModifyNodeUnitTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySecret(self, request):
         """修改Secret
 
         :param request: Request instance for ModifySecret.
         :type request: :class:`tencentcloud.iecp.v20210914.models.ModifySecretRequest`
@@ -2319,15 +2319,15 @@
             model = models.ModifySecretResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RedeployEdgeUnitApplication(self, request):
         """单元应用重部署
 
         :param request: Request instance for RedeployEdgeUnitApplication.
         :type request: :class:`tencentcloud.iecp.v20210914.models.RedeployEdgeUnitApplicationRequest`
@@ -2342,15 +2342,15 @@
             model = models.RedeployEdgeUnitApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetRouteOnOff(self, request):
         """开关消息路由
 
         :param request: Request instance for SetRouteOnOff.
         :type request: :class:`tencentcloud.iecp.v20210914.models.SetRouteOnOffRequest`
@@ -2365,8 +2365,8 @@
             model = models.SetRouteOnOffResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/errorcodes.py` & `tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/iecp/v20210914/models.py` & `tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/iecp/v20210914/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iecp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-iecp-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iecp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iecp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/tencentcloud_sdk_python_iecp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iecp-3.0.938/tencentcloud_sdk_python_iecp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iecp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Iecp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iecp-3.0.937/README.rst` & `tencentcloud-sdk-python-iecp-3.0.938/README.rst`

 * *Files identical despite different names*

