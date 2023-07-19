# Comparing `tmp/tencentcloud-sdk-python-gse-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-gse-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gse-3.0.937.tar", last modified: Tue Jul 18 00:24:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gse-3.0.938.tar", last modified: Wed Jul 19 00:40:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gse-3.0.937.tar` & `tencentcloud-sdk-python-gse-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89075 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/gse_client.py
--rw-r--r--   0 root         (0) root         (0)   387109 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:24:42.000000 tencentcloud-sdk-python-gse-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89371 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/gse_client.py
+-rw-r--r--   0 root         (0) root         (0)   387109 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:40:00.000000 tencentcloud-sdk-python-gse-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-gse-3.0.937/setup.py` & `tencentcloud-sdk-python-gse-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/errorcodes.py` & `tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/gse_client.py` & `tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/gse_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.AttachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyFleet(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CopyFleet）用于复制服务器舰队。
 
@@ -69,15 +69,15 @@
             model = models.CopyFleetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAlias(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateAlias）用于创建别名。
 
@@ -94,15 +94,15 @@
             model = models.CreateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAsset(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateAsset）用于创建生成包。
         通过获取上传cos的临时密钥，将文件上传至cos，然后将生成包的zip名称下发给本接口完成资源创建。
@@ -132,15 +132,15 @@
             model = models.CreateAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAssetWithImage(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateAssetWithImage）用于创建生成包镜像信息。
 
@@ -157,15 +157,15 @@
             model = models.CreateAssetWithImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFleet(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateFleet）用于创建服务器舰队。
 
@@ -182,15 +182,15 @@
             model = models.CreateFleetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGameServerSession(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateGameServerSession）用于创建游戏服务会话。
 
@@ -207,15 +207,15 @@
             model = models.CreateGameServerSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateGameServerSessionQueue(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（CreateGameServerSessionQueue）用于创建游戏服务器会话队列。
 
@@ -232,15 +232,15 @@
             model = models.CreateGameServerSessionQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAlias(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteAlias）用于删除别名。
 
@@ -257,15 +257,15 @@
             model = models.DeleteAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAsset(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteAsset）用于删除生成包。
 
@@ -282,15 +282,15 @@
             model = models.DeleteAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFleet(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteFleet）用于删除服务器舰队。
 
@@ -307,15 +307,15 @@
             model = models.DeleteFleetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteGameServerSessionQueue(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteGameServerSessionQueue）用于删除游戏服务器会话队列。
 
@@ -332,15 +332,15 @@
             model = models.DeleteGameServerSessionQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScalingPolicy(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteScalingPolicy）用于删除服务器舰队的扩缩容策略。
         通过服务器舰队ID和策略名称删除服务器舰队的扩缩容策略，只传递服务器舰队ID时，会将这个服务器舰队下的所有策略都删除。
@@ -359,15 +359,15 @@
             model = models.DeleteScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTimerScalingPolicy(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DeleteTimerScalingPolicy）用于删除fleet下的定时器。
 
@@ -384,15 +384,15 @@
             model = models.DeleteTimerScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAlias(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeAlias）用于获取别名详情。
 
@@ -409,15 +409,15 @@
             model = models.DescribeAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAsset(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeAsset）获取生成包信息。
 
@@ -434,15 +434,15 @@
             model = models.DescribeAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssetSystems(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeAssetSystems）用于获取生成包支持的操作系统。
 
@@ -459,15 +459,15 @@
             model = models.DescribeAssetSystemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAssets(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeAssets）用于获取生成包列表。
 
@@ -484,15 +484,15 @@
             model = models.DescribeAssetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcnInstances(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeCcnInstances）用于查询云联网实例。
 
@@ -509,15 +509,15 @@
             model = models.DescribeCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetAttributes(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetAttributes）用于查询服务器舰队属性。
 
@@ -534,15 +534,15 @@
             model = models.DescribeFleetAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetCapacity(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetCapacity）用于查询服务部署容量配置。
 
@@ -559,15 +559,15 @@
             model = models.DescribeFleetCapacityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetEvents(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetEvents）用于查询服务器舰队相关的事件列表。
 
@@ -584,15 +584,15 @@
             model = models.DescribeFleetEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetPortSettings(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetPortSettings）用于获取服务器舰队安全组信息。
 
@@ -609,15 +609,15 @@
             model = models.DescribeFleetPortSettingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetRelatedResources(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetRelatedResources）用于获取与游戏服务器舰队关联的资源信息，如别名、队列
 
@@ -634,15 +634,15 @@
             model = models.DescribeFleetRelatedResourcesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetStatisticDetails(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetStatisticDetails）用于查询服务部署统计详情。
 
@@ -659,15 +659,15 @@
             model = models.DescribeFleetStatisticDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetStatisticFlows(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetStatisticFlows）用于查询服务部署统计用量。
 
@@ -684,15 +684,15 @@
             model = models.DescribeFleetStatisticFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetStatisticSummary(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetStatisticSummary）用于查询服务部署统计汇总信息。
 
@@ -709,15 +709,15 @@
             model = models.DescribeFleetStatisticSummaryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFleetUtilization(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeFleetUtilization）用于查询服务器舰队的利用率信息。
 
@@ -734,15 +734,15 @@
             model = models.DescribeFleetUtilizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGameServerSessionDetails(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeGameServerSessionDetails）用于查询游戏服务器会话详情列表。
 
@@ -759,15 +759,15 @@
             model = models.DescribeGameServerSessionDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGameServerSessionPlacement(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeGameServerSessionPlacement）用于查询游戏服务器会话的放置。
 
@@ -784,15 +784,15 @@
             model = models.DescribeGameServerSessionPlacementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGameServerSessionQueues(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeGameServerSessionQueues）用于查询游戏服务器会话队列。
 
@@ -809,15 +809,15 @@
             model = models.DescribeGameServerSessionQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGameServerSessions(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeGameServerSessions）用于查询游戏服务器会话列表。
 
@@ -834,15 +834,15 @@
             model = models.DescribeGameServerSessionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLimit(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeInstanceLimit）用于查询用户实例数限额。
 
@@ -859,15 +859,15 @@
             model = models.DescribeInstanceLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceTypes(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeInstanceTypes）用于获取服务器实例类型列表。
 
@@ -884,15 +884,15 @@
             model = models.DescribeInstanceTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeInstances）用于查询服务器实例列表。
 
@@ -909,15 +909,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesExtend(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeInstancesExtend）用于查询实例扩展信息列表。
 
@@ -934,15 +934,15 @@
             model = models.DescribeInstancesExtendResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayerSessions(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribePlayerSessions）用于获取玩家会话列表。
 
@@ -959,15 +959,15 @@
             model = models.DescribePlayerSessionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuntimeConfiguration(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeRuntimeConfiguration）用于获取服务器舰队运行配置。
 
@@ -984,15 +984,15 @@
             model = models.DescribeRuntimeConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScalingPolicies(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeScalingPolicies）用于查询服务器舰队的动态扩缩容策略列表。
 
@@ -1009,15 +1009,15 @@
             model = models.DescribeScalingPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTimerScalingPolicies(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeTimerScalingPolicies）用于查询fleet下的定时器列表。可以通过fleetid，定时器名称分页查询。
 
@@ -1034,15 +1034,15 @@
             model = models.DescribeTimerScalingPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserQuota(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeUserQuota）获取用户单个模块配额。
 
@@ -1059,15 +1059,15 @@
             model = models.DescribeUserQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserQuotas(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DescribeUserQuotas）用于获取用户配额
 
@@ -1084,15 +1084,15 @@
             model = models.DescribeUserQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachCcnInstances(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（DetachCcnInstances）用于解关联云联网实例。
 
@@ -1109,15 +1109,15 @@
             model = models.DetachCcnInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EndGameServerSessionAndProcess(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（EndGameServerSessionAndProcess）用于终止游戏服务器会话和对应的进程，适用于时限保护和不保护。
 
@@ -1134,15 +1134,15 @@
             model = models.EndGameServerSessionAndProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetGameServerInstanceLogUrl(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口用于获取游戏服务器实例的日志URL。
 
@@ -1159,15 +1159,15 @@
             model = models.GetGameServerInstanceLogUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetGameServerSessionLogUrl(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（GetGameServerSessionLogUrl）用于获取游戏服务器会话的日志URL。
 
@@ -1184,15 +1184,15 @@
             model = models.GetGameServerSessionLogUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetInstanceAccess(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（GetInstanceAccess）用于获取实例登录所需要的凭据。
 
@@ -1209,15 +1209,15 @@
             model = models.GetInstanceAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetUploadCredentials(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（GetUploadCredentials）获取上传文件授权信息。
         通过 [GetUploadCredentials](https://cloud.tencent.com/document/product/1165/48727) 接口获取临时授权信息后，调用 COS API将数据上传，根据上传的 BucketKey 信息进行生成包 [CreateAsset](https://cloud.tencent.com/document/product/1165/48731) 的创建。参考下面的示例部分。
@@ -1235,15 +1235,15 @@
             model = models.GetUploadCredentialsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetUploadFederationToken(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（GetUploadFederationToken）用于 获取生成包上传所需要的临时密钥。
 
@@ -1260,15 +1260,15 @@
             model = models.GetUploadFederationTokenResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def JoinGameServerSession(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（JoinGameServerSession）用于加入游戏服务器会话。
 
@@ -1285,15 +1285,15 @@
             model = models.JoinGameServerSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def JoinGameServerSessionBatch(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（JoinGameServerSessionBatch）用于批量加入游戏服务器会话。
 
@@ -1310,15 +1310,15 @@
             model = models.JoinGameServerSessionBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListAliases(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（ListAliases）用于检索帐户下的所有别名。
 
@@ -1335,15 +1335,15 @@
             model = models.ListAliasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListFleets(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（ListFleets）用于获取服务器舰队列表。
 
@@ -1360,15 +1360,15 @@
             model = models.ListFleetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutScalingPolicy(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（PutScalingPolicy）用于设置服务器舰队的动态扩缩容策略。
 
@@ -1482,15 +1482,15 @@
             model = models.PutScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PutTimerScalingPolicy(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（PutTimerScalingPolicy）用于给fleet创建或更新定时器。
 
@@ -1509,15 +1509,15 @@
             model = models.PutTimerScalingPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResolveAlias(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（ResolveAlias）用于获取别名当前指向的fleetId。
 
@@ -1534,15 +1534,15 @@
             model = models.ResolveAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchGameServerSessions(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（SearchGameServerSessions）用于搜索游戏服务器会话列表。
 
@@ -1559,15 +1559,15 @@
             model = models.SearchGameServerSessionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetServerReserved(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（SetServerReserved）用于将异常的实例标记为保留，用于问题排查。
 
@@ -1586,15 +1586,15 @@
             model = models.SetServerReservedResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetServerWeight(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（SetServerWeight）用于设置服务器权重。
 
@@ -1611,15 +1611,15 @@
             model = models.SetServerWeightResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartFleetActions(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（StartFleetActions）用于启用服务器舰队自动扩缩容。
 
@@ -1636,15 +1636,15 @@
             model = models.StartFleetActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartGameServerSessionPlacement(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（StartGameServerSessionPlacement）用于开始放置游戏服务器会话。
 
@@ -1661,15 +1661,15 @@
             model = models.StartGameServerSessionPlacementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopFleetActions(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（StopFleetActions）用于停止服务器舰队自动扩缩容，改为手动扩缩容。
 
@@ -1686,15 +1686,15 @@
             model = models.StopFleetActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopGameServerSessionPlacement(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（StopGameServerSessionPlacement）用于停止放置游戏服务器会话。
 
@@ -1711,15 +1711,15 @@
             model = models.StopGameServerSessionPlacementResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAlias(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateAlias）用于更新别名的属性。
 
@@ -1736,15 +1736,15 @@
             model = models.UpdateAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAsset(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateAsset）用于修改生成包信息。
 
@@ -1761,15 +1761,15 @@
             model = models.UpdateAssetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateBucketAccelerateOpt(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateBucketAccelerateOpt）用于开启cos全球加速。
 
@@ -1786,15 +1786,15 @@
             model = models.UpdateBucketAccelerateOptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateBucketCORSOpt(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateBucketCORSOpt）用于设置cos跨域访问。
 
@@ -1811,15 +1811,15 @@
             model = models.UpdateBucketCORSOptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFleetAttributes(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateFleetAttributes）用于更新服务器舰队属性。
 
@@ -1836,15 +1836,15 @@
             model = models.UpdateFleetAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFleetCapacity(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateFleetCapacity）用于更新服务器舰队容量配置。
 
@@ -1861,15 +1861,15 @@
             model = models.UpdateFleetCapacityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFleetName(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateFleetName）用于更新服务器舰队名称。
 
@@ -1886,15 +1886,15 @@
             model = models.UpdateFleetNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateFleetPortSettings(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateFleetPortSettings）用于更新服务器舰队安全组。
 
@@ -1911,15 +1911,15 @@
             model = models.UpdateFleetPortSettingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGameServerSession(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateGameServerSession）用于更新游戏服务器会话。
 
@@ -1936,15 +1936,15 @@
             model = models.UpdateGameServerSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateGameServerSessionQueue(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateGameServerSessionQueue）用于修改游戏服务器会话队列。
 
@@ -1961,15 +1961,15 @@
             model = models.UpdateGameServerSessionQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRuntimeConfiguration(self, request):
         """此接口无法使用，游戏服务器引擎GSE已于6.1正式下架，感谢您的支持
 
         本接口（UpdateRuntimeConfiguration）用于更新服务器舰队配置。
 
@@ -1986,8 +1986,8 @@
             model = models.UpdateRuntimeConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-gse-3.0.937/tencentcloud/gse/v20191112/models.py` & `tencentcloud-sdk-python-gse-3.0.938/tencentcloud/gse/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gse-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gse-3.0.937/tencentcloud_sdk_python_gse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gse-3.0.938/tencentcloud_sdk_python_gse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gse-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-gse-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gse-3.0.937/README.rst` & `tencentcloud-sdk-python-gse-3.0.938/README.rst`

 * *Files identical despite different names*

