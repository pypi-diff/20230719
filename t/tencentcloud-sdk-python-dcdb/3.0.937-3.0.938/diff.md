# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.937.tar", last modified: Tue Jul 18 00:22:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.938.tar", last modified: Wed Jul 19 00:37:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.937.tar` & `tencentcloud-sdk-python-dcdb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72082 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)    14052 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   401661 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:22:24.000000 tencentcloud-sdk-python-dcdb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72374 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14052 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   401661 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:37:40.000000 tencentcloud-sdk-python-dcdb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ActiveHourDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSecurityGroups(self, request):
         """本接口 (AssociateSecurityGroups) 用于安全组批量绑定云资源。
 
         :param request: Request instance for AssociateSecurityGroups.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.AssociateSecurityGroupsRequest`
@@ -65,15 +65,15 @@
             model = models.AssociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelDcnJob(self, request):
         """取消DCN同步
 
         :param request: Request instance for CancelDcnJob.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CancelDcnJobRequest`
@@ -88,15 +88,15 @@
             model = models.CancelDcnJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloneAccount(self, request):
         """本接口（CloneAccount）用于克隆实例账户。
 
         :param request: Request instance for CloneAccount.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CloneAccountRequest`
@@ -111,15 +111,15 @@
             model = models.CloneAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseDBExtranetAccess(self, request):
         """本接口(CloseDBExtranetAccess)用于关闭云数据库实例的外网访问。关闭外网访问后，外网地址将不可访问，查询实例列表接口将不返回对应实例的外网域名和端口信息。
 
         :param request: Request instance for CloseDBExtranetAccess.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CloseDBExtranetAccessRequest`
@@ -134,15 +134,15 @@
             model = models.CloseDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyAccountPrivileges(self, request):
         """本接口（CopyAccountPrivileges）用于复制云数据库账号的权限。
         注意：相同用户名，不同Host是不同的账号，Readonly属性相同的账号之间才能复制权限。
 
         :param request: Request instance for CopyAccountPrivileges.
@@ -158,15 +158,15 @@
             model = models.CopyAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccount(self, request):
         """本接口（CreateAccount）用于创建云数据库账号。一个实例可以创建多个不同的账号，相同的用户名+不同的host是不同的账号。
 
         :param request: Request instance for CreateAccount.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateAccountRequest`
@@ -181,15 +181,15 @@
             model = models.CreateAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDCDBInstance(self, request):
         """本接口（CreateDCDBInstance）用于创建包年包月的TDSQL实例，可通过传入实例规格、数据库版本号、购买时长等信息创建云数据库实例。
 
         :param request: Request instance for CreateDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateDCDBInstanceRequest`
@@ -204,15 +204,15 @@
             model = models.CreateDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDedicatedClusterDCDBInstance(self, request):
         """创建TDSQL独享集群实例
 
         :param request: Request instance for CreateDedicatedClusterDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateDedicatedClusterDCDBInstanceRequest`
@@ -227,15 +227,15 @@
             model = models.CreateDedicatedClusterDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHourDCDBInstance(self, request):
         """创建TDSQL按量计费实例
 
         :param request: Request instance for CreateHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateHourDCDBInstanceRequest`
@@ -250,15 +250,15 @@
             model = models.CreateHourDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTmpDCDBInstance(self, request):
         """回档TDSQL实例
 
         :param request: Request instance for CreateTmpDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateTmpDCDBInstanceRequest`
@@ -273,15 +273,15 @@
             model = models.CreateTmpDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccount(self, request):
         """本接口（DeleteAccount）用于删除云数据库账号。用户名+host唯一确定一个账号。
 
         :param request: Request instance for DeleteAccount.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DeleteAccountRequest`
@@ -296,15 +296,15 @@
             model = models.DeleteAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountPrivileges(self, request):
         """本接口（DescribeAccountPrivileges）用于查询云数据库账号权限。
         注意：注意：相同用户名，不同Host是不同的账号。
 
         :param request: Request instance for DescribeAccountPrivileges.
@@ -320,15 +320,15 @@
             model = models.DescribeAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """本接口（DescribeAccounts）用于查询指定云数据库实例的账号列表。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeAccountsRequest`
@@ -343,15 +343,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupFiles(self, request):
         """本接口(DescribeBackupFiles)用于查看备份文件列表。
 
         :param request: Request instance for DescribeBackupFiles.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeBackupFilesRequest`
