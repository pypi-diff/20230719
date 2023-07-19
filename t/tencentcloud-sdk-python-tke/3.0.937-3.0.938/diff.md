# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.937.tar", last modified: Tue Jul 18 00:33:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.938.tar", last modified: Wed Jul 19 00:51:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.937.tar` & `tencentcloud-sdk-python-tke-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190375 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19591 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1059069 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:28.000000 tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191187 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1059069 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:51:06.000000 tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.937/setup.py` & `tencentcloud-sdk-python-tke-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AcquireClusterAdminRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddClusterCIDR(self, request):
         """给GR集群增加可用的ClusterCIDR
 
         :param request: Request instance for AddClusterCIDR.
         :type request: :class:`tencentcloud.tke.v20180525.models.AddClusterCIDRRequest`
@@ -65,15 +65,15 @@
             model = models.AddClusterCIDRResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddExistedInstances(self, request):
         """添加已经存在的实例到集群
 
         :param request: Request instance for AddExistedInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.AddExistedInstancesRequest`
@@ -88,15 +88,15 @@
             model = models.AddExistedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddNodeToNodePool(self, request):
         """将集群内节点移入节点池
 
         :param request: Request instance for AddNodeToNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.AddNodeToNodePoolRequest`
@@ -111,15 +111,15 @@
             model = models.AddNodeToNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddVpcCniSubnets(self, request):
         """针对VPC-CNI模式的集群，增加集群容器网络可使用的子网
 
         :param request: Request instance for AddVpcCniSubnets.
         :type request: :class:`tencentcloud.tke.v20180525.models.AddVpcCniSubnetsRequest`
@@ -134,15 +134,15 @@
             model = models.AddVpcCniSubnetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelClusterRelease(self, request):
         """在应用市场中取消安装失败的应用
 
         :param request: Request instance for CancelClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.CancelClusterReleaseRequest`
@@ -157,15 +157,15 @@
             model = models.CancelClusterReleaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckEdgeClusterCIDR(self, request):
         """检查边缘计算集群的CIDR是否冲突
 
         :param request: Request instance for CheckEdgeClusterCIDR.
         :type request: :class:`tencentcloud.tke.v20180525.models.CheckEdgeClusterCIDRRequest`
@@ -180,15 +180,15 @@
             model = models.CheckEdgeClusterCIDRResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckInstancesUpgradeAble(self, request):
         """检查给定节点列表中哪些是可升级的
 
         :param request: Request instance for CheckInstancesUpgradeAble.
         :type request: :class:`tencentcloud.tke.v20180525.models.CheckInstancesUpgradeAbleRequest`
@@ -203,15 +203,15 @@
             model = models.CheckInstancesUpgradeAbleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackupStorageLocation(self, request):
         """创建备份仓库，指定了存储仓库类型（如COS）、COS桶地区、名称等信息，当前最多允许创建100个仓库， 注意此接口当前是全局接口，多个地域的TKE集群如果要备份到相同的备份仓库中，不需要重复创建备份仓库
 
         :param request: Request instance for CreateBackupStorageLocation.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateBackupStorageLocationRequest`
@@ -226,15 +226,15 @@
             model = models.CreateBackupStorageLocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """创建集群
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterRequest`
@@ -249,15 +249,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterEndpoint(self, request):
         """创建集群访问端口
 
         :param request: Request instance for CreateClusterEndpoint.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterEndpointRequest`
@@ -272,15 +272,15 @@
             model = models.CreateClusterEndpointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterEndpointVip(self, request):
         """创建托管集群外网访问端口（不再维护，准备下线）请使用新接口：CreateClusterEndpoint
 
         :param request: Request instance for CreateClusterEndpointVip.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterEndpointVipRequest`
@@ -295,15 +295,15 @@
             model = models.CreateClusterEndpointVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterInstances(self, request):
         """扩展(新建)集群节点
 
         :param request: Request instance for CreateClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterInstancesRequest`
@@ -318,15 +318,15 @@
             model = models.CreateClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterNodePool(self, request):
         """创建节点池
 
         :param request: Request instance for CreateClusterNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterNodePoolRequest`
@@ -341,15 +341,15 @@
             model = models.CreateClusterNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterRelease(self, request):
         """集群创建应用
 
         :param request: Request instance for CreateClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterReleaseRequest`
@@ -364,15 +364,15 @@
             model = models.CreateClusterReleaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterRoute(self, request):
         """创建集群路由
 
         :param request: Request instance for CreateClusterRoute.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterRouteRequest`
@@ -387,15 +387,15 @@
             model = models.CreateClusterRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterRouteTable(self, request):
         """创建集群路由表
 
         :param request: Request instance for CreateClusterRouteTable.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterRouteTableRequest`
@@ -410,15 +410,15 @@
             model = models.CreateClusterRouteTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterVirtualNode(self, request):
         """创建虚拟节点
 
         :param request: Request instance for CreateClusterVirtualNode.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterVirtualNodeRequest`
@@ -433,15 +433,15 @@
             model = models.CreateClusterVirtualNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterVirtualNodePool(self, request):
         """创建虚拟节点池
 
         :param request: Request instance for CreateClusterVirtualNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterVirtualNodePoolRequest`
@@ -456,15 +456,15 @@
             model = models.CreateClusterVirtualNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateECMInstances(self, request):
         """创建边缘计算ECM机器
 
         :param request: Request instance for CreateECMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateECMInstancesRequest`
@@ -479,15 +479,15 @@
             model = models.CreateECMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEKSCluster(self, request):
         """创建弹性集群
 
         :param request: Request instance for CreateEKSCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateEKSClusterRequest`
@@ -502,15 +502,15 @@
             model = models.CreateEKSClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEKSContainerInstances(self, request):
         """创建容器实例
 
         :param request: Request instance for CreateEKSContainerInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateEKSContainerInstancesRequest`
@@ -525,15 +525,15 @@
             model = models.CreateEKSContainerInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeCVMInstances(self, request):
         """创建边缘容器CVM机器
 
         :param request: Request instance for CreateEdgeCVMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateEdgeCVMInstancesRequest`
@@ -548,15 +548,15 @@
             model = models.CreateEdgeCVMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEdgeLogConfig(self, request):
         """创建边缘集群日志采集配置
 
         :param request: Request instance for CreateEdgeLogConfig.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateEdgeLogConfigRequest`
