# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.937.tar", last modified: Tue Jul 18 00:30:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.938.tar", last modified: Wed Jul 19 00:45:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.937.tar` & `tencentcloud-sdk-python-sqlserver-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   108687 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9722 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   572158 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-18 00:30:10.000000 tencentcloud-sdk-python-sqlserver-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   109131 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   572158 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-19 00:45:23.000000 tencentcloud-sdk-python-sqlserver-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 11% similar despite different names*

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
 
 
     def CloneDB(self, request):
         """本接口（CloneDB）用于克隆数据库，只支持克隆到本实例，克隆时必须指定新库名称。
 
         :param request: Request instance for CloneDB.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CloneDBRequest`
@@ -65,15 +65,15 @@
             model = models.CloneDBResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseInterCommunication(self, request):
         """本接口（CloseInterCommunication）用于关闭实例互通。
 
         :param request: Request instance for CloseInterCommunication.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CloseInterCommunicationRequest`
@@ -88,15 +88,15 @@
             model = models.CloseInterCommunicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompleteExpansion(self, request):
         """本接口（CompleteExpansion）在实例发起扩容后，实例状态处于“升级待切换”时，可立即完成实例升级切换操作，无需等待可维护时间窗。本接口需要在实例低峰时调用，在完全切换成功前，存在部分库不可访问的风险。
 
         :param request: Request instance for CompleteExpansion.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CompleteExpansionRequest`
@@ -111,15 +111,15 @@
             model = models.CompleteExpansionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompleteMigration(self, request):
         """本接口（CompleteMigration）作用是完成一个迁移任务
 
         :param request: Request instance for CompleteMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CompleteMigrationRequest`
@@ -134,15 +134,15 @@
             model = models.CompleteMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccount(self, request):
         """本接口（CreateAccount）用于创建实例账号
 
         :param request: Request instance for CreateAccount.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateAccountRequest`
@@ -157,15 +157,15 @@
             model = models.CreateAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackup(self, request):
         """本接口(CreateBackup)用于创建备份。
 
         :param request: Request instance for CreateBackup.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateBackupRequest`
@@ -180,15 +180,15 @@
             model = models.CreateBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackupMigration(self, request):
         """本接口（CreateBackupMigration）用于创建备份导入任务。
 
         :param request: Request instance for CreateBackupMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateBackupMigrationRequest`
@@ -203,15 +203,15 @@
             model = models.CreateBackupMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBasicDBInstances(self, request):
         """本接口（CreateBasicDBInstances）用于创建SQL server基础版实例。
 
         :param request: Request instance for CreateBasicDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateBasicDBInstancesRequest`
@@ -226,15 +226,15 @@
             model = models.CreateBasicDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBusinessDBInstances(self, request):
         """本接口（CreateBusinessDBInstances）用于创建商业智能服务实例。
 
         :param request: Request instance for CreateBusinessDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateBusinessDBInstancesRequest`
@@ -249,15 +249,15 @@
             model = models.CreateBusinessDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBusinessIntelligenceFile(self, request):
         """本接口（CreateBusinessIntelligenceFile）用于添加商业智能服务文件。
 
         :param request: Request instance for CreateBusinessIntelligenceFile.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateBusinessIntelligenceFileRequest`
@@ -272,15 +272,15 @@
             model = models.CreateBusinessIntelligenceFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudDBInstances(self, request):
         """本接口（CreateCloudDBInstances）用于创建高可用实例(虚拟机版本)。
 
         :param request: Request instance for CreateCloudDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudDBInstancesRequest`
@@ -295,15 +295,15 @@
             model = models.CreateCloudDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudReadOnlyDBInstances(self, request):
         """本接口（CreateCloudReadOnlyDBInstances）用于添加只读副本实例(虚拟机版本)。
 
         :param request: Request instance for CreateCloudReadOnlyDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudReadOnlyDBInstancesRequest`
