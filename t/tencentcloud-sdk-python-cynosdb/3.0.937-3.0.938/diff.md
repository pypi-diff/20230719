# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.937.tar", last modified: Tue Jul 18 00:21:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.938.tar", last modified: Wed Jul 19 00:37:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.937.tar` & `tencentcloud-sdk-python-cynosdb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)   118494 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11292 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   684756 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:49.000000 tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   119006 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   684756 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:37:01.000000 tencentcloud-sdk-python-cynosdb-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:02.000000 tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ActivateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddClusterSlaveZone(self, request):
         """增加从可用区
 
         :param request: Request instance for AddClusterSlaveZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.AddClusterSlaveZoneRequest`
@@ -65,15 +65,15 @@
             model = models.AddClusterSlaveZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AddInstances(self, request):
         """本接口（AddInstances）用于集群添加实例
 
         :param request: Request instance for AddInstances.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.AddInstancesRequest`
@@ -88,15 +88,15 @@
             model = models.AddInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSecurityGroups(self, request):
         """安全组批量绑定云资源
 
         :param request: Request instance for AssociateSecurityGroups.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.AssociateSecurityGroupsRequest`
@@ -111,15 +111,15 @@
             model = models.AssociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BindClusterResourcePackages(self, request):
         """为集群绑定资源包
 
         :param request: Request instance for BindClusterResourcePackages.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.BindClusterResourcePackagesRequest`
@@ -134,15 +134,15 @@
             model = models.BindClusterResourcePackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseAuditService(self, request):
         """TDSQL-C for MySQL实例关闭审计服务
 
         :param request: Request instance for CloseAuditService.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseAuditServiceRequest`
@@ -157,15 +157,15 @@
             model = models.CloseAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseClusterPasswordComplexity(self, request):
         """本接口（CloseClusterPasswordComplexity）用于关闭集群密码复杂度
 
         :param request: Request instance for CloseClusterPasswordComplexity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseClusterPasswordComplexityRequest`
@@ -180,15 +180,15 @@
             model = models.CloseClusterPasswordComplexityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseProxy(self, request):
         """关闭数据库代理
 
         :param request: Request instance for CloseProxy.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseProxyRequest`
@@ -203,15 +203,15 @@
             model = models.CloseProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseWan(self, request):
         """本接口（CloseWan）用于关闭外网
 
         :param request: Request instance for CloseWan.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseWanRequest`
@@ -226,15 +226,15 @@
             model = models.CloseWanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CopyClusterPasswordComplexity(self, request):
         """本接口（CopyClusterPasswordComplexity）用于复制集群密码复杂度
 
         :param request: Request instance for CopyClusterPasswordComplexity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CopyClusterPasswordComplexityRequest`
@@ -249,15 +249,15 @@
             model = models.CopyClusterPasswordComplexityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAccounts(self, request):
         """创建账号
 
         :param request: Request instance for CreateAccounts.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateAccountsRequest`
@@ -272,15 +272,15 @@
             model = models.CreateAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAuditLogFile(self, request):
         """本接口(CreateAuditLogFile)用于创建云数据库实例的审计日志文件。
 
         :param request: Request instance for CreateAuditLogFile.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateAuditLogFileRequest`
@@ -295,15 +295,15 @@
             model = models.CreateAuditLogFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAuditRuleTemplate(self, request):
         """创建审计规则模版
 
         :param request: Request instance for CreateAuditRuleTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateAuditRuleTemplateRequest`
@@ -318,15 +318,15 @@
             model = models.CreateAuditRuleTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackup(self, request):
         """为集群创建手动备份
 
         :param request: Request instance for CreateBackup.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateBackupRequest`
@@ -341,15 +341,15 @@
             model = models.CreateBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusterDatabase(self, request):
         """创建数据库
 
         :param request: Request instance for CreateClusterDatabase.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateClusterDatabaseRequest`
@@ -364,15 +364,15 @@
             model = models.CreateClusterDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateClusters(self, request):
         """创建集群
 
         :param request: Request instance for CreateClusters.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateClustersRequest`
