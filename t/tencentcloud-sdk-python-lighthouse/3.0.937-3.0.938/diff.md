# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.937.tar", last modified: Tue Jul 18 00:26:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.938.tar", last modified: Wed Jul 19 00:42:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.937.tar` & `tencentcloud-sdk-python-lighthouse-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92544 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)    26127 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   360397 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:26:36.000000 tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92864 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)    26127 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360767 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:42:00.000000 tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             model = models.ApplyDiskBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ApplyInstanceSnapshot(self, request):
         """本接口（ApplyInstanceSnapshot）用于回滚指定实例的系统盘快照。
         <li>仅支持回滚到原系统盘。</li>
         <li>用于回滚的快照必须处于 NORMAL 状态。快照状态可以通过 DescribeSnapshots 接口查询，见输出参数中 SnapshotState 字段解释。</li>
         <li>回滚快照时，实例的状态必须为 STOPPED 或 RUNNING，可通过 DescribeInstances 接口查询实例状态。处于 RUNNING 状态的实例会强制关机，然后回滚快照。</li>
@@ -74,15 +74,15 @@
             model = models.ApplyInstanceSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AssociateInstancesKeyPairs(self, request):
         """本接口（AssociateInstancesKeyPairs）用于绑定用户指定密钥对到实例。
         * 只支持 [RUNNING, STOPPED] 状态的 LINUX_UNIX 操作系统的实例。处于 RUNNING 状态的实例会强制关机，然后绑定。
         * 将密钥的公钥写入到实例的 SSH 配置当中，用户就可以通过该密钥的私钥来登录实例。
         * 如果实例原来绑定过密钥，那么原来的密钥将失效。
@@ -103,15 +103,15 @@
             model = models.AssociateInstancesKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachCcn(self, request):
         """本接口 (AttachCcn) 用于建立与云联网的关联。
 
         :param request: Request instance for AttachCcn.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.AttachCcnRequest`
@@ -126,15 +126,15 @@
             model = models.AttachCcnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def AttachDisks(self, request):
         """本接口（AttachDisks）用于挂载一个或多个云硬盘。
 
         :param request: Request instance for AttachDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.AttachDisksRequest`
@@ -149,15 +149,15 @@
             model = models.AttachDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBlueprint(self, request):
         """本接口 (CreateBlueprint) 用于创建镜像。
 
         :param request: Request instance for CreateBlueprint.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateBlueprintRequest`
@@ -172,15 +172,15 @@
             model = models.CreateBlueprintResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDiskBackup(self, request):
         """本接口 ( CreateDiskBackup  ) 用于创建指定云硬盘（当前只支持数据盘）的备份点。
 
         :param request: Request instance for CreateDiskBackup.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateDiskBackupRequest`
@@ -195,15 +195,15 @@
             model = models.CreateDiskBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDisks(self, request):
         """本接口(CreateDisks)用于创建一个或多个云硬盘。
 
         :param request: Request instance for CreateDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateDisksRequest`
@@ -218,15 +218,15 @@
             model = models.CreateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFirewallRules(self, request):
         """本接口（CreateFirewallRules）用于在实例上添加防火墙规则。
 
 
         * FirewallVersion 为防火墙版本号，用户每次更新防火墙规则版本会自动加1，防止您更新的规则已过期，不填不考虑冲突。
@@ -251,15 +251,15 @@
             model = models.CreateFirewallRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstanceSnapshot(self, request):
         """本接口（CreateInstanceSnapshot）用于创建指定实例的系统盘快照。
 
         :param request: Request instance for CreateInstanceSnapshot.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateInstanceSnapshotRequest`
@@ -274,15 +274,15 @@
             model = models.CreateInstanceSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstances(self, request):
         """本接口(CreateInstances)用于创建一个或多个指定套餐的轻量应用服务器实例。
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateInstancesRequest`
@@ -297,15 +297,15 @@
             model = models.CreateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateKeyPair(self, request):
         """本接口（CreateKeyPair）用于创建一个密钥对。
 
         :param request: Request instance for CreateKeyPair.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.CreateKeyPairRequest`
@@ -320,15 +320,15 @@
             model = models.CreateKeyPairResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBlueprints(self, request):
         """本接口 (DeleteBlueprints) 用于删除镜像。
 
         :param request: Request instance for DeleteBlueprints.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DeleteBlueprintsRequest`
