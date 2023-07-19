# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.937.tar", last modified: Tue Jul 18 00:32:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.938.tar", last modified: Wed Jul 19 00:50:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.937.tar` & `tencentcloud-sdk-python-thpc-3.0.938.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)    17699 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   157753 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    63030 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)    16733 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4733 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   142732 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:32:39.000000 tencentcloud-sdk-python-thpc-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:40.000000 tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   157753 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    63030 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)    16797 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   142732 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:20.000000 tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/setup.py` & `tencentcloud-sdk-python-thpc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddNodes(self, request):
         """本接口(AddNodes)用于添加一个或者多个计算节点或者登录节点到指定集群。
 
         :param request: Request instance for AddNodes.
         :type request: :class:`tencentcloud.thpc.v20230321.models.AddNodesRequest`
@@ -65,15 +65,15 @@
             model = models.AddNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddQueue(self, request):
         """本接口(AddQueue)用于添加队列到指定集群。
         * 本接口为目前只支持SchedulerType为SLURM的集群。
         * 单个集群中队列数量上限为10个。
 
@@ -90,15 +90,15 @@
             model = models.AddQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """本接口 (CreateCluster) 用于创建并启动集群。
 
         * 本接口为异步接口， 当创建集群请求下发成功后会返回一个集群`ID`和一个`RequestId`，此时创建集群操作并未立即完成。在此期间集群的状态将会处于“PENDING”或者“INITING”，集群创建结果可以通过调用 [DescribeClusters](https://cloud.tencent.com/document/product/1527/72100)  接口查询，如果集群状态(ClusterStatus)变为“RUNNING(运行中)”，则代表集群创建成功，“ INIT_FAILED”代表集群创建失败。
 
@@ -115,15 +115,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """本接口（DeleteCluster）用于删除一个指定的集群。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DeleteClusterRequest`
@@ -138,15 +138,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterStorageOption(self, request):
         """本接口 (DeleteClusterStorageOption) 用于删除集群存储选项信息。
 
         :param request: Request instance for DeleteClusterStorageOption.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DeleteClusterStorageOptionRequest`
@@ -161,15 +161,15 @@
             model = models.DeleteClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNodes(self, request):
         """本接口(DeleteNodes)用于删除指定集群中一个或者多个计算节点或者登录节点。
 
         :param request: Request instance for DeleteNodes.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DeleteNodesRequest`
@@ -184,15 +184,15 @@
             model = models.DeleteNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteQueue(self, request):
         """本接口(DeleteQueue)用于从指定集群删除队列。
         * 本接口为目前只支持SchedulerType为SLURM的集群。
 
         * 删除队列时，需要保证队列内不存在节点。
@@ -210,15 +210,15 @@
             model = models.DeleteQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingConfiguration(self, request):
         """本接口(DescribeAutoScalingConfiguration)用于查询集群弹性伸缩配置信息。本接口仅适用于弹性伸缩类型为THPC_AS的集群。
 
         :param request: Request instance for DescribeAutoScalingConfiguration.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeAutoScalingConfigurationRequest`
@@ -233,15 +233,15 @@
             model = models.DescribeAutoScalingConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterActivities(self, request):
         """本接口（DescribeClusterActivities）用于查询集群活动历史记录列表。
 
         :param request: Request instance for DescribeClusterActivities.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeClusterActivitiesRequest`
@@ -256,15 +256,15 @@
             model = models.DescribeClusterActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterStorageOption(self, request):
         """本接口 (DescribeClusterStorageOption) 用于查询集群存储选项信息。
 
         :param request: Request instance for DescribeClusterStorageOption.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeClusterStorageOptionRequest`
@@ -279,15 +279,15 @@
             model = models.DescribeClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """本接口（DescribeClusters）用于查询集群列表。
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeClustersRequest`
@@ -302,15 +302,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInitNodeScripts(self, request):
         """本接口 (DescribeInitNodeScripts) 用于查询节点初始化脚本列表。
 
         :param request: Request instance for DescribeInitNodeScripts.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeInitNodeScriptsRequest`
@@ -325,15 +325,15 @@
             model = models.DescribeInitNodeScriptsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNodes(self, request):
         """本接口 (DescribeNodes) 用于查询指定集群节点概览信息列表。
 
         :param request: Request instance for DescribeNodes.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeNodesRequest`
@@ -348,15 +348,15 @@
             model = models.DescribeNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQueues(self, request):
         """本接口(DescribeQueues)用于查询指定集群队列概览信息列表。
 
         :param request: Request instance for DescribeQueues.
         :type request: :class:`tencentcloud.thpc.v20230321.models.DescribeQueuesRequest`
@@ -371,15 +371,15 @@
             model = models.DescribeQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInitNodeScripts(self, request):
         """本接口 (ModifyInitNodeScripts) 用于修改节点初始化脚本。
 
         :param request: Request instance for ModifyInitNodeScripts.
         :type request: :class:`tencentcloud.thpc.v20230321.models.ModifyInitNodeScriptsRequest`
