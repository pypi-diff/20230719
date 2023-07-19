# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.937.tar", last modified: Tue Jul 18 00:29:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.938.tar", last modified: Wed Jul 19 00:44:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.937.tar` & `tencentcloud-sdk-python-redis-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87353 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   467524 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87721 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   467524 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:44:24.000000 tencentcloud-sdk-python-redis-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-redis-3.0.937/setup.py` & `tencentcloud-sdk-python-redis-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.938/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.AddReplicationInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AllocateWanAddress(self, request):
         """开通外网
 
         :param request: Request instance for AllocateWanAddress.
         :type request: :class:`tencentcloud.redis.v20180412.models.AllocateWanAddressRequest`
@@ -65,15 +65,15 @@
             model = models.AllocateWanAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyParamsTemplate(self, request):
         """应用参数模板到实例
 
         :param request: Request instance for ApplyParamsTemplate.
         :type request: :class:`tencentcloud.redis.v20180412.models.ApplyParamsTemplateRequest`
@@ -88,15 +88,15 @@
             model = models.ApplyParamsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateSecurityGroups(self, request):
         """本接口 (AssociateSecurityGroups) 用于安全组批量绑定多个指定实例。
 
         :param request: Request instance for AssociateSecurityGroups.
         :type request: :class:`tencentcloud.redis.v20180412.models.AssociateSecurityGroupsRequest`
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
 
 
     def ChangeInstanceRole(self, request):
         """复制组实例更换角色
 
         :param request: Request instance for ChangeInstanceRole.
         :type request: :class:`tencentcloud.redis.v20180412.models.ChangeInstanceRoleRequest`
@@ -134,15 +134,15 @@
             model = models.ChangeInstanceRoleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeMasterInstance(self, request):
         """该接口（ChangeMasterInstance）用于将复制组内只读实例设置为主实例。
 
         :param request: Request instance for ChangeMasterInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.ChangeMasterInstanceRequest`
@@ -157,15 +157,15 @@
             model = models.ChangeMasterInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeReplicaToMaster(self, request):
         """本接口（ChangeReplicaToMaster）适用于实例副本组提主或副本提主。
 
         :param request: Request instance for ChangeReplicaToMaster.
         :type request: :class:`tencentcloud.redis.v20180412.models.ChangeReplicaToMasterRequest`
@@ -180,15 +180,15 @@
             model = models.ChangeReplicaToMasterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CleanUpInstance(self, request):
         """回收站实例立即下线
 
         :param request: Request instance for CleanUpInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.CleanUpInstanceRequest`
@@ -203,15 +203,15 @@
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
         """清空Redis实例的实例数据。
 
         :param request: Request instance for ClearInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.ClearInstanceRequest`
@@ -226,15 +226,15 @@
             model = models.ClearInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloneInstances(self, request):
         """本接口（CloneInstances）用于基于当前实例的备份文件克隆一个完整的新实例。
 
         :param request: Request instance for CloneInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.CloneInstancesRequest`
@@ -249,15 +249,15 @@
             model = models.CloneInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CloseSSL(self, request):
         """关闭SSL
 
         :param request: Request instance for CloseSSL.
         :type request: :class:`tencentcloud.redis.v20180412.models.CloseSSLRequest`
@@ -272,15 +272,15 @@
             model = models.CloseSSLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstanceAccount(self, request):
         """创建实例子账号
 
         :param request: Request instance for CreateInstanceAccount.
         :type request: :class:`tencentcloud.redis.v20180412.models.CreateInstanceAccountRequest`
@@ -295,15 +295,15 @@
             model = models.CreateInstanceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstances(self, request):
         """本接口（CreateInstances）用于创建 Redis 实例。
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.CreateInstancesRequest`
@@ -318,15 +318,15 @@
             model = models.CreateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateParamTemplate(self, request):
         """创建参数模板。
 
         :param request: Request instance for CreateParamTemplate.
         :type request: :class:`tencentcloud.redis.v20180412.models.CreateParamTemplateRequest`