@@ -387,15 +387,15 @@
             model = models.CreateClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateParamTemplate(self, request):
         """本接口（CreateParamTemplate）用于创建参数模板
 
         :param request: Request instance for CreateParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateParamTemplateRequest`
@@ -410,15 +410,15 @@
             model = models.CreateParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxy(self, request):
         """创建数据库代理
 
         :param request: Request instance for CreateProxy.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyRequest`
@@ -433,15 +433,15 @@
             model = models.CreateProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateProxyEndPoint(self, request):
         """创建数据库代理连接点
 
         :param request: Request instance for CreateProxyEndPoint.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyEndPointRequest`
@@ -456,15 +456,15 @@
             model = models.CreateProxyEndPointResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateResourcePackage(self, request):
         """新购资源包
 
         :param request: Request instance for CreateResourcePackage.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateResourcePackageRequest`
@@ -479,15 +479,15 @@
             model = models.CreateResourcePackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAccounts(self, request):
         """删除账号
 
         :param request: Request instance for DeleteAccounts.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteAccountsRequest`
@@ -502,15 +502,15 @@
             model = models.DeleteAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAuditLogFile(self, request):
         """本接口(DeleteAuditLogFile)用于删除云数据库实例的审计日志文件。
 
         :param request: Request instance for DeleteAuditLogFile.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteAuditLogFileRequest`
@@ -525,15 +525,15 @@
             model = models.DeleteAuditLogFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAuditRuleTemplates(self, request):
         """删除审计规则模版
 
         :param request: Request instance for DeleteAuditRuleTemplates.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteAuditRuleTemplatesRequest`
@@ -548,15 +548,15 @@
             model = models.DeleteAuditRuleTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBackup(self, request):
         """为集群删除手动备份，无法删除自动备份
 
         :param request: Request instance for DeleteBackup.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteBackupRequest`
@@ -571,15 +571,15 @@
             model = models.DeleteBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteClusterDatabase(self, request):
         """删除数据库
 
         :param request: Request instance for DeleteClusterDatabase.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteClusterDatabaseRequest`