@@ -571,15 +571,15 @@
             model = models.CreateEdgeLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImageCache(self, request):
         """创建镜像缓存的接口。创建过程中，请勿删除EKSCI实例和云盘，否则镜像缓存将创建失败。
 
         :param request: Request instance for CreateImageCache.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateImageCacheRequest`
@@ -594,15 +594,15 @@
             model = models.CreateImageCacheResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusAlertPolicyRequest`
@@ -617,15 +617,15 @@
             model = models.CreatePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusAlertRule(self, request):
         """创建告警规则
 
         :param request: Request instance for CreatePrometheusAlertRule.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusAlertRuleRequest`
@@ -640,15 +640,15 @@
             model = models.CreatePrometheusAlertRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusClusterAgent(self, request):
         """与云监控融合的2.0实例关联集群
 
         :param request: Request instance for CreatePrometheusClusterAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusClusterAgentRequest`
@@ -663,15 +663,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusConfigRequest`
@@ -686,15 +686,15 @@
             model = models.CreatePrometheusConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusDashboard(self, request):
         """创建grafana监控面板
 
         :param request: Request instance for CreatePrometheusDashboard.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusDashboardRequest`
@@ -709,15 +709,15 @@
             model = models.CreatePrometheusDashboardResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusGlobalNotificationRequest`
@@ -732,15 +732,15 @@
             model = models.CreatePrometheusGlobalNotificationResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusRecordRuleYamlRequest`
@@ -755,15 +755,15 @@
             model = models.CreatePrometheusRecordRuleYamlResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusTempRequest`
@@ -778,15 +778,15 @@
             model = models.CreatePrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrometheusTemplate(self, request):
         """创建一个云原生Prometheus模板实例
 
         :param request: Request instance for CreatePrometheusTemplate.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreatePrometheusTemplateRequest`
@@ -801,15 +801,15 @@
             model = models.CreatePrometheusTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTKEEdgeCluster(self, request):
         """创建边缘计算集群
 
         :param request: Request instance for CreateTKEEdgeCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateTKEEdgeClusterRequest`
@@ -824,15 +824,15 @@
             model = models.CreateTKEEdgeClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAddon(self, request):
         """删除一个addon
 
         :param request: Request instance for DeleteAddon.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteAddonRequest`
@@ -847,15 +847,15 @@
             model = models.DeleteAddonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBackupStorageLocation(self, request):
         """删除备份仓库
 
         :param request: Request instance for DeleteBackupStorageLocation.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteBackupStorageLocationRequest`
@@ -870,15 +870,15 @@
             model = models.DeleteBackupStorageLocationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """删除集群(YUNAPI V3版本)
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterRequest`
@@ -893,15 +893,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterAsGroups(self, request):
         """删除集群伸缩组
 
         :param request: Request instance for DeleteClusterAsGroups.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterAsGroupsRequest`
@@ -916,15 +916,15 @@
             model = models.DeleteClusterAsGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterEndpoint(self, request):
         """删除集群访问端口
 
         :param request: Request instance for DeleteClusterEndpoint.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterEndpointRequest`
@@ -939,15 +939,15 @@
             model = models.DeleteClusterEndpointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterEndpointVip(self, request):
         """删除托管集群外网访问端口（老的方式，仅支持托管集群外网端口）
 
         :param request: Request instance for DeleteClusterEndpointVip.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterEndpointVipRequest`
@@ -962,15 +962,15 @@
             model = models.DeleteClusterEndpointVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterInstances(self, request):
         """删除集群中的实例
 
         :param request: Request instance for DeleteClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterInstancesRequest`
@@ -985,15 +985,15 @@
             model = models.DeleteClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterNodePool(self, request):
         """删除节点池
 
         :param request: Request instance for DeleteClusterNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterNodePoolRequest`
@@ -1008,15 +1008,15 @@
             model = models.DeleteClusterNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterRoute(self, request):
         """删除集群路由
 
         :param request: Request instance for DeleteClusterRoute.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterRouteRequest`
@@ -1031,15 +1031,15 @@
             model = models.DeleteClusterRouteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterRouteTable(self, request):
         """删除集群路由表
 
         :param request: Request instance for DeleteClusterRouteTable.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterRouteTableRequest`
@@ -1054,15 +1054,15 @@
             model = models.DeleteClusterRouteTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterVirtualNode(self, request):
         """删除虚拟节点
 
         :param request: Request instance for DeleteClusterVirtualNode.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterVirtualNodeRequest`
@@ -1077,15 +1077,15 @@
             model = models.DeleteClusterVirtualNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterVirtualNodePool(self, request):
         """删除虚拟节点池
 
         :param request: Request instance for DeleteClusterVirtualNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterVirtualNodePoolRequest`
@@ -1100,15 +1100,15 @@
             model = models.DeleteClusterVirtualNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteECMInstances(self, request):
         """删除ECM实例
 
         :param request: Request instance for DeleteECMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteECMInstancesRequest`
@@ -1123,15 +1123,15 @@
             model = models.DeleteECMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEKSCluster(self, request):
         """删除弹性集群(yunapiv3)
 
         :param request: Request instance for DeleteEKSCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteEKSClusterRequest`
@@ -1146,15 +1146,15 @@
             model = models.DeleteEKSClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEKSContainerInstances(self, request):
         """删除容器实例，可批量删除
 
         :param request: Request instance for DeleteEKSContainerInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteEKSContainerInstancesRequest`
@@ -1169,15 +1169,15 @@
             model = models.DeleteEKSContainerInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeCVMInstances(self, request):
         """删除边缘容器CVM实例
 
         :param request: Request instance for DeleteEdgeCVMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteEdgeCVMInstancesRequest`
@@ -1192,15 +1192,15 @@
             model = models.DeleteEdgeCVMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEdgeClusterInstances(self, request):
         """删除边缘计算实例
 
         :param request: Request instance for DeleteEdgeClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteEdgeClusterInstancesRequest`
@@ -1215,15 +1215,15 @@
             model = models.DeleteEdgeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageCaches(self, request):
         """批量删除镜像缓存
 
         :param request: Request instance for DeleteImageCaches.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteImageCachesRequest`
@@ -1238,15 +1238,15 @@
             model = models.DeleteImageCachesResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusAlertPolicyRequest`
@@ -1261,15 +1261,15 @@
             model = models.DeletePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusAlertRule(self, request):
         """删除告警规则
 
         :param request: Request instance for DeletePrometheusAlertRule.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusAlertRuleRequest`
@@ -1284,15 +1284,15 @@
             model = models.DeletePrometheusAlertRuleResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusClusterAgentRequest`
@@ -1307,15 +1307,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusConfigRequest`
@@ -1330,15 +1330,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusRecordRuleYamlRequest`
@@ -1353,15 +1353,15 @@
             model = models.DeletePrometheusRecordRuleYamlResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusTempRequest`
@@ -1376,15 +1376,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusTempSyncRequest`
@@ -1399,15 +1399,15 @@
             model = models.DeletePrometheusTempSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusTemplate(self, request):
         """删除一个云原生Prometheus配置模板
 
         :param request: Request instance for DeletePrometheusTemplate.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusTemplateRequest`
@@ -1422,15 +1422,15 @@
             model = models.DeletePrometheusTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePrometheusTemplateSync(self, request):
         """取消模板同步，这将会删除目标中该模板所生产的配置
 
         :param request: Request instance for DeletePrometheusTemplateSync.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeletePrometheusTemplateSyncRequest`
@@ -1445,15 +1445,15 @@
             model = models.DeletePrometheusTemplateSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTKEEdgeCluster(self, request):
         """删除边缘计算集群
 
         :param request: Request instance for DeleteTKEEdgeCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteTKEEdgeClusterRequest`
@@ -1468,15 +1468,15 @@
             model = models.DeleteTKEEdgeClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddon(self, request):
         """获取addon列表
 
         :param request: Request instance for DescribeAddon.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAddonRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeAddonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAddonValues(self, request):
         """获取一个addon的参数
 
         :param request: Request instance for DescribeAddonValues.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAddonValuesRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeAddonValuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableClusterVersion(self, request):
         """获取集群可以升级的所有版本
 
         :param request: Request instance for DescribeAvailableClusterVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAvailableClusterVersionRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeAvailableClusterVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableTKEEdgeVersion(self, request):
         """边缘计算支持版本和k8s版本
 
         :param request: Request instance for DescribeAvailableTKEEdgeVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAvailableTKEEdgeVersionRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeAvailableTKEEdgeVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupStorageLocations(self, request):
         """查询备份仓库信息
 
         :param request: Request instance for DescribeBackupStorageLocations.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeBackupStorageLocationsRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeBackupStorageLocationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterAsGroupOption(self, request):
         """集群弹性伸缩配置
 
         :param request: Request instance for DescribeClusterAsGroupOption.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterAsGroupOptionRequest`
@@ -1606,15 +1606,15 @@
             model = models.DescribeClusterAsGroupOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterAsGroups(self, request):
         """集群关联的伸缩组列表
 
         :param request: Request instance for DescribeClusterAsGroups.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterAsGroupsRequest`
@@ -1629,15 +1629,15 @@
             model = models.DescribeClusterAsGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterAuthenticationOptions(self, request):
         """查看集群认证配置
 
         :param request: Request instance for DescribeClusterAuthenticationOptions.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterAuthenticationOptionsRequest`
@@ -1652,15 +1652,15 @@
             model = models.DescribeClusterAuthenticationOptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterCommonNames(self, request):
         """获取指定子账户在RBAC授权模式中对应kube-apiserver客户端证书的CommonName字段，如果没有客户端证书，将会签发一个，此接口有最大传入子账户数量上限，当前为50
 
         :param request: Request instance for DescribeClusterCommonNames.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterCommonNamesRequest`
@@ -1675,15 +1675,15 @@
             model = models.DescribeClusterCommonNamesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterControllers(self, request):
         """用于查询Kubernetes的各个原生控制器是否开启
 
         :param request: Request instance for DescribeClusterControllers.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterControllersRequest`
@@ -1698,15 +1698,15 @@
             model = models.DescribeClusterControllersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterEndpointStatus(self, request):
         """查询集群访问端口状态(独立集群开启内网/外网访问，托管集群支持开启内网访问)
 
         :param request: Request instance for DescribeClusterEndpointStatus.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterEndpointStatusRequest`
@@ -1721,15 +1721,15 @@
             model = models.DescribeClusterEndpointStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterEndpointVipStatus(self, request):
         """查询集群开启端口流程状态(仅支持托管集群外网端口)
 
         :param request: Request instance for DescribeClusterEndpointVipStatus.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterEndpointVipStatusRequest`
@@ -1744,15 +1744,15 @@
             model = models.DescribeClusterEndpointVipStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterEndpoints(self, request):
         """获取集群的访问地址，包括内网地址，外网地址，外网域名，外网访问安全策略
 
         :param request: Request instance for DescribeClusterEndpoints.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterEndpointsRequest`
@@ -1767,15 +1767,15 @@
             model = models.DescribeClusterEndpointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterInspectionResultsOverview(self, request):
         """查询用户单个Region下的所有集群巡检结果概览信息
 
         :param request: Request instance for DescribeClusterInspectionResultsOverview.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterInspectionResultsOverviewRequest`
@@ -1790,15 +1790,15 @@
             model = models.DescribeClusterInspectionResultsOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterInstances(self, request):
         """查询集群下节点实例信息
 
         :param request: Request instance for DescribeClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterInstancesRequest`
@@ -1813,15 +1813,15 @@
             model = models.DescribeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterKubeconfig(self, request):
         """获取集群的kubeconfig文件，不同子账户获取自己的kubeconfig文件，该文件中有每个子账户自己的kube-apiserver的客户端证书，默认首次调此接口时候创建客户端证书，时效20年，未授予任何权限，如果是集群所有者或者主账户，则默认是cluster-admin权限。
 
         :param request: Request instance for DescribeClusterKubeconfig.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterKubeconfigRequest`