@@ -318,15 +318,15 @@
             model = models.CreateCloudReadOnlyDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDB(self, request):
         """本接口（CreateDB）用于创建数据库。
 
         :param request: Request instance for CreateDB.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateDBRequest`
@@ -341,15 +341,15 @@
             model = models.CreateDBResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstances(self, request):
         """本接口（CreateDBInstances）用于创建实例。
 
         :param request: Request instance for CreateDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateDBInstancesRequest`
@@ -364,15 +364,15 @@
             model = models.CreateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIncrementalMigration(self, request):
         """本接口（CreateIncrementalMigration）用于创建增量备份导入任务。
 
         :param request: Request instance for CreateIncrementalMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateIncrementalMigrationRequest`
@@ -387,15 +387,15 @@
             model = models.CreateIncrementalMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigration(self, request):
         """本接口（CreateMigration）作用是创建一个迁移任务
 
         :param request: Request instance for CreateMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateMigrationRequest`
@@ -410,15 +410,15 @@
             model = models.CreateMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePublishSubscribe(self, request):
         """本接口（CreatePublishSubscribe）用于创建两个数据库之间的发布订阅关系。作为订阅者，不能再充当发布者，作为发布者可以有多个订阅者实例。
 
         :param request: Request instance for CreatePublishSubscribe.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreatePublishSubscribeRequest`
@@ -433,15 +433,15 @@
             model = models.CreatePublishSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReadOnlyDBInstances(self, request):
         """本接口（CreateReadOnlyDBInstances）用于添加只读副本实例。
 
         :param request: Request instance for CreateReadOnlyDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateReadOnlyDBInstancesRequest`
@@ -456,15 +456,15 @@
             model = models.CreateReadOnlyDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccount(self, request):
         """本接口（DeleteAccount）用于删除实例账号。
 
         :param request: Request instance for DeleteAccount.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteAccountRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBackupMigration(self, request):
         """本接口（DeleteBackupMigration）用于删除备份导入任务。
 
         :param request: Request instance for DeleteBackupMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteBackupMigrationRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteBackupMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBusinessIntelligenceFile(self, request):
         """本接口（DeleteBusinessIntelligenceFile）用于删除商业智能文件。
 
         :param request: Request instance for DeleteBusinessIntelligenceFile.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteBusinessIntelligenceFileRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteBusinessIntelligenceFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDB(self, request):
         """本接口(DeleteDB)用于删除数据库。
 
         :param request: Request instance for DeleteDB.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteDBRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteDBResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDBInstance(self, request):
         """本接口（DeleteDBInstance）用于释放回收站中的SQL server实例(立即下线)。释放后的实例将保存一段时间后物理销毁。其发布订阅将自动解除，其ro副本将自动释放。
 
         :param request: Request instance for DeleteDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteDBInstanceRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIncrementalMigration(self, request):
         """本接口（DeleteIncrementalMigration）用于删除增量备份导入任务。
 
         :param request: Request instance for DeleteIncrementalMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteIncrementalMigrationRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteIncrementalMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMigration(self, request):
         """本接口（DeleteMigration）用于删除迁移任务
 
         :param request: Request instance for DeleteMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeleteMigrationRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePublishSubscribe(self, request):
         """本接口（DeletePublishSubscribe）用于删除两个数据库间的发布订阅关系。
 
         :param request: Request instance for DeletePublishSubscribe.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DeletePublishSubscribeRequest`
@@ -640,15 +640,15 @@
             model = models.DeletePublishSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """本接口（DescribeAccounts）用于拉取实例账户列表。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeAccountsRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupByFlowId(self, request):
         """本接口(DescribeBackupByFlowId)用于通过备份创建流程的ID查询创建的备份详情，流程ID可从接口CreateBackup中获得。
 
         :param request: Request instance for DescribeBackupByFlowId.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupByFlowIdRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeBackupByFlowIdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupCommand(self, request):
         """本接口（DescribeBackupCommand）用于查询以规范的格式创建备份的命令。
 
         :param request: Request instance for DescribeBackupCommand.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupCommandRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeBackupCommandResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupFiles(self, request):
         """本接口(DescribeBackupFiles)用于查询单库备份明细
 
         :param request: Request instance for DescribeBackupFiles.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupFilesRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeBackupFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupMigration(self, request):
         """本接口（DescribeBackupMigration）用于创建增量备份导入任务。
 
         :param request: Request instance for DescribeBackupMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupMigrationRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeBackupMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupUploadSize(self, request):
         """本接口（DescribeBackupUploadSize）用于查询上传的备份文件大小。在备份上传类型是COS_UPLOAD(备份放在业务的对象存储上)时有效。
 
         :param request: Request instance for DescribeBackupUploadSize.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupUploadSizeRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeBackupUploadSizeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackups(self, request):
         """本接口(DescribeBackups)用于查询备份列表。
 
         :param request: Request instance for DescribeBackups.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBackupsRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBusinessIntelligenceFile(self, request):
         """本接口（DescribeBusinessIntelligenceFile）用于查询商业智能服务需要的文件。
 
         :param request: Request instance for DescribeBusinessIntelligenceFile.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeBusinessIntelligenceFileRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeBusinessIntelligenceFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCrossRegionZone(self, request):
         """本接口(DescribeCrossRegionZone)根据主实例查询备机的容灾地域和可用区。
 
         :param request: Request instance for DescribeCrossRegionZone.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeCrossRegionZoneRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeCrossRegionZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBCharsets(self, request):
         """本接口（DescribeDBCharsets）用于查询实例支持的数据库字符集。
 
         :param request: Request instance for DescribeDBCharsets.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBCharsetsRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeDBCharsetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceInter(self, request):
         """本接口（DescribeDBInstanceInter）用于查询互通实例的信息。
 
         :param request: Request instance for DescribeDBInstanceInter.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBInstanceInterRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeDBInstanceInterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstances(self, request):
         """本接口(DescribeDBInstances)用于查询实例列表。
 
         :param request: Request instance for DescribeDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBInstancesRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstancesAttribute(self, request):
         """本接口（DescribeDBInstancesAttribute）用于查询实例附属属性
 
         :param request: Request instance for DescribeDBInstancesAttribute.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBInstancesAttributeRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeDBInstancesAttributeResponse()
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
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBSecurityGroupsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeDBSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBs(self, request):
         """本接口（DescribeDBs）用于查询数据库列表。
 
         :param request: Request instance for DescribeDBs.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBsRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeDBsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBsNormal(self, request):
         """本接口(DescribeDBsNormal)用于查询数据库配置信息，此接口不包含数据库的关联账号
 
         :param request: Request instance for DescribeDBsNormal.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeDBsNormalRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeDBsNormalResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowStatus(self, request):
         """本接口(DescribeFlowStatus)用于查询流程状态。
 
         :param request: Request instance for DescribeFlowStatus.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeFlowStatusRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeFlowStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIncrementalMigration(self, request):
         """本接口（DescribeIncrementalMigration）用于查询增量备份导入任务。
 
         :param request: Request instance for DescribeIncrementalMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeIncrementalMigrationRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeIncrementalMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceParamRecords(self, request):
         """该接口（DescribeInstanceParamRecords）用于查询实例参数修改历史。
 
         :param request: Request instance for DescribeInstanceParamRecords.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceParamRecordsRequest`
