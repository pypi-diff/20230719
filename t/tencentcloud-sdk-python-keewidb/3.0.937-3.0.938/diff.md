# Comparing `tmp/tencentcloud-sdk-python-keewidb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-keewidb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.937.tar", last modified: Tue Jul 18 00:26:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.938.tar", last modified: Wed Jul 19 00:41:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-keewidb-3.0.937.tar` & `tencentcloud-sdk-python-keewidb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/
--rw-r--r--   0 root         (0) root         (0)    37283 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/keewidb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   218455 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:26:20.000000 tencentcloud-sdk-python-keewidb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/
+-rw-r--r--   0 root         (0) root         (0)    37435 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/keewidb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   219041 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:41:46.000000 tencentcloud-sdk-python-keewidb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/setup.py` & `tencentcloud-sdk-python-keewidb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/keewidb_client.py` & `tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/keewidb_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AssociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeInstanceMaster(self, request):
         """本接口（ChangeInstanceMaster）用于将副本节点提升为主节点。
 
         :param request: Request instance for ChangeInstanceMaster.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ChangeInstanceMasterRequest`
@@ -65,15 +65,15 @@
             model = models.ChangeInstanceMasterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CleanUpInstance(self, request):
         """本接口（CleanUpInstance）用于立即下线回收站已隔离的实例。
 
         :param request: Request instance for CleanUpInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.CleanUpInstanceRequest`
@@ -88,15 +88,15 @@
             model = models.CleanUpInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ClearInstance(self, request):
         """本接口（ClearInstance）用于清空实例数据。
 
         :param request: Request instance for ClearInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ClearInstanceRequest`
@@ -111,15 +111,15 @@
             model = models.ClearInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackupManually(self, request):
         """手动发起备份
 
         :param request: Request instance for CreateBackupManually.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.CreateBackupManuallyRequest`
@@ -134,15 +134,15 @@
             model = models.CreateBackupManuallyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstances(self, request):
         """创建数据库实例
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.CreateInstancesRequest`
@@ -157,15 +157,15 @@
             model = models.CreateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoBackupConfig(self, request):
         """本接口（DescribeAutoBackupConfig）用于获取自动备份配置。
 
         :param request: Request instance for DescribeAutoBackupConfig.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeAutoBackupConfigRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeAutoBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeConnectionConfig(self, request):
         """本接口（DescribeConnectionConfig）用于查询实例连接配置，包括出流量和入流量带宽、最大连接数限制。
 
         :param request: Request instance for DescribeConnectionConfig.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeConnectionConfigRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeConnectionConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSecurityGroups(self, request):
         """本接口(DescribeDBSecurityGroups)用于查询实例的安全组详情。
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeDBSecurityGroupsRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeDBSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceBackups(self, request):
         """本接口（DescribeInstanceBackups）用于查询实例全量备份列表。
 
         :param request: Request instance for DescribeInstanceBackups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceBackupsRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeInstanceBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceBinlogs(self, request):
         """本接口（DescribeInstanceBinlogs）用于查询增量备份列表。
 
         :param request: Request instance for DescribeInstanceBinlogs.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceBinlogsRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeInstanceBinlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceDealDetail(self, request):
         """本接口（DescribeInstanceDealDetail）用于查询预付费订单信息。
 
         :param request: Request instance for DescribeInstanceDealDetail.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceDealDetailRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeInstanceDealDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceNodeInfo(self, request):
         """本接口（DescribeInstanceNodeInfo）查询实例节点信息。
 
         :param request: Request instance for DescribeInstanceNodeInfo.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceNodeInfoRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeInstanceNodeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceParamRecords(self, request):
         """本接口（DescribeInstanceParamRecords）查询参数配置修改历史列表。
 
         :param request: Request instance for DescribeInstanceParamRecords.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceParamRecordsRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeInstanceParamRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceParams(self, request):
         """本接口（DescribeInstanceParams）用于查询实例的参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceParamsRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceReplicas(self, request):
         """本接口（DescribeInstanceReplicas）用于获取实例副本节点信息。
 
         :param request: Request instance for DescribeInstanceReplicas.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstanceReplicasRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeInstanceReplicasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口（DescribeInstances）可以根据地域、网络、实例id、标签、计费方式等条件，搜索查询实例列表。
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeInstancesRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMaintenanceWindow(self, request):
         """本接口（DescribeMaintenanceWindow）用于查询实例维护时间窗。
 
         :param request: Request instance for DescribeMaintenanceWindow.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeMaintenanceWindowRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeMaintenanceWindowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductInfo(self, request):
         """本接口查询指定可用区和实例类型下keewidb 的售卖规格， 如果用户不在购买白名单中，将不能查询该可用区或该类型的售卖规格详情。申请购买某地域白名单可以提交工单
 
         :param request: Request instance for DescribeProductInfo.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeProductInfoRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeProductInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectSecurityGroups(self, request):
         """本接口(DescribeProjectSecurityGroups)用于查询项目的安全组详情。
 
         :param request: Request instance for DescribeProjectSecurityGroups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeProjectSecurityGroupsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeProjectSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxySlowLog(self, request):
         """本接口（DescribeProxySlowLog）用于查询代理（Proxy）慢日志。
 
         :param request: Request instance for DescribeProxySlowLog.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeProxySlowLogRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeProxySlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInfo(self, request):
         """本接口（DescribeTaskInfo）用于查询异步任务结果。
 
         :param request: Request instance for DescribeTaskInfo.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeTaskInfoRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeTaskInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskList(self, request):
         """本接口（DescribeTaskList）用于查询任务列表信息。
 
         :param request: Request instance for DescribeTaskList.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeTaskListRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeTaskListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTendisSlowLog(self, request):
         """本接口（DescribeTendisSlowLog）用于查询实例慢日志。
 
         :param request: Request instance for DescribeTendisSlowLog.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeTendisSlowLogRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeTendisSlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyPostpaidInstance(self, request):
         """本接口（DestroyPostpaidInstance）用于退还按量计费实例。
 
         :param request: Request instance for DestroyPostpaidInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DestroyPostpaidInstanceRequest`
