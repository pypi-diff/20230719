# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.937.tar", last modified: Tue Jul 18 00:27:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.938.tar", last modified: Wed Jul 19 00:42:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.937.tar` & `tencentcloud-sdk-python-mongodb-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)    36443 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   235050 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    13571 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    76740 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:28.000000 tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)    36587 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   235050 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    13623 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    76740 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:51.000000 tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AssignProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccountUser(self, request):
         """本接口（CreateAccountUser）用于自定义实例访问账号。
 
         :param request: Request instance for CreateAccountUser.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateAccountUserRequest`
@@ -65,15 +65,15 @@
             model = models.CreateAccountUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackupDBInstance(self, request):
         """本接口（CreateBackupDBInstance）用于备份实例。
 
         :param request: Request instance for CreateBackupDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateBackupDBInstanceRequest`
@@ -88,15 +88,15 @@
             model = models.CreateBackupDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackupDownloadTask(self, request):
         """本接口用来创建某个备份文件的下载任务
 
         :param request: Request instance for CreateBackupDownloadTask.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateBackupDownloadTaskRequest`
@@ -111,15 +111,15 @@
             model = models.CreateBackupDownloadTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstance(self, request):
         """本接口(CreateDBInstance)用于创建包年包月的MongoDB云数据库实例。接口支持的售卖规格，可从查询云数据库的售卖规格（DescribeSpecInfo）获取。
 
         :param request: Request instance for CreateDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateDBInstanceRequest`
@@ -134,15 +134,15 @@
             model = models.CreateDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstanceHour(self, request):
         """本接口（CreateDBInstanceHour）用于创建按量计费的MongoDB云数据库实例。
 
         :param request: Request instance for CreateDBInstanceHour.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateDBInstanceHourRequest`
@@ -157,15 +157,15 @@
             model = models.CreateDBInstanceHourResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccountUser(self, request):
         """本接口（DeleteAccountUser）用于删除实例的自定义账号。
 
         :param request: Request instance for DeleteAccountUser.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DeleteAccountUserRequest`
@@ -180,15 +180,15 @@
             model = models.DeleteAccountUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountUsers(self, request):
         """本接口（DescribeAccountUsers）用于获取当前实例的全部账号。
 
         :param request: Request instance for DescribeAccountUsers.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeAccountUsersRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeAccountUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAsyncRequestInfo(self, request):
         """查询异步任务状态接口
 
         :param request: Request instance for DescribeAsyncRequestInfo.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeAsyncRequestInfoRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeAsyncRequestInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupDownloadTask(self, request):
         """查询备份下载任务信息
 
         :param request: Request instance for DescribeBackupDownloadTask.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeBackupDownloadTaskRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeBackupDownloadTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClientConnections(self, request):
         """本接口（DescribeClientConnections）用于查询实例客户端连接信息，包括连接 IP 和连接数量。
 
         :param request: Request instance for DescribeClientConnections.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeClientConnectionsRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeClientConnectionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCurrentOp(self, request):
         """本接口(DescribeCurrentOp)用于查询MongoDB云数据库实例的当前正在执行的操作。
 
         :param request: Request instance for DescribeCurrentOp.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeCurrentOpRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeCurrentOpResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBBackups(self, request):
         """本接口（DescribeDBBackups）用于查询实例备份列表，目前只支持查询7天内的备份记录。
 
         :param request: Request instance for DescribeDBBackups.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeDBBackupsRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeDBBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceDeal(self, request):
         """本接口（DescribeDBInstanceDeal）用于获取MongoDB购买、续费及变配订单详细。
 
         :param request: Request instance for DescribeDBInstanceDeal.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeDBInstanceDealRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeDBInstanceDealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceNodeProperty(self, request):
         """本接口用于查询节点的属性，包括节点所在可用区、节点名称、地址、角色、状态、主从延迟、优先级、投票权、标签等属性。
 
         :param request: Request instance for DescribeDBInstanceNodeProperty.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeDBInstanceNodePropertyRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeDBInstanceNodePropertyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstances(self, request):
         """本接口（DescribeDBInstances）用于查询云数据库实例列表，支持通过项目ID、实例ID、实例状态等过滤条件来筛选主实例、灾备实例和只读实例信息列表。
 
         :param request: Request instance for DescribeDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeDBInstancesRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceParams(self, request):
         """本接口（DescribeInstanceParams）用于查询当前实例可修改的参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeInstanceParamsRequest`
@@ -410,15 +410,15 @@
             model = models.DescribeInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSecurityGroup(self, request):
         """本接口（DescribeSecurityGroup）用于查询实例绑定的安全组。
 
         :param request: Request instance for DescribeSecurityGroup.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeSecurityGroupRequest`
