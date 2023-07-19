# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.937.tar", last modified: Tue Jul 18 00:27:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.938.tar", last modified: Wed Jul 19 00:42:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.937.tar` & `tencentcloud-sdk-python-mariadb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)    71772 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14932 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   354627 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:27:02.000000 tencentcloud-sdk-python-mariadb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:27:01.000000 tencentcloud-sdk-python-mariadb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    72060 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14932 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   354627 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:42:23.000000 tencentcloud-sdk-python-mariadb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ActivateHourDBInstanceResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.AssociateSecurityGroupsRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CancelDcnJobRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CloneAccountRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CloseDBExtranetAccessRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateAccountRequest`
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
 
 
     def CreateDBInstance(self, request):
         """本接口（CreateDBInstance）用于创建包年包月的MariaDB云数据库实例，可通过传入实例规格、数据库版本号、购买时长和数量等信息创建云数据库实例。
 
         :param request: Request instance for CreateDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateDBInstanceRequest`
@@ -204,15 +204,15 @@
             model = models.CreateDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDedicatedClusterDBInstance(self, request):
         """创建Mariadb独享集群实例
 
         :param request: Request instance for CreateDedicatedClusterDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateDedicatedClusterDBInstanceRequest`
@@ -227,15 +227,15 @@
             model = models.CreateDedicatedClusterDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateHourDBInstance(self, request):
         """创建MariaDB按量计费实例
 
         :param request: Request instance for CreateHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateHourDBInstanceRequest`
@@ -250,15 +250,15 @@
             model = models.CreateHourDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTmpInstances(self, request):
         """本接口（CreateTmpInstances）用于创建临时实例。
 
         :param request: Request instance for CreateTmpInstances.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateTmpInstancesRequest`
@@ -273,15 +273,15 @@
             model = models.CreateTmpInstancesResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DeleteAccountRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeAccountsRequest`
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeBackupFilesRequest`
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
 
 
     def DescribeBackupTime(self, request):
         """本接口（DescribeBackupTime）用于获取云数据库的备份时间。后台系统将根据此配置定期进行实例备份。
 
         :param request: Request instance for DescribeBackupTime.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeBackupTimeRequest`
@@ -389,15 +389,15 @@
             model = models.DescribeBackupTimeResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBEncryptAttributesRequest`
@@ -412,15 +412,15 @@
             model = models.DescribeDBEncryptAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceDetail(self, request):
         """本接口(DescribeDBInstanceDetail)用于查询指定实例的详细信息。
 
         :param request: Request instance for DescribeDBInstanceDetail.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBInstanceDetailRequest`
@@ -435,15 +435,15 @@
             model = models.DescribeDBInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceSpecs(self, request):
         """本接口(DescribeDBInstanceSpecs)用于查询可创建的云数据库可售卖的规格配置。
 
         :param request: Request instance for DescribeDBInstanceSpecs.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBInstanceSpecsRequest`
@@ -458,15 +458,15 @@
             model = models.DescribeDBInstanceSpecsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstances(self, request):
         """本接口（DescribeDBInstances）用于查询云数据库实例列表，支持通过项目ID、实例ID、内网地址、实例名称等来筛选实例。
         如果不指定任何筛选条件，则默认返回20条实例记录，单次请求最多支持返回100条实例记录。
 
         :param request: Request instance for DescribeDBInstances.
@@ -482,15 +482,15 @@
             model = models.DescribeDBInstancesResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBLogFilesRequest`
@@ -505,15 +505,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBParametersRequest`
@@ -528,15 +528,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBSecurityGroupsRequest`
@@ -551,15 +551,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBSlowLogsRequest`
@@ -574,15 +574,15 @@
             model = models.DescribeDBSlowLogsResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBTmpInstancesRequest`
@@ -597,15 +597,15 @@
             model = models.DescribeDBTmpInstancesResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDatabaseObjectsRequest`
@@ -620,15 +620,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDatabaseTableRequest`
@@ -643,15 +643,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDatabasesRequest`
@@ -666,15 +666,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDcnDetailRequest`
@@ -689,15 +689,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeFileDownloadUrlRequest`
@@ -712,15 +712,15 @@
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
         """本接口（DescribeFlow）用于查询流程状态。
 
         :param request: Request instance for DescribeFlow.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeFlowRequest`