@@ -1077,15 +1077,15 @@
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
         """该接口（DescribeInstanceParams）用于查询实例的参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceParamsRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMaintenanceSpan(self, request):
         """本接口（DescribeMaintenanceSpan）根据实例ID查询该实例的可维护时间窗。
 
         :param request: Request instance for DescribeMaintenanceSpan.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeMaintenanceSpanRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeMaintenanceSpanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationDatabases(self, request):
         """本接口（DescribeMigrationDatabases）的作用是查询待迁移数据库列表
 
         :param request: Request instance for DescribeMigrationDatabases.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeMigrationDatabasesRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeMigrationDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationDetail(self, request):
         """本接口（DescribeMigrationDetail）用于查询迁移任务的详细情况
 
         :param request: Request instance for DescribeMigrationDetail.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeMigrationDetailRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeMigrationDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrations(self, request):
         """本接口（DescribeMigrations）根据输入的限定条件，查询符合条件的迁移任务列表
 
         :param request: Request instance for DescribeMigrations.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeMigrationsRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeMigrationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrders(self, request):
         """本接口（DescribeOrders）用于查询订单信息
 
         :param request: Request instance for DescribeOrders.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeOrdersRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductConfig(self, request):
         """本接口 (DescribeProductConfig) 用于查询售卖规格配置。
 
         :param request: Request instance for DescribeProductConfig.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeProductConfigRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeProductConfigResponse()
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
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeProjectSecurityGroupsRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeProjectSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePublishSubscribe(self, request):
         """本接口（DescribePublishSubscribe）用于查询发布订阅关系列表。
 
         :param request: Request instance for DescribePublishSubscribe.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribePublishSubscribeRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribePublishSubscribeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReadOnlyGroupByReadOnlyInstance(self, request):
         """本接口（DescribeReadOnlyGroupByReadOnlyInstance）用于通过只读副本实例ID查询其所在的只读组。
 
         :param request: Request instance for DescribeReadOnlyGroupByReadOnlyInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeReadOnlyGroupByReadOnlyInstanceRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeReadOnlyGroupByReadOnlyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReadOnlyGroupDetails(self, request):
         """本接口（DescribeReadOnlyGroupDetails）用于查询只读组详情。
 
         :param request: Request instance for DescribeReadOnlyGroupDetails.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeReadOnlyGroupDetailsRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeReadOnlyGroupDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReadOnlyGroupList(self, request):
         """本接口（DescribeReadOnlyGroupList）用于查询只读组列表。
 
         :param request: Request instance for DescribeReadOnlyGroupList.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeReadOnlyGroupListRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeReadOnlyGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """本接口 (DescribeRegions) 用于查询售卖地域信息。
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeRegionsRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRollbackTime(self, request):
         """本接口（DescribeRollbackTime）用于查询实例可回档时间范围
 
         :param request: Request instance for DescribeRollbackTime.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeRollbackTimeRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeRollbackTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowlogs(self, request):
         """本接口（DescribeSlowlogs）用于获取慢查询日志文件信息
 
         :param request: Request instance for DescribeSlowlogs.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeSlowlogsRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeSlowlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUploadBackupInfo(self, request):
         """本接口（DescribeUploadBackupInfo）用于查询备份上传权限。
 
         :param request: Request instance for DescribeUploadBackupInfo.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeUploadBackupInfoRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeUploadBackupInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUploadIncrementalInfo(self, request):
         """本接口（DescribeUploadIncrementalInfo）用于查询增量备份上传权限。
 
         :param request: Request instance for DescribeUploadIncrementalInfo.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeUploadIncrementalInfoRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeUploadIncrementalInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeXEvents(self, request):
         """本接口（DescribeXEvents）用于查询扩展事件列表。
 
         :param request: Request instance for DescribeXEvents.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeXEventsRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeXEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """本接口 (DescribeZones) 用于查询当前可售卖的可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeZonesRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeZonesResponse()
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
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DisassociateSecurityGroupsRequest`
@@ -1537,15 +1537,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateDBInstances(self, request):
         """本接口（InquiryPriceCreateDBInstances）用于查询申请实例价格。
 
         :param request: Request instance for InquiryPriceCreateDBInstances.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceCreateDBInstancesRequest`
@@ -1560,15 +1560,15 @@
             model = models.InquiryPriceCreateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRenewDBInstance(self, request):
         """本接口（InquiryPriceRenewDBInstance）用于查询包年包月实例的续费价格。
 
         :param request: Request instance for InquiryPriceRenewDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.InquiryPriceRenewDBInstanceRequest`
@@ -1583,15 +1583,15 @@
             model = models.InquiryPriceRenewDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceUpgradeDBInstance(self, request):
         """本接口（InquiryPriceUpgradeDBInstance）用于查询包年包月实例升级变配的价格。
         按量计费实例变配后的价格参考InquiryPriceCreateDBInstances接口。
 
         :param request: Request instance for InquiryPriceUpgradeDBInstance.