@@ -366,15 +366,15 @@
             model = models.DescribeBackupFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBEncryptAttributes(self, request):
         """本接口(DescribeDBEncryptAttributes)用于查询实例数据加密状态。
 
         :param request: Request instance for DescribeDBEncryptAttributes.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBEncryptAttributesRequest`
@@ -389,15 +389,15 @@
             model = models.DescribeDBEncryptAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBLogFiles(self, request):
         """本接口(DescribeDBLogFiles)用于获取数据库的各种日志列表，包括冷备、binlog、errlog和slowlog。
 
         :param request: Request instance for DescribeDBLogFiles.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBLogFilesRequest`
@@ -412,15 +412,15 @@
             model = models.DescribeDBLogFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBParameters(self, request):
         """本接口(DescribeDBParameters)用于获取数据库的当前参数设置。
 
         :param request: Request instance for DescribeDBParameters.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBParametersRequest`
@@ -435,15 +435,15 @@
             model = models.DescribeDBParametersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSecurityGroups(self, request):
         """本接口（DescribeDBSecurityGroups）用于查询实例安全组信息
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBSecurityGroupsRequest`
@@ -458,15 +458,15 @@
             model = models.DescribeDBSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSlowLogs(self, request):
         """本接口(DescribeDBSlowLogs)用于查询慢查询日志列表。
 
         :param request: Request instance for DescribeDBSlowLogs.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBSlowLogsRequest`
@@ -481,15 +481,15 @@
             model = models.DescribeDBSlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSyncMode(self, request):
         """本接口（DescribeDBSyncMode）用于查询云数据库实例的同步模式。
 
         :param request: Request instance for DescribeDBSyncMode.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBSyncModeRequest`
@@ -504,15 +504,15 @@
             model = models.DescribeDBSyncModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBTmpInstances(self, request):
         """本接口（DescribeDBTmpInstances）用于获取实例回档生成的临时实例
 
         :param request: Request instance for DescribeDBTmpInstances.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBTmpInstancesRequest`
@@ -527,15 +527,15 @@
             model = models.DescribeDBTmpInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBInstanceDetail(self, request):
         """本接口（DescribeDCDBInstanceDetail）用于获取TDSQL实例详情
 
         :param request: Request instance for DescribeDCDBInstanceDetail.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBInstanceDetailRequest`
@@ -550,15 +550,15 @@
             model = models.DescribeDCDBInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBInstanceNodeInfo(self, request):
         """本接口（DescribeDCDBInstanceNodeInfo）用于获取实例节点信息
 
         :param request: Request instance for DescribeDCDBInstanceNodeInfo.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBInstanceNodeInfoRequest`
@@ -573,15 +573,15 @@
             model = models.DescribeDCDBInstanceNodeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBInstances(self, request):
         """查询云数据库实例列表，支持通过项目ID、实例ID、内网地址、实例名称等来筛选实例。
         如果不指定任何筛选条件，则默认返回10条实例记录，单次请求最多支持返回100条实例记录。
 
         :param request: Request instance for DescribeDCDBInstances.
@@ -597,15 +597,15 @@
             model = models.DescribeDCDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBPrice(self, request):
         """本接口（DescribeDCDBPrice）用于在购买实例前，查询实例的价格。
 
         :param request: Request instance for DescribeDCDBPrice.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBPriceRequest`
@@ -620,15 +620,15 @@
             model = models.DescribeDCDBPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBRenewalPrice(self, request):
         """本接口（DescribeDCDBRenewalPrice）用于在续费分布式数据库实例时，查询续费的价格。
 
         :param request: Request instance for DescribeDCDBRenewalPrice.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBRenewalPriceRequest`
@@ -643,15 +643,15 @@
             model = models.DescribeDCDBRenewalPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBSaleInfo(self, request):
         """本接口(DescribeDCDBSaleInfo)用于查询分布式数据库可售卖的地域和可用区信息。
 
         :param request: Request instance for DescribeDCDBSaleInfo.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBSaleInfoRequest`
@@ -666,15 +666,15 @@
             model = models.DescribeDCDBSaleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBShards(self, request):
         """本接口（DescribeDCDBShards）用于查询云数据库实例的分片信息。
 
         :param request: Request instance for DescribeDCDBShards.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBShardsRequest`
@@ -689,15 +689,15 @@
             model = models.DescribeDCDBShardsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDCDBUpgradePrice(self, request):
         """本接口（DescribeDCDBUpgradePrice）用于查询变配分布式数据库实例价格。
 
         :param request: Request instance for DescribeDCDBUpgradePrice.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBUpgradePriceRequest`