@@ -341,15 +341,15 @@
             model = models.CreateParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateReplicationGroup(self, request):
         """该接口（CreateReplicationGroup）用于创建复制组。
 
         :param request: Request instance for CreateReplicationGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.CreateReplicationGroupRequest`
@@ -364,15 +364,15 @@
             model = models.CreateReplicationGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstanceAccount(self, request):
         """删除实例子账号
 
         :param request: Request instance for DeleteInstanceAccount.
         :type request: :class:`tencentcloud.redis.v20180412.models.DeleteInstanceAccountRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteInstanceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteParamTemplate(self, request):
         """删除参数模板
 
         :param request: Request instance for DeleteParamTemplate.
         :type request: :class:`tencentcloud.redis.v20180412.models.DeleteParamTemplateRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteReplicationInstance(self, request):
         """移除复制组成员 注：接口下线中，请使用 RemoveReplicationInstance
 
         :param request: Request instance for DeleteReplicationInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.DeleteReplicationInstanceRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteReplicationInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoBackupConfig(self, request):
         """本接口（DescribeAutoBackupConfig）用于获取自动备份配置规则。
 
         :param request: Request instance for DescribeAutoBackupConfig.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeAutoBackupConfigRequest`
@@ -456,15 +456,15 @@
             model = models.DescribeAutoBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupDownloadRestriction(self, request):
         """本接口（DescribeBackupDownloadRestriction）用于查询当前地域数据库备份文件的下载地址。
 
         :param request: Request instance for DescribeBackupDownloadRestriction.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeBackupDownloadRestrictionRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeBackupDownloadRestrictionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupUrl(self, request):
         """本接口（DescribeBackupUrl）用于查询备份 Rdb 文件的下载地址。
 
         :param request: Request instance for DescribeBackupUrl.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeBackupUrlRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeBackupUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBandwidthRange(self, request):
         """本接口（DescribeBandwidthRange）用于查询实例带宽信息。
 
         :param request: Request instance for DescribeBandwidthRange.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeBandwidthRangeRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeBandwidthRangeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCommonDBInstances(self, request):
         """查询Redis实例列表信息。该接口已废弃。
 
         :param request: Request instance for DescribeCommonDBInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeCommonDBInstancesRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeCommonDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDBSecurityGroups(self, request):
         """本接口（DescribeDBSecurityGroups）用于查询实例的安全组详情。
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeDBSecurityGroupsRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeDBSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceAccount(self, request):
         """本接口（DescribeInstanceAccount）用于查看实例子账号信息。
 
         :param request: Request instance for DescribeInstanceAccount.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceAccountRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeInstanceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceBackups(self, request):
         """本接口（DescribeInstanceBackups）用于查询实例备份列表。
 
         :param request: Request instance for DescribeInstanceBackups.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceBackupsRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeInstanceBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceDTSInfo(self, request):
         """查询实例DTS信息
 
         :param request: Request instance for DescribeInstanceDTSInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceDTSInfoRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeInstanceDTSInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceDealDetail(self, request):
         """本接口（DescribeInstanceDealDetail）用于查询订单信息。
 
         :param request: Request instance for DescribeInstanceDealDetail.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceDealDetailRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeInstanceDealDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorBigKey(self, request):
         """腾讯云数据库 Redis 已经于2022年10月31日下线查询实例大 Key 接口。具体公告，请参见[查询实例大 Key 接口下线公告](https://cloud.tencent.com/document/product/239/81005)。
 
         :param request: Request instance for DescribeInstanceMonitorBigKey.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorBigKeyRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeInstanceMonitorBigKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorBigKeySizeDist(self, request):
         """腾讯云数据库 Redis 已经于2022年10月31日下线查询实例大 Key 接口。具体公告，请参见 [查询实例大 Key 接口下线公告](https://cloud.tencent.com/document/product/239/81005)。
 
         :param request: Request instance for DescribeInstanceMonitorBigKeySizeDist.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorBigKeySizeDistRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeInstanceMonitorBigKeySizeDistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorBigKeyTypeDist(self, request):
         """腾讯云数据库 Redis 已经于2022年10月31日下线查询实例大 Key 接口。具体公告，请参见 [查询实例大 Key 接口下线公告](https://cloud.tencent.com/document/product/239/81005)。
 
         :param request: Request instance for DescribeInstanceMonitorBigKeyTypeDist.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorBigKeyTypeDistRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeInstanceMonitorBigKeyTypeDistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorHotKey(self, request):
         """查询实例热Key
 
         :param request: Request instance for DescribeInstanceMonitorHotKey.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorHotKeyRequest`