@@ -1607,15 +1607,15 @@
             model = models.InquiryPriceUpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountPrivilege(self, request):
         """本接口（ModifyAccountPrivilege）用于修改实例账户权限。
 
         :param request: Request instance for ModifyAccountPrivilege.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyAccountPrivilegeRequest`
@@ -1630,15 +1630,15 @@
             model = models.ModifyAccountPrivilegeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountRemark(self, request):
         """本接口（ModifyAccountRemark）用于修改账户备注。
 
         :param request: Request instance for ModifyAccountRemark.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyAccountRemarkRequest`
@@ -1653,15 +1653,15 @@
             model = models.ModifyAccountRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupMigration(self, request):
         """本接口（ModifyBackupMigration）用于修改备份导入任务。
 
         :param request: Request instance for ModifyBackupMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyBackupMigrationRequest`
@@ -1676,15 +1676,15 @@
             model = models.ModifyBackupMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupName(self, request):
         """本接口(ModifyBackupName)用于修改备份任务名称。
 
         :param request: Request instance for ModifyBackupName.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyBackupNameRequest`
@@ -1699,15 +1699,15 @@
             model = models.ModifyBackupNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupStrategy(self, request):
         """本接口（ModifyBackupStrategy）用于修改备份策略
 
         :param request: Request instance for ModifyBackupStrategy.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyBackupStrategyRequest`
@@ -1722,15 +1722,15 @@
             model = models.ModifyBackupStrategyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBEncryptAttributes(self, request):
         """本接口（ModifyDBEncryptAttributes）用于开启、关闭数据库的TDE加密功能。
 
         :param request: Request instance for ModifyDBEncryptAttributes.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBEncryptAttributesRequest`
@@ -1745,15 +1745,15 @@
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
         """本接口（ModifyDBInstanceName）用于修改实例名字。
 
         :param request: Request instance for ModifyDBInstanceName.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBInstanceNameRequest`
@@ -1768,15 +1768,15 @@
             model = models.ModifyDBInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceNetwork(self, request):
         """本接口（ModifyDBInstanceNetwork）用于修改运行中实例的网络，仅支持从VPC网络到VPC网络的转换
 
         :param request: Request instance for ModifyDBInstanceNetwork.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBInstanceNetworkRequest`
@@ -1791,15 +1791,15 @@
             model = models.ModifyDBInstanceNetworkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceProject(self, request):
         """本接口（ModifyDBInstanceProject）用于修改数据库实例所属项目。
 
         :param request: Request instance for ModifyDBInstanceProject.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBInstanceProjectRequest`
@@ -1814,15 +1814,15 @@
             model = models.ModifyDBInstanceProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceRenewFlag(self, request):
         """本接口（ModifyDBInstanceRenewFlag）用于修改实例续费标记
 
         :param request: Request instance for ModifyDBInstanceRenewFlag.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBInstanceRenewFlagRequest`
@@ -1837,15 +1837,15 @@
             model = models.ModifyDBInstanceRenewFlagResponse()
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
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -1860,15 +1860,15 @@
             model = models.ModifyDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBName(self, request):
         """本接口（ModifyDBName）用于更新数据库名。
 
         :param request: Request instance for ModifyDBName.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBNameRequest`
@@ -1883,15 +1883,15 @@
             model = models.ModifyDBNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBRemark(self, request):
         """本接口（ModifyDBRemark）用于修改数据库备注。
 
         :param request: Request instance for ModifyDBRemark.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDBRemarkRequest`
@@ -1906,15 +1906,15 @@
             model = models.ModifyDBRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatabaseCDC(self, request):
         """本接口(ModifyDatabaseCDC)用于开启、关闭数据库数据变更捕获(CDC)
 
         :param request: Request instance for ModifyDatabaseCDC.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDatabaseCDCRequest`
@@ -1929,15 +1929,15 @@
             model = models.ModifyDatabaseCDCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatabaseCT(self, request):
         """本接口(ModifyDatabaseCT)用于启用、禁用数据库数据变更跟踪(CT)
 
         :param request: Request instance for ModifyDatabaseCT.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDatabaseCTRequest`
@@ -1952,15 +1952,15 @@
             model = models.ModifyDatabaseCTResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDatabaseMdf(self, request):
         """本接口(ModifyDatabaseMdf)用于收缩数据库mdf(Shrink mdf)
 
         :param request: Request instance for ModifyDatabaseMdf.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyDatabaseMdfRequest`