@@ -735,15 +735,15 @@
             model = models.DescribeFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceNodeInfo(self, request):
         """本接口（DescribeInstanceNodeInfo）用于获取数据库实例主备节点信息
 
         :param request: Request instance for DescribeInstanceNodeInfo.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeInstanceNodeInfoRequest`
@@ -758,15 +758,15 @@
             model = models.DescribeInstanceNodeInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogFileRetentionPeriod(self, request):
         """本接口(DescribeLogFileRetentionPeriod)用于查看数据库备份日志的备份天数的设置情况。
 
         :param request: Request instance for DescribeLogFileRetentionPeriod.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeLogFileRetentionPeriodRequest`
@@ -781,15 +781,15 @@
             model = models.DescribeLogFileRetentionPeriodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrders(self, request):
         """本接口（DescribeOrders）用于查询云数据库订单信息。传入订单ID来查询订单关联的云数据库实例，和对应的任务流程ID。
 
         :param request: Request instance for DescribeOrders.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeOrdersRequest`
@@ -804,15 +804,15 @@
             model = models.DescribeOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePrice(self, request):
         """本接口（DescribePrice）用于在购买实例前，查询实例的价格。
 
         :param request: Request instance for DescribePrice.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribePriceRequest`
@@ -827,15 +827,15 @@
             model = models.DescribePriceResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeProjectSecurityGroupsRequest`
@@ -850,15 +850,15 @@
             model = models.DescribeProjectSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRenewalPrice(self, request):
         """本接口（DescribeRenewalPrice）用于在续费云数据库实例时，查询续费的价格。
 
         :param request: Request instance for DescribeRenewalPrice.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeRenewalPriceRequest`
@@ -873,15 +873,15 @@
             model = models.DescribeRenewalPriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSaleInfo(self, request):
         """本接口(DescribeSaleInfo)用于查询云数据库可售卖的地域和可用区信息。
 
         :param request: Request instance for DescribeSaleInfo.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeSaleInfoRequest`
@@ -896,15 +896,15 @@
             model = models.DescribeSaleInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUpgradePrice(self, request):
         """本接口（DescribeUpgradePrice）用于在扩容云数据库实例时，查询变配的价格。
 
         :param request: Request instance for DescribeUpgradePrice.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeUpgradePriceRequest`
@@ -919,15 +919,15 @@
             model = models.DescribeUpgradePriceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyDBInstance(self, request):
         """本接口(DestroyDBInstance)用于销毁已隔离的包年包月实例。
 
         :param request: Request instance for DestroyDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DestroyDBInstanceRequest`
@@ -942,15 +942,15 @@
             model = models.DestroyDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyHourDBInstance(self, request):
         """本接口（DestroyHourDBInstance）用于销毁MariaDB按量计费实例。
 
         :param request: Request instance for DestroyHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DestroyHourDBInstanceRequest`
@@ -965,15 +965,15 @@
             model = models.DestroyHourDBInstanceResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DisassociateSecurityGroupsRequest`
@@ -988,15 +988,15 @@
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
         """相当于在mysqld中执行flush logs，完成切分的binlog将展示在实例控制台binlog列表里。
 
         :param request: Request instance for FlushBinlog.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.FlushBinlogRequest`
@@ -1011,15 +1011,15 @@
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
@@ -1035,15 +1035,15 @@
             model = models.GrantAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InitDBInstances(self, request):
         """本接口(InitDBInstances)用于初始化云数据库实例，包括设置默认字符集、表名大小写敏感等。
 
         :param request: Request instance for InitDBInstances.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.InitDBInstancesRequest`
@@ -1058,15 +1058,15 @@
             model = models.InitDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDBInstance(self, request):
         """本接口(IsolateDBInstance)用于隔离云数据库MariaDB实例（包年包月），隔离后不能通过IP和端口访问数据库。隔离的实例可在回收站中进行开机。若为欠费隔离，请尽快进行充值。
 
         :param request: Request instance for IsolateDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.IsolateDBInstanceRequest`
@@ -1081,15 +1081,15 @@
             model = models.IsolateDBInstanceResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.IsolateDedicatedDBInstanceRequest`
@@ -1104,15 +1104,15 @@
             model = models.IsolateDedicatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateHourDBInstance(self, request):
         """隔离MariaDB按量计费实例
 
         :param request: Request instance for IsolateHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.IsolateHourDBInstanceRequest`
@@ -1127,15 +1127,15 @@
             model = models.IsolateHourDBInstanceResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.KillSessionRequest`
@@ -1150,15 +1150,15 @@
             model = models.KillSessionResponse()
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
@@ -1174,15 +1174,15 @@
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
@@ -1202,15 +1202,15 @@
             model = models.ModifyAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupTime(self, request):
         """本接口（ModifyBackupTime）用于设置云数据库实例的备份时间。后台系统将根据此配置定期进行实例备份。
 
         :param request: Request instance for ModifyBackupTime.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyBackupTimeRequest`
@@ -1225,15 +1225,15 @@
             model = models.ModifyBackupTimeResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBEncryptAttributesRequest`