@@ -594,15 +594,15 @@
             model = models.DeleteClusterDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteParamTemplate(self, request):
         """本接口（DeleteParamTemplate）用于删除用户创建的参数模板。
 
         :param request: Request instance for DeleteParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteParamTemplateRequest`
@@ -617,15 +617,15 @@
             model = models.DeleteParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountAllGrantPrivileges(self, request):
         """账号所有权限
 
         :param request: Request instance for DescribeAccountAllGrantPrivileges.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAccountAllGrantPrivilegesRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeAccountAllGrantPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccountPrivileges(self, request):
         """查询账号已有权限
 
         :param request: Request instance for DescribeAccountPrivileges.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAccountPrivilegesRequest`
@@ -663,15 +663,15 @@
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
         """本接口(DescribeAccounts)用于查询数据库管理账号。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAccountsRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeAccountsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditLogFiles(self, request):
         """本接口(DescribeAuditLogFiles)用于查询云数据库实例的审计日志文件。
 
         :param request: Request instance for DescribeAuditLogFiles.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAuditLogFilesRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeAuditLogFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditLogs(self, request):
         """本接口(DescribeAuditLogs)用于查询数据库审计日志。
 
         :param request: Request instance for DescribeAuditLogs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAuditLogsRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeAuditLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditRuleTemplates(self, request):
         """查询审计规则模版信息
 
         :param request: Request instance for DescribeAuditRuleTemplates.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAuditRuleTemplatesRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeAuditRuleTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuditRuleWithInstanceIds(self, request):
         """获取实例的审计规则
 
         :param request: Request instance for DescribeAuditRuleWithInstanceIds.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeAuditRuleWithInstanceIdsRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeAuditRuleWithInstanceIdsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupConfig(self, request):
         """获取指定集群的备份配置信息，包括全量备份时间段，备份文件保留时间
 
         :param request: Request instance for DescribeBackupConfig.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBackupConfigRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupDownloadUrl(self, request):
         """此接口（DescribeBackupDownloadUrl）用于查询集群备份文件下载地址。
 
         :param request: Request instance for DescribeBackupDownloadUrl.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBackupDownloadUrlRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeBackupDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupList(self, request):
         """查询备份文件列表
 
         :param request: Request instance for DescribeBackupList.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBackupListRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeBackupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBinlogDownloadUrl(self, request):
         """此接口（DescribeBinlogDownloadUrl）用于查询Binlog的下载地址。
 
         :param request: Request instance for DescribeBinlogDownloadUrl.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBinlogDownloadUrlRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeBinlogDownloadUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBinlogSaveDays(self, request):
         """此接口（DescribeBinlogSaveDays）用于查询集群的Binlog保留天数。
 
         :param request: Request instance for DescribeBinlogSaveDays.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBinlogSaveDaysRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeBinlogSaveDaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBinlogs(self, request):
         """此接口（DescribeBinlogs）用来查询集群Binlog日志列表。
 
         :param request: Request instance for DescribeBinlogs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeBinlogsRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeBinlogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterDetail(self, request):
         """该接口（DescribeClusterDetail）显示集群详情
 
         :param request: Request instance for DescribeClusterDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterDetailRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeClusterDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterDetailDatabases(self, request):
         """查询数据库列表
 
         :param request: Request instance for DescribeClusterDetailDatabases.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterDetailDatabasesRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeClusterDetailDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterInstanceGrps(self, request):
         """本接口（DescribeClusterInstanceGrps）用于查询实例组信息。
 
         :param request: Request instance for DescribeClusterInstanceGrps.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterInstanceGrpsRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeClusterInstanceGrpsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterParamLogs(self, request):
         """本接口（DescribeClusterParamLogs）查询参数修改日志
 
         :param request: Request instance for DescribeClusterParamLogs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterParamLogsRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeClusterParamLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterParams(self, request):
         """本接口（DescribeClusterParams）用于查询集群参数
 
         :param request: Request instance for DescribeClusterParams.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterParamsRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeClusterParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterPasswordComplexity(self, request):
         """本接口（DescribeClusterPasswordComplexity）用于查看集群密码复杂度详情
 
         :param request: Request instance for DescribeClusterPasswordComplexity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClusterPasswordComplexityRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeClusterPasswordComplexityResponse()
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
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeClustersRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSecurityGroups(self, request):
         """查询实例安全组信息
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeDBSecurityGroupsRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeDBSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlow(self, request):
         """本接口（DescribeFlow）用于查询任务流信息
 
         :param request: Request instance for DescribeFlow.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeFlowRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceDetail(self, request):
         """本接口(DescribeInstanceDetail)用于查询实例详情。
 
         :param request: Request instance for DescribeInstanceDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceDetailRequest`
@@ -1146,15 +1146,15 @@
             model = models.DescribeInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceErrorLogs(self, request):
         """查询实例错误日志列表
 
         :param request: Request instance for DescribeInstanceErrorLogs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceErrorLogsRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeInstanceErrorLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceParams(self, request):
         """该接口(DescribeInstanceParams)查询实例参数列表
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceParamsRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceSlowQueries(self, request):
         """此接口（DescribeInstanceSlowQueries）用于查询实例慢查询日志。
 
         :param request: Request instance for DescribeInstanceSlowQueries.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceSlowQueriesRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeInstanceSlowQueriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceSpecs(self, request):
         """本接口（DescribeInstanceSpecs）用于查询实例规格
 
         :param request: Request instance for DescribeInstanceSpecs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceSpecsRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeInstanceSpecsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口(DescribeInstances)用于查询实例列表。
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstancesRequest`
@@ -1261,15 +1261,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMaintainPeriod(self, request):
         """查询实例维护时间窗
 
         :param request: Request instance for DescribeMaintainPeriod.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeMaintainPeriodRequest`
@@ -1284,15 +1284,15 @@
             model = models.DescribeMaintainPeriodResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParamTemplateDetail(self, request):
         """本接口（DescribeParamTemplateDetail）用于查询用户参数模板详情
 
         :param request: Request instance for DescribeParamTemplateDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeParamTemplateDetailRequest`
@@ -1307,15 +1307,15 @@
             model = models.DescribeParamTemplateDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParamTemplates(self, request):
         """查询用户指定产品下的所有参数模板信息
 
         :param request: Request instance for DescribeParamTemplates.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeParamTemplatesRequest`
@@ -1330,15 +1330,15 @@
             model = models.DescribeParamTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectSecurityGroups(self, request):
         """查询项目安全组信息
 
         :param request: Request instance for DescribeProjectSecurityGroups.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProjectSecurityGroupsRequest`
@@ -1353,15 +1353,15 @@
             model = models.DescribeProjectSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxies(self, request):
         """查询数据库代理列表
 
         :param request: Request instance for DescribeProxies.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxiesRequest`
