# Comparing `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.937.tar", last modified: Tue Jul 18 00:31:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.938.tar", last modified: Wed Jul 19 00:48:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937.tar` & `tencentcloud-sdk-python-tcaplusdb-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/
--rw-r--r--   0 root         (0) root         (0)    48988 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   309129 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-18 00:31:18.000000 tencentcloud-sdk-python-tcaplusdb-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/
+-rw-r--r--   0 root         (0) root         (0)    49200 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   309129 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-19 00:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/setup.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ClearTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CompareIdlFiles(self, request):
         """选中目标表格，上传并校验改表文件，返回是否允许修改表格结构的结果。
 
         :param request: Request instance for CompareIdlFiles.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CompareIdlFilesRequest`
@@ -65,15 +65,15 @@
             model = models.CompareIdlFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateBackup(self, request):
         """用户创建备份任务
 
         :param request: Request instance for CreateBackup.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CreateBackupRequest`
@@ -88,15 +88,15 @@
             model = models.CreateBackupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """本接口用于创建TcaplusDB集群
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CreateClusterRequest`
@@ -111,15 +111,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSnapshots(self, request):
         """构造表格过去时间点的快照
 
         :param request: Request instance for CreateSnapshots.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CreateSnapshotsRequest`
@@ -134,15 +134,15 @@
             model = models.CreateSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTableGroup(self, request):
         """在TcaplusDB集群下创建表格组
 
         :param request: Request instance for CreateTableGroup.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CreateTableGroupRequest`
@@ -157,15 +157,15 @@
             model = models.CreateTableGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTables(self, request):
         """根据选择的IDL文件列表，批量创建表格
 
         :param request: Request instance for CreateTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.CreateTablesRequest`
@@ -180,15 +180,15 @@
             model = models.CreateTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteBackupRecords(self, request):
         """删除手工备份
 
         :param request: Request instance for DeleteBackupRecords.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteBackupRecordsRequest`
@@ -203,15 +203,15 @@
             model = models.DeleteBackupRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCluster(self, request):
         """删除TcaplusDB集群，必须在集群所属所有资源（包括表格组，表）都已经释放的情况下才会成功。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteClusterRequest`
@@ -226,15 +226,15 @@
             model = models.DeleteClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIdlFiles(self, request):
         """指定集群ID和待删除IDL文件的信息，删除目标文件，如果文件正在被表关联则删除失败。
 
         :param request: Request instance for DeleteIdlFiles.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteIdlFilesRequest`
@@ -249,15 +249,15 @@
             model = models.DeleteIdlFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshots(self, request):
         """删除表格的快照
 
         :param request: Request instance for DeleteSnapshots.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteSnapshotsRequest`
@@ -272,15 +272,15 @@
             model = models.DeleteSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTableDataFlow(self, request):
         """删除表格的数据订阅
 
         :param request: Request instance for DeleteTableDataFlow.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteTableDataFlowRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteTableDataFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTableGroup(self, request):
         """删除表格组
 
         :param request: Request instance for DeleteTableGroup.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteTableGroupRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteTableGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTableIndex(self, request):
         """删除表格的分布式索引
 
         :param request: Request instance for DeleteTableIndex.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteTableIndexRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteTableIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTables(self, request):
         """删除指定的表,第一次调用此接口代表将表移动至回收站，再次调用代表将此表格从回收站中彻底删除。
 
         :param request: Request instance for DeleteTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteTablesRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApplications(self, request):
         """获取审批管理的申请单
 
         :param request: Request instance for DescribeApplications.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeApplicationsRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBackupRecords(self, request):
         """查询备份记录
 
         查询集群级别时， 将TableGroupId设置为"-1", 将TableName设置为"-1"
         查询集群+表格组级别时， 将TableName设置为"-1"
@@ -414,15 +414,15 @@
             model = models.DescribeBackupRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterTags(self, request):
         """获取集群关联的标签列表
 
         :param request: Request instance for DescribeClusterTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeClusterTagsRequest`
@@ -437,15 +437,15 @@
             model = models.DescribeClusterTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusters(self, request):
         """查询TcaplusDB集群列表，包含集群详细信息。
 
         :param request: Request instance for DescribeClusters.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeClustersRequest`