@@ -343,15 +343,15 @@
             model = models.DeleteBlueprintsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDiskBackups(self, request):
         """本接口（DeleteDiskBackups）用于删除云硬盘备份点。
         云硬盘备份点必须处于 NORMAL 状态，云硬盘备份点状态可以通过 [DescribeDiskBackups](https://cloud.tencent.com/document/api/1207/84379)接口查询，见输出参数中 DiskBackupState 字段解释。
 
         :param request: Request instance for DeleteDiskBackups.
@@ -367,15 +367,15 @@
             model = models.DeleteDiskBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteFirewallRules(self, request):
         """本接口（DeleteFirewallRules）用于删除实例的防火墙规则。
 
         * FirewallVersion 用于指定要操作的防火墙的版本。传入 FirewallVersion 版本号若不等于当前防火墙的最新版本，将返回失败；若不传 FirewallVersion 则直接删除指定的规则。
 
@@ -399,15 +399,15 @@
             model = models.DeleteFirewallRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteKeyPairs(self, request):
         """本接口（DeleteKeyPairs）用于删除密钥对。
 
         :param request: Request instance for DeleteKeyPairs.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DeleteKeyPairsRequest`
@@ -422,15 +422,15 @@
             model = models.DeleteKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshots(self, request):
         """本接口（DeleteSnapshots）用于删除快照。
         快照必须处于 NORMAL 状态，快照状态可以通过 DescribeSnapshots 接口查询，见输出参数中 SnapshotState 字段解释。
 
         :param request: Request instance for DeleteSnapshots.
@@ -446,15 +446,15 @@
             model = models.DeleteSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllScenes(self, request):
         """本接口(DescribeAllScenes)用于查询全地域使用场景列表。
 
         :param request: Request instance for DescribeAllScenes.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeAllScenesRequest`
@@ -469,15 +469,15 @@
             model = models.DescribeAllScenesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBlueprintInstances(self, request):
         """本接口（DescribeBlueprintInstances）用于查询镜像实例信息。
 
         :param request: Request instance for DescribeBlueprintInstances.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeBlueprintInstancesRequest`
@@ -492,15 +492,15 @@
             model = models.DescribeBlueprintInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBlueprints(self, request):
         """本接口（DescribeBlueprints）用于查询镜像信息。
 
         :param request: Request instance for DescribeBlueprints.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeBlueprintsRequest`
@@ -515,15 +515,15 @@
             model = models.DescribeBlueprintsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBundleDiscount(self, request):
         """本接口（DescribeBundleDiscount）用于查询套餐折扣信息。
 
         :param request: Request instance for DescribeBundleDiscount.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeBundleDiscountRequest`
@@ -538,15 +538,15 @@
             model = models.DescribeBundleDiscountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBundles(self, request):
         """本接口（DescribeBundles）用于查询套餐信息。
 
         :param request: Request instance for DescribeBundles.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeBundlesRequest`
@@ -561,15 +561,15 @@
             model = models.DescribeBundlesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCcnAttachedInstances(self, request):
         """本接口 (DescribeCcnAttachedInstances) 用于查询云联网关联的实例信息。
 
         :param request: Request instance for DescribeCcnAttachedInstances.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeCcnAttachedInstancesRequest`
@@ -584,15 +584,15 @@
             model = models.DescribeCcnAttachedInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiskBackups(self, request):
         """本接口（DescribeDiskBackups）用于查询云硬盘备份点的详细信息。
 
         :param request: Request instance for DescribeDiskBackups.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDiskBackupsRequest`
@@ -607,15 +607,15 @@
             model = models.DescribeDiskBackupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiskBackupsDeniedActions(self, request):
         """本接口（DescribeDiskBackupsDeniedActions）用于查询一个或多个云硬盘备份点的操作限制列表信息。
 
         :param request: Request instance for DescribeDiskBackupsDeniedActions.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDiskBackupsDeniedActionsRequest`
@@ -630,15 +630,15 @@
             model = models.DescribeDiskBackupsDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiskConfigs(self, request):
         """本接口（DescribeDiskConfigs）用于查询云硬盘配置。
 
         :param request: Request instance for DescribeDiskConfigs.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDiskConfigsRequest`