@@ -1975,15 +1975,15 @@
             model = models.ModifyDatabaseMdfResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyIncrementalMigration(self, request):
         """本接口（ModifyIncrementalMigration）用于修改增量备份导入任务。
 
         :param request: Request instance for ModifyIncrementalMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyIncrementalMigrationRequest`
@@ -1998,15 +1998,15 @@
             model = models.ModifyIncrementalMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceEncryptAttributes(self, request):
         """本接口（ModifyInstanceEncryptAttributes）用于开通实例的TDE加密功能。
 
         :param request: Request instance for ModifyInstanceEncryptAttributes.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyInstanceEncryptAttributesRequest`
@@ -2021,15 +2021,15 @@
             model = models.ModifyInstanceEncryptAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceParam(self, request):
         """本接口(ModifyInstanceParam)用于修改云数据库实例的参数。
         <b>注意</b>：如果修改的参数是需要<b>重启实例</b>的，那么实例将会按照WaitSwitch参数的设置(可能是立即执行也可能在可维护时间窗内自动执行)在执行参数修改时<b>重启实例</b>。
         您可以通过DescribeInstanceParams接口查询修改参数时是否会重启实例，以免导致您的实例不符合预期重启。
 
@@ -2046,15 +2046,15 @@
             model = models.ModifyInstanceParamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMaintenanceSpan(self, request):
         """本接口（ModifyMaintenanceSpan）用于修改实例的可维护时间窗
 
         :param request: Request instance for ModifyMaintenanceSpan.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyMaintenanceSpanRequest`
@@ -2069,15 +2069,15 @@
             model = models.ModifyMaintenanceSpanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMigration(self, request):
         """本接口（ModifyMigration）可以修改已有的迁移任务信息
 
         :param request: Request instance for ModifyMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyMigrationRequest`
@@ -2092,15 +2092,15 @@
             model = models.ModifyMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPublishSubscribeName(self, request):
         """本接口（ModifyPublishSubscribeName）修改发布订阅的名称。
 
         :param request: Request instance for ModifyPublishSubscribeName.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyPublishSubscribeNameRequest`
@@ -2115,15 +2115,15 @@
             model = models.ModifyPublishSubscribeNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyReadOnlyGroupDetails(self, request):
         """本接口（ModifyReadOnlyGroupDetails）用于修改只读组详情。
 
         :param request: Request instance for ModifyReadOnlyGroupDetails.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ModifyReadOnlyGroupDetailsRequest`
@@ -2138,15 +2138,15 @@
             model = models.ModifyReadOnlyGroupDetailsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenInterCommunication(self, request):
         """本接口（OpenInterCommunication）用于打开实例的互通，实例互通可以实现商业智能服务相互联通。
 
         :param request: Request instance for OpenInterCommunication.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.OpenInterCommunicationRequest`
@@ -2161,15 +2161,15 @@
             model = models.OpenInterCommunicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryMigrationCheckProcess(self, request):
         """本接口（QueryMigrationCheckProcess）的作用是查询迁移检查任务的进度，适用于迁移源的类型为TencentDB for SQLServer 的迁移方式
 
         :param request: Request instance for QueryMigrationCheckProcess.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.QueryMigrationCheckProcessRequest`
@@ -2184,15 +2184,15 @@
             model = models.QueryMigrationCheckProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecycleDBInstance(self, request):
         """本接口（RecycleDBInstance）用于主动回收已下线的SQLSERVER实例
 
         :param request: Request instance for RecycleDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RecycleDBInstanceRequest`