@@ -712,15 +712,15 @@
             model = models.DescribeDCDBUpgradePriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabaseObjects(self, request):
         """本接口（DescribeDatabaseObjects）用于查询云数据库实例的数据库中的对象列表，包含表、存储过程、视图和函数。
 
         :param request: Request instance for DescribeDatabaseObjects.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDatabaseObjectsRequest`
@@ -735,15 +735,15 @@
             model = models.DescribeDatabaseObjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabaseTable(self, request):
         """本接口（DescribeDatabaseTable）用于查询云数据库实例的表信息。
 
         :param request: Request instance for DescribeDatabaseTable.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDatabaseTableRequest`
@@ -758,15 +758,15 @@
             model = models.DescribeDatabaseTableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabases(self, request):
         """本接口（DescribeDatabases）用于查询云数据库实例的数据库列表。
 
         :param request: Request instance for DescribeDatabases.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDatabasesRequest`
@@ -781,15 +781,15 @@
             model = models.DescribeDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDcnDetail(self, request):
         """获取实例灾备详情
 
         :param request: Request instance for DescribeDcnDetail.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDcnDetailRequest`
@@ -804,15 +804,15 @@
             model = models.DescribeDcnDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFileDownloadUrl(self, request):
         """本接口(DescribeFileDownloadUrl)用于获取数据库指定备份或日志文件的下载连接。
 
         :param request: Request instance for DescribeFileDownloadUrl.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeFileDownloadUrlRequest`
@@ -827,15 +827,15 @@
             model = models.DescribeFileDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlow(self, request):
         """本接口（DescribeFlow）用于查询流程状态
 
         :param request: Request instance for DescribeFlow.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeFlowRequest`
@@ -850,15 +850,15 @@
             model = models.DescribeFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrders(self, request):
         """本接口（DescribeOrders）用于查询分布式数据库订单信息。传入订单ID来查询订单关联的分布式数据库实例，和对应的任务流程ID。
 
         :param request: Request instance for DescribeOrders.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeOrdersRequest`
@@ -873,15 +873,15 @@
             model = models.DescribeOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectSecurityGroups(self, request):
         """本接口（DescribeProjectSecurityGroups）用于查询项目安全组信息
 
         :param request: Request instance for DescribeProjectSecurityGroups.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeProjectSecurityGroupsRequest`
@@ -896,15 +896,15 @@
             model = models.DescribeProjectSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjects(self, request):
         """本接口（DescribeProjects）用于查询项目列表
 
         :param request: Request instance for DescribeProjects.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeProjectsRequest`
@@ -919,15 +919,15 @@
             model = models.DescribeProjectsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeShardSpec(self, request):
         """查询可创建的分布式数据库可售卖的分片规格配置。
 
         :param request: Request instance for DescribeShardSpec.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeShardSpecRequest`
@@ -942,15 +942,15 @@
             model = models.DescribeShardSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSqlLogs(self, request):
         """已废弃接口
 
         本接口（DescribeSqlLogs）用于获取实例SQL日志。
 
@@ -967,15 +967,15 @@
             model = models.DescribeSqlLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserTasks(self, request):
         """本接口（DescribeUserTasks）用于拉取用户任务列表
 
         :param request: Request instance for DescribeUserTasks.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeUserTasksRequest`
@@ -990,15 +990,15 @@
             model = models.DescribeUserTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyDCDBInstance(self, request):
         """本接口(DestroyDCDBInstance)用于销毁已隔离的TDSQL包年包月实例。
 
         :param request: Request instance for DestroyDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DestroyDCDBInstanceRequest`
@@ -1013,15 +1013,15 @@
             model = models.DestroyDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyHourDCDBInstance(self, request):
         """本接口（DestroyHourDCDBInstance）用于TDSQL销毁按量计费实例。
 
         :param request: Request instance for DestroyHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DestroyHourDCDBInstanceRequest`