@@ -653,15 +653,15 @@
             model = models.DescribeDiskConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDiskDiscount(self, request):
         """本接口(DescribeDiskDiscount)用于查询云硬盘折扣信息。
 
         :param request: Request instance for DescribeDiskDiscount.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDiskDiscountRequest`
@@ -676,15 +676,15 @@
             model = models.DescribeDiskDiscountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisks(self, request):
         """本接口（DescribeDisks）用于查询云硬盘信息。
 
         :param request: Request instance for DescribeDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDisksRequest`
@@ -699,15 +699,15 @@
             model = models.DescribeDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisksDeniedActions(self, request):
         """本接口（DescribeDisksDeniedActions）用于查询一个或多个云硬盘的操作限制列表信息。
 
         :param request: Request instance for DescribeDisksDeniedActions.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDisksDeniedActionsRequest`
@@ -722,15 +722,15 @@
             model = models.DescribeDisksDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDisksReturnable(self, request):
         """本接口（DescribeDisksReturnable）用于查询云硬盘是否可退还。
 
         :param request: Request instance for DescribeDisksReturnable.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeDisksReturnableRequest`
@@ -745,15 +745,15 @@
             model = models.DescribeDisksReturnableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirewallRules(self, request):
         """本接口（DescribeFirewallRules）用于查询实例的防火墙规则。
 
         :param request: Request instance for DescribeFirewallRules.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeFirewallRulesRequest`
@@ -768,15 +768,15 @@
             model = models.DescribeFirewallRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFirewallRulesTemplate(self, request):
         """本接口（DescribeFirewallRulesTemplate）用于查询防火墙规则模板。
 
         :param request: Request instance for DescribeFirewallRulesTemplate.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeFirewallRulesTemplateRequest`
@@ -791,15 +791,15 @@
             model = models.DescribeFirewallRulesTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGeneralResourceQuotas(self, request):
         """本接口（DescribeGeneralResourceQuotas）用于查询通用资源配额信息。
 
         :param request: Request instance for DescribeGeneralResourceQuotas.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeGeneralResourceQuotasRequest`
@@ -814,15 +814,15 @@
             model = models.DescribeGeneralResourceQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceLoginKeyPairAttribute(self, request):
         """本接口用于查询实例默认登录密钥属性。
 
         :param request: Request instance for DescribeInstanceLoginKeyPairAttribute.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeInstanceLoginKeyPairAttributeRequest`
@@ -837,15 +837,15 @@
             model = models.DescribeInstanceLoginKeyPairAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceVncUrl(self, request):
         """本接口 ( DescribeInstanceVncUrl ) 用于查询实例管理终端地址，获取的地址可用于实例的 VNC 登录。
 
         * 处于 `STOPPED` 状态的机器无法使用此功能。
         * 管理终端地址的有效期为 15 秒，调用接口成功后如果 15 秒内不使用该链接进行访问，管理终端地址自动失效，您需要重新查询。
@@ -872,15 +872,15 @@
             model = models.DescribeInstanceVncUrlResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """本接口（DescribeInstances）用于查询一个或多个实例的详细信息。
 
         * 可以根据实例 ID、实例名称或者实例的内网 IP 查询实例的详细信息。
         * 过滤信息详细请见过滤器 [Filters](https://cloud.tencent.com/document/product/1207/47576#Filter) 。
@@ -900,15 +900,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesDeniedActions(self, request):
         """本接口（DescribeInstancesDeniedActions）用于查询一个或多个实例的操作限制列表信息。
 
         :param request: Request instance for DescribeInstancesDeniedActions.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeInstancesDeniedActionsRequest`
@@ -923,15 +923,15 @@
             model = models.DescribeInstancesDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesDiskNum(self, request):
         """本接口(DescribeInstancesDiskNum)用于查询实例挂载云硬盘数量。
 
         :param request: Request instance for DescribeInstancesDiskNum.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeInstancesDiskNumRequest`
@@ -946,15 +946,15 @@
             model = models.DescribeInstancesDiskNumResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesReturnable(self, request):
         """本接口（DescribeInstancesReturnable）用于查询实例是否可退还。
 
         :param request: Request instance for DescribeInstancesReturnable.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeInstancesReturnableRequest`
@@ -969,15 +969,15 @@
             model = models.DescribeInstancesReturnableResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesTrafficPackages(self, request):
         """本接口（DescribeInstancesTrafficPackages）用于查询一个或多个实例的流量包详情。
 
         :param request: Request instance for DescribeInstancesTrafficPackages.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeInstancesTrafficPackagesRequest`
@@ -992,15 +992,15 @@
             model = models.DescribeInstancesTrafficPackagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKeyPairs(self, request):
         """本接口 (DescribeKeyPairs) 用于查询用户密钥对信息。
 
         :param request: Request instance for DescribeKeyPairs.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeKeyPairsRequest`
@@ -1015,15 +1015,15 @@
             model = models.DescribeKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeModifyInstanceBundles(self, request):
         """本接口（DescribeModifyInstanceBundles）用于查询实例可变更套餐列表。
 
         :param request: Request instance for DescribeModifyInstanceBundles.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeModifyInstanceBundlesRequest`
@@ -1038,15 +1038,15 @@
             model = models.DescribeModifyInstanceBundlesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """本接口（DescribeRegions）用于查询地域信息。
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeRegionsRequest`
@@ -1061,15 +1061,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResetInstanceBlueprints(self, request):
         """本接口（DescribeResetInstanceBlueprints）查询重置实例的镜像信息。
 
         :param request: Request instance for DescribeResetInstanceBlueprints.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeResetInstanceBlueprintsRequest`
@@ -1084,15 +1084,15 @@
             model = models.DescribeResetInstanceBlueprintsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeScenes(self, request):
         """本接口(DescribeScenes)用于查看使用场景列表。
 
         :param request: Request instance for DescribeScenes.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeScenesRequest`
@@ -1107,15 +1107,15 @@
             model = models.DescribeScenesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshots(self, request):
         """本接口（DescribeSnapshots）用于查询快照的详细信息。
 
         :param request: Request instance for DescribeSnapshots.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeSnapshotsRequest`
@@ -1130,15 +1130,15 @@
             model = models.DescribeSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotsDeniedActions(self, request):
         """本接口（DescribeSnapshotsDeniedActions）用于查询一个或多个快照的操作限制列表信息。
 
         :param request: Request instance for DescribeSnapshotsDeniedActions.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeSnapshotsDeniedActionsRequest`
@@ -1153,15 +1153,15 @@
             model = models.DescribeSnapshotsDeniedActionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeZones(self, request):
         """查询地域下可用区
 
         :param request: Request instance for DescribeZones.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DescribeZonesRequest`
@@ -1176,15 +1176,15 @@
             model = models.DescribeZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachCcn(self, request):
         """本接口 (DetachCcn) 用于解除与云联网的关联。
 
         :param request: Request instance for DetachCcn.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DetachCcnRequest`
@@ -1199,15 +1199,15 @@
             model = models.DetachCcnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetachDisks(self, request):
         """本接口（DetachDisks）用于卸载一个或多个云硬盘。
 
         :param request: Request instance for DetachDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.DetachDisksRequest`
@@ -1222,15 +1222,15 @@
             model = models.DetachDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisassociateInstancesKeyPairs(self, request):
         """本接口（DisassociateInstancesKeyPairs）用于解除实例与指定密钥对的绑定关系。
 
         * 只支持 [RUNNING, STOPPED] 状态的 LINUX_UNIX 操作系统的实例。处于 RUNNING 状态的实例会强制关机，然后解绑。
         * 解绑密钥后，实例可以通过原来设置的密码登录。