@@ -755,15 +755,15 @@
             model = models.DescribeInstanceMonitorHotKeyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorSIP(self, request):
         """查询实例访问来源信息
 
         :param request: Request instance for DescribeInstanceMonitorSIP.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorSIPRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeInstanceMonitorSIPResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorTookDist(self, request):
         """查询实例访问的耗时分布
 
         :param request: Request instance for DescribeInstanceMonitorTookDist.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorTookDistRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeInstanceMonitorTookDistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorTopNCmd(self, request):
         """查询实例访问命令
 
         :param request: Request instance for DescribeInstanceMonitorTopNCmd.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorTopNCmdRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeInstanceMonitorTopNCmdResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceMonitorTopNCmdTook(self, request):
         """查询实例CPU耗时
 
         :param request: Request instance for DescribeInstanceMonitorTopNCmdTook.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceMonitorTopNCmdTookRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeInstanceMonitorTopNCmdTookResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceNodeInfo(self, request):
         """本接口（DescribeInstanceNodeInfo）用于查询实例节点信息。
 
         :param request: Request instance for DescribeInstanceNodeInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceNodeInfoRequest`
@@ -870,15 +870,15 @@
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
         """查询参数修改历史列表
 
         :param request: Request instance for DescribeInstanceParamRecords.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceParamRecordsRequest`
@@ -893,15 +893,15 @@
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
         """本接口（DescribeInstanceParams）用于查询实例参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceParamsRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceSecurityGroup(self, request):
         """本接口（DescribeInstanceSecurityGroup）用于查询实例安全组信息。
 
         :param request: Request instance for DescribeInstanceSecurityGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceSecurityGroupRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeInstanceSecurityGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceShards(self, request):
         """本接口（DescribeInstanceShards）用于获取集群架构实例的分片信息。
 
         :param request: Request instance for DescribeInstanceShards.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceShardsRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeInstanceShardsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceZoneInfo(self, request):
         """本接口（DescribeInstanceZoneInfo）用于查询 Redis 节点详细信息。
 
         :param request: Request instance for DescribeInstanceZoneInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceZoneInfoRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeInstanceZoneInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口（DescribeInstances）用于查询Redis实例列表。
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstancesRequest`
@@ -1008,15 +1008,15 @@
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
         """查询实例维护时间窗，在实例需要进行版本升级或者架构升级的时候，会在维护时间窗时间内进行切换
 
         :param request: Request instance for DescribeMaintenanceWindow.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeMaintenanceWindowRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeMaintenanceWindowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParamTemplateInfo(self, request):
         """本接口（DescribeParamTemplateInfo）用于查询参数模板详情。
 
         :param request: Request instance for DescribeParamTemplateInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeParamTemplateInfoRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeParamTemplateInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeParamTemplates(self, request):
         """查询参数模板列表
 
         :param request: Request instance for DescribeParamTemplates.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeParamTemplatesRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeParamTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProductInfo(self, request):
         """本接口（DescribeProductInfo）用于查询全地域 Redis 的售卖规格。
 
         :param request: Request instance for DescribeProductInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeProductInfoRequest`
@@ -1100,15 +1100,15 @@
             model = models.DescribeProductInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProjectSecurityGroup(self, request):
         """查询项目安全组信息
 
         :param request: Request instance for DescribeProjectSecurityGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeProjectSecurityGroupRequest`
@@ -1123,15 +1123,15 @@
             model = models.DescribeProjectSecurityGroupResponse()
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
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeProjectSecurityGroupsRequest`
@@ -1146,15 +1146,15 @@
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
         """本接口（DescribeProxySlowLog）用于查询代理慢查询。
 
         :param request: Request instance for DescribeProxySlowLog.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeProxySlowLogRequest`
@@ -1169,15 +1169,15 @@
             model = models.DescribeProxySlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeReplicationGroup(self, request):
         """本接口（DescribeReplicationGroup）用于查询复制组。
 
         :param request: Request instance for DescribeReplicationGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeReplicationGroupRequest`
@@ -1192,15 +1192,15 @@
             model = models.DescribeReplicationGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSSLStatus(self, request):
         """本接口（DescribeSSLStatus）用于查询实例 SSL 认证相关信息，包括开启状态、配置状态、证书地址等。
 
         :param request: Request instance for DescribeSSLStatus.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeSSLStatusRequest`
@@ -1215,15 +1215,15 @@
             model = models.DescribeSSLStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSlowLog(self, request):
         """本接口（DescribeSlowLog）查询实例慢查询记录。
 
         :param request: Request instance for DescribeSlowLog.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeSlowLogRequest`
@@ -1238,15 +1238,15 @@
             model = models.DescribeSlowLogResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskInfo(self, request):
         """本接口（DescribeTaskInfo）用于获取指定任务的执行情况。
 
         :param request: Request instance for DescribeTaskInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeTaskInfoRequest`
@@ -1261,15 +1261,15 @@
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
         """本接口（DescribeTaskList）用于查询指定实例的任务列表信息。
 
         :param request: Request instance for DescribeTaskList.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeTaskListRequest`
@@ -1284,15 +1284,15 @@
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
         """查询Tendis慢查询
 
         :param request: Request instance for DescribeTendisSlowLog.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeTendisSlowLogRequest`
@@ -1307,15 +1307,15 @@
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
         """按量计费实例销毁
 
         :param request: Request instance for DestroyPostpaidInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.DestroyPostpaidInstanceRequest`
@@ -1330,15 +1330,15 @@
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
         """包年包月实例退还
 
         :param request: Request instance for DestroyPrepaidInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.DestroyPrepaidInstanceRequest`
@@ -1353,15 +1353,15 @@
             model = models.DestroyPrepaidInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableReplicaReadonly(self, request):
         """禁用读写分离
 
         :param request: Request instance for DisableReplicaReadonly.
         :type request: :class:`tencentcloud.redis.v20180412.models.DisableReplicaReadonlyRequest`
@@ -1376,15 +1376,15 @@
             model = models.DisableReplicaReadonlyResponse()
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
         :type request: :class:`tencentcloud.redis.v20180412.models.DisassociateSecurityGroupsRequest`
@@ -1399,15 +1399,15 @@
             model = models.DisassociateSecurityGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableReplicaReadonly(self, request):
         """启用读写分离
 
         :param request: Request instance for EnableReplicaReadonly.
         :type request: :class:`tencentcloud.redis.v20180412.models.EnableReplicaReadonlyRequest`
@@ -1422,15 +1422,15 @@
             model = models.EnableReplicaReadonlyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateInstance(self, request):
         """查询新购实例价格
 
         :param request: Request instance for InquiryPriceCreateInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.InquiryPriceCreateInstanceRequest`