@@ -1036,15 +1036,15 @@
             model = models.DestroyHourDCDBInstanceResponse()
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
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DisassociateSecurityGroupsRequest`
@@ -1059,15 +1059,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FlushBinlog(self, request):
         """相当于在所有分片的mysqld中执行flush logs，完成切分的binlog将展示在各个分片控制台binlog列表里。
 
         :param request: Request instance for FlushBinlog.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.FlushBinlogRequest`
@@ -1082,15 +1082,15 @@
             model = models.FlushBinlogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GrantAccountPrivileges(self, request):
         """本接口（GrantAccountPrivileges）用于给云数据库账号赋权。
         注意：相同用户名，不同Host是不同的账号。
 
         :param request: Request instance for GrantAccountPrivileges.
@@ -1106,15 +1106,15 @@
             model = models.GrantAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InitDCDBInstances(self, request):
         """本接口(InitDCDBInstances)用于初始化云数据库实例，包括设置默认字符集、表名大小写敏感等。
 
         :param request: Request instance for InitDCDBInstances.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.InitDCDBInstancesRequest`
@@ -1129,15 +1129,15 @@
             model = models.InitDCDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDCDBInstance(self, request):
         """本接口(IsolateDCDBInstance)用于隔离分布式数据库TDSQL实例（包年包月），隔离后不能通过IP和端口访问数据库。隔离的实例可在回收站中进行开机。若为欠费隔离，请尽快进行充值。
 
         :param request: Request instance for IsolateDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateDCDBInstanceRequest`
@@ -1152,15 +1152,15 @@
             model = models.IsolateDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDedicatedDBInstance(self, request):
         """本接口（IsolateDedicatedDBInstance）用于隔离独享云数据库实例。
 
         :param request: Request instance for IsolateDedicatedDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateDedicatedDBInstanceRequest`
@@ -1175,15 +1175,15 @@
             model = models.IsolateDedicatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateHourDCDBInstance(self, request):
         """隔离TDSQL按量计费实例
 
         :param request: Request instance for IsolateHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateHourDCDBInstanceRequest`
@@ -1198,15 +1198,15 @@
             model = models.IsolateHourDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KillSession(self, request):
         """本接口（KillSession）用于杀死指定会话。
 
         :param request: Request instance for KillSession.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.KillSessionRequest`
@@ -1221,15 +1221,15 @@
             model = models.KillSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountConfig(self, request):
         """修改账号的一些配置，比如 max_user_connections
 
         :param request: Request instance for ModifyAccountConfig.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyAccountConfigRequest`
@@ -1244,15 +1244,15 @@
             model = models.ModifyAccountConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountDescription(self, request):
         """本接口（ModifyAccountDescription）用于修改云数据库账号备注。
         注意：相同用户名，不同Host是不同的账号。
 
         :param request: Request instance for ModifyAccountDescription.
@@ -1268,15 +1268,15 @@
             model = models.ModifyAccountDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountPrivileges(self, request):
         """本接口(ModifyAccountPrivileges)用于修改云数据库的账户的权限信息。
 
         **注意**
         - 系统保留库："mysql"，只开放["SELECT"]权限
@@ -1296,15 +1296,15 @@
             model = models.ModifyAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBEncryptAttributes(self, request):
         """本接口(ModifyDBEncryptAttributes)用于修改实例数据加密。
 
         :param request: Request instance for ModifyDBEncryptAttributes.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBEncryptAttributesRequest`
@@ -1319,15 +1319,15 @@
             model = models.ModifyDBEncryptAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceName(self, request):
         """本接口（ModifyDBInstanceName）用于修改实例名字
 
         :param request: Request instance for ModifyDBInstanceName.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBInstanceNameRequest`
@@ -1342,15 +1342,15 @@
             model = models.ModifyDBInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSecurityGroups(self, request):
         """本接口（ModifyDBInstanceSecurityGroups）用于修改云数据库安全组
 
         :param request: Request instance for ModifyDBInstanceSecurityGroups.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -1365,15 +1365,15 @@
             model = models.ModifyDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstancesProject(self, request):
         """本接口（ModifyDBInstancesProject）用于修改云数据库实例所属项目。
 
         :param request: Request instance for ModifyDBInstancesProject.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBInstancesProjectRequest`
@@ -1388,15 +1388,15 @@
             model = models.ModifyDBInstancesProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBParameters(self, request):
         """本接口(ModifyDBParameters)用于修改数据库参数。
 
         :param request: Request instance for ModifyDBParameters.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBParametersRequest`