@@ -1251,15 +1251,15 @@
             model = models.DisassociateInstancesKeyPairsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportKeyPair(self, request):
         """本接口（ImportKeyPair）用于导入用户指定密钥对。
 
         :param request: Request instance for ImportKeyPair.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ImportKeyPairRequest`
@@ -1274,15 +1274,15 @@
             model = models.ImportKeyPairResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreateBlueprint(self, request):
         """本接口 (InquirePriceCreateBlueprint) 用于创建镜像询价。
 
         :param request: Request instance for InquirePriceCreateBlueprint.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.InquirePriceCreateBlueprintRequest`
@@ -1297,15 +1297,15 @@
             model = models.InquirePriceCreateBlueprintResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreateDisks(self, request):
         """本接口（InquirePriceCreateDisks）用于新购云硬盘询价。
 
         :param request: Request instance for InquirePriceCreateDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.InquirePriceCreateDisksRequest`
@@ -1320,15 +1320,15 @@
             model = models.InquirePriceCreateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceCreateInstances(self, request):
         """本接口（InquiryPriceCreateInstances）用于创建实例询价。
 
         :param request: Request instance for InquirePriceCreateInstances.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.InquirePriceCreateInstancesRequest`
@@ -1343,15 +1343,15 @@
             model = models.InquirePriceCreateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceRenewDisks(self, request):
         """本接口（InquirePriceRenewDisks）用于续费云硬盘询价。
 
         :param request: Request instance for InquirePriceRenewDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.InquirePriceRenewDisksRequest`
@@ -1366,15 +1366,15 @@
             model = models.InquirePriceRenewDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceRenewInstances(self, request):
         """本接口（InquirePriceRenewInstances）用于续费实例询价。
 
         :param request: Request instance for InquirePriceRenewInstances.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.InquirePriceRenewInstancesRequest`
@@ -1389,15 +1389,15 @@
             model = models.InquirePriceRenewInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateDisks(self, request):
         """本接口(IsolateDisks)用于退还一个或多个轻量应用服务器云硬盘。
 
         只有状态为 UNATTACHED 的数据盘才可以进行此操作。
         接口调用成功后，云硬盘会进入SHUTDOWN 状态。
@@ -1417,15 +1417,15 @@
             model = models.IsolateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def IsolateInstances(self, request):
         """本接口(IsolateInstances)用于退还一个或多个轻量应用服务器实例。
         * 只有状态为 RUNNING 或 STOPPED 的实例才可以进行此操作。
         * 接口调用成功后，实例会进入SHUTDOWN 状态。
         * 支持批量操作。每次请求批量资源（包括实例与数据盘）的上限为 20。
@@ -1444,15 +1444,15 @@
             model = models.IsolateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyBlueprintAttribute(self, request):
         """本接口 (ModifyBlueprintAttribute) 用于修改镜像属性。
 
         :param request: Request instance for ModifyBlueprintAttribute.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ModifyBlueprintAttributeRequest`
@@ -1467,15 +1467,15 @@
             model = models.ModifyBlueprintAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDiskBackupsAttribute(self, request):
         """本接口 (ModifyDiskBackupsAttribute) 用于修改云硬盘备份点属性。
 
         :param request: Request instance for ModifyDiskBackupsAttribute.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ModifyDiskBackupsAttributeRequest`
@@ -1490,15 +1490,15 @@
             model = models.ModifyDiskBackupsAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDisksAttribute(self, request):
         """本接口(ModifyDisksAttribute)用于修改云硬盘属性。
 
         :param request: Request instance for ModifyDisksAttribute.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ModifyDisksAttributeRequest`
@@ -1513,15 +1513,15 @@
             model = models.ModifyDisksAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDisksRenewFlag(self, request):
         """本接口（ModifyDisksRenewFlag）用于修改云硬盘续费标识。
 
         :param request: Request instance for ModifyDisksRenewFlag.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ModifyDisksRenewFlagRequest`
@@ -1536,15 +1536,15 @@
             model = models.ModifyDisksRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFirewallRuleDescription(self, request):
         """本接口（ModifyFirewallRuleDescription）用于修改单条防火墙规则描述。
 
         * FirewallVersion 用于指定要操作的防火墙的版本。传入 FirewallVersion 版本号若不等于当前防火墙的最新版本，将返回失败；若不传 FirewallVersion 则直接修改防火墙规则备注。
 