@@ -1376,15 +1376,15 @@
             model = models.DescribeProxiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxyNodes(self, request):
         """本接口（DescribeProxyNodes）用于查询代理接口列表。
 
         :param request: Request instance for DescribeProxyNodes.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxyNodesRequest`
@@ -1399,15 +1399,15 @@
             model = models.DescribeProxyNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProxySpecs(self, request):
         """查询数据库代理规格
 
         :param request: Request instance for DescribeProxySpecs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxySpecsRequest`
@@ -1422,15 +1422,15 @@
             model = models.DescribeProxySpecsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcePackageDetail(self, request):
         """查询资源包使用详情
 
         :param request: Request instance for DescribeResourcePackageDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageDetailRequest`
@@ -1445,15 +1445,15 @@
             model = models.DescribeResourcePackageDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcePackageList(self, request):
         """查询资源包列表
 
         :param request: Request instance for DescribeResourcePackageList.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageListRequest`
@@ -1468,15 +1468,15 @@
             model = models.DescribeResourcePackageListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcePackageSaleSpec(self, request):
         """查询资源包规格
 
         :param request: Request instance for DescribeResourcePackageSaleSpec.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageSaleSpecRequest`
@@ -1491,15 +1491,15 @@
             model = models.DescribeResourcePackageSaleSpecResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourcesByDealName(self, request):
         """根据计费订单id查询资源列表
 
         :param request: Request instance for DescribeResourcesByDealName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcesByDealNameRequest`
@@ -1514,15 +1514,15 @@
             model = models.DescribeResourcesByDealNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRollbackTimeRange(self, request):
         """查询指定集群有效回滚时间范围
 
         :param request: Request instance for DescribeRollbackTimeRange.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeRollbackTimeRangeRequest`
@@ -1537,15 +1537,15 @@
             model = models.DescribeRollbackTimeRangeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRollbackTimeValidity(self, request):
         """指定时间和集群查询是否可回滚
 
         :param request: Request instance for DescribeRollbackTimeValidity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeRollbackTimeValidityRequest`
@@ -1560,15 +1560,15 @@
             model = models.DescribeRollbackTimeValidityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSupportProxyVersion(self, request):
         """查询支持的数据库代理版本
 
         :param request: Request instance for DescribeSupportProxyVersion.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeSupportProxyVersionRequest`
@@ -1583,15 +1583,15 @@
             model = models.DescribeSupportProxyVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """本接口(DescribeZones)用于查询可售卖地域可用区信息。
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeZonesRequest`
@@ -1606,15 +1606,15 @@
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
         """安全组批量解绑云资源
 
         :param request: Request instance for DisassociateSecurityGroups.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DisassociateSecurityGroupsRequest`
@@ -1629,15 +1629,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportInstanceErrorLogs(self, request):
         """此接口（ExportInstanceErrorLogs）用于导出实例错误日志。
 
         :param request: Request instance for ExportInstanceErrorLogs.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ExportInstanceErrorLogsRequest`
@@ -1652,15 +1652,15 @@
             model = models.ExportInstanceErrorLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExportInstanceSlowQueries(self, request):
         """此接口（ExportInstanceSlowQueries）用于导出实例慢日志。
 
         :param request: Request instance for ExportInstanceSlowQueries.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ExportInstanceSlowQueriesRequest`
@@ -1675,15 +1675,15 @@
             model = models.ExportInstanceSlowQueriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GrantAccountPrivileges(self, request):
         """批量授权账号权限
 
         :param request: Request instance for GrantAccountPrivileges.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.GrantAccountPrivilegesRequest`
@@ -1698,15 +1698,15 @@
             model = models.GrantAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreate(self, request):
         """查询新购集群价格
 
         :param request: Request instance for InquirePriceCreate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.InquirePriceCreateRequest`
@@ -1721,15 +1721,15 @@
             model = models.InquirePriceCreateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceRenew(self, request):
         """查询续费集群价格
 
         :param request: Request instance for InquirePriceRenew.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.InquirePriceRenewRequest`
@@ -1744,15 +1744,15 @@
             model = models.InquirePriceRenewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateCluster(self, request):
         """隔离集群
 
         :param request: Request instance for IsolateCluster.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.IsolateClusterRequest`
@@ -1767,15 +1767,15 @@
             model = models.IsolateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateInstance(self, request):
         """本接口(IsolateInstance)用于隔离实例。
 
         :param request: Request instance for IsolateInstance.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.IsolateInstanceRequest`