@@ -594,15 +594,15 @@
             model = models.DestroyPostpaidInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyPrepaidInstance(self, request):
         """本接口（DestroyPrepaidInstance）用于退还包年包月计费实例。
 
         :param request: Request instance for DestroyPrepaidInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DestroyPrepaidInstanceRequest`
@@ -617,15 +617,15 @@
             model = models.DestroyPrepaidInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateSecurityGroups(self, request):
         """本接口(DisassociateSecurityGroups)用于安全组批量解绑实例。
 
         :param request: Request instance for DisassociateSecurityGroups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DisassociateSecurityGroupsRequest`
@@ -640,15 +640,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAutoBackupConfig(self, request):
         """本接口（ModifyAutoBackupConfig）用于修改自动备份配置。
 
         :param request: Request instance for ModifyAutoBackupConfig.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyAutoBackupConfigRequest`
@@ -663,15 +663,15 @@
             model = models.ModifyAutoBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConnectionConfig(self, request):
         """本接口（ModifyConnectionConfig）用于修改实例的连接配置，包括带宽和最大连接数。
 
         :param request: Request instance for ModifyConnectionConfig.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyConnectionConfigRequest`
@@ -686,15 +686,15 @@
             model = models.ModifyConnectionConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSecurityGroups(self, request):
         """本接口(ModifyDBInstanceSecurityGroups)用于修改实例绑定的安全组。
 
         :param request: Request instance for ModifyDBInstanceSecurityGroups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -709,15 +709,15 @@
             model = models.ModifyDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstance(self, request):
         """本接口（ModifyInstance）用于修改实例相关信息。
 
         :param request: Request instance for ModifyInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyInstanceRequest`
@@ -732,15 +732,15 @@
             model = models.ModifyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceParams(self, request):
         """本接口（ModifyInstanceParams）用于修改实例参数配置。
 
         :param request: Request instance for ModifyInstanceParams.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyInstanceParamsRequest`
@@ -755,15 +755,15 @@
             model = models.ModifyInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMaintenanceWindow(self, request):
         """本接口（ModifyMaintenanceWindow）修改实例维护时间窗时间。
 
         :param request: Request instance for ModifyMaintenanceWindow.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyMaintenanceWindowRequest`
@@ -778,15 +778,15 @@
             model = models.ModifyMaintenanceWindowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyNetworkConfig(self, request):
         """本接口（ModifyNetworkConfig）用于修改实例网络配置。
 
         :param request: Request instance for ModifyNetworkConfig.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ModifyNetworkConfigRequest`
@@ -801,15 +801,15 @@
             model = models.ModifyNetworkConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstance(self, request):
         """本接口（RenewInstance）用于为包年包月计费实例续费。
 
         :param request: Request instance for RenewInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.RenewInstanceRequest`
@@ -824,15 +824,15 @@
             model = models.RenewInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetPassword(self, request):
         """本接口（ResetPassword）用于重置数据库访问密码。
 
         :param request: Request instance for ResetPassword.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.ResetPasswordRequest`
