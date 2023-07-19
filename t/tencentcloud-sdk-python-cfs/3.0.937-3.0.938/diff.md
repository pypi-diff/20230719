# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.937.tar", last modified: Tue Jul 18 00:19:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.938.tar", last modified: Wed Jul 19 00:23:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.937.tar` & `tencentcloud-sdk-python-cfs-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    39879 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   194257 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:19:46.000000 tencentcloud-sdk-python-cfs-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    40047 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   194257 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:23:53.000000 tencentcloud-sdk-python-cfs-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/setup.py` & `tencentcloud-sdk-python-cfs-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BindAutoSnapshotPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAutoSnapshotPolicy(self, request):
         """创建定期快照策略
 
         :param request: Request instance for CreateAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.CreateAutoSnapshotPolicyRequest`
@@ -65,15 +65,15 @@
             model = models.CreateAutoSnapshotPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCfsFileSystem(self, request):
         """用于添加新文件系统
 
         :param request: Request instance for CreateCfsFileSystem.
         :type request: :class:`tencentcloud.cfs.v20190719.models.CreateCfsFileSystemRequest`
@@ -88,15 +88,15 @@
             model = models.CreateCfsFileSystemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCfsPGroup(self, request):
         """本接口（CreateCfsPGroup）用于创建权限组
 
         :param request: Request instance for CreateCfsPGroup.
         :type request: :class:`tencentcloud.cfs.v20190719.models.CreateCfsPGroupRequest`
@@ -111,15 +111,15 @@
             model = models.CreateCfsPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCfsRule(self, request):
         """本接口（CreateCfsRule）用于创建权限组规则。
 
         :param request: Request instance for CreateCfsRule.
         :type request: :class:`tencentcloud.cfs.v20190719.models.CreateCfsRuleRequest`
@@ -134,15 +134,15 @@
             model = models.CreateCfsRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCfsSnapshot(self, request):
         """创建文件系统快照
 
         :param request: Request instance for CreateCfsSnapshot.
         :type request: :class:`tencentcloud.cfs.v20190719.models.CreateCfsSnapshotRequest`
@@ -157,15 +157,15 @@
             model = models.CreateCfsSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMigrationTask(self, request):
         """用于创建迁移任务。
         此接口需提交工单，开启白名单之后才能使用。
 
         :param request: Request instance for CreateMigrationTask.
@@ -181,15 +181,15 @@
             model = models.CreateMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAutoSnapshotPolicy(self, request):
         """删除快照定期策略
 
         :param request: Request instance for DeleteAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteAutoSnapshotPolicyRequest`
@@ -204,15 +204,15 @@
             model = models.DeleteAutoSnapshotPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCfsFileSystem(self, request):
         """用于删除文件系统
 
         :param request: Request instance for DeleteCfsFileSystem.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteCfsFileSystemRequest`
@@ -227,15 +227,15 @@
             model = models.DeleteCfsFileSystemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCfsPGroup(self, request):
         """本接口（DeleteCfsPGroup）用于删除权限组。
 
         :param request: Request instance for DeleteCfsPGroup.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteCfsPGroupRequest`
@@ -250,15 +250,15 @@
             model = models.DeleteCfsPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCfsRule(self, request):
         """本接口（DeleteCfsRule）用于删除权限组规则。
 
         :param request: Request instance for DeleteCfsRule.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteCfsRuleRequest`
@@ -273,15 +273,15 @@
             model = models.DeleteCfsRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCfsSnapshot(self, request):
         """删除文件系统快照
 
         :param request: Request instance for DeleteCfsSnapshot.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteCfsSnapshotRequest`
@@ -296,15 +296,15 @@
             model = models.DeleteCfsSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMigrationTask(self, request):
         """用于删除迁移任务。
         此接口需提交工单，开启白名单之后才能使用。
 
         :param request: Request instance for DeleteMigrationTask.
@@ -320,15 +320,15 @@
             model = models.DeleteMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMountTarget(self, request):
         """本接口（DeleteMountTarget）用于删除挂载点
 
         :param request: Request instance for DeleteMountTarget.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteMountTargetRequest`