@@ -394,15 +394,15 @@
             model = models.ModifyInitNodeScriptsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAutoScalingConfiguration(self, request):
         """本接口(SetAutoScalingConfiguration)用于为集群设置集群弹性伸缩配置信息。
 
         :param request: Request instance for SetAutoScalingConfiguration.
         :type request: :class:`tencentcloud.thpc.v20230321.models.SetAutoScalingConfigurationRequest`
@@ -417,8 +417,8 @@
             model = models.SetAutoScalingConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20230321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """本接口 (CreateCluster) 用于创建并启动集群。
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.thpc.v20211109.models.CreateClusterRequest`
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
 
 
     def DeleteCluster(self, request):
         """本接口（DeleteCluster）用于删除一个指定的集群。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.thpc.v20211109.models.DeleteClusterRequest`
@@ -88,15 +88,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """本接口（DescribeClusters）用于查询集群列表。
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.thpc.v20211109.models.DescribeClustersRequest`
@@ -111,8 +111,8 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddNodes(self, request):
         """本接口(AddNodes)用于添加一个或者多个计算节点或者登录节点到指定集群。
 
         :param request: Request instance for AddNodes.
         :type request: :class:`tencentcloud.thpc.v20220401.models.AddNodesRequest`
@@ -65,15 +65,15 @@
             model = models.AddNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddQueue(self, request):
         """本接口(AddQueue)用于添加队列到指定集群。
         * 本接口为目前只支持SchedulerType为SLURM的集群。
         * 单个集群中队列数量上限为10个。
 
@@ -90,15 +90,15 @@
             model = models.AddQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindAutoScalingGroup(self, request):
         """本接口(BindAutoScalingGroup)用于为集群队列绑定弹性伸缩组
 
         :param request: Request instance for BindAutoScalingGroup.
         :type request: :class:`tencentcloud.thpc.v20220401.models.BindAutoScalingGroupRequest`
@@ -113,15 +113,15 @@
             model = models.BindAutoScalingGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """本接口 (CreateCluster) 用于创建并启动集群。
 
         * 本接口为异步接口， 当创建集群请求下发成功后会返回一个集群`ID`和一个`RequestId`，此时创建集群操作并未立即完成。在此期间集群的状态将会处于“PENDING”或者“INITING”，集群创建结果可以通过调用 [DescribeClusters](https://cloud.tencent.com/document/product/1527/72100)  接口查询，如果集群状态(ClusterStatus)变为“RUNNING(运行中)”，则代表集群创建成功，“ INIT_FAILED”代表集群创建失败。
 
@@ -138,15 +138,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """本接口（DeleteCluster）用于删除一个指定的集群。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DeleteClusterRequest`
@@ -161,15 +161,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterStorageOption(self, request):
         """本接口 (DeleteClusterStorageOption) 用于删除集群存储选项信息。
 
         :param request: Request instance for DeleteClusterStorageOption.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DeleteClusterStorageOptionRequest`
@@ -184,15 +184,15 @@
             model = models.DeleteClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteNodes(self, request):
         """本接口(DeleteNodes)用于删除指定集群中一个或者多个计算节点或者登录节点。
 
         :param request: Request instance for DeleteNodes.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DeleteNodesRequest`
@@ -207,15 +207,15 @@
             model = models.DeleteNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteQueue(self, request):
         """本接口(DeleteQueue)用于从指定集群删除队列。
         * 本接口为目前只支持SchedulerType为SLURM的集群。
 
         * 删除队列时，需要保证队列内不存在节点。
@@ -233,15 +233,15 @@
             model = models.DeleteQueueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoScalingConfiguration(self, request):
         """本接口(DescribeAutoScalingConfiguration)用于查询集群弹性伸缩配置信息。本接口仅适用于弹性伸缩类型为THPC_AS的集群。
 
         :param request: Request instance for DescribeAutoScalingConfiguration.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeAutoScalingConfigurationRequest`
@@ -256,15 +256,15 @@
             model = models.DescribeAutoScalingConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterActivities(self, request):
         """本接口（DescribeClusterActivities）用于查询集群活动历史记录列表。
 
         :param request: Request instance for DescribeClusterActivities.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeClusterActivitiesRequest`
@@ -279,15 +279,15 @@
             model = models.DescribeClusterActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterStorageOption(self, request):
         """本接口 (DescribeClusterStorageOption) 用于查询集群存储选项信息。
 
         :param request: Request instance for DescribeClusterStorageOption.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeClusterStorageOptionRequest`
@@ -302,15 +302,15 @@
             model = models.DescribeClusterStorageOptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """本接口（DescribeClusters）用于查询集群列表。
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeClustersRequest`
@@ -325,15 +325,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeNodes(self, request):
         """本接口 (DescribeNodes) 用于查询指定集群节点概览信息列表。
 
         :param request: Request instance for DescribeNodes.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeNodesRequest`
@@ -348,15 +348,15 @@
             model = models.DescribeNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQueues(self, request):
         """本接口(DescribeQueues)用于查询指定集群队列概览信息列表。
 
         :param request: Request instance for DescribeQueues.
         :type request: :class:`tencentcloud.thpc.v20220401.models.DescribeQueuesRequest`
@@ -371,15 +371,15 @@
             model = models.DescribeQueuesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAutoScalingConfiguration(self, request):
         """本接口(SetAutoScalingConfiguration)用于为集群设置集群弹性伸缩配置信息。
 
         :param request: Request instance for SetAutoScalingConfiguration.
         :type request: :class:`tencentcloud.thpc.v20220401.models.SetAutoScalingConfigurationRequest`
@@ -394,8 +394,8 @@
             model = models.SetAutoScalingConfigurationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/README.rst` & `tencentcloud-sdk-python-thpc-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.937/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.938/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