@@ -1790,15 +1790,15 @@
             model = models.IsolateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountDescription(self, request):
         """本接口(ModifyAccountDescription)用于修改数据库账号描述信息。
 
         :param request: Request instance for ModifyAccountDescription.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAccountDescriptionRequest`
@@ -1813,15 +1813,15 @@
             model = models.ModifyAccountDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountHost(self, request):
         """修改账号主机
 
         :param request: Request instance for ModifyAccountHost.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAccountHostRequest`
@@ -1836,15 +1836,15 @@
             model = models.ModifyAccountHostResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountParams(self, request):
         """修改账号参数
 
         :param request: Request instance for ModifyAccountParams.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAccountParamsRequest`
@@ -1859,15 +1859,15 @@
             model = models.ModifyAccountParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccountPrivileges(self, request):
         """修改账号权限
 
         :param request: Request instance for ModifyAccountPrivileges.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAccountPrivilegesRequest`
@@ -1882,15 +1882,15 @@
             model = models.ModifyAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAuditRuleTemplates(self, request):
         """修改审计规则模版
 
         :param request: Request instance for ModifyAuditRuleTemplates.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAuditRuleTemplatesRequest`
@@ -1905,15 +1905,15 @@
             model = models.ModifyAuditRuleTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAuditService(self, request):
         """本接口(ModifyAuditService)用于修改云数据库审计日志保存时长、审计规则等服务配置。
 
         :param request: Request instance for ModifyAuditService.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyAuditServiceRequest`
@@ -1928,15 +1928,15 @@
             model = models.ModifyAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupConfig(self, request):
         """修改指定集群的备份配置
 
         :param request: Request instance for ModifyBackupConfig.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyBackupConfigRequest`
@@ -1951,15 +1951,15 @@
             model = models.ModifyBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupName(self, request):
         """此接口（ModifyBackupName）用于修改备份文件备注名。
 
         :param request: Request instance for ModifyBackupName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyBackupNameRequest`
@@ -1974,15 +1974,15 @@
             model = models.ModifyBackupNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBinlogSaveDays(self, request):
         """此接口（ModifyBinlogSaveDays）用于修改集群Binlog保留天数。
 
         :param request: Request instance for ModifyBinlogSaveDays.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyBinlogSaveDaysRequest`
@@ -1997,15 +1997,15 @@
             model = models.ModifyBinlogSaveDaysResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterDatabase(self, request):
         """修改数据库
 
         :param request: Request instance for ModifyClusterDatabase.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterDatabaseRequest`
@@ -2020,15 +2020,15 @@
             model = models.ModifyClusterDatabaseResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterName(self, request):
         """修改集群名称
 
         :param request: Request instance for ModifyClusterName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterNameRequest`
@@ -2043,15 +2043,15 @@
             model = models.ModifyClusterNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterParam(self, request):
         """修改集群参数
 
         :param request: Request instance for ModifyClusterParam.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterParamRequest`
@@ -2066,15 +2066,15 @@
             model = models.ModifyClusterParamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterPasswordComplexity(self, request):
         """本接口（ModifyClusterPasswordComplexity）用于修改/开启集群密码复杂度
 
         :param request: Request instance for ModifyClusterPasswordComplexity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterPasswordComplexityRequest`
@@ -2089,15 +2089,15 @@
             model = models.ModifyClusterPasswordComplexityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterSlaveZone(self, request):
         """修改从可用区
 
         :param request: Request instance for ModifyClusterSlaveZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterSlaveZoneRequest`
@@ -2112,15 +2112,15 @@
             model = models.ModifyClusterSlaveZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterStorage(self, request):
         """升级预付费存储
 
         :param request: Request instance for ModifyClusterStorage.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyClusterStorageRequest`
@@ -2135,15 +2135,15 @@
             model = models.ModifyClusterStorageResponse()
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
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyDBInstanceSecurityGroupsRequest`
@@ -2158,15 +2158,15 @@
             model = models.ModifyDBInstanceSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceName(self, request):
         """本接口(ModifyInstanceName)用于修改实例名称。
 
         :param request: Request instance for ModifyInstanceName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyInstanceNameRequest`
