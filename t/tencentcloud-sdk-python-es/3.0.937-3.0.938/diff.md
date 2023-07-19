# Comparing `tmp/tencentcloud-sdk-python-es-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-es-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.937.tar", last modified: Tue Jul 18 00:23:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.938.tar", last modified: Wed Jul 19 00:38:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-es-3.0.937.tar` & `tencentcloud-sdk-python-es-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35974 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/es_client.py
--rw-r--r--   0 root         (0) root         (0)   293112 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:23:42.000000 tencentcloud-sdk-python-es-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    36126 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)   293112 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:38:56.000000 tencentcloud-sdk-python-es-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-es-3.0.937/tencentcloud_sdk_python_es.egg-info/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.938/tencentcloud_sdk_python_es.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.937/setup.py` & `tencentcloud-sdk-python-es-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-es-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/es_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstance(self, request):
         """创建指定规格的ES集群实例
 
         :param request: Request instance for CreateInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.CreateInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.CreateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateLogstashInstance(self, request):
         """用于创建Logstash实例
 
         :param request: Request instance for CreateLogstashInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.CreateLogstashInstanceRequest`
@@ -88,15 +88,15 @@
             model = models.CreateLogstashInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIndex(self, request):
         """删除索引
 
         :param request: Request instance for DeleteIndex.
         :type request: :class:`tencentcloud.es.v20180416.models.DeleteIndexRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstance(self, request):
         """销毁集群实例
 
         :param request: Request instance for DeleteInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.DeleteInstanceRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLogstashInstance(self, request):
         """用于删除Logstash实例
 
         :param request: Request instance for DeleteLogstashInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.DeleteLogstashInstanceRequest`
@@ -157,15 +157,15 @@
             model = models.DeleteLogstashInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLogstashPipelines(self, request):
         """用于批量删除Logstash管道
 
         :param request: Request instance for DeleteLogstashPipelines.
         :type request: :class:`tencentcloud.es.v20180416.models.DeleteLogstashPipelinesRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteLogstashPipelinesResponse()
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
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeIndexListRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeIndexListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIndexMeta(self, request):
         """获取索引元数据
 
         :param request: Request instance for DescribeIndexMeta.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeIndexMetaRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeIndexMetaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLogs(self, request):
         """查询用户该地域下符合条件的ES集群的日志
 
         :param request: Request instance for DescribeInstanceLogs.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeInstanceLogsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeInstanceLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceOperations(self, request):
         """查询实例指定条件下的操作记录
 
         :param request: Request instance for DescribeInstanceOperations.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeInstanceOperationsRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeInstanceOperationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """查询用户该地域下符合条件的所有实例
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeInstancesRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogstashInstanceLogs(self, request):
         """查询用户该地域下符合条件的Logstash实例的日志
 
         :param request: Request instance for DescribeLogstashInstanceLogs.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeLogstashInstanceLogsRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeLogstashInstanceLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogstashInstanceOperations(self, request):
         """查询实例指定条件下的操作记录
 
         :param request: Request instance for DescribeLogstashInstanceOperations.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeLogstashInstanceOperationsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeLogstashInstanceOperationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogstashInstances(self, request):
         """查询用户该地域下符合条件的所有Logstash实例
 
         :param request: Request instance for DescribeLogstashInstances.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeLogstashInstancesRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeLogstashInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogstashPipelines(self, request):
         """用于获取Logstash实例管道列表
 
         :param request: Request instance for DescribeLogstashPipelines.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeLogstashPipelinesRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeLogstashPipelinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeViews(self, request):
         """查询集群各视图数据，包括集群维度、节点维度、Kibana维度
 
         :param request: Request instance for DescribeViews.
         :type request: :class:`tencentcloud.es.v20180416.models.DescribeViewsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeViewsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DiagnoseInstance(self, request):
         """智能运维诊断集群
 
         :param request: Request instance for DiagnoseInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.DiagnoseInstanceRequest`
@@ -433,15 +433,15 @@
             model = models.DiagnoseInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRequestTargetNodeTypes(self, request):
         """获取接收客户端请求的节点类型
 
         :param request: Request instance for GetRequestTargetNodeTypes.
         :type request: :class:`tencentcloud.es.v20180416.models.GetRequestTargetNodeTypesRequest`
@@ -456,15 +456,15 @@
             model = models.GetRequestTargetNodeTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyEsVipSecurityGroup(self, request):
         """修改绑定VIP的安全组，传安全组id列表
 
         :param request: Request instance for ModifyEsVipSecurityGroup.
         :type request: :class:`tencentcloud.es.v20180416.models.ModifyEsVipSecurityGroupRequest`
@@ -479,15 +479,15 @@
             model = models.ModifyEsVipSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartInstance(self, request):
         """重启ES集群实例(用于系统版本更新等操作)
 
         :param request: Request instance for RestartInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.RestartInstanceRequest`