@@ -847,15 +847,15 @@
             model = models.ResetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartUpInstance(self, request):
         """本接口（StartUpInstance）用于按量计费实例解隔离
 
         :param request: Request instance for StartUpInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.StartUpInstanceRequest`
@@ -870,15 +870,15 @@
             model = models.StartUpInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeInstance(self, request):
         """本接口（UpgradeInstance）用于对实例进行配置变更。
 
         :param request: Request instance for UpgradeInstance.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.UpgradeInstanceRequest`
@@ -893,8 +893,8 @@
             model = models.UpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/errorcodes.py` & `tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/keewidb/v20220308/models.py` & `tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/keewidb/v20220308/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,16 +626,14 @@
         :type GoodsNum: int
         :param _Period: 选择包年包月计费模式（BillingMode 设置为1）时，您需要选择购买实例的时长。单位：月，取值范围 [1,2,3,4,5,6,7,8,9,10,11,12,24,36]。按量计费（BillingMode 设置为0）实例该参数设置为1即可。
         :type Period: int
         :param _ShardNum: 分片数量，支持选择3、5、6、8、9、10、12、15、16、18、20、21、24、25、27、30、32、33、35、36、39、40、42、45、48、50、51、54、55、56、57、60、63、64分片。
         :type ShardNum: int
         :param _ReplicasNum: 副本数。当前仅支持设置1个副本节点，即每一个分片仅包含1个主节点与1个副本节点，数据主从实时热备。
         :type ReplicasNum: int
-        :param _MachineCpu: 计算cpu核心数。
-        :type MachineCpu: int
         :param _MachineMemory: 实例内存容量，单位：GB。
 KeeWiDB 内存容量<b>MachineMemory</b>与持久内存容量<b>MemSize</b>为固定搭配，即2GB内存，固定分配8GB的持久内存，不可选择。具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。
         :type MachineMemory: int
         :param _ZoneId: 实例所属的可用区ID。<ul><li>具体取值，请参见[地域和可用区](https://cloud.tencent.com/document/product/239/4106)获取。</li><li>参数<b>ZoneId</b>和<b>ZoneName</b>至少配置其中一个。</li></u>
         :type ZoneId: int
         :param _ZoneName: 实例所属的可用区名称。<ul><li>具体取值，请参见[地域和可用区](https://cloud.tencent.com/document/product/239/4106)获取。</li><li>参数<b>ZoneId</b>和<b>ZoneName</b>至少配置其中一个。</li></u>
         :type ZoneName: str
@@ -657,39 +655,44 @@
         :type ResourceTags: list of ResourceTag
         :param _MemSize: 混合存储版，单分片持久化内存容量，单位：GB。
 KeeWiDB 内存容量<b>MachineMemory</b>与持久内存容量<b>MemSize</b>为固定搭配，即2GB内存，固定分配8GB的持久内存，不可选择。具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。
         :type MemSize: int
         :param _DiskSize: 每个分片硬盘的容量。单位：GB。
 每一缓存分片容量，对应的磁盘容量范围不同。具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。
         :type DiskSize: int
+        :param _MachineCpu: 计算 CPU 核数，可忽略不传。CPU 核数与内存为固定搭配，具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。
+        :type MachineCpu: int
         :param _ProjectId: 项目id，取值以用户账户>用户账户相关接口查询>项目列表返回的projectId为准。
         :type ProjectId: int
+        :param _Compression: 数据压缩开关。<ul><li>ON：开启，默认开启压缩。</li><li>OFF：关闭。</li>
+        :type Compression: str
         """
         self._TypeId = None
         self._UniqVpcId = None
         self._UniqSubnetId = None
         self._BillingMode = None
         self._GoodsNum = None
         self._Period = None
         self._ShardNum = None
         self._ReplicasNum = None
-        self._MachineCpu = None
         self._MachineMemory = None
         self._ZoneId = None
         self._ZoneName = None
         self._InstanceName = None
         self._NoAuth = None
         self._Password = None
         self._VPort = None
         self._AutoRenew = None
         self._SecurityGroupIdList = None
         self._ResourceTags = None
         self._MemSize = None
         self._DiskSize = None
+        self._MachineCpu = None
         self._ProjectId = None
+        self._Compression = None
 
     @property
     def TypeId(self):
         return self._TypeId
 
     @TypeId.setter
     def TypeId(self, TypeId):
@@ -748,22 +751,14 @@
         return self._ReplicasNum
 
     @ReplicasNum.setter
     def ReplicasNum(self, ReplicasNum):
         self._ReplicasNum = ReplicasNum
 
     @property
-    def MachineCpu(self):
-        return self._MachineCpu
-
-    @MachineCpu.setter
-    def MachineCpu(self, MachineCpu):
-        self._MachineCpu = MachineCpu
-
-    @property
     def MachineMemory(self):
         return self._MachineMemory
 
     @MachineMemory.setter
     def MachineMemory(self, MachineMemory):
         self._MachineMemory = MachineMemory
 
@@ -852,32 +847,47 @@
         return self._DiskSize
 
     @DiskSize.setter
     def DiskSize(self, DiskSize):
         self._DiskSize = DiskSize
 
     @property
+    def MachineCpu(self):
+        return self._MachineCpu
+
+    @MachineCpu.setter
+    def MachineCpu(self, MachineCpu):
+        self._MachineCpu = MachineCpu
+
+    @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
         self._ProjectId = ProjectId
 
+    @property
+    def Compression(self):
+        return self._Compression
+
+    @Compression.setter
+    def Compression(self, Compression):
+        self._Compression = Compression
+
 
     def _deserialize(self, params):
         self._TypeId = params.get("TypeId")
         self._UniqVpcId = params.get("UniqVpcId")
         self._UniqSubnetId = params.get("UniqSubnetId")
         self._BillingMode = params.get("BillingMode")
         self._GoodsNum = params.get("GoodsNum")
         self._Period = params.get("Period")
         self._ShardNum = params.get("ShardNum")
         self._ReplicasNum = params.get("ReplicasNum")
-        self._MachineCpu = params.get("MachineCpu")
         self._MachineMemory = params.get("MachineMemory")
         self._ZoneId = params.get("ZoneId")
         self._ZoneName = params.get("ZoneName")
         self._InstanceName = params.get("InstanceName")
         self._NoAuth = params.get("NoAuth")
         self._Password = params.get("Password")
         self._VPort = params.get("VPort")
@@ -887,15 +897,17 @@
             self._ResourceTags = []
             for item in params.get("ResourceTags"):
                 obj = ResourceTag()
                 obj._deserialize(item)
                 self._ResourceTags.append(obj)
         self._MemSize = params.get("MemSize")
         self._DiskSize = params.get("DiskSize")
+        self._MachineCpu = params.get("MachineCpu")
         self._ProjectId = params.get("ProjectId")
+        self._Compression = params.get("Compression")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7384,15 +7396,15 @@
     def __init__(self):
         r"""
         :param _InstanceId: 实例 ID。
         :type InstanceId: str
         :param _MemSize: 配置变更后，每个分片持久化内存容量，单位：GB。
 <ul><li>KeeWiDB 内存容量<b>MachineMemory</b>与持久内存容量<b>MemSize</b>为固定搭配，即2GB内存，固定分配8GB的持久内存，不可选择。具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。</li><li>变更实例内存、持久化内存与磁盘、变更实例的分片数量，每次只能变更一项。</li></ul>
         :type MemSize: int
-        :param _MachineCpu: CPU 核数。
+        :param _MachineCpu: CPU 核数，可忽略不传
         :type MachineCpu: int
         :param _MachineMemory: 实例内存容量，单位：GB。
 <ul><li>KeeWiDB 内存容量<b>MachineMemory</b>与持久内存容量<b>MemSize</b>为固定搭配，即2GB内存，固定分配8GB的持久内存，不可选择。具体信息，请参见[产品规格](https://cloud.tencent.com/document/product/1520/80808)。</li><li>变更实例内存、持久化内存与磁盘、变更实例的分片数量，每次只能变更一项。</li></ul>
         :type MachineMemory: int
         :param _ShardNum: 配置变更后，分片数量。
 <ul><li>增加后分片的数量务必为增加之前数量的整数倍。分片数量支持选择3、5、6、8、9、10、12、15、16、18、20、21、24、25、27、30、32、33、35、36、39、40、42、45、48、50、51、54、55、56、57、60、63、64分片。</li><li>变更实例内存、持久化内存与磁盘、变更实例的分片数量，每次只能变更一项。</li></ul>
         :type ShardNum: int
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-keewidb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.937/README.rst` & `tencentcloud-sdk-python-keewidb-3.0.938/README.rst`

 * *Files identical despite different names*