@@ -1411,15 +1411,15 @@
             model = models.ModifyDBParametersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBSyncMode(self, request):
         """本接口（ModifyDBSyncMode）用于修改云数据库实例的同步模式。
 
         :param request: Request instance for ModifyDBSyncMode.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyDBSyncModeRequest`
@@ -1434,15 +1434,15 @@
             model = models.ModifyDBSyncModeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceNetwork(self, request):
         """本接口（ModifyInstanceNetwork）用于修改实例所属网络。
 
         :param request: Request instance for ModifyInstanceNetwork.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyInstanceNetworkRequest`
@@ -1457,15 +1457,15 @@
             model = models.ModifyInstanceNetworkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceVip(self, request):
         """本接口（ModifyInstanceVip）用于修改实例Vip
 
         :param request: Request instance for ModifyInstanceVip.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyInstanceVipRequest`
@@ -1480,15 +1480,15 @@
             model = models.ModifyInstanceVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceVport(self, request):
         """本接口（ModifyInstanceVport）用于修改实例VPORT
 
         :param request: Request instance for ModifyInstanceVport.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyInstanceVportRequest`
@@ -1503,15 +1503,15 @@
             model = models.ModifyInstanceVportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRealServerAccessStrategy(self, request):
         """本接口(ModifyRealServerAccessStrategy)用于修改云数据库的VPCGW到RS的访问策略。
 
         **注意**
         - 修改策略后只对新建立的连接生效，老连接不受影响
@@ -1531,15 +1531,15 @@
             model = models.ModifyRealServerAccessStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenDBExtranetAccess(self, request):
         """本接口（OpenDBExtranetAccess）用于开通云数据库实例的外网访问。开通外网访问后，您可通过外网域名和端口访问实例，可使用查询实例列表接口获取外网域名和端口信息。
 
         :param request: Request instance for OpenDBExtranetAccess.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.OpenDBExtranetAccessRequest`
@@ -1554,15 +1554,15 @@
             model = models.OpenDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDCDBInstance(self, request):
         """本接口（RenewDCDBInstance）用于续费分布式数据库实例。
 
         :param request: Request instance for RenewDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.RenewDCDBInstanceRequest`
@@ -1577,15 +1577,15 @@
             model = models.RenewDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAccountPassword(self, request):
         """本接口（ResetAccountPassword）用于重置云数据库账号的密码。
         注意：相同用户名，不同Host是不同的账号。
 
         :param request: Request instance for ResetAccountPassword.
@@ -1601,15 +1601,15 @@
             model = models.ResetAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchDBInstanceHA(self, request):
         """本接口(SwitchDBInstanceHA)用于实例主备切换。
 
         :param request: Request instance for SwitchDBInstanceHA.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.SwitchDBInstanceHARequest`
@@ -1624,15 +1624,15 @@
             model = models.SwitchDBInstanceHAResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDedicatedDBInstance(self, request):
         """本接口（TerminateDedicatedDBInstance）用于销毁已隔离的独享分布式数据库实例。
 
         :param request: Request instance for TerminateDedicatedDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.TerminateDedicatedDBInstanceRequest`
@@ -1647,15 +1647,15 @@
             model = models.TerminateDedicatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDCDBInstance(self, request):
         """本接口（UpgradeDCDBInstance）用于升级分布式数据库实例。本接口完成下单和支付两个动作，如果发生支付失败的错误，调用用户账户相关接口中的支付订单接口（PayDeals）重新支付即可。
 
         :param request: Request instance for UpgradeDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDCDBInstanceRequest`
@@ -1670,15 +1670,15 @@
             model = models.UpgradeDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDedicatedDCDBInstance(self, request):
         """本接口（UpgradeDedicatedDCDBInstance）用于升级TDSQL独享集群实例
 
         :param request: Request instance for UpgradeDedicatedDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDedicatedDCDBInstanceRequest`
@@ -1693,15 +1693,15 @@
             model = models.UpgradeDedicatedDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeHourDCDBInstance(self, request):
         """本接口（UpgradeHourDCDBInstance）用于升级分布式数据库TDSQL按量计费实例。
 
         :param request: Request instance for UpgradeHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeHourDCDBInstanceRequest`
@@ -1716,8 +1716,8 @@
             model = models.UpgradeHourDCDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/dcdb/v20180411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.938/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.937/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.938/README.rst`

 * *Files identical despite different names*