@@ -2207,15 +2207,15 @@
             model = models.RecycleDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecycleReadOnlyGroup(self, request):
         """本接口（RecycleReadOnlyGroup）立即回收只读组的资源，只读组占用的vip等资源将立即释放且不可找回。
 
         :param request: Request instance for RecycleReadOnlyGroup.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RecycleReadOnlyGroupRequest`
@@ -2230,15 +2230,15 @@
             model = models.RecycleReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveBackups(self, request):
         """本接口（RemoveBackups）可以删除用户手动创建的备份文件。待删除的备份策略可以是实例备份，也可以是多库备份。
 
         :param request: Request instance for RemoveBackups.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RemoveBackupsRequest`
@@ -2253,15 +2253,15 @@
             model = models.RemoveBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDBInstance(self, request):
         """本接口（RenewDBInstance）用于续费实例。当被续费实例是按量计费实例时，则按量计费实例转为包年包月计费方式。
         按量计费实例转包年包月询价可通过(InquiryPriceRenewDBInstance)接口获得。
 
         :param request: Request instance for RenewDBInstance.
@@ -2277,15 +2277,15 @@
             model = models.RenewDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewPostpaidDBInstance(self, request):
         """本接口（RenewPostpaidDBInstance）用于将通过接口TerminateDBInstance手动隔离的按量计费实例从回收站中恢复。
 
         :param request: Request instance for RenewPostpaidDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RenewPostpaidDBInstanceRequest`
@@ -2300,15 +2300,15 @@
             model = models.RenewPostpaidDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAccountPassword(self, request):
         """本接口（ResetAccountPassword）用于重置实例的账户密码。
 
         :param request: Request instance for ResetAccountPassword.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.ResetAccountPasswordRequest`
@@ -2323,15 +2323,15 @@
             model = models.ResetAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartDBInstance(self, request):
         """本接口（RestartDBInstance）用于重启数据库实例。
 
         :param request: Request instance for RestartDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RestartDBInstanceRequest`
@@ -2346,15 +2346,15 @@
             model = models.RestartDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestoreInstance(self, request):
         """本接口（RestoreInstance）用于按照备份集回档数据库。
 
         :param request: Request instance for RestoreInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RestoreInstanceRequest`
@@ -2369,15 +2369,15 @@
             model = models.RestoreInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackInstance(self, request):
         """本接口（RollbackInstance）用于按照时间点回档实例
 
         :param request: Request instance for RollbackInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RollbackInstanceRequest`
@@ -2392,15 +2392,15 @@
             model = models.RollbackInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunMigration(self, request):
         """本接口（RunMigration）用于启动迁移任务，开始迁移
 
         :param request: Request instance for RunMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RunMigrationRequest`
@@ -2415,15 +2415,15 @@
             model = models.RunMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartBackupMigration(self, request):
         """本接口（StartBackupMigration）用于启动备份导入任务。
 
         :param request: Request instance for StartBackupMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartBackupMigrationRequest`
@@ -2438,15 +2438,15 @@
             model = models.StartBackupMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartIncrementalMigration(self, request):
         """本接口（StartIncrementalMigration）用于启动增量备份导入任务。
 
         :param request: Request instance for StartIncrementalMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartIncrementalMigrationRequest`
@@ -2461,15 +2461,15 @@
             model = models.StartIncrementalMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartInstanceXEvent(self, request):
         """本接口（StartInstanceXEvent）用于开启、关闭扩展事件。
 
         :param request: Request instance for StartInstanceXEvent.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartInstanceXEventRequest`
@@ -2484,15 +2484,15 @@
             model = models.StartInstanceXEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartMigrationCheck(self, request):
         """本接口（StartMigrationCheck）的作用是启动一个迁移前的校验任务，适用于迁移源的类型为TencentDB for SQLServer 的迁移方式
 
         :param request: Request instance for StartMigrationCheck.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StartMigrationCheckRequest`
@@ -2507,15 +2507,15 @@
             model = models.StartMigrationCheckResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMigration(self, request):
         """本接口（StopMigration）作用是中止一个迁移任务
 
         :param request: Request instance for StopMigration.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.StopMigrationRequest`
@@ -2530,15 +2530,15 @@
             model = models.StopMigrationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDBInstance(self, request):
         """本接口(TerminateDBInstance)用于主动隔离实例，使得实例进入回收站。
 
         :param request: Request instance for TerminateDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.TerminateDBInstanceRequest`
@@ -2553,15 +2553,15 @@
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
         """本接口（UpgradeDBInstance）用于升级实例
 
         :param request: Request instance for UpgradeDBInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.UpgradeDBInstanceRequest`
@@ -2576,8 +2576,8 @@
             model = models.UpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud/sqlserver/v20180328/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.938/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.937/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.938/README.rst`

 * *Files identical despite different names*