@@ -2181,15 +2181,15 @@
             model = models.ModifyInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceParam(self, request):
         """本接口（ModifyInstanceParam）用于修改实例参数。
 
         :param request: Request instance for ModifyInstanceParam.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyInstanceParamRequest`
@@ -2204,15 +2204,15 @@
             model = models.ModifyInstanceParamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMaintainPeriodConfig(self, request):
         """修改维护时间配置
 
         :param request: Request instance for ModifyMaintainPeriodConfig.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyMaintainPeriodConfigRequest`
@@ -2227,15 +2227,15 @@
             model = models.ModifyMaintainPeriodConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyParamTemplate(self, request):
         """本接口（ModifyParamTemplate）用于修改用户参数模板。
 
         :param request: Request instance for ModifyParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyParamTemplateRequest`
@@ -2250,15 +2250,15 @@
             model = models.ModifyParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxyDesc(self, request):
         """修改数据库代理描述
 
         :param request: Request instance for ModifyProxyDesc.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyDescRequest`
@@ -2273,15 +2273,15 @@
             model = models.ModifyProxyDescResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyProxyRwSplit(self, request):
         """配置数据库代理读写分离
 
         :param request: Request instance for ModifyProxyRwSplit.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyRwSplitRequest`
@@ -2296,15 +2296,15 @@
             model = models.ModifyProxyRwSplitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourcePackageClusters(self, request):
         """给资源包绑定集群
 
         :param request: Request instance for ModifyResourcePackageClusters.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageClustersRequest`
@@ -2319,15 +2319,15 @@
             model = models.ModifyResourcePackageClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourcePackageName(self, request):
         """修改资源包名称
 
         :param request: Request instance for ModifyResourcePackageName.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageNameRequest`
@@ -2342,15 +2342,15 @@
             model = models.ModifyResourcePackageNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVipVport(self, request):
         """修改实例组ip，端口
 
         :param request: Request instance for ModifyVipVport.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyVipVportRequest`
@@ -2365,15 +2365,15 @@
             model = models.ModifyVipVportResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OfflineCluster(self, request):
         """下线集群
 
         :param request: Request instance for OfflineCluster.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OfflineClusterRequest`
@@ -2388,15 +2388,15 @@
             model = models.OfflineClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OfflineInstance(self, request):
         """下线实例
 
         :param request: Request instance for OfflineInstance.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OfflineInstanceRequest`
@@ -2411,15 +2411,15 @@
             model = models.OfflineInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenAuditService(self, request):
         """TDSQL-C for MySQL实例开通审计服务
 
         :param request: Request instance for OpenAuditService.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenAuditServiceRequest`
@@ -2434,15 +2434,15 @@
             model = models.OpenAuditServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenClusterPasswordComplexity(self, request):
         """本接口（OpenClusterPasswordComplexity）用于开启集群密码复杂度
 
         :param request: Request instance for OpenClusterPasswordComplexity.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenClusterPasswordComplexityRequest`
@@ -2457,15 +2457,15 @@
             model = models.OpenClusterPasswordComplexityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenReadOnlyInstanceExclusiveAccess(self, request):
         """开通只读实例独有访问接入组
 
         :param request: Request instance for OpenReadOnlyInstanceExclusiveAccess.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenReadOnlyInstanceExclusiveAccessRequest`
@@ -2480,15 +2480,15 @@
             model = models.OpenReadOnlyInstanceExclusiveAccessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenWan(self, request):
         """本接口（OpenWan）用于开通外网
 
         :param request: Request instance for OpenWan.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenWanRequest`
@@ -2503,15 +2503,15 @@
             model = models.OpenWanResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PauseServerless(self, request):
         """暂停serverless集群
 
         :param request: Request instance for PauseServerless.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.PauseServerlessRequest`
@@ -2526,15 +2526,15 @@
             model = models.PauseServerlessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RefundResourcePackage(self, request):
         """退款资源包
 
         :param request: Request instance for RefundResourcePackage.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RefundResourcePackageRequest`
@@ -2549,15 +2549,15 @@
             model = models.RefundResourcePackageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReloadBalanceProxyNode(self, request):
         """负载均衡数据库代理
 
         :param request: Request instance for ReloadBalanceProxyNode.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ReloadBalanceProxyNodeRequest`
@@ -2572,15 +2572,15 @@
             model = models.ReloadBalanceProxyNodeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveClusterSlaveZone(self, request):
         """删除从可用区
 
         :param request: Request instance for RemoveClusterSlaveZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RemoveClusterSlaveZoneRequest`