@@ -343,15 +343,15 @@
             model = models.DeleteMountTargetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserQuota(self, request):
         """指定条件删除文件系统配额
 
         :param request: Request instance for DeleteUserQuota.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DeleteUserQuotaRequest`
@@ -366,15 +366,15 @@
             model = models.DeleteUserQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAutoSnapshotPolicies(self, request):
         """查询文件系统快照定期策略列表信息
 
         :param request: Request instance for DescribeAutoSnapshotPolicies.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeAutoSnapshotPoliciesRequest`
@@ -389,15 +389,15 @@
             model = models.DescribeAutoSnapshotPoliciesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAvailableZoneInfo(self, request):
         """本接口（DescribeAvailableZoneInfo）用于查询区域的可用情况。
 
         :param request: Request instance for DescribeAvailableZoneInfo.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeAvailableZoneInfoRequest`
@@ -412,15 +412,15 @@
             model = models.DescribeAvailableZoneInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBucketList(self, request):
         """用于获取数据源桶列表。
         此接口需提交工单，开启白名单之后才能使用。
 
         :param request: Request instance for DescribeBucketList.
@@ -436,15 +436,15 @@
             model = models.DescribeBucketListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsFileSystemClients(self, request):
         """查询挂载该文件系统的客户端。此功能需要客户端安装CFS监控插件。
 
         :param request: Request instance for DescribeCfsFileSystemClients.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsFileSystemClientsRequest`
@@ -459,15 +459,15 @@
             model = models.DescribeCfsFileSystemClientsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsFileSystems(self, request):
         """本接口（DescribeCfsFileSystems）用于查询文件系统
 
         :param request: Request instance for DescribeCfsFileSystems.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsFileSystemsRequest`
@@ -482,15 +482,15 @@
             model = models.DescribeCfsFileSystemsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsPGroups(self, request):
         """本接口（DescribeCfsPGroups）用于查询权限组列表。
 
         :param request: Request instance for DescribeCfsPGroups.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsPGroupsRequest`
@@ -505,15 +505,15 @@
             model = models.DescribeCfsPGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsRules(self, request):
         """本接口（DescribeCfsRules）用于查询权限组规则列表。
 
         :param request: Request instance for DescribeCfsRules.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsRulesRequest`
@@ -528,15 +528,15 @@
             model = models.DescribeCfsRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsServiceStatus(self, request):
         """本接口（DescribeCfsServiceStatus）用于查询用户使用CFS的服务状态。
 
         :param request: Request instance for DescribeCfsServiceStatus.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsServiceStatusRequest`
@@ -551,15 +551,15 @@
             model = models.DescribeCfsServiceStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsSnapshotOverview(self, request):
         """文件系统快照概览
 
         :param request: Request instance for DescribeCfsSnapshotOverview.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsSnapshotOverviewRequest`
@@ -574,15 +574,15 @@
             model = models.DescribeCfsSnapshotOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCfsSnapshots(self, request):
         """查询文件系统快照列表
 
         :param request: Request instance for DescribeCfsSnapshots.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeCfsSnapshotsRequest`
@@ -597,15 +597,15 @@
             model = models.DescribeCfsSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMigrationTasks(self, request):
         """用于获取迁移任务列表。
         此接口需提交工单，开启白名单之后才能使用。
 
         :param request: Request instance for DescribeMigrationTasks.
@@ -621,15 +621,15 @@
             model = models.DescribeMigrationTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMountTargets(self, request):
         """本接口（DescribeMountTargets）用于查询文件系统挂载点信息
 
         :param request: Request instance for DescribeMountTargets.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeMountTargetsRequest`