@@ -460,15 +460,15 @@
             model = models.DescribeClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIdlFileInfos(self, request):
         """查询表描述文件详情
 
         :param request: Request instance for DescribeIdlFileInfos.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeIdlFileInfosRequest`
@@ -483,15 +483,15 @@
             model = models.DescribeIdlFileInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMachine(self, request):
         """查询独占集群可以申请的剩余机器
 
         :param request: Request instance for DescribeMachine.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeMachineRequest`
@@ -506,15 +506,15 @@
             model = models.DescribeMachineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRegions(self, request):
         """查询TcaplusDB服务支持的地域列表
 
         :param request: Request instance for DescribeRegions.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeRegionsRequest`
@@ -529,15 +529,15 @@
             model = models.DescribeRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshots(self, request):
         """查询快照列表
 
         :param request: Request instance for DescribeSnapshots.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeSnapshotsRequest`
@@ -552,15 +552,15 @@
             model = models.DescribeSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableGroupTags(self, request):
         """获取表格组关联的标签列表
 
         :param request: Request instance for DescribeTableGroupTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTableGroupTagsRequest`
@@ -575,15 +575,15 @@
             model = models.DescribeTableGroupTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableGroups(self, request):
         """查询表格组列表
 
         :param request: Request instance for DescribeTableGroups.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTableGroupsRequest`
@@ -598,15 +598,15 @@
             model = models.DescribeTableGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTableTags(self, request):
         """获取表格标签
 
         :param request: Request instance for DescribeTableTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTableTagsRequest`
@@ -621,15 +621,15 @@
             model = models.DescribeTableTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTables(self, request):
         """查询表详情
 
         :param request: Request instance for DescribeTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTablesRequest`
@@ -644,15 +644,15 @@
             model = models.DescribeTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTablesInRecycle(self, request):
         """查询回收站中的表详情
 
         :param request: Request instance for DescribeTablesInRecycle.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTablesInRecycleRequest`
@@ -667,15 +667,15 @@
             model = models.DescribeTablesInRecycleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """查询任务列表
 
         :param request: Request instance for DescribeTasks.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeTasksRequest`
@@ -690,15 +690,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUinInWhitelist(self, request):
         """查询本用户是否在白名单中，控制是否能创建TDR类型的APP或表
 
         :param request: Request instance for DescribeUinInWhitelist.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeUinInWhitelistRequest`
@@ -713,15 +713,15 @@
             model = models.DescribeUinInWhitelistResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableRestProxy(self, request):
         """当restful api为关闭状态时，可以通过此接口关闭restful api
 
         :param request: Request instance for DisableRestProxy.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DisableRestProxyRequest`
@@ -736,15 +736,15 @@
             model = models.DisableRestProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableRestProxy(self, request):
         """当restful api为关闭状态时，可以通过此接口开启restful apu
 
         :param request: Request instance for EnableRestProxy.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.EnableRestProxyRequest`
@@ -759,15 +759,15 @@
             model = models.EnableRestProxyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportSnapshots(self, request):
         """将快照数据导入到新表或当前表
 
         :param request: Request instance for ImportSnapshots.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ImportSnapshotsRequest`
@@ -782,15 +782,15 @@
             model = models.ImportSnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MergeTablesData(self, request):
         """合并指定表格
 
         :param request: Request instance for MergeTablesData.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.MergeTablesDataRequest`
@@ -805,15 +805,15 @@
             model = models.MergeTablesDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCensorship(self, request):
         """修改集群审批状态
 
         :param request: Request instance for ModifyCensorship.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyCensorshipRequest`
@@ -828,15 +828,15 @@
             model = models.ModifyCensorshipResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterMachine(self, request):
         """修改独占集群机器
 
         :param request: Request instance for ModifyClusterMachine.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyClusterMachineRequest`
@@ -851,15 +851,15 @@
             model = models.ModifyClusterMachineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterName(self, request):
         """修改指定的集群名称
 
         :param request: Request instance for ModifyClusterName.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyClusterNameRequest`