@@ -502,15 +502,15 @@
             model = models.RestartInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartKibana(self, request):
         """重启Kibana
 
         :param request: Request instance for RestartKibana.
         :type request: :class:`tencentcloud.es.v20180416.models.RestartKibanaRequest`
@@ -525,15 +525,15 @@
             model = models.RestartKibanaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartLogstashInstance(self, request):
         """用于重启Logstash实例
 
         :param request: Request instance for RestartLogstashInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.RestartLogstashInstanceRequest`
@@ -548,15 +548,15 @@
             model = models.RestartLogstashInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartNodes(self, request):
         """用于重启集群节点
 
         :param request: Request instance for RestartNodes.
         :type request: :class:`tencentcloud.es.v20180416.models.RestartNodesRequest`
@@ -571,15 +571,15 @@
             model = models.RestartNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SaveAndDeployLogstashPipeline(self, request):
         """用于下发并且部署管道
 
         :param request: Request instance for SaveAndDeployLogstashPipeline.
         :type request: :class:`tencentcloud.es.v20180416.models.SaveAndDeployLogstashPipelineRequest`
@@ -594,15 +594,15 @@
             model = models.SaveAndDeployLogstashPipelineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartLogstashPipelines(self, request):
         """用于启动Logstash管道
 
         :param request: Request instance for StartLogstashPipelines.
         :type request: :class:`tencentcloud.es.v20180416.models.StartLogstashPipelinesRequest`
@@ -617,15 +617,15 @@
             model = models.StartLogstashPipelinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopLogstashPipelines(self, request):
         """用于批量停止Logstash管道
 
         :param request: Request instance for StopLogstashPipelines.
         :type request: :class:`tencentcloud.es.v20180416.models.StopLogstashPipelinesRequest`
@@ -640,15 +640,15 @@
             model = models.StopLogstashPipelinesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDiagnoseSettings(self, request):
         """更新智能运维配置
 
         :param request: Request instance for UpdateDiagnoseSettings.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateDiagnoseSettingsRequest`
@@ -663,15 +663,15 @@
             model = models.UpdateDiagnoseSettingsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateDictionaries(self, request):
         """更新ES集群词典
 
         :param request: Request instance for UpdateDictionaries.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateDictionariesRequest`
@@ -686,15 +686,15 @@
             model = models.UpdateDictionariesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateIndex(self, request):
         """更新索引
 
         :param request: Request instance for UpdateIndex.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateIndexRequest`
@@ -709,15 +709,15 @@
             model = models.UpdateIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateInstance(self, request):
         """对集群进行节点规格变更，修改实例名称，修改配置，重置密码， 添加Kibana黑白名单等操作。参数中InstanceId为必传参数，ForceRestart为选填参数，剩余参数传递组合及含义如下：
         - InstanceName：修改实例名称(仅用于标识实例)
         - NodeInfoList: 修改节点配置（节点横向扩缩容，纵向扩缩容，增加主节点，增加冷节点等）
         - EsConfig：修改集群配置
@@ -739,15 +739,15 @@
             model = models.UpdateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateJdk(self, request):
         """更新实例Jdk配置
 
         :param request: Request instance for UpdateJdk.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateJdkRequest`
@@ -762,15 +762,15 @@
             model = models.UpdateJdkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateLogstashInstance(self, request):
         """对集群进行节点规格变更，修改实例名称，修改配置，等操作。参数中InstanceId为必传参数，参数传递组合及含义如下：
         - InstanceName：修改实例名称(仅用于标识实例)
         - NodeNum: 修改实例节点数量（节点横向扩缩容，纵向扩缩容等）
         - YMLConfig: 修改实例YML配置
@@ -790,15 +790,15 @@
             model = models.UpdateLogstashInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateLogstashPipelineDesc(self, request):
         """用于更新管道描述信息
 
         :param request: Request instance for UpdateLogstashPipelineDesc.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateLogstashPipelineDescRequest`
@@ -813,15 +813,15 @@
             model = models.UpdateLogstashPipelineDescResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdatePlugins(self, request):
         """变更插件列表
 
         :param request: Request instance for UpdatePlugins.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdatePluginsRequest`
@@ -836,15 +836,15 @@
             model = models.UpdatePluginsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRequestTargetNodeTypes(self, request):
         """更新接收客户端请求的节点类型
 
         :param request: Request instance for UpdateRequestTargetNodeTypes.
         :type request: :class:`tencentcloud.es.v20180416.models.UpdateRequestTargetNodeTypesRequest`
@@ -859,15 +859,15 @@
             model = models.UpdateRequestTargetNodeTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeInstance(self, request):
         """升级ES集群版本
 
         :param request: Request instance for UpgradeInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.UpgradeInstanceRequest`
@@ -882,15 +882,15 @@
             model = models.UpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeLicense(self, request):
         """升级ES商业特性
 
         :param request: Request instance for UpgradeLicense.
         :type request: :class:`tencentcloud.es.v20180416.models.UpgradeLicenseRequest`
@@ -905,8 +905,8 @@
             model = models.UpgradeLicenseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-es-3.0.937/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-es-3.0.938/tencentcloud/es/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.937/README.rst` & `tencentcloud-sdk-python-es-3.0.938/README.rst`

 * *Files identical despite different names*