@@ -1836,15 +1836,15 @@
             model = models.DescribeClusterKubeconfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterLevelAttribute(self, request):
         """获取集群规模
 
         :param request: Request instance for DescribeClusterLevelAttribute.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterLevelAttributeRequest`
@@ -1859,15 +1859,15 @@
             model = models.DescribeClusterLevelAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterLevelChangeRecords(self, request):
         """查询集群变配记录
 
         :param request: Request instance for DescribeClusterLevelChangeRecords.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterLevelChangeRecordsRequest`
@@ -1882,15 +1882,15 @@
             model = models.DescribeClusterLevelChangeRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterNodePoolDetail(self, request):
         """查询节点池详情
 
         :param request: Request instance for DescribeClusterNodePoolDetail.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterNodePoolDetailRequest`
@@ -1905,15 +1905,15 @@
             model = models.DescribeClusterNodePoolDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterNodePools(self, request):
         """查询节点池列表
 
         :param request: Request instance for DescribeClusterNodePools.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterNodePoolsRequest`
@@ -1928,15 +1928,15 @@
             model = models.DescribeClusterNodePoolsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterPendingReleases(self, request):
         """在应用市场中查询正在安装中的应用列表
 
         :param request: Request instance for DescribeClusterPendingReleases.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterPendingReleasesRequest`
@@ -1951,15 +1951,15 @@
             model = models.DescribeClusterPendingReleasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterReleaseDetails(self, request):
         """查询通过应用市场安装的某个应用详情
 
         :param request: Request instance for DescribeClusterReleaseDetails.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterReleaseDetailsRequest`
@@ -1974,15 +1974,15 @@
             model = models.DescribeClusterReleaseDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterReleaseHistory(self, request):
         """查询集群在应用市场中某个已安装应用的版本历史
 
         :param request: Request instance for DescribeClusterReleaseHistory.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterReleaseHistoryRequest`
@@ -1997,15 +1997,15 @@
             model = models.DescribeClusterReleaseHistoryResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterReleases(self, request):
         """查询集群在应用市场中已安装应用列表
 
         :param request: Request instance for DescribeClusterReleases.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterReleasesRequest`
@@ -2020,15 +2020,15 @@
             model = models.DescribeClusterReleasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterRouteTables(self, request):
         """查询集群路由表
 
         :param request: Request instance for DescribeClusterRouteTables.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterRouteTablesRequest`
@@ -2043,15 +2043,15 @@
             model = models.DescribeClusterRouteTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterRoutes(self, request):
         """查询集群路由
 
         :param request: Request instance for DescribeClusterRoutes.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterRoutesRequest`
@@ -2066,15 +2066,15 @@
             model = models.DescribeClusterRoutesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterSecurity(self, request):
         """集群的密钥信息
 
         :param request: Request instance for DescribeClusterSecurity.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterSecurityRequest`
@@ -2089,15 +2089,15 @@
             model = models.DescribeClusterSecurityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterStatus(self, request):
         """查看集群状态列表
 
         :param request: Request instance for DescribeClusterStatus.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterStatusRequest`
@@ -2112,15 +2112,15 @@
             model = models.DescribeClusterStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterVirtualNode(self, request):
         """查看虚拟节点列表
 
         :param request: Request instance for DescribeClusterVirtualNode.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterVirtualNodeRequest`
@@ -2135,15 +2135,15 @@
             model = models.DescribeClusterVirtualNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterVirtualNodePools(self, request):
         """查看虚拟节点池列表
 
         :param request: Request instance for DescribeClusterVirtualNodePools.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterVirtualNodePoolsRequest`
@@ -2158,15 +2158,15 @@
             model = models.DescribeClusterVirtualNodePoolsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """查询集群列表
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClustersRequest`
@@ -2181,15 +2181,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeECMInstances(self, request):
         """获取ECM实例相关信息
 
         :param request: Request instance for DescribeECMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeECMInstancesRequest`
@@ -2204,15 +2204,15 @@
             model = models.DescribeECMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEKSClusterCredential(self, request):
         """获取弹性容器集群的接入认证信息
 
         :param request: Request instance for DescribeEKSClusterCredential.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEKSClusterCredentialRequest`
@@ -2227,15 +2227,15 @@
             model = models.DescribeEKSClusterCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEKSClusters(self, request):
         """查询弹性集群列表
 
         :param request: Request instance for DescribeEKSClusters.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEKSClustersRequest`
@@ -2250,15 +2250,15 @@
             model = models.DescribeEKSClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEKSContainerInstanceEvent(self, request):
         """查询容器实例的事件
 
         :param request: Request instance for DescribeEKSContainerInstanceEvent.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEKSContainerInstanceEventRequest`
@@ -2273,15 +2273,15 @@
             model = models.DescribeEKSContainerInstanceEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEKSContainerInstanceRegions(self, request):
         """查询容器实例支持的地域
 
         :param request: Request instance for DescribeEKSContainerInstanceRegions.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEKSContainerInstanceRegionsRequest`
@@ -2296,15 +2296,15 @@
             model = models.DescribeEKSContainerInstanceRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEKSContainerInstances(self, request):
         """查询容器实例
 
         :param request: Request instance for DescribeEKSContainerInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEKSContainerInstancesRequest`
@@ -2319,15 +2319,15 @@
             model = models.DescribeEKSContainerInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeAvailableExtraArgs(self, request):
         """查询边缘容器集群可用的自定义参数
 
         :param request: Request instance for DescribeEdgeAvailableExtraArgs.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeAvailableExtraArgsRequest`
@@ -2342,15 +2342,15 @@
             model = models.DescribeEdgeAvailableExtraArgsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeCVMInstances(self, request):
         """获取边缘容器CVM实例相关信息
 
         :param request: Request instance for DescribeEdgeCVMInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeCVMInstancesRequest`
@@ -2365,15 +2365,15 @@
             model = models.DescribeEdgeCVMInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeClusterExtraArgs(self, request):
         """查询边缘集群自定义参数
 
         :param request: Request instance for DescribeEdgeClusterExtraArgs.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeClusterExtraArgsRequest`
@@ -2388,15 +2388,15 @@
             model = models.DescribeEdgeClusterExtraArgsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeClusterInstances(self, request):
         """查询边缘计算集群的节点信息
 
         :param request: Request instance for DescribeEdgeClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeClusterInstancesRequest`
@@ -2411,15 +2411,15 @@
             model = models.DescribeEdgeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeClusterUpgradeInfo(self, request):
         """可以查询边缘集群升级信息，包含可以升级的组件，当前升级状态和升级错误信息
 
         :param request: Request instance for DescribeEdgeClusterUpgradeInfo.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeClusterUpgradeInfoRequest`
@@ -2434,15 +2434,15 @@
             model = models.DescribeEdgeClusterUpgradeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEdgeLogSwitches(self, request):
         """获取事件、审计和日志的状态
 
         :param request: Request instance for DescribeEdgeLogSwitches.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEdgeLogSwitchesRequest`
@@ -2457,15 +2457,15 @@
             model = models.DescribeEdgeLogSwitchesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEksContainerInstanceLog(self, request):
         """查询容器实例中容器日志
 
         :param request: Request instance for DescribeEksContainerInstanceLog.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEksContainerInstanceLogRequest`
@@ -2480,15 +2480,15 @@
             model = models.DescribeEksContainerInstanceLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnableVpcCniProgress(self, request):
         """本接口用于查询开启vpc-cni模式的任务进度
 
         :param request: Request instance for DescribeEnableVpcCniProgress.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEnableVpcCniProgressRequest`
@@ -2503,15 +2503,15 @@
             model = models.DescribeEnableVpcCniProgressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEncryptionStatus(self, request):
         """查询etcd数据是否进行加密
 
         :param request: Request instance for DescribeEncryptionStatus.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeEncryptionStatusRequest`
@@ -2526,15 +2526,15 @@
             model = models.DescribeEncryptionStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExistedInstances(self, request):
         """查询已经存在的节点，判断是否可以加入集群
 
         :param request: Request instance for DescribeExistedInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeExistedInstancesRequest`
@@ -2549,15 +2549,15 @@
             model = models.DescribeExistedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeExternalClusterSpec(self, request):
         """获取导入第三方集群YAML定义
 
         :param request: Request instance for DescribeExternalClusterSpec.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeExternalClusterSpecRequest`
@@ -2572,15 +2572,15 @@
             model = models.DescribeExternalClusterSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageCaches(self, request):
         """查询镜像缓存信息接口
 
         :param request: Request instance for DescribeImageCaches.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeImageCachesRequest`
@@ -2595,15 +2595,15 @@
             model = models.DescribeImageCachesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """获取镜像信息
 
         :param request: Request instance for DescribeImages.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeImagesRequest`
@@ -2618,15 +2618,15 @@
             model = models.DescribeImagesResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusAgentInstancesRequest`
@@ -2641,15 +2641,15 @@
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
         """获取被关联集群列表
 
         :param request: Request instance for DescribePrometheusAgents.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusAgentsRequest`
@@ -2664,15 +2664,15 @@
             model = models.DescribePrometheusAgentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusAlertHistory(self, request):
         """获取告警历史
 
         :param request: Request instance for DescribePrometheusAlertHistory.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusAlertHistoryRequest`
@@ -2687,15 +2687,15 @@
             model = models.DescribePrometheusAlertHistoryResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusAlertPolicyRequest`
@@ -2710,15 +2710,15 @@
             model = models.DescribePrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusAlertRule(self, request):
         """获取告警规则列表
 
         :param request: Request instance for DescribePrometheusAlertRule.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusAlertRuleRequest`
@@ -2733,15 +2733,15 @@
             model = models.DescribePrometheusAlertRuleResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusClusterAgentsRequest`
@@ -2756,15 +2756,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusConfigRequest`
@@ -2779,15 +2779,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusGlobalConfigRequest`
@@ -2802,15 +2802,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusGlobalNotificationRequest`
@@ -2825,15 +2825,15 @@
             model = models.DescribePrometheusGlobalNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstance(self, request):
         """获取实例详细信息
 
         :param request: Request instance for DescribePrometheusInstance.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusInstanceRequest`
@@ -2848,15 +2848,15 @@
             model = models.DescribePrometheusInstanceResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusInstanceInitStatusRequest`
@@ -2871,15 +2871,15 @@
             model = models.DescribePrometheusInstanceInitStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusInstancesOverview(self, request):
         """获取与云监控融合实例列表
 
         :param request: Request instance for DescribePrometheusInstancesOverview.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusInstancesOverviewRequest`
@@ -2894,15 +2894,15 @@
             model = models.DescribePrometheusInstancesOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusOverviews(self, request):
         """获取实例列表
 
         :param request: Request instance for DescribePrometheusOverviews.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusOverviewsRequest`
@@ -2917,15 +2917,15 @@
             model = models.DescribePrometheusOverviewsResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusRecordRulesRequest`
@@ -2940,15 +2940,15 @@
             model = models.DescribePrometheusRecordRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTargets(self, request):
         """获取targets信息
 
         :param request: Request instance for DescribePrometheusTargets.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusTargetsRequest`
@@ -2963,15 +2963,15 @@
             model = models.DescribePrometheusTargetsResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusTempRequest`
@@ -2986,15 +2986,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusTempSyncRequest`
@@ -3009,15 +3009,15 @@
             model = models.DescribePrometheusTempSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTemplateSync(self, request):
         """获取模板同步信息
 
         :param request: Request instance for DescribePrometheusTemplateSync.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusTemplateSyncRequest`
@@ -3032,15 +3032,15 @@
             model = models.DescribePrometheusTemplateSyncResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrometheusTemplates(self, request):
         """拉取模板列表，默认模板将总是在最前面
 
         :param request: Request instance for DescribePrometheusTemplates.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribePrometheusTemplatesRequest`
@@ -3055,15 +3055,15 @@
             model = models.DescribePrometheusTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """获取容器服务支持的所有地域
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeRegionsRequest`
@@ -3078,15 +3078,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceUsage(self, request):
         """获取集群资源使用量
 
         :param request: Request instance for DescribeResourceUsage.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeResourceUsageRequest`
@@ -3101,15 +3101,15 @@
             model = models.DescribeResourceUsageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRouteTableConflicts(self, request):
         """查询路由表冲突列表
 
         :param request: Request instance for DescribeRouteTableConflicts.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeRouteTableConflictsRequest`
@@ -3124,15 +3124,15 @@
             model = models.DescribeRouteTableConflictsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTKEEdgeClusterCredential(self, request):
         """获取边缘计算集群的认证信息
 
         :param request: Request instance for DescribeTKEEdgeClusterCredential.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeTKEEdgeClusterCredentialRequest`
@@ -3147,15 +3147,15 @@
             model = models.DescribeTKEEdgeClusterCredentialResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTKEEdgeClusterStatus(self, request):
         """获取边缘计算集群的当前状态以及过程信息
 
         :param request: Request instance for DescribeTKEEdgeClusterStatus.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeTKEEdgeClusterStatusRequest`
@@ -3170,15 +3170,15 @@
             model = models.DescribeTKEEdgeClusterStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTKEEdgeClusters(self, request):
         """查询边缘集群列表
 
         :param request: Request instance for DescribeTKEEdgeClusters.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeTKEEdgeClustersRequest`
@@ -3193,15 +3193,15 @@
             model = models.DescribeTKEEdgeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTKEEdgeExternalKubeconfig(self, request):
         """获取边缘计算外部访问的kubeconfig
 
         :param request: Request instance for DescribeTKEEdgeExternalKubeconfig.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeTKEEdgeExternalKubeconfigRequest`
@@ -3216,15 +3216,15 @@
             model = models.DescribeTKEEdgeExternalKubeconfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTKEEdgeScript(self, request):
         """获取边缘脚本链接，此接口用于添加第三方节点，通过下载脚本从而将节点添加到边缘集群。
 
         :param request: Request instance for DescribeTKEEdgeScript.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeTKEEdgeScriptRequest`
@@ -3239,15 +3239,15 @@
             model = models.DescribeTKEEdgeScriptResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVersions(self, request):
         """获取集群版本信息
 
         :param request: Request instance for DescribeVersions.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeVersionsRequest`
@@ -3262,15 +3262,15 @@
             model = models.DescribeVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVpcCniPodLimits(self, request):
         """本接口查询当前用户和地域在指定可用区下的机型可支持的最大 TKE VPC-CNI 网络模式的 Pod 数量
 
         :param request: Request instance for DescribeVpcCniPodLimits.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeVpcCniPodLimitsRequest`
@@ -3285,15 +3285,15 @@
             model = models.DescribeVpcCniPodLimitsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableClusterAudit(self, request):
         """关闭集群审计
 
         :param request: Request instance for DisableClusterAudit.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableClusterAuditRequest`
@@ -3308,15 +3308,15 @@
             model = models.DisableClusterAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableClusterDeletionProtection(self, request):
         """关闭集群删除保护
 
         :param request: Request instance for DisableClusterDeletionProtection.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableClusterDeletionProtectionRequest`
@@ -3331,15 +3331,15 @@
             model = models.DisableClusterDeletionProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableEncryptionProtection(self, request):
         """关闭加密信息保护
 
         :param request: Request instance for DisableEncryptionProtection.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableEncryptionProtectionRequest`
@@ -3354,15 +3354,15 @@
             model = models.DisableEncryptionProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableEventPersistence(self, request):
         """关闭事件持久化功能
 
         :param request: Request instance for DisableEventPersistence.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableEventPersistenceRequest`
@@ -3377,15 +3377,15 @@
             model = models.DisableEventPersistenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableVpcCniNetworkType(self, request):
         """提供给附加了VPC-CNI能力的Global-Route集群关闭VPC-CNI
 
         :param request: Request instance for DisableVpcCniNetworkType.
         :type request: :class:`tencentcloud.tke.v20180525.models.DisableVpcCniNetworkTypeRequest`
@@ -3400,15 +3400,15 @@
             model = models.DisableVpcCniNetworkTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DrainClusterVirtualNode(self, request):
         """驱逐虚拟节点
 
         :param request: Request instance for DrainClusterVirtualNode.
         :type request: :class:`tencentcloud.tke.v20180525.models.DrainClusterVirtualNodeRequest`
@@ -3423,15 +3423,15 @@
             model = models.DrainClusterVirtualNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableClusterAudit(self, request):
         """开启集群审计
 
         :param request: Request instance for EnableClusterAudit.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableClusterAuditRequest`
@@ -3446,15 +3446,15 @@
             model = models.EnableClusterAuditResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableClusterDeletionProtection(self, request):
         """启用集群删除保护
 
         :param request: Request instance for EnableClusterDeletionProtection.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableClusterDeletionProtectionRequest`
@@ -3469,15 +3469,15 @@
             model = models.EnableClusterDeletionProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableEncryptionProtection(self, request):
         """开启加密数据保护
 
         :param request: Request instance for EnableEncryptionProtection.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableEncryptionProtectionRequest`
@@ -3492,15 +3492,15 @@
             model = models.EnableEncryptionProtectionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableEventPersistence(self, request):
         """开启事件持久化功能
 
         :param request: Request instance for EnableEventPersistence.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableEventPersistenceRequest`
@@ -3515,15 +3515,15 @@
             model = models.EnableEventPersistenceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableVpcCniNetworkType(self, request):
         """GR集群可以通过本接口附加vpc-cni容器网络插件，开启vpc-cni容器网络能力
 
         :param request: Request instance for EnableVpcCniNetworkType.
         :type request: :class:`tencentcloud.tke.v20180525.models.EnableVpcCniNetworkTypeRequest`
@@ -3538,15 +3538,15 @@
             model = models.EnableVpcCniNetworkTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForwardApplicationRequestV3(self, request):
         """操作TKE集群的addon
 
         :param request: Request instance for ForwardApplicationRequestV3.
         :type request: :class:`tencentcloud.tke.v20180525.models.ForwardApplicationRequestV3Request`
@@ -3561,15 +3561,15 @@
             model = models.ForwardApplicationRequestV3Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForwardTKEEdgeApplicationRequestV3(self, request):
         """操作TKEEdge集群的addon
 
         :param request: Request instance for ForwardTKEEdgeApplicationRequestV3.
         :type request: :class:`tencentcloud.tke.v20180525.models.ForwardTKEEdgeApplicationRequestV3Request`
@@ -3584,15 +3584,15 @@
             model = models.ForwardTKEEdgeApplicationRequestV3Response()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetClusterLevelPrice(self, request):
         """获取集群规模价格
 
         :param request: Request instance for GetClusterLevelPrice.
         :type request: :class:`tencentcloud.tke.v20180525.models.GetClusterLevelPriceRequest`
@@ -3607,15 +3607,15 @@
             model = models.GetClusterLevelPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetMostSuitableImageCache(self, request):
         """根据镜像列表，查询匹配的镜像缓存
 
         :param request: Request instance for GetMostSuitableImageCache.
         :type request: :class:`tencentcloud.tke.v20180525.models.GetMostSuitableImageCacheRequest`
@@ -3630,15 +3630,15 @@
             model = models.GetMostSuitableImageCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTkeAppChartList(self, request):
         """获取TKE支持的App列表
 
         :param request: Request instance for GetTkeAppChartList.
         :type request: :class:`tencentcloud.tke.v20180525.models.GetTkeAppChartListRequest`
@@ -3653,15 +3653,15 @@
             model = models.GetTkeAppChartListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetUpgradeInstanceProgress(self, request):
         """获得节点升级当前的进度
 
         :param request: Request instance for GetUpgradeInstanceProgress.
         :type request: :class:`tencentcloud.tke.v20180525.models.GetUpgradeInstanceProgressRequest`
@@ -3676,15 +3676,15 @@
             model = models.GetUpgradeInstanceProgressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InstallAddon(self, request):
         """为目标集群安装一个addon
 
         :param request: Request instance for InstallAddon.
         :type request: :class:`tencentcloud.tke.v20180525.models.InstallAddonRequest`
@@ -3699,15 +3699,15 @@
             model = models.InstallAddonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InstallEdgeLogAgent(self, request):
         """在tke@edge集群的边缘节点上安装日志采集组件
 
         :param request: Request instance for InstallEdgeLogAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.InstallEdgeLogAgentRequest`
