# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.937.tar", last modified: Tue Jul 18 00:28:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.938.tar", last modified: Wed Jul 19 00:44:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.937.tar` & `tencentcloud-sdk-python-postgres-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20749 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    85776 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   446339 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    86120 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)   446339 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-19 00:44:06.000000 tencentcloud-sdk-python-postgres-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/setup.py` & `tencentcloud-sdk-python-postgres-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddDBInstanceToReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloneDBInstance(self, request):
         """用于克隆实例，支持指定备份集、指定时间点进行克隆。
 
         :param request: Request instance for CloneDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CloneDBInstanceRequest`
@@ -65,15 +65,15 @@
             model = models.CloneDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseDBExtranetAccess(self, request):
         """本接口（CloseDBExtranetAccess）用于关闭实例公网地址。
 
         :param request: Request instance for CloseDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CloseDBExtranetAccessRequest`
@@ -88,15 +88,15 @@
             model = models.CloseDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseServerlessDBExtranetAccess(self, request):
         """本接口（CloseServerlessDBExtranetAccess）用于关闭serverlessDB实例公网地址
 
         :param request: Request instance for CloseServerlessDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CloseServerlessDBExtranetAccessRequest`
@@ -111,15 +111,15 @@
             model = models.CloseServerlessDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBaseBackup(self, request):
         """本接口（CreateBaseBackup）用于创建实例的全量备份。
 
         :param request: Request instance for CreateBaseBackup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateBaseBackupRequest`
@@ -134,15 +134,15 @@
             model = models.CreateBaseBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstanceNetworkAccess(self, request):
         """本接口（CreateDBInstanceNetworkAccess）用于创建实例网络。
 
         :param request: Request instance for CreateDBInstanceNetworkAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateDBInstanceNetworkAccessRequest`
@@ -157,15 +157,15 @@
             model = models.CreateDBInstanceNetworkAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDBInstances(self, request):
         """本接口（CreateDBInstances）用于创建一个或者多个PostgreSQL实例,仅发货实例不会进行初始化。本接口已废弃，推荐使用接口[CreateInstances](https://cloud.tencent.com/document/api/409/56107)替代。
 
         :param request: Request instance for CreateDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateDBInstancesRequest`
@@ -180,15 +180,15 @@
             model = models.CreateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstances(self, request):
         """本接口 (CreateInstances) 用于创建一个或者多个PostgreSQL实例，通过此接口创建的实例无需进行初始化，可直接使用。
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateInstancesRequest`
@@ -203,15 +203,15 @@
             model = models.CreateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateParameterTemplate(self, request):
         """本接口 (CreateParameterTemplate) 用于创建参数模板。
 
         :param request: Request instance for CreateParameterTemplate.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateParameterTemplateRequest`
@@ -226,15 +226,15 @@
             model = models.CreateParameterTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReadOnlyDBInstance(self, request):
         """本接口(CreateReadOnlyDBInstance)用于创建只读实例
 
         :param request: Request instance for CreateReadOnlyDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateReadOnlyDBInstanceRequest`
@@ -249,15 +249,15 @@
             model = models.CreateReadOnlyDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReadOnlyGroup(self, request):
         """本接口（CreateReadOnlyGroup）用于创建只读组
 
         :param request: Request instance for CreateReadOnlyGroup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateReadOnlyGroupRequest`
@@ -272,15 +272,15 @@
             model = models.CreateReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReadOnlyGroupNetworkAccess(self, request):
         """本接口（CreateReadOnlyGroupNetworkAccess）用于创建RO组的网络。
 
         :param request: Request instance for CreateReadOnlyGroupNetworkAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateReadOnlyGroupNetworkAccessRequest`
@@ -295,15 +295,15 @@
             model = models.CreateReadOnlyGroupNetworkAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServerlessDBInstance(self, request):
         """本接口 (CreateServerlessDBInstance) 用于创建一个ServerlessDB实例，创建成功返回实例ID。
 
         :param request: Request instance for CreateServerlessDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateServerlessDBInstanceRequest`
@@ -318,15 +318,15 @@
             model = models.CreateServerlessDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBaseBackup(self, request):
         """本接口（DeleteBaseBackup）用于删除实例指定全量备份。
 
         :param request: Request instance for DeleteBaseBackup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteBaseBackupRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteBaseBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDBInstanceNetworkAccess(self, request):
         """可对实例进行网络的删除操作。
 
         :param request: Request instance for DeleteDBInstanceNetworkAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteDBInstanceNetworkAccessRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteDBInstanceNetworkAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLogBackup(self, request):
         """本接口（DeleteLogBackup）用于删除实例指定日志备份。
 
         :param request: Request instance for DeleteLogBackup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteLogBackupRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteLogBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteParameterTemplate(self, request):
         """本接口（DeleteParameterTemplate）主要用于删除某个参数模板。
 
         :param request: Request instance for DeleteParameterTemplate.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteParameterTemplateRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteParameterTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReadOnlyGroup(self, request):
         """本接口(DeleteReadOnlyGroup)用于删除指定的只读组
 
         :param request: Request instance for DeleteReadOnlyGroup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteReadOnlyGroupRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReadOnlyGroupNetworkAccess(self, request):
         """可对RO组进行网络的删除操作。
 
         :param request: Request instance for DeleteReadOnlyGroupNetworkAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteReadOnlyGroupNetworkAccessRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteReadOnlyGroupNetworkAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServerlessDBInstance(self, request):
         """本接口 (DeleteServerlessDBInstance) 用于删除一个ServerlessDB实例。
 
         :param request: Request instance for DeleteServerlessDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DeleteServerlessDBInstanceRequest`
@@ -479,15 +479,15 @@
             model = models.DeleteServerlessDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccounts(self, request):
         """本接口（DescribeAccounts）用于查询实例的数据库账号列表。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeAccountsRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableRecoveryTime(self, request):
         """本接口（DescribeAvailableRecoveryTime）用于查询实例可恢复的时间范围。
 
         :param request: Request instance for DescribeAvailableRecoveryTime.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeAvailableRecoveryTimeRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeAvailableRecoveryTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupDownloadRestriction(self, request):
         """本接口（DescribeBackupDownloadRestriction）用于查询备份文件下载限制。
 
         :param request: Request instance for DescribeBackupDownloadRestriction.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadRestrictionRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeBackupDownloadRestrictionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupDownloadURL(self, request):
         """本接口 (DescribeBackupDownloadURL) 用于查询指定备份集的下载地址，可包括全量备份集、增量日志备份集。
 
         :param request: Request instance for DescribeBackupDownloadURL.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadURLRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeBackupDownloadURLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupOverview(self, request):
         """本接口（DescribeBackupOverview）用于查询用户的备份概览信息。返回用户当前备份个数、备份占用容量、免费容量、收费容量等信息（容量单位为字节）。
 
         :param request: Request instance for DescribeBackupOverview.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupOverviewRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeBackupOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupPlans(self, request):
         """本接口 (DescribeBackupPlans) 用于实例所有的备份计划查询
 
         :param request: Request instance for DescribeBackupPlans.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupPlansRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeBackupPlansResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupSummaries(self, request):
         """本接口(DescribeBackupSummaries)用于查询实例备份的统计信息，返回以实例为维度的备份个数、占用容量等信息（容量单位为字节）。
 
         :param request: Request instance for DescribeBackupSummaries.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupSummariesRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeBackupSummariesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBaseBackups(self, request):
         """本接口（DescribeBaseBackups）用于查询基础备份列表。
 
         :param request: Request instance for DescribeBaseBackups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBaseBackupsRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeBaseBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClasses(self, request):
         """本接口（DescribeClasses）用于查询实例售卖规格。
 
         :param request: Request instance for DescribeClasses.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeClassesRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeClassesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloneDBInstanceSpec(self, request):
         """本接口（DescribeCloneDBInstanceSpec）用于查询克隆实例可选择的最小规格，包括SpecCode和磁盘。
 
         :param request: Request instance for DescribeCloneDBInstanceSpec.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeCloneDBInstanceSpecRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeCloneDBInstanceSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBBackups(self, request):
         """本接口（DescribeDBBackups）用于查询实例备份列表。本接口已废弃，推荐使用接口[DescribeBaseBackups](https://cloud.tencent.com/document/api/409/89022)替代。
 
         :param request: Request instance for DescribeDBBackups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBBackupsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeDBBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBErrlogs(self, request):
         """本接口（DescribeDBErrlogs）用于查询错误日志。
 
         :param request: Request instance for DescribeDBErrlogs.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBErrlogsRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeDBErrlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceAttribute(self, request):
         """本接口 (DescribeDBInstanceAttribute) 用于查询某个实例的详情信息。
 
         :param request: Request instance for DescribeDBInstanceAttribute.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceAttributeRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeDBInstanceAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceParameters(self, request):
         """本接口（DescribeDBInstanceAttribute）用于查询实例的参数信息。
 
         :param request: Request instance for DescribeDBInstanceParameters.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceParametersRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeDBInstanceParametersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstanceSecurityGroups(self, request):
         """本接口（DescribeDBInstanceSecurityGroups）用于查询实例安全组。
 
         :param request: Request instance for DescribeDBInstanceSecurityGroups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceSecurityGroupsRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBInstances(self, request):
         """本接口 (DescribeDBInstances) 用于查询一个或多个实例的详细信息。
 
         :param request: Request instance for DescribeDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstancesRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSlowlogs(self, request):
         """本接口（DescribeDBSlowlogs）用于获取慢查询日志。本接口已于2021.09.01日废弃，后续此接口将不再返回任何数据，推荐使用接口[DescribeSlowQueryList](https://cloud.tencent.com/document/api/409/60540)替代。
 
         :param request: Request instance for DescribeDBSlowlogs.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBSlowlogsRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeDBSlowlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBVersions(self, request):
         """本接口（DescribeDBVersions）用于查询支持的数据库版本。
 
         :param request: Request instance for DescribeDBVersions.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBVersionsRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeDBVersionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBXlogs(self, request):
         """本接口（DescribeDBXlogs）用于获取实例Xlog列表。本接口已废弃，推荐使用接口[DescribeLogBackups](https://cloud.tencent.com/document/api/409/89021)替代。
 
         :param request: Request instance for DescribeDBXlogs.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBXlogsRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeDBXlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDatabases(self, request):
         """接口（DescribeDatabases）用来查询实例的数据库列表。
 
         :param request: Request instance for DescribeDatabases.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDatabasesRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDefaultParameters(self, request):
         """本接口（DescribeDefaultParameters）主要用于查询某个数据库版本和引擎支持的所有参数。
 
         :param request: Request instance for DescribeDefaultParameters.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDefaultParametersRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeDefaultParametersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEncryptionKeys(self, request):
         """本接口 （DescribeEncryptionKeys） 用于查询实例的密钥信息列表。
 
         :param request: Request instance for DescribeEncryptionKeys.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeEncryptionKeysRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeEncryptionKeysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLogBackups(self, request):
         """本接口（DescribeLogBackups）用于查询日志备份列表。
 
         :param request: Request instance for DescribeLogBackups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeLogBackupsRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeLogBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrders(self, request):
         """本接口（DescribeOrders）用于查询订单信息。
 
         :param request: Request instance for DescribeOrders.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeOrdersRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParameterTemplateAttributes(self, request):
         """本接口（DescribeParameterTemplateAttributes）用于查询某个参数模板的具体内容，包括基本信息和参数信息。
 
         :param request: Request instance for DescribeParameterTemplateAttributes.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeParameterTemplateAttributesRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeParameterTemplateAttributesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParameterTemplates(self, request):
         """本接口 (DescribeParameterTemplates) 用于查询参数模板列表。
 
         :param request: Request instance for DescribeParameterTemplates.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeParameterTemplatesRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeParameterTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParamsEvent(self, request):
         """本接口（DescribeParamsEvent）用于查询参数修改事件。
 
         :param request: Request instance for DescribeParamsEvent.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeParamsEventRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeParamsEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductConfig(self, request):
         """本接口（DescribeProductConfig）用于查询售卖规格配置。本接口已废弃，推荐使用新接口[DescribeClasses](https://cloud.tencent.com/document/api/409/89019)。
 
         :param request: Request instance for DescribeProductConfig.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeProductConfigRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeProductConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReadOnlyGroups(self, request):
         """本接口（DescribeReadOnlyGroups）用于查询只读组列表
 
         :param request: Request instance for DescribeReadOnlyGroups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeReadOnlyGroupsRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeReadOnlyGroupsResponse()
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
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeRegionsRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServerlessDBInstances(self, request):
         """用于查询一个或多个serverlessDB实例的详细信息
 
         :param request: Request instance for DescribeServerlessDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeServerlessDBInstancesRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeServerlessDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowQueryAnalysis(self, request):
         """此接口（DescribeSlowQueryAnalysis）用于统计指定时间范围内的所有慢查询，根据SQL语句抽象参数后，进行聚合分析，并返回同类SQL列表。
 
         :param request: Request instance for DescribeSlowQueryAnalysis.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeSlowQueryAnalysisRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeSlowQueryAnalysisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowQueryList(self, request):
         """此接口（DescribeSlowQueryList）用于查询指定时间范围内的所有慢查询。
 
         :param request: Request instance for DescribeSlowQueryList.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeSlowQueryListRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeSlowQueryListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """本接口 (DescribeZones) 用于查询支持的可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeZonesRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DestroyDBInstance(self, request):
         """本接口 (DestroyDBInstance) 用于彻底销毁指定DBInstanceId对应的实例，销毁后实例数据将彻底删除，无法找回，调用前请仔细确认要操作的实例。只能销毁隔离中的实例。
 
         :param request: Request instance for DestroyDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DestroyDBInstanceRequest`
@@ -1284,15 +1284,15 @@
             model = models.DestroyDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisIsolateDBInstances(self, request):
         """本接口（DisIsolateDBInstances）用于解隔离实例
 
         :param request: Request instance for DisIsolateDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DisIsolateDBInstancesRequest`
@@ -1307,15 +1307,15 @@
             model = models.DisIsolateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InitDBInstances(self, request):
         """本接口（InitDBInstances）用于初始化云数据库PostgreSQL实例。本接口已废弃，推荐使用接口[CreateInstances](https://cloud.tencent.com/document/api/409/56107)替代。
 
         :param request: Request instance for InitDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.InitDBInstancesRequest`
@@ -1330,15 +1330,15 @@
             model = models.InitDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateDBInstances(self, request):
         """本接口 (InquiryPriceCreateDBInstances) 用于查询购买实例的价格信息。
 
         :param request: Request instance for InquiryPriceCreateDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.InquiryPriceCreateDBInstancesRequest`
@@ -1353,15 +1353,15 @@
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
         """本接口（InquiryPriceRenewDBInstance）用于查询续费实例的价格。
 
         :param request: Request instance for InquiryPriceRenewDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.InquiryPriceRenewDBInstanceRequest`
@@ -1376,15 +1376,15 @@
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
         """本接口（InquiryPriceUpgradeDBInstance）用于查询升级实例的价格。只支持按量计费实例。
 
         :param request: Request instance for InquiryPriceUpgradeDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.InquiryPriceUpgradeDBInstanceRequest`
@@ -1399,15 +1399,15 @@
             model = models.InquiryPriceUpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDBInstances(self, request):
         """本接口（IsolateDBInstances）用于隔离实例。
 
         :param request: Request instance for IsolateDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.IsolateDBInstancesRequest`
@@ -1422,15 +1422,15 @@
             model = models.IsolateDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountRemark(self, request):
         """本接口（ModifyAccountRemark）用于修改帐号备注。
 
         :param request: Request instance for ModifyAccountRemark.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyAccountRemarkRequest`
@@ -1445,15 +1445,15 @@
             model = models.ModifyAccountRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupDownloadRestriction(self, request):
         """本接口（ModifyBackupDownloadRestriction）用于修改备份文件下载限制。
 
         :param request: Request instance for ModifyBackupDownloadRestriction.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupDownloadRestrictionRequest`
@@ -1468,15 +1468,15 @@
             model = models.ModifyBackupDownloadRestrictionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupPlan(self, request):
         """本接口 (ModifyBackupPlan) 用于实例备份计划的修改，默认是在每天的凌晨开始全量备份，备份保留时长是7天。可以根据此接口指定时间进行实例的备份。
 
         :param request: Request instance for ModifyBackupPlan.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupPlanRequest`
@@ -1491,15 +1491,15 @@
             model = models.ModifyBackupPlanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBaseBackupExpireTime(self, request):
         """本接口（ModifyBaseBackupExpireTime）用于修改实例指定全量备份的过期时间。
 
         :param request: Request instance for ModifyBaseBackupExpireTime.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyBaseBackupExpireTimeRequest`
@@ -1514,15 +1514,15 @@
             model = models.ModifyBaseBackupExpireTimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceChargeType(self, request):
         """支持实例的计费类型转换（目前仅支持按量计费转包年包月）
 
         :param request: Request instance for ModifyDBInstanceChargeType.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceChargeTypeRequest`
@@ -1537,15 +1537,15 @@
             model = models.ModifyDBInstanceChargeTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceDeployment(self, request):
         """本接口（ModifyDBInstanceDeployment）用于修改节点可用区部署方式，仅支持主实例。
 
         :param request: Request instance for ModifyDBInstanceDeployment.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceDeploymentRequest`
@@ -1560,15 +1560,15 @@
             model = models.ModifyDBInstanceDeploymentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceName(self, request):
         """本接口（ModifyDBInstanceName）用于修改postgresql实例名字。
 
         :param request: Request instance for ModifyDBInstanceName.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceNameRequest`
@@ -1583,15 +1583,15 @@
             model = models.ModifyDBInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceParameters(self, request):
         """本接口 (ModifyDBInstanceParameters) 用于修改实例参数。
 
         :param request: Request instance for ModifyDBInstanceParameters.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceParametersRequest`
@@ -1606,15 +1606,15 @@
             model = models.ModifyDBInstanceParametersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceReadOnlyGroup(self, request):
         """本接口（ModifyDBInstanceReadOnlyGroup）用于修改实例所属的只读组
 
         :param request: Request instance for ModifyDBInstanceReadOnlyGroup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceReadOnlyGroupRequest`
@@ -1629,15 +1629,15 @@
             model = models.ModifyDBInstanceReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSecurityGroups(self, request):
         """本接口（ModifyDBInstanceSecurityGroups）用于修改实例安全组。
 
         :param request: Request instance for ModifyDBInstanceSecurityGroups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -1652,15 +1652,15 @@
             model = models.ModifyDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstanceSpec(self, request):
         """本接口（ModifyDBInstanceSpec）用于修改实例规格，包括内存、磁盘。
 
         :param request: Request instance for ModifyDBInstanceSpec.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceSpecRequest`
@@ -1675,15 +1675,15 @@
             model = models.ModifyDBInstanceSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDBInstancesProject(self, request):
         """本接口（ModifyDBInstancesProject）用于修改实例所属项目。
 
         :param request: Request instance for ModifyDBInstancesProject.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstancesProjectRequest`
@@ -1698,15 +1698,15 @@
             model = models.ModifyDBInstancesProjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyParameterTemplate(self, request):
         """本接口（ModifyParameterTemplate）主要用于修改参数模板名称，描述等配置，也可用于管理参数模板中的参数列表。
 
         :param request: Request instance for ModifyParameterTemplate.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyParameterTemplateRequest`
@@ -1721,15 +1721,15 @@
             model = models.ModifyParameterTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyReadOnlyGroupConfig(self, request):
         """本接口(ModifyReadOnlyGroupConfig)用于更新只读组配置信息
 
         :param request: Request instance for ModifyReadOnlyGroupConfig.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyReadOnlyGroupConfigRequest`
@@ -1744,15 +1744,15 @@
             model = models.ModifyReadOnlyGroupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySwitchTimePeriod(self, request):
         """当升级完成后，对处于等待切换状态下的实例，强制实例立即切换。
 
         :param request: Request instance for ModifySwitchTimePeriod.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifySwitchTimePeriodRequest`
@@ -1767,15 +1767,15 @@
             model = models.ModifySwitchTimePeriodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenDBExtranetAccess(self, request):
         """本接口（OpenDBExtranetAccess）用于开通实例公网地址。
 
         :param request: Request instance for OpenDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.OpenDBExtranetAccessRequest`
@@ -1790,15 +1790,15 @@
             model = models.OpenDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenServerlessDBExtranetAccess(self, request):
         """本接口（OpenServerlessDBExtranetAccess）用于开通serverlessDB实例公网地址。
 
         :param request: Request instance for OpenServerlessDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.OpenServerlessDBExtranetAccessRequest`
@@ -1813,15 +1813,15 @@
             model = models.OpenServerlessDBExtranetAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebalanceReadOnlyGroup(self, request):
         """本接口(RebalanceReadOnlyGroup)用于重新均衡 RO 组内实例的负载。注意，RO 组内 RO 实例会有一次数据库连接瞬断，请确保应用程序能重连数据库，谨慎操作。
 
         :param request: Request instance for RebalanceReadOnlyGroup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.RebalanceReadOnlyGroupRequest`
@@ -1836,15 +1836,15 @@
             model = models.RebalanceReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveDBInstanceFromReadOnlyGroup(self, request):
         """本接口（RemoveDBInstanceFromReadOnlyGroup）用户将只读实例从只读组中移除
 
         :param request: Request instance for RemoveDBInstanceFromReadOnlyGroup.
         :type request: :class:`tencentcloud.postgres.v20170312.models.RemoveDBInstanceFromReadOnlyGroupRequest`
@@ -1859,15 +1859,15 @@
             model = models.RemoveDBInstanceFromReadOnlyGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstance(self, request):
         """本接口（RenewInstance）用于续费实例。
 
         :param request: Request instance for RenewInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.RenewInstanceRequest`
@@ -1882,15 +1882,15 @@
             model = models.RenewInstanceResponse()
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
         :type request: :class:`tencentcloud.postgres.v20170312.models.ResetAccountPasswordRequest`
@@ -1905,15 +1905,15 @@
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
         """本接口（RestartDBInstance）用于重启实例。
 
         :param request: Request instance for RestartDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.RestartDBInstanceRequest`
@@ -1928,15 +1928,15 @@
             model = models.RestartDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetAutoRenewFlag(self, request):
         """本接口（SetAutoRenewFlag）用于设置自动续费。
 
         :param request: Request instance for SetAutoRenewFlag.
         :type request: :class:`tencentcloud.postgres.v20170312.models.SetAutoRenewFlagRequest`
@@ -1951,15 +1951,15 @@
             model = models.SetAutoRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDBInstance(self, request):
         """本接口（UpgradeDBInstance）用于升级实例配置。本接口已废弃，推荐使用接口[ModifyDBInstanceSpec](https://cloud.tencent.com/document/api/409/63689)替代。
 
         :param request: Request instance for UpgradeDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.UpgradeDBInstanceRequest`
@@ -1974,15 +1974,15 @@
             model = models.UpgradeDBInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeDBInstanceKernelVersion(self, request):
         """本接口（UpgradeDBInstanceKernelVersion）用于升级实例的内核版本号。
 
         :param request: Request instance for UpgradeDBInstanceKernelVersion.
         :type request: :class:`tencentcloud.postgres.v20170312.models.UpgradeDBInstanceKernelVersionRequest`
@@ -1997,8 +1997,8 @@
             model = models.UpgradeDBInstanceKernelVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.938/tencentcloud/postgres/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.938/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.937/README.rst` & `tencentcloud-sdk-python-postgres-3.0.938/README.rst`

 * *Files identical despite different names*