@@ -1445,15 +1445,15 @@
             model = models.InquiryPriceCreateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceRenewInstance(self, request):
         """查询实例续费价格（包年包月）
 
         :param request: Request instance for InquiryPriceRenewInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.InquiryPriceRenewInstanceRequest`
@@ -1468,15 +1468,15 @@
             model = models.InquiryPriceRenewInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceUpgradeInstance(self, request):
         """查询实例扩容价格
 
         :param request: Request instance for InquiryPriceUpgradeInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.InquiryPriceUpgradeInstanceRequest`
@@ -1491,15 +1491,15 @@
             model = models.InquiryPriceUpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def KillMasterGroup(self, request):
         """本接口（KillMasterGroup）模拟故障。
 
         :param request: Request instance for KillMasterGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.KillMasterGroupRequest`
@@ -1514,15 +1514,15 @@
             model = models.KillMasterGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManualBackupInstance(self, request):
         """本接口（ManualBackupInstance）用于手动备份Redis实例。
 
         :param request: Request instance for ManualBackupInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.ManualBackupInstanceRequest`
@@ -1537,15 +1537,15 @@
             model = models.ManualBackupInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModfiyInstancePassword(self, request):
         """本接口（ModfiyInstancePassword）用于修改实例访问密码。
 
         :param request: Request instance for ModfiyInstancePassword.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModfiyInstancePasswordRequest`
@@ -1560,15 +1560,15 @@
             model = models.ModfiyInstancePasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAutoBackupConfig(self, request):
         """本接口（ModifyAutoBackupConfig）用于设置自动备份的配置。
 
         :param request: Request instance for ModifyAutoBackupConfig.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyAutoBackupConfigRequest`
@@ -1583,15 +1583,15 @@
             model = models.ModifyAutoBackupConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBackupDownloadRestriction(self, request):
         """本接口（ModifyBackupDownloadRestriction）用于修改备份文件下载的网络信息与地址。
 
         :param request: Request instance for ModifyBackupDownloadRestriction.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyBackupDownloadRestrictionRequest`
@@ -1606,15 +1606,15 @@
             model = models.ModifyBackupDownloadRestrictionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyConnectionConfig(self, request):
         """修改实例的连接配置，包括带宽和最大连接数。
 
         :param request: Request instance for ModifyConnectionConfig.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyConnectionConfigRequest`
@@ -1629,15 +1629,15 @@
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
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyDBInstanceSecurityGroupsRequest`
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
 
 
     def ModifyInstance(self, request):
         """修改实例相关信息
 
         :param request: Request instance for ModifyInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyInstanceRequest`
@@ -1675,15 +1675,15 @@
             model = models.ModifyInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceAccount(self, request):
         """修改实例子账号
 
         :param request: Request instance for ModifyInstanceAccount.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyInstanceAccountRequest`
@@ -1698,15 +1698,15 @@
             model = models.ModifyInstanceAccountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceParams(self, request):
         """本接口(ModifyInstanceParams)用于修改Redis实例的参数配置。
 
         :param request: Request instance for ModifyInstanceParams.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyInstanceParamsRequest`
@@ -1721,15 +1721,15 @@
             model = models.ModifyInstanceParamsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceReadOnly(self, request):
         """设置实例输入模式
 
         :param request: Request instance for ModifyInstanceReadOnly.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyInstanceReadOnlyRequest`
@@ -1744,15 +1744,15 @@
             model = models.ModifyInstanceReadOnlyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMaintenanceWindow(self, request):
         """修改实例维护时间窗时间，需要进行版本升级或者架构升级的实例，会在维护时间窗内进行时间切换。注意：已经发起版本升级或者架构升级的实例，无法修改维护时间窗。
 
         :param request: Request instance for ModifyMaintenanceWindow.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyMaintenanceWindowRequest`
@@ -1767,15 +1767,15 @@
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
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyNetworkConfigRequest`
@@ -1790,15 +1790,15 @@
             model = models.ModifyNetworkConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyParamTemplate(self, request):
         """修改参数模板
 
         :param request: Request instance for ModifyParamTemplate.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyParamTemplateRequest`
@@ -1813,15 +1813,15 @@
             model = models.ModifyParamTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OpenSSL(self, request):
         """开启SSL
 
         :param request: Request instance for OpenSSL.
         :type request: :class:`tencentcloud.redis.v20180412.models.OpenSSLRequest`
