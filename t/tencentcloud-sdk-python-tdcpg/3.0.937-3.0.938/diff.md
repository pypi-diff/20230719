# Comparing `tmp/tencentcloud-sdk-python-tdcpg-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tdcpg-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdcpg-3.0.937.tar", last modified: Tue Jul 18 00:32:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdcpg-3.0.938.tar", last modified: Wed Jul 19 00:49:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdcpg-3.0.937.tar` & `tencentcloud-sdk-python-tdcpg-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/
--rw-r--r--   0 root         (0) root         (0)    24777 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/tdcpg_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   102873 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:32:04.000000 tencentcloud-sdk-python-tdcpg-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/
+-rw-r--r--   0 root         (0) root         (0)    24877 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/tdcpg_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   102873 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:49:45.000000 tencentcloud-sdk-python-tdcpg-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/setup.py` & `tencentcloud-sdk-python-tdcpg-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud_sdk_python_tdcpg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud_sdk_python_tdcpg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdcpg
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdcpg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/tdcpg_client.py` & `tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/tdcpg_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CloneClusterToPointInTimeResponse()
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
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.CreateClusterRequest`
@@ -65,15 +65,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterInstances(self, request):
         """在集群中新建实例
 
         :param request: Request instance for CreateClusterInstances.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.CreateClusterInstancesRequest`
@@ -88,15 +88,15 @@
             model = models.CreateClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """删除集群，集群中的实例和数据都将被删除，且无法恢复。只有当集群状态处于isolated(已隔离)时才生效。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DeleteClusterRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterInstances(self, request):
         """删除实例。只有当实例状态处于isolated(已隔离)时才生效。
 
         :param request: Request instance for DeleteClusterInstances.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DeleteClusterInstancesRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """查询数据库账号信息
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeAccountsRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterBackups(self, request):
         """查询集群的备份集
 
         :param request: Request instance for DescribeClusterBackups.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeClusterBackupsRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeClusterBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterEndpoints(self, request):
         """查询集群接入点信息
 
         :param request: Request instance for DescribeClusterEndpoints.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeClusterEndpointsRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeClusterEndpointsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterInstances(self, request):
         """查询实例
 
         :param request: Request instance for DescribeClusterInstances.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeClusterInstancesRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterRecoveryTimeRange(self, request):
         """查询集群可回档时间范围
 
         :param request: Request instance for DescribeClusterRecoveryTimeRange.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeClusterRecoveryTimeRangeRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeClusterRecoveryTimeRangeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """查询集群
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeClustersRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcesByDealName(self, request):
         """根据订单号获取资源信息
 
         :param request: Request instance for DescribeResourcesByDealName.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.DescribeResourcesByDealNameRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeResourcesByDealNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateCluster(self, request):
         """隔离集群，集群的接入点网络将会断掉无法连接使用数据库。只有当集群状态处于running(运行中)时才生效。
 
         :param request: Request instance for IsolateCluster.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.IsolateClusterRequest`
@@ -318,15 +318,15 @@
             model = models.IsolateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateClusterInstances(self, request):
         """隔离实例。此接口只针对状态为running的实例生效，使用场景包括：
          - 批量隔离集群内所有的实例
          - 在读写实例为running(运行中)时，单个/批量隔离只读实例
          - 集群内所有只读实例为isolated(已隔离)时，单独隔离读写实例
@@ -344,15 +344,15 @@
             model = models.IsolateClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountDescription(self, request):
         """修改数据库账号描述
 
         :param request: Request instance for ModifyAccountDescription.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ModifyAccountDescriptionRequest`
@@ -367,15 +367,15 @@
             model = models.ModifyAccountDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterEndpointWanStatus(self, request):
         """开启或者关闭接入点外网
 
         :param request: Request instance for ModifyClusterEndpointWanStatus.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ModifyClusterEndpointWanStatusRequest`
@@ -390,15 +390,15 @@
             model = models.ModifyClusterEndpointWanStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterInstancesSpec(self, request):
         """修改实例规格，此接口只针对状态为running(运行中)的实例生效
 
         :param request: Request instance for ModifyClusterInstancesSpec.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ModifyClusterInstancesSpecRequest`
@@ -413,15 +413,15 @@
             model = models.ModifyClusterInstancesSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterName(self, request):
         """修改集群名字
 
         :param request: Request instance for ModifyClusterName.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ModifyClusterNameRequest`
@@ -436,15 +436,15 @@
             model = models.ModifyClusterNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClustersAutoRenewFlag(self, request):
         """修改集群自动续费，只对预付费集群生效。
 
         :param request: Request instance for ModifyClustersAutoRenewFlag.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ModifyClustersAutoRenewFlagRequest`
@@ -459,15 +459,15 @@
             model = models.ModifyClustersAutoRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverCluster(self, request):
         """恢复集群，恢复集群的接入点网络，恢复后继续连接使用数据库。只有当集群状态处于isolated(已隔离)时才生效。
 
         :param request: Request instance for RecoverCluster.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.RecoverClusterRequest`
@@ -482,15 +482,15 @@
             model = models.RecoverClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverClusterInstances(self, request):
         """恢复实例。此接口的使用场景包括：
          - 读写实例状态为running(运行中)时，批量恢复状态为isolated(已隔离)的只读实例
          - 读写实例状态为isolated(已隔离)时，恢复读写实例
          - 读写实例状态为isolated(已隔离)时，批量恢复读写实例以及状态为isolated(已隔离)的只读实例
@@ -508,15 +508,15 @@
             model = models.RecoverClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewCluster(self, request):
         """续费集群
 
         :param request: Request instance for RenewCluster.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.RenewClusterRequest`
@@ -531,15 +531,15 @@
             model = models.RenewClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAccountPassword(self, request):
         """重置数据库账号密码
 
         :param request: Request instance for ResetAccountPassword.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.ResetAccountPasswordRequest`
@@ -554,15 +554,15 @@
             model = models.ResetAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartClusterInstances(self, request):
         """重启实例，此接口只针对状态为running(运行中)的实例生效。
 
         :param request: Request instance for RestartClusterInstances.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.RestartClusterInstancesRequest`
@@ -577,15 +577,15 @@
             model = models.RestartClusterInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TransformClusterPayMode(self, request):
         """转换集群付费模式，目前只支持从 后付费 转换成 与预付费。
 
         :param request: Request instance for TransformClusterPayMode.
         :type request: :class:`tencentcloud.tdcpg.v20211118.models.TransformClusterPayModeRequest`
@@ -600,8 +600,8 @@
             model = models.TransformClusterPayModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/errorcodes.py` & `tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/tencentcloud/tdcpg/v20211118/models.py` & `tencentcloud-sdk-python-tdcpg-3.0.938/tencentcloud/tdcpg/v20211118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tdcpg-3.0.938/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdcpg
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tdcpg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdcpg-3.0.937/README.rst` & `tencentcloud-sdk-python-tdcpg-3.0.938/README.rst`

 * *Files identical despite different names*