@@ -3722,15 +3722,15 @@
             model = models.InstallEdgeLogAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InstallLogAgent(self, request):
         """在TKE集群中安装CLS日志采集组件
 
         :param request: Request instance for InstallLogAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.InstallLogAgentRequest`
@@ -3745,15 +3745,15 @@
             model = models.InstallLogAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListClusterInspectionResults(self, request):
         """查询指定集群的巡检结果信息
 
         :param request: Request instance for ListClusterInspectionResults.
         :type request: :class:`tencentcloud.tke.v20180525.models.ListClusterInspectionResultsRequest`
@@ -3768,15 +3768,15 @@
             model = models.ListClusterInspectionResultsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListClusterInspectionResultsItems(self, request):
         """查询集群巡检结果历史列表
 
         :param request: Request instance for ListClusterInspectionResultsItems.
         :type request: :class:`tencentcloud.tke.v20180525.models.ListClusterInspectionResultsItemsRequest`
@@ -3791,15 +3791,15 @@
             model = models.ListClusterInspectionResultsItemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterAsGroupAttribute(self, request):
         """修改集群伸缩组属性
 
         :param request: Request instance for ModifyClusterAsGroupAttribute.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterAsGroupAttributeRequest`
@@ -3814,15 +3814,15 @@
             model = models.ModifyClusterAsGroupAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterAsGroupOptionAttribute(self, request):
         """修改集群弹性伸缩属性
 
         :param request: Request instance for ModifyClusterAsGroupOptionAttribute.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterAsGroupOptionAttributeRequest`
@@ -3837,15 +3837,15 @@
             model = models.ModifyClusterAsGroupOptionAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterAttribute(self, request):
         """修改集群属性
 
         :param request: Request instance for ModifyClusterAttribute.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterAttributeRequest`
@@ -3860,15 +3860,15 @@
             model = models.ModifyClusterAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterAuthenticationOptions(self, request):
         """修改集群认证配置
 
         :param request: Request instance for ModifyClusterAuthenticationOptions.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterAuthenticationOptionsRequest`
@@ -3883,15 +3883,15 @@
             model = models.ModifyClusterAuthenticationOptionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterEndpointSP(self, request):
         """修改托管集群外网端口的安全策略（老的方式，仅支持托管集群外网端口）
 
         :param request: Request instance for ModifyClusterEndpointSP.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterEndpointSPRequest`
@@ -3906,15 +3906,15 @@
             model = models.ModifyClusterEndpointSPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterNodePool(self, request):
         """编辑节点池
 
         :param request: Request instance for ModifyClusterNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterNodePoolRequest`
@@ -3929,15 +3929,15 @@
             model = models.ModifyClusterNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterVirtualNodePool(self, request):
         """修改虚拟节点池
 
         :param request: Request instance for ModifyClusterVirtualNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyClusterVirtualNodePoolRequest`
@@ -3952,15 +3952,15 @@
             model = models.ModifyClusterVirtualNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNodePoolDesiredCapacityAboutAsg(self, request):
         """修改节点池关联伸缩组的期望实例数
 
         :param request: Request instance for ModifyNodePoolDesiredCapacityAboutAsg.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyNodePoolDesiredCapacityAboutAsgRequest`
@@ -3975,15 +3975,15 @@
             model = models.ModifyNodePoolDesiredCapacityAboutAsgResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNodePoolInstanceTypes(self, request):
         """修改节点池的机型配置
 
         :param request: Request instance for ModifyNodePoolInstanceTypes.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyNodePoolInstanceTypesRequest`
@@ -3998,15 +3998,15 @@
             model = models.ModifyNodePoolInstanceTypesResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusAgentExternalLabelsRequest`
@@ -4021,15 +4021,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusAlertPolicyRequest`
@@ -4044,15 +4044,15 @@
             model = models.ModifyPrometheusAlertPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusAlertRule(self, request):
         """修改告警规则
 
         :param request: Request instance for ModifyPrometheusAlertRule.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusAlertRuleRequest`
@@ -4067,15 +4067,15 @@
             model = models.ModifyPrometheusAlertRuleResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusConfigRequest`
@@ -4090,15 +4090,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusGlobalNotificationRequest`
@@ -4113,15 +4113,15 @@
             model = models.ModifyPrometheusGlobalNotificationResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusRecordRuleYamlRequest`
@@ -4136,15 +4136,15 @@
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
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusTempRequest`
@@ -4159,15 +4159,15 @@
             model = models.ModifyPrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPrometheusTemplate(self, request):
         """修改模板内容
 
         :param request: Request instance for ModifyPrometheusTemplate.
         :type request: :class:`tencentcloud.tke.v20180525.models.ModifyPrometheusTemplateRequest`
@@ -4182,15 +4182,15 @@
             model = models.ModifyPrometheusTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveNodeFromNodePool(self, request):
         """移出节点池节点，但保留在集群内
 
         :param request: Request instance for RemoveNodeFromNodePool.
         :type request: :class:`tencentcloud.tke.v20180525.models.RemoveNodeFromNodePoolRequest`
@@ -4205,15 +4205,15 @@
             model = models.RemoveNodeFromNodePoolResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartEKSContainerInstances(self, request):
         """重启弹性容器实例，支持批量操作
 
         :param request: Request instance for RestartEKSContainerInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.RestartEKSContainerInstancesRequest`
@@ -4228,15 +4228,15 @@
             model = models.RestartEKSContainerInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackClusterRelease(self, request):
         """在应用市场中集群回滚应用至某个历史版本
 
         :param request: Request instance for RollbackClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.RollbackClusterReleaseRequest`
@@ -4251,15 +4251,15 @@
             model = models.RollbackClusterReleaseResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.RunPrometheusInstanceRequest`
@@ -4274,15 +4274,15 @@
             model = models.RunPrometheusInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleInClusterMaster(self, request):
         """缩容独立集群master节点
 
         :param request: Request instance for ScaleInClusterMaster.
         :type request: :class:`tencentcloud.tke.v20180525.models.ScaleInClusterMasterRequest`
@@ -4297,15 +4297,15 @@
             model = models.ScaleInClusterMasterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleOutClusterMaster(self, request):
         """扩容独立集群master节点
 
         :param request: Request instance for ScaleOutClusterMaster.
         :type request: :class:`tencentcloud.tke.v20180525.models.ScaleOutClusterMasterRequest`
@@ -4320,15 +4320,15 @@
             model = models.ScaleOutClusterMasterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetNodePoolNodeProtection(self, request):
         """仅能设置节点池中处于伸缩组的节点
 
         :param request: Request instance for SetNodePoolNodeProtection.
         :type request: :class:`tencentcloud.tke.v20180525.models.SetNodePoolNodeProtectionRequest`
@@ -4343,15 +4343,15 @@
             model = models.SetNodePoolNodeProtectionResponse()
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
         :type request: :class:`tencentcloud.tke.v20180525.models.SyncPrometheusTempRequest`
@@ -4366,15 +4366,15 @@
             model = models.SyncPrometheusTempResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncPrometheusTemplate(self, request):
         """同步模板到实例或者集群
 
         :param request: Request instance for SyncPrometheusTemplate.
         :type request: :class:`tencentcloud.tke.v20180525.models.SyncPrometheusTemplateRequest`
@@ -4389,15 +4389,15 @@
             model = models.SyncPrometheusTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UninstallClusterRelease(self, request):
         """在应用市场中集群删除某个应用
 
         :param request: Request instance for UninstallClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.UninstallClusterReleaseRequest`
@@ -4412,15 +4412,15 @@
             model = models.UninstallClusterReleaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UninstallEdgeLogAgent(self, request):
         """从tke@edge集群边缘节点上卸载日志采集组件
 
         :param request: Request instance for UninstallEdgeLogAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.UninstallEdgeLogAgentRequest`
@@ -4435,15 +4435,15 @@
             model = models.UninstallEdgeLogAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UninstallLogAgent(self, request):
         """从TKE集群中卸载CLS日志采集组件
 
         :param request: Request instance for UninstallLogAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.UninstallLogAgentRequest`
@@ -4458,15 +4458,15 @@
             model = models.UninstallLogAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAddon(self, request):
         """更新一个addon的参数和版本
 
         :param request: Request instance for UpdateAddon.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateAddonRequest`
@@ -4481,15 +4481,15 @@
             model = models.UpdateAddonResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateClusterKubeconfig(self, request):
         """对集群的Kubeconfig信息进行更新
 
         :param request: Request instance for UpdateClusterKubeconfig.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateClusterKubeconfigRequest`
@@ -4504,15 +4504,15 @@
             model = models.UpdateClusterKubeconfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateClusterVersion(self, request):
         """升级集群 Master 组件到指定版本
 
         :param request: Request instance for UpdateClusterVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateClusterVersionRequest`
@@ -4527,15 +4527,15 @@
             model = models.UpdateClusterVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEKSCluster(self, request):
         """修改弹性集群名称等属性
 
         :param request: Request instance for UpdateEKSCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateEKSClusterRequest`
@@ -4550,15 +4550,15 @@
             model = models.UpdateEKSClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEKSContainerInstance(self, request):
         """更新容器实例
 
         :param request: Request instance for UpdateEKSContainerInstance.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateEKSContainerInstanceRequest`
@@ -4573,15 +4573,15 @@
             model = models.UpdateEKSContainerInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateEdgeClusterVersion(self, request):
         """升级边缘集群组件到指定版本，此版本为TKEEdge专用版本。
 
         :param request: Request instance for UpdateEdgeClusterVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateEdgeClusterVersionRequest`
@@ -4596,15 +4596,15 @@
             model = models.UpdateEdgeClusterVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateImageCache(self, request):
         """更新镜像缓存接口
 
         :param request: Request instance for UpdateImageCache.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateImageCacheRequest`
@@ -4619,15 +4619,15 @@
             model = models.UpdateImageCacheResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateTKEEdgeCluster(self, request):
         """修改边缘计算集群名称等属性
 
         :param request: Request instance for UpdateTKEEdgeCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateTKEEdgeClusterRequest`
@@ -4642,15 +4642,15 @@
             model = models.UpdateTKEEdgeClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeClusterInstances(self, request):
         """给集群的一批work节点进行升级
 
         :param request: Request instance for UpgradeClusterInstances.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpgradeClusterInstancesRequest`
@@ -4665,15 +4665,15 @@
             model = models.UpgradeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeClusterRelease(self, request):
         """升级集群中已安装的应用
 
         :param request: Request instance for UpgradeClusterRelease.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpgradeClusterReleaseRequest`
@@ -4688,8 +4688,8 @@
             model = models.UpgradeClusterReleaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.937/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.938/tencentcloud/tke/v20180525/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.937/README.rst` & `tencentcloud-sdk-python-tke-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.937/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.938/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