@@ -433,15 +433,15 @@
             model = models.DescribeSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogPatterns(self, request):
         """本接口（DescribeSlowLogPatterns）用于获取数据库实例慢日志的统计信息。
 
         :param request: Request instance for DescribeSlowLogPatterns.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeSlowLogPatternsRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeSlowLogPatternsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLogs(self, request):
         """本接口（DescribeSlowLogs）用于获取云数据库慢日志信息。接口只支持查询最近7天内慢日志。
 
         :param request: Request instance for DescribeSlowLogs.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeSlowLogsRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeSlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSpecInfo(self, request):
         """本接口(DescribeSpecInfo)用于查询实例的售卖规格。
 
         :param request: Request instance for DescribeSpecInfo.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeSpecInfoRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeSpecInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FlushInstanceRouterConfig(self, request):
         """在所有mongos上执行FlushRouterConfig命令
 
         :param request: Request instance for FlushInstanceRouterConfig.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.FlushInstanceRouterConfigRequest`
@@ -525,15 +525,15 @@
             model = models.FlushInstanceRouterConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreateDBInstances(self, request):
         """本接口（InquirePriceCreateDBInstances）用于创建数据库实例询价。本接口参数中必须传入region参数，否则无法通过校验。本接口仅允许针对购买限制范围内的实例配置进行询价。
 
         :param request: Request instance for InquirePriceCreateDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.InquirePriceCreateDBInstancesRequest`
@@ -548,15 +548,15 @@
             model = models.InquirePriceCreateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceModifyDBInstanceSpec(self, request):
         """本接口 (InquirePriceModifyDBInstanceSpec) 用于查询实例配置变更后的价格。
 
         :param request: Request instance for InquirePriceModifyDBInstanceSpec.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.InquirePriceModifyDBInstanceSpecRequest`
@@ -571,15 +571,15 @@
             model = models.InquirePriceModifyDBInstanceSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceRenewDBInstances(self, request):
         """本接口 (InquiryPriceRenewDBInstances) 用于续费包年包月实例询价。
 
         :param request: Request instance for InquirePriceRenewDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.InquirePriceRenewDBInstancesRequest`
@@ -594,15 +594,15 @@
             model = models.InquirePriceRenewDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDBInstance(self, request):
         """本接口(IsolateDBInstance)用于隔离MongoDB云数据库按量计费实例。隔离后实例保留在回收站中，不能再写入数据。隔离一定时间后，实例会彻底删除，回收站保存时间请参考按量计费的服务条款。在隔离中的按量计费实例无法恢复，请谨慎操作。
 
         :param request: Request instance for IsolateDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.IsolateDBInstanceRequest`
@@ -617,15 +617,15 @@
             model = models.IsolateDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KillOps(self, request):
         """本接口(KillOps)用于终止MongoDB云数据库实例上执行的特定操作。
 
         :param request: Request instance for KillOps.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.KillOpsRequest`
@@ -640,15 +640,15 @@
             model = models.KillOpsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceNetworkAddress(self, request):
         """本接口(ModifyDBInstanceNetworkAddress)用于修改云数据库实例的网络信息，可进行基础网络转VPC网络和VPC网络之间的变换。
 
         :param request: Request instance for ModifyDBInstanceNetworkAddress.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.ModifyDBInstanceNetworkAddressRequest`
@@ -663,15 +663,15 @@
             model = models.ModifyDBInstanceNetworkAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSecurityGroup(self, request):
         """本接口（ModifyDBInstanceSecurityGroup）用于修改实例绑定的安全组
 
         :param request: Request instance for ModifyDBInstanceSecurityGroup.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.ModifyDBInstanceSecurityGroupRequest`
@@ -686,15 +686,15 @@
             model = models.ModifyDBInstanceSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSpec(self, request):
         """本接口(ModifyDBInstanceSpec)用于调整MongoDB云数据库实例配置。接口支持的售卖规格，可从查询云数据库的售卖规格（DescribeSpecInfo）获取。
 
         :param request: Request instance for ModifyDBInstanceSpec.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.ModifyDBInstanceSpecRequest`
@@ -709,15 +709,15 @@
             model = models.ModifyDBInstanceSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OfflineIsolatedDBInstance(self, request):
         """本接口(OfflineIsolatedDBInstance)用于立即下线隔离状态的云数据库实例。进行操作的实例状态必须为隔离状态。
 
         :param request: Request instance for OfflineIsolatedDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.OfflineIsolatedDBInstanceRequest`
@@ -732,15 +732,15 @@
             model = models.OfflineIsolatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenameInstance(self, request):
         """本接口(RenameInstance)用于修改云数据库实例的名称。
 
         :param request: Request instance for RenameInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.RenameInstanceRequest`