@@ -874,15 +874,15 @@
             model = models.ModifyClusterNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterPassword(self, request):
         """修改指定集群的密码，后台将在旧密码失效之前同时支持TcaplusDB SDK使用旧密码和新密码访问数据库。在旧密码失效之前不能提交新的密码修改请求，在旧密码失效之后不能提交修改旧密码过期时间的请求。
 
         :param request: Request instance for ModifyClusterPassword.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyClusterPasswordRequest`
@@ -897,15 +897,15 @@
             model = models.ModifyClusterPasswordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyClusterTags(self, request):
         """修改集群标签
 
         :param request: Request instance for ModifyClusterTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyClusterTagsRequest`
@@ -920,15 +920,15 @@
             model = models.ModifyClusterTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySnapshots(self, request):
         """修改表格快照的过期时间
 
         :param request: Request instance for ModifySnapshots.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifySnapshotsRequest`
@@ -943,15 +943,15 @@
             model = models.ModifySnapshotsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTableGroupName(self, request):
         """修改TcaplusDB表格组名称
 
         :param request: Request instance for ModifyTableGroupName.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTableGroupNameRequest`
@@ -966,15 +966,15 @@
             model = models.ModifyTableGroupNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTableGroupTags(self, request):
         """修改表格组标签
 
         :param request: Request instance for ModifyTableGroupTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTableGroupTagsRequest`
@@ -989,15 +989,15 @@
             model = models.ModifyTableGroupTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTableMemos(self, request):
         """修改表备注信息
 
         :param request: Request instance for ModifyTableMemos.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTableMemosRequest`
@@ -1012,15 +1012,15 @@
             model = models.ModifyTableMemosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTableQuotas(self, request):
         """表格扩缩容
 
         :param request: Request instance for ModifyTableQuotas.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTableQuotasRequest`
@@ -1035,15 +1035,15 @@
             model = models.ModifyTableQuotasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTableTags(self, request):
         """修改表格标签
 
         :param request: Request instance for ModifyTableTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTableTagsRequest`
@@ -1058,15 +1058,15 @@
             model = models.ModifyTableTagsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTables(self, request):
         """根据用户选定的表定义IDL文件，批量修改指定的表
 
         :param request: Request instance for ModifyTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.ModifyTablesRequest`
@@ -1081,15 +1081,15 @@
             model = models.ModifyTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecoverRecycleTables(self, request):
         """恢复回收站中，用户自行删除的表。对欠费待释放的表无效。
 
         :param request: Request instance for RecoverRecycleTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.RecoverRecycleTablesRequest`
@@ -1104,15 +1104,15 @@
             model = models.RecoverRecycleTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackTables(self, request):
         """表格数据回档
 
         :param request: Request instance for RollbackTables.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.RollbackTablesRequest`
@@ -1127,15 +1127,15 @@
             model = models.RollbackTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetBackupExpireRule(self, request):
         """新增、删除、修改备份过期策略， ClusterId必须为具体的集群Id（appid）
 
         :param request: Request instance for SetBackupExpireRule.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.SetBackupExpireRuleRequest`
@@ -1150,15 +1150,15 @@
             model = models.SetBackupExpireRuleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTableDataFlow(self, request):
         """新增、修改表格数据订阅
 
         :param request: Request instance for SetTableDataFlow.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.SetTableDataFlowRequest`
@@ -1173,15 +1173,15 @@
             model = models.SetTableDataFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetTableIndex(self, request):
         """设置表格分布式索引
 
         :param request: Request instance for SetTableIndex.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.SetTableIndexRequest`
@@ -1196,15 +1196,15 @@
             model = models.SetTableIndexResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateApply(self, request):
         """更新申请单状态
 
         :param request: Request instance for UpdateApply.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.UpdateApplyRequest`
@@ -1219,15 +1219,15 @@
             model = models.UpdateApplyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyIdlFiles(self, request):
         """上传并校验创建表格文件，返回校验合法的表格定义
 
         :param request: Request instance for VerifyIdlFiles.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.VerifyIdlFilesRequest`
@@ -1242,8 +1242,8 @@
             model = models.VerifyIdlFilesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud/tcaplusdb/v20190823/models.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud/tcaplusdb/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.937/README.rst` & `tencentcloud-sdk-python-tcaplusdb-3.0.938/README.rst`

 * *Files identical despite different names*