@@ -1836,15 +1836,15 @@
             model = models.OpenSSLResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseWanAddress(self, request):
         """关闭外网
 
         :param request: Request instance for ReleaseWanAddress.
         :type request: :class:`tencentcloud.redis.v20180412.models.ReleaseWanAddressRequest`
@@ -1859,15 +1859,15 @@
             model = models.ReleaseWanAddressResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RemoveReplicationInstance(self, request):
         """移除复制组成员
 
         :param request: Request instance for RemoveReplicationInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.RemoveReplicationInstanceRequest`
@@ -1882,15 +1882,15 @@
             model = models.RemoveReplicationInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstance(self, request):
         """本接口（RenewInstance）可用于为实例续费。
 
         :param request: Request instance for RenewInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.RenewInstanceRequest`
@@ -1905,15 +1905,15 @@
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
         """重置密码
 
         :param request: Request instance for ResetPassword.
         :type request: :class:`tencentcloud.redis.v20180412.models.ResetPasswordRequest`
@@ -1928,15 +1928,15 @@
             model = models.ResetPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RestoreInstance(self, request):
         """恢复 CRS 实例
 
         :param request: Request instance for RestoreInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.RestoreInstanceRequest`
@@ -1951,15 +1951,15 @@
             model = models.RestoreInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartupInstance(self, request):
         """实例解隔离
 
         :param request: Request instance for StartupInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.StartupInstanceRequest`
@@ -1974,15 +1974,15 @@
             model = models.StartupInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchInstanceVip(self, request):
         """在通过DTS支持跨可用区灾备的场景中，通过该接口交换实例VIP完成实例灾备切换。交换VIP后目标实例可写，源和目标实例VIP互换，同时源与目标实例间DTS同步任务断开
 
         :param request: Request instance for SwitchInstanceVip.
         :type request: :class:`tencentcloud.redis.v20180412.models.SwitchInstanceVipRequest`
@@ -1997,15 +1997,15 @@
             model = models.SwitchInstanceVipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchProxy(self, request):
         """Proxy模拟故障接口
 
         :param request: Request instance for SwitchProxy.
         :type request: :class:`tencentcloud.redis.v20180412.models.SwitchProxyRequest`
@@ -2020,15 +2020,15 @@
             model = models.SwitchProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeInstance(self, request):
         """变更实例配置
 
         :param request: Request instance for UpgradeInstance.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeInstanceRequest`
@@ -2043,15 +2043,15 @@
             model = models.UpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeInstanceVersion(self, request):
         """将当前实例升级到更高版本，或者将当前标准架构升级至集群架构。
 
         :param request: Request instance for UpgradeInstanceVersion.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeInstanceVersionRequest`
@@ -2066,15 +2066,15 @@
             model = models.UpgradeInstanceVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeProxyVersion(self, request):
         """实例proxy版本升级
 
         :param request: Request instance for UpgradeProxyVersion.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeProxyVersionRequest`
@@ -2089,15 +2089,15 @@
             model = models.UpgradeProxyVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeSmallVersion(self, request):
         """实例小版本升级
 
         :param request: Request instance for UpgradeSmallVersion.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeSmallVersionRequest`
@@ -2112,15 +2112,15 @@
             model = models.UpgradeSmallVersionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpgradeVersionToMultiAvailabilityZones(self, request):
         """升级实例支持多AZ
 
         :param request: Request instance for UpgradeVersionToMultiAvailabilityZones.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeVersionToMultiAvailabilityZonesRequest`
@@ -2135,8 +2135,8 @@
             model = models.UpgradeVersionToMultiAvailabilityZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.938/tencentcloud/redis/v20180412/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.938/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.937/README.rst` & `tencentcloud-sdk-python-redis-3.0.938/README.rst`

 * *Files identical despite different names*