@@ -1568,15 +1568,15 @@
             model = models.ModifyFirewallRuleDescriptionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyFirewallRules(self, request):
         """本接口（ModifyFirewallRules）用于重置实例防火墙规则。
 
         本接口先删除当前实例的所有防火墙规则，然后添加新的规则。
 
@@ -1602,15 +1602,15 @@
             model = models.ModifyFirewallRulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesAttribute(self, request):
         """本接口（ModifyInstancesAttribute）用于修改实例的属性。
         * “实例名称”仅为方便用户自己管理之用。
         * 支持批量操作。每次请求批量实例的上限为 100。
 
@@ -1627,15 +1627,15 @@
             model = models.ModifyInstancesAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesBundle(self, request):
         """本接口(ModifyInstancesBundle)用于变更一个或多个轻量应用服务器实例套餐。
         * 只有状态为 RUNNING，STOPPED的实例才可以进行此操作。
         * 支持批量操作。每次请求批量实例的上限为 30。
         * 本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。实例操作结果可以通过调用 DescribeInstances 接口查询，如果实例的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
@@ -1653,15 +1653,15 @@
             model = models.ModifyInstancesBundleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesLoginKeyPairAttribute(self, request):
         """本接口用于设置实例默认登录密钥对属性。
 
 
         :param request: Request instance for ModifyInstancesLoginKeyPairAttribute.
@@ -1677,15 +1677,15 @@
             model = models.ModifyInstancesLoginKeyPairAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstancesRenewFlag(self, request):
         """本接口 (ModifyInstancesRenewFlag) 用于修改包年包月实例续费标识。
 
         * 实例被标识为自动续费后，每次在实例到期时，会自动续费一个月。
         * 支持批量操作。每次请求批量实例的上限为100。
@@ -1703,15 +1703,15 @@
             model = models.ModifyInstancesRenewFlagResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySnapshotAttribute(self, request):
         """本接口（ModifySnapshotAttribute）用于修改指定快照的属性。
         <li>“快照名称”仅为方便用户自己管理之用。</li>
 
         :param request: Request instance for ModifySnapshotAttribute.
@@ -1727,15 +1727,15 @@
             model = models.ModifySnapshotAttributeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RebootInstances(self, request):
         """本接口（RebootInstances）用于重启实例。
 
         * 只有状态为 RUNNING 的实例才可以进行此操作。
         * 接口调用成功时，实例会进入 REBOOTING 状态；重启实例成功时，实例会进入 RUNNING 状态。
@@ -1755,15 +1755,15 @@
             model = models.RebootInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewDisks(self, request):
         """本接口(RenewDisks)用于续费一个或多个轻量应用服务器云硬盘。
 
         只有状态为 ATTACHED，UNATTACHED 或 SHUTDOWN 的数据盘才可以进行此操作。
         支持批量操作。每次请求批量云硬盘的上限为 50。