@@ -2595,15 +2595,15 @@
             model = models.RemoveClusterSlaveZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAccountPassword(self, request):
         """本接口(ResetAccountPassword)用于重置实例的数据库账号密码。
 
         :param request: Request instance for ResetAccountPassword.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ResetAccountPasswordRequest`
@@ -2618,15 +2618,15 @@
             model = models.ResetAccountPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestartInstance(self, request):
         """重启实例
 
         :param request: Request instance for RestartInstance.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RestartInstanceRequest`
@@ -2641,15 +2641,15 @@
             model = models.RestartInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResumeServerless(self, request):
         """恢复serverless集群
 
         :param request: Request instance for ResumeServerless.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ResumeServerlessRequest`
@@ -2664,15 +2664,15 @@
             model = models.ResumeServerlessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RevokeAccountPrivileges(self, request):
         """批量回收账号权限
 
         :param request: Request instance for RevokeAccountPrivileges.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RevokeAccountPrivilegesRequest`
@@ -2687,15 +2687,15 @@
             model = models.RevokeAccountPrivilegesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollBackCluster(self, request):
         """本接口（RollBackCluster）用于回档集群
 
         :param request: Request instance for RollBackCluster.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RollBackClusterRequest`
@@ -2710,15 +2710,15 @@
             model = models.RollBackClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchClusterDatabases(self, request):
         """本接口(SearchClusterDatabases)搜索集群database列表
 
         :param request: Request instance for SearchClusterDatabases.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SearchClusterDatabasesRequest`
@@ -2733,15 +2733,15 @@
             model = models.SearchClusterDatabasesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SearchClusterTables(self, request):
         """本接口(SearchClusterTables)搜索集群数据表列表
 
         :param request: Request instance for SearchClusterTables.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SearchClusterTablesRequest`
@@ -2756,15 +2756,15 @@
             model = models.SearchClusterTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetRenewFlag(self, request):
         """SetRenewFlag设置实例的自动续费功能
 
         :param request: Request instance for SetRenewFlag.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SetRenewFlagRequest`
@@ -2779,15 +2779,15 @@
             model = models.SetRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchClusterVpc(self, request):
         """更换集群vpc
 
         :param request: Request instance for SwitchClusterVpc.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SwitchClusterVpcRequest`
@@ -2802,15 +2802,15 @@
             model = models.SwitchClusterVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchClusterZone(self, request):
         """切换到从可用区
 
         :param request: Request instance for SwitchClusterZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SwitchClusterZoneRequest`
@@ -2825,15 +2825,15 @@
             model = models.SwitchClusterZoneResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchProxyVpc(self, request):
         """本接口(SwitchProxyVpc)更换数据库代理vpc
 
         :param request: Request instance for SwitchProxyVpc.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.SwitchProxyVpcRequest`
@@ -2848,15 +2848,15 @@
             model = models.SwitchProxyVpcResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindClusterResourcePackages(self, request):
         """cynos解绑资源包
 
         :param request: Request instance for UnbindClusterResourcePackages.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UnbindClusterResourcePackagesRequest`
@@ -2871,15 +2871,15 @@
             model = models.UnbindClusterResourcePackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeClusterVersion(self, request):
         """更新集群Cynos内核版本
 
         :param request: Request instance for UpgradeClusterVersion.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeClusterVersionRequest`
@@ -2894,15 +2894,15 @@
             model = models.UpgradeClusterVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeInstance(self, request):
         """升级实例
 
         :param request: Request instance for UpgradeInstance.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeInstanceRequest`
@@ -2917,15 +2917,15 @@
             model = models.UpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeProxy(self, request):
         """升级数据库代理配置
 
         :param request: Request instance for UpgradeProxy.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyRequest`
@@ -2940,15 +2940,15 @@
             model = models.UpgradeProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeProxyVersion(self, request):
         """升级数据库代理版本
 
         :param request: Request instance for UpgradeProxyVersion.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyVersionRequest`
@@ -2963,8 +2963,8 @@
             model = models.UpgradeProxyVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud/cynosdb/v20190107/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.937/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.938/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