@@ -1248,15 +1248,15 @@
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
         """本接口（ModifyDBInstanceName）用于修改云数据库实例的名称。
 
         :param request: Request instance for ModifyDBInstanceName.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBInstanceNameRequest`
@@ -1271,15 +1271,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -1294,15 +1294,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBInstancesProjectRequest`
@@ -1317,15 +1317,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBParametersRequest`
@@ -1340,15 +1340,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyDBSyncModeRequest`
@@ -1363,15 +1363,15 @@
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
         """本接口（ModifyInstanceNetwork）用于修改实例所属网络
 
         :param request: Request instance for ModifyInstanceNetwork.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyInstanceNetworkRequest`
@@ -1386,15 +1386,15 @@
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
         """本接口（ModifyInstanceVip）用于修改实例VIP
 
         :param request: Request instance for ModifyInstanceVip.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyInstanceVipRequest`
@@ -1409,15 +1409,15 @@
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyInstanceVportRequest`
@@ -1432,15 +1432,15 @@
             model = models.ModifyInstanceVportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyLogFileRetentionPeriod(self, request):
         """本接口(ModifyLogFileRetentionPeriod)用于修改数据库备份日志保存天数。
 
         :param request: Request instance for ModifyLogFileRetentionPeriod.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifyLogFileRetentionPeriodRequest`
@@ -1455,15 +1455,15 @@
             model = models.ModifyLogFileRetentionPeriodResponse()
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
@@ -1483,15 +1483,15 @@
             model = models.ModifyRealServerAccessStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySyncTaskAttribute(self, request):
         """本接口 (ModifySyncTaskAttribute) 用于修改同步任务的属性（目前只支持修改任务名称）
 
         :param request: Request instance for ModifySyncTaskAttribute.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ModifySyncTaskAttributeRequest`
@@ -1506,15 +1506,15 @@
             model = models.ModifySyncTaskAttributeResponse()
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
         :type request: :class:`tencentcloud.mariadb.v20170312.models.OpenDBExtranetAccessRequest`
@@ -1529,15 +1529,15 @@
             model = models.OpenDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDBInstance(self, request):
         """本接口（RenewDBInstance）用于续费云数据库实例。
 
         :param request: Request instance for RenewDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.RenewDBInstanceRequest`
@@ -1552,15 +1552,15 @@
             model = models.RenewDBInstanceResponse()
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
@@ -1576,15 +1576,15 @@
             model = models.ResetAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartDBInstances(self, request):
         """本接口（RestartDBInstances）用于重启数据库实例
 
         :param request: Request instance for RestartDBInstances.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.RestartDBInstancesRequest`
@@ -1599,15 +1599,15 @@
             model = models.RestartDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchDBInstanceHA(self, request):
         """本接口（SwitchDBInstanceHA）用于发起实例主备切换。
 
         :param request: Request instance for SwitchDBInstanceHA.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.SwitchDBInstanceHARequest`
@@ -1622,15 +1622,15 @@
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
         """本接口（TerminateDedicatedDBInstance）用于销毁已隔离的独享云数据库实例。
 
         :param request: Request instance for TerminateDedicatedDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.TerminateDedicatedDBInstanceRequest`
@@ -1645,15 +1645,15 @@
             model = models.TerminateDedicatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDBInstance(self, request):
         """本接口(UpgradeDBInstance)用于扩容云数据库实例。本接口完成下单和支付两个动作，如果发生支付失败的错误，调用用户账户相关接口中的支付订单接口（PayDeals）重新支付即可。
 
         :param request: Request instance for UpgradeDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.UpgradeDBInstanceRequest`
@@ -1668,15 +1668,15 @@
             model = models.UpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDedicatedDBInstance(self, request):
         """本接口(UpgradeDedicatedDBInstance)用于扩容独享云数据库实例。
 
         :param request: Request instance for UpgradeDedicatedDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.UpgradeDedicatedDBInstanceRequest`
@@ -1691,8 +1691,8 @@
             model = models.UpgradeDedicatedDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/mariadb/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.937/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.938/README.rst`

 * *Files identical despite different names*