@@ -1782,15 +1782,15 @@
             model = models.RenewDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RenewInstances(self, request):
         """本接口(RenewInstances)用于续费一个或多个轻量应用服务器实例。
         * 只有状态为 RUNNING，STOPPED 或 SHUTDOWN 的实例才可以进行此操作。
         * 支持批量操作。每次请求批量实例的上限为 100。
         * 本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。实例操作结果可以通过调用 DescribeInstances 接口查询，如果实例的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
@@ -1808,15 +1808,15 @@
             model = models.RenewInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetAttachCcn(self, request):
         """本接口 (ResetAttachCcn) 用于关联云联网实例申请过期时，重新申请关联操作。
 
         :param request: Request instance for ResetAttachCcn.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ResetAttachCcnRequest`
@@ -1831,15 +1831,15 @@
             model = models.ResetAttachCcnResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstance(self, request):
         """本接口（ResetInstance）用于重装指定实例上的镜像。
 
         * 如果指定了 BlueprintId 参数，则使用指定的镜像重装；否则按照当前实例使用的镜像进行重装。
         * 系统盘将会被格式化，并重置；请确保系统盘中无重要文件。
@@ -1859,15 +1859,15 @@
             model = models.ResetInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetInstancesPassword(self, request):
         """本接口（ResetInstancesPassword）用于将实例操作系统的密码重置为用户指定的密码。
         * 只修改管理员帐号的密码。实例的操作系统不同，管理员帐号也会不一样（Windows 为 Administrator，Ubuntu 为 ubuntu ，其它系统为 root）。
         * 支持批量操作。将多个实例操作系统的密码重置为相同的密码。每次请求批量实例的上限为 100。
         * 建议对运行中的实例先手动关机，然后再进行密码重置。如实例处于运行中状态，本接口操作过程中会对实例进行关机操作，尝试正常关机失败后进行强制关机。
@@ -1887,15 +1887,15 @@
             model = models.ResetInstancesPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartInstances(self, request):
         """本接口（StartInstances）用于启动一个或多个实例。
 
         * 只有状态为 STOPPED 的实例才可以进行此操作。
         * 接口调用成功时，实例会进入 STARTING 状态；启动实例成功时，实例会进入 RUNNING 状态。
@@ -1915,15 +1915,15 @@
             model = models.StartInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopInstances(self, request):
         """本接口（StopInstances）用于关闭一个或多个实例。
         * 只有状态为 RUNNING 的实例才可以进行此操作。
         * 接口调用成功时，实例会进入 STOPPING 状态；关闭实例成功时，实例会进入 STOPPED 状态。
         * 支持批量操作。每次请求批量实例的上限为 100。
@@ -1942,15 +1942,15 @@
             model = models.StopInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateDisks(self, request):
         """本接口（TerminateDisks）用于销毁一个或多个云硬盘。
 
         :param request: Request instance for TerminateDisks.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.TerminateDisksRequest`
@@ -1965,15 +1965,15 @@
             model = models.TerminateDisksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateInstances(self, request):
         """本接口 (TerminateInstances) 用于销毁实例。
 
         * 处于 SHUTDOWN 状态的实例，可通过本接口销毁，且不可恢复。
         * 支持批量操作，每次请求批量实例的上限为100。
@@ -1992,8 +1992,8 @@
             model = models.TerminateInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7033,21 +7033,24 @@
         :type Envs: list of ContainerEnv
         :param _PublishPorts: 容器端口主机端口映射列表
         :type PublishPorts: list of DockerContainerPublishPort
         :param _Volumes: 容器加载本地卷列表
         :type Volumes: list of DockerContainerVolume
         :param _Command: 运行的命令
         :type Command: str
+        :param _RestartPolicy: 容器重启策略
+        :type RestartPolicy: str
         """
         self._ContainerImage = None
         self._ContainerName = None
         self._Envs = None
         self._PublishPorts = None
         self._Volumes = None
         self._Command = None
+        self._RestartPolicy = None
 
     @property
     def ContainerImage(self):
         return self._ContainerImage
 
     @ContainerImage.setter
     def ContainerImage(self, ContainerImage):
@@ -7089,14 +7092,22 @@
     def Command(self):
         return self._Command
 
     @Command.setter
     def Command(self, Command):
         self._Command = Command
 
+    @property
+    def RestartPolicy(self):
+        return self._RestartPolicy
+
+    @RestartPolicy.setter
+    def RestartPolicy(self, RestartPolicy):
+        self._RestartPolicy = RestartPolicy
+
 
     def _deserialize(self, params):
         self._ContainerImage = params.get("ContainerImage")
         self._ContainerName = params.get("ContainerName")
         if params.get("Envs") is not None:
             self._Envs = []
             for item in params.get("Envs"):
@@ -7112,14 +7123,15 @@
         if params.get("Volumes") is not None:
             self._Volumes = []
             for item in params.get("Volumes"):
                 obj = DockerContainerVolume()
                 obj._deserialize(item)
                 self._Volumes.append(obj)
         self._Command = params.get("Command")
+        self._RestartPolicy = params.get("RestartPolicy")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.937/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.938/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