@@ -644,15 +644,15 @@
             model = models.DescribeMountTargetsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotOperationLogs(self, request):
         """查询快照操作日志
 
         :param request: Request instance for DescribeSnapshotOperationLogs.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeSnapshotOperationLogsRequest`
@@ -667,15 +667,15 @@
             model = models.DescribeSnapshotOperationLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserQuota(self, request):
         """查询文件系统配额（仅部分Turbo实例能使用，若需要调用请提交工单与我们联系）
 
         :param request: Request instance for DescribeUserQuota.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeUserQuotaRequest`
@@ -690,15 +690,15 @@
             model = models.DescribeUserQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFileSystemAutoScaleUpRule(self, request):
         """用来设置文件系统扩容策略
 
         :param request: Request instance for ModifyFileSystemAutoScaleUpRule.
         :type request: :class:`tencentcloud.cfs.v20190719.models.ModifyFileSystemAutoScaleUpRuleRequest`
@@ -713,15 +713,15 @@
             model = models.ModifyFileSystemAutoScaleUpRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleUpFileSystem(self, request):
         """该接口用于对turbo 文件系统扩容使用
 
         :param request: Request instance for ScaleUpFileSystem.
         :type request: :class:`tencentcloud.cfs.v20190719.models.ScaleUpFileSystemRequest`
@@ -736,15 +736,15 @@
             model = models.ScaleUpFileSystemResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetUserQuota(self, request):
         """设置文件系统配额，提供UID/GID的配额设置的接口
 
         :param request: Request instance for SetUserQuota.
         :type request: :class:`tencentcloud.cfs.v20190719.models.SetUserQuotaRequest`
@@ -759,15 +759,15 @@
             model = models.SetUserQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SignUpCfsService(self, request):
         """本接口（SignUpCfsService）用于开通CFS服务。
 
         :param request: Request instance for SignUpCfsService.
         :type request: :class:`tencentcloud.cfs.v20190719.models.SignUpCfsServiceRequest`
@@ -782,15 +782,15 @@
             model = models.SignUpCfsServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMigrationTask(self, request):
         """用于终止迁移任务。
         此接口需提交工单，开启白名单之后才能使用。
 
         :param request: Request instance for StopMigrationTask.
@@ -806,15 +806,15 @@
             model = models.StopMigrationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnbindAutoSnapshotPolicy(self, request):
         """解除文件系统绑定的快照策略
 
         :param request: Request instance for UnbindAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UnbindAutoSnapshotPolicyRequest`
@@ -829,15 +829,15 @@
             model = models.UnbindAutoSnapshotPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAutoSnapshotPolicy(self, request):
         """更新定期自动快照策略
 
         :param request: Request instance for UpdateAutoSnapshotPolicy.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateAutoSnapshotPolicyRequest`
@@ -852,15 +852,15 @@
             model = models.UpdateAutoSnapshotPolicyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsFileSystemName(self, request):
         """本接口（UpdateCfsFileSystemName）用于更新文件系统名
 
         :param request: Request instance for UpdateCfsFileSystemName.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsFileSystemNameRequest`
@@ -875,15 +875,15 @@
             model = models.UpdateCfsFileSystemNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsFileSystemPGroup(self, request):
         """本接口（UpdateCfsFileSystemPGroup）用于更新文件系统所使用的权限组
 
         :param request: Request instance for UpdateCfsFileSystemPGroup.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsFileSystemPGroupRequest`
@@ -898,15 +898,15 @@
             model = models.UpdateCfsFileSystemPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsFileSystemSizeLimit(self, request):
         """本接口（UpdateCfsFileSystemSizeLimit）用于更新文件系统存储容量限制。
 
         :param request: Request instance for UpdateCfsFileSystemSizeLimit.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsFileSystemSizeLimitRequest`
@@ -921,15 +921,15 @@
             model = models.UpdateCfsFileSystemSizeLimitResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsPGroup(self, request):
         """本接口（UpdateCfsPGroup）更新权限组信息。
 
         :param request: Request instance for UpdateCfsPGroup.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsPGroupRequest`
@@ -944,15 +944,15 @@
             model = models.UpdateCfsPGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsRule(self, request):
         """本接口（UpdateCfsRule）用于更新权限规则。
 
         :param request: Request instance for UpdateCfsRule.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsRuleRequest`
@@ -967,15 +967,15 @@
             model = models.UpdateCfsRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCfsSnapshotAttribute(self, request):
         """更新文件系统快照名称及保留时长
 
         :param request: Request instance for UpdateCfsSnapshotAttribute.
         :type request: :class:`tencentcloud.cfs.v20190719.models.UpdateCfsSnapshotAttributeRequest`
@@ -990,8 +990,8 @@
             model = models.UpdateCfsSnapshotAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.938/tencentcloud/cfs/v20190719/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.938/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.937/README.rst` & `tencentcloud-sdk-python-cfs-3.0.938/README.rst`

 * *Files identical despite different names*