@@ -755,15 +755,15 @@
             model = models.RenameInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDBInstances(self, request):
         """本接口(RenewDBInstance)用于续费云数据库实例，仅支持付费模式为包年包月的实例。按量计费实例不需要续费。
 
         :param request: Request instance for RenewDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.RenewDBInstancesRequest`
@@ -778,15 +778,15 @@
             model = models.RenewDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetDBInstancePassword(self, request):
         """修改实例用户的密码
 
         :param request: Request instance for ResetDBInstancePassword.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.ResetDBInstancePasswordRequest`
@@ -801,15 +801,15 @@
             model = models.ResetDBInstancePasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAccountUserPrivilege(self, request):
         """本接口（SetAccountUserPrivilege）用于设置实例的账号权限。
 
         :param request: Request instance for SetAccountUserPrivilege.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.SetAccountUserPrivilegeRequest`
@@ -824,15 +824,15 @@
             model = models.SetAccountUserPrivilegeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDBInstances(self, request):
         """本接口（TerminateDBInstances）可将包年包月实例退还隔离。
 
         :param request: Request instance for TerminateDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.TerminateDBInstancesRequest`
@@ -847,8 +847,8 @@
             model = models.TerminateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20190725/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.AssignProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstance(self, request):
         """本接口(CreateDBInstance)用于创建包年包月的MongoDB云数据库实例。
 
         :param request: Request instance for CreateDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.CreateDBInstanceRequest`
@@ -66,15 +66,15 @@
             model = models.CreateDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstanceHour(self, request):
         """本接口(CreateDBInstanceHour)用于创建按量计费的MongoDB云数据库实例（包括主实例、灾备实例和只读实例），可通过传入实例规格、实例类型、MongoDB版本、购买时长和数量等信息创建云数据库实例。
 
         :param request: Request instance for CreateDBInstanceHour.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.CreateDBInstanceHourRequest`
@@ -89,15 +89,15 @@
             model = models.CreateDBInstanceHourResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClientConnections(self, request):
         """本接口(DescribeClientConnections)用于查询实例客户端连接信息，包括连接IP和连接数量。目前只支持3.2版本的MongoDB实例。
 
         :param request: Request instance for DescribeClientConnections.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.DescribeClientConnectionsRequest`
@@ -112,15 +112,15 @@
             model = models.DescribeClientConnectionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstances(self, request):
         """本接口(DescribeDBInstances)用于查询云数据库实例列表，支持通过项目ID、实例ID、实例状态等过滤条件来筛选实例。支持查询主实例、灾备实例和只读实例信息列表。
 
         :param request: Request instance for DescribeDBInstances.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.DescribeDBInstancesRequest`
@@ -135,15 +135,15 @@
             model = models.DescribeDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLog(self, request):
         """本接口(DescribeSlowLogs)用于获取云数据库实例的慢查询日志。
 
         :param request: Request instance for DescribeSlowLog.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.DescribeSlowLogRequest`
@@ -158,15 +158,15 @@
             model = models.DescribeSlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSpecInfo(self, request):
         """本接口(DescribeSpecInfo)用于查询实例的售卖规格。
 
         :param request: Request instance for DescribeSpecInfo.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.DescribeSpecInfoRequest`
@@ -181,15 +181,15 @@
             model = models.DescribeSpecInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenameInstance(self, request):
         """本接口(RenameInstance)用于修改云数据库实例的名称。
 
         :param request: Request instance for RenameInstance.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.RenameInstanceRequest`
@@ -204,15 +204,15 @@
             model = models.RenameInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAutoRenew(self, request):
         """本接口(SetAutoRenew)用于设置包年包月云数据库实例的续费选项。
 
         :param request: Request instance for SetAutoRenew.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.SetAutoRenewRequest`
@@ -227,15 +227,15 @@
             model = models.SetAutoRenewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetPassword(self, request):
         """本接口(SetPassword)用于设置云数据库账户的密码。
 
 
         :param request: Request instance for SetPassword.
@@ -251,15 +251,15 @@
             model = models.SetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDBInstance(self, request):
         """本接口(TerminateDBInstance)用于销毁按量计费的MongoDB云数据库实例
 
         :param request: Request instance for TerminateDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.TerminateDBInstanceRequest`
@@ -274,15 +274,15 @@
             model = models.TerminateDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDBInstance(self, request):
         """本接口(UpgradeDBInstance)用于升级包年包月的MongoDB云数据库实例，可以扩容内存、存储以及Oplog
 
         :param request: Request instance for UpgradeDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.UpgradeDBInstanceRequest`
@@ -297,15 +297,15 @@
             model = models.UpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDBInstanceHour(self, request):
         """本接口(UpgradeDBInstanceHour)用于升级按量计费的MongoDB云数据库实例，可以扩容内存、存储以及oplog
 
         :param request: Request instance for UpgradeDBInstanceHour.
         :type request: :class:`tencentcloud.mongodb.v20180408.models.UpgradeDBInstanceHourRequest`
@@ -320,8 +320,8 @@
             model = models.UpgradeDBInstanceHourResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.937/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.938/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

