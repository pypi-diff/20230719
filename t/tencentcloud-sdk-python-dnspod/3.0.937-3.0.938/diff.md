# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.937.tar", last modified: Tue Jul 18 00:22:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.938.tar", last modified: Wed Jul 19 00:37:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.937.tar` & `tencentcloud-sdk-python-dnspod-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    60713 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24039 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   340184 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    60981 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24039 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   340184 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-19 00:37:52.000000 tencentcloud-sdk-python-dnspod-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CheckRecordSnapshotRollbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CheckSnapshotRollback(self, request):
         """快照回滚前检查
 
         :param request: Request instance for CheckSnapshotRollback.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CheckSnapshotRollbackRequest`
@@ -65,15 +65,15 @@
             model = models.CheckSnapshotRollbackResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDeal(self, request):
         """DNSPod商品下单
 
         :param request: Request instance for CreateDeal.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateDealRequest`
@@ -88,15 +88,15 @@
             model = models.CreateDealResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomain(self, request):
         """添加域名
 
         :param request: Request instance for CreateDomain.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateDomainRequest`
@@ -111,15 +111,15 @@
             model = models.CreateDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomainAlias(self, request):
         """创建域名别名
 
         :param request: Request instance for CreateDomainAlias.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateDomainAliasRequest`
@@ -134,15 +134,15 @@
             model = models.CreateDomainAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomainBatch(self, request):
         """批量添加域名
 
         :param request: Request instance for CreateDomainBatch.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateDomainBatchRequest`
@@ -157,15 +157,15 @@
             model = models.CreateDomainBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDomainGroup(self, request):
         """创建域名分组
 
         :param request: Request instance for CreateDomainGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateDomainGroupRequest`
@@ -180,15 +180,15 @@
             model = models.CreateDomainGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecord(self, request):
         """添加记录
 
         :param request: Request instance for CreateRecord.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateRecordRequest`
@@ -203,15 +203,15 @@
             model = models.CreateRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecordBatch(self, request):
         """批量添加记录
 
         :param request: Request instance for CreateRecordBatch.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateRecordBatchRequest`
@@ -226,15 +226,15 @@
             model = models.CreateRecordBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecordGroup(self, request):
         """添加记录分组
 
         :param request: Request instance for CreateRecordGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateRecordGroupRequest`
@@ -249,15 +249,15 @@
             model = models.CreateRecordGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSnapshot(self, request):
         """创建快照
 
         :param request: Request instance for CreateSnapshot.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.CreateSnapshotRequest`
@@ -272,15 +272,15 @@
             model = models.CreateSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomain(self, request):
         """删除域名
 
         :param request: Request instance for DeleteDomain.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteDomainRequest`
@@ -295,15 +295,15 @@
             model = models.DeleteDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomainAlias(self, request):
         """删除域名别名
 
         :param request: Request instance for DeleteDomainAlias.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteDomainAliasRequest`
@@ -318,15 +318,15 @@
             model = models.DeleteDomainAliasResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDomainBatch(self, request):
         """批量删除域名
 
         :param request: Request instance for DeleteDomainBatch.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteDomainBatchRequest`
@@ -341,15 +341,15 @@
             model = models.DeleteDomainBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecord(self, request):
         """删除记录
 
         :param request: Request instance for DeleteRecord.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordRequest`
@@ -364,15 +364,15 @@
             model = models.DeleteRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecordBatch(self, request):
         """批量删除解析记录
 
         :param request: Request instance for DeleteRecordBatch.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordBatchRequest`
@@ -387,15 +387,15 @@
             model = models.DeleteRecordBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRecordGroup(self, request):
         """删除记录分组
 
         :param request: Request instance for DeleteRecordGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteRecordGroupRequest`
@@ -410,15 +410,15 @@
             model = models.DeleteRecordGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteShareDomain(self, request):
         """删除域名共享
 
         :param request: Request instance for DeleteShareDomain.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteShareDomainRequest`
@@ -433,15 +433,15 @@
             model = models.DeleteShareDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshot(self, request):
         """删除快照
 
         :param request: Request instance for DeleteSnapshot.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DeleteSnapshotRequest`
@@ -456,15 +456,15 @@
             model = models.DeleteSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeBatchTask(self, request):
         """获取任务详情
 
         :param request: Request instance for DescribeBatchTask.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeBatchTaskRequest`
@@ -479,15 +479,15 @@
             model = models.DescribeBatchTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomain(self, request):
         """获取域名信息
 
         :param request: Request instance for DescribeDomain.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainRequest`
@@ -502,15 +502,15 @@
             model = models.DescribeDomainResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainAliasList(self, request):
         """获取域名别名列表
 
         :param request: Request instance for DescribeDomainAliasList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainAliasListRequest`
@@ -525,15 +525,15 @@
             model = models.DescribeDomainAliasListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainAnalytics(self, request):
         """统计各个域名的解析量，帮助您了解流量情况、时间段分布。支持查看近 3 个月内的统计情况
 
         :param request: Request instance for DescribeDomainAnalytics.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainAnalyticsRequest`
@@ -548,15 +548,15 @@
             model = models.DescribeDomainAnalyticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainFilterList(self, request):
         """获取域名筛选列表
 
         :param request: Request instance for DescribeDomainFilterList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainFilterListRequest`
@@ -571,15 +571,15 @@
             model = models.DescribeDomainFilterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainGroupList(self, request):
         """获取域名分组列表
 
         :param request: Request instance for DescribeDomainGroupList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainGroupListRequest`
@@ -594,15 +594,15 @@
             model = models.DescribeDomainGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainList(self, request):
         """获取域名列表
 
         :param request: Request instance for DescribeDomainList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainListRequest`
@@ -617,15 +617,15 @@
             model = models.DescribeDomainListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainLogList(self, request):
         """获取域名日志
 
         :param request: Request instance for DescribeDomainLogList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainLogListRequest`
@@ -640,15 +640,15 @@
             model = models.DescribeDomainLogListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainPreview(self, request):
         """获取域名概览信息
 
         :param request: Request instance for DescribeDomainPreview.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainPreviewRequest`
@@ -663,15 +663,15 @@
             model = models.DescribeDomainPreviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainPurview(self, request):
         """获取域名权限
 
         :param request: Request instance for DescribeDomainPurview.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainPurviewRequest`
@@ -686,15 +686,15 @@
             model = models.DescribeDomainPurviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainShareInfo(self, request):
         """获取域名共享信息
 
         :param request: Request instance for DescribeDomainShareInfo.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainShareInfoRequest`
@@ -709,15 +709,15 @@
             model = models.DescribeDomainShareInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDomainWhois(self, request):
         """获取域名Whois信息
 
         :param request: Request instance for DescribeDomainWhois.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainWhoisRequest`
@@ -732,15 +732,15 @@
             model = models.DescribeDomainWhoisResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePackageDetail(self, request):
         """获取各套餐配置详情
 
         :param request: Request instance for DescribePackageDetail.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribePackageDetailRequest`
@@ -755,15 +755,15 @@
             model = models.DescribePackageDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecord(self, request):
         """获取记录信息
 
         :param request: Request instance for DescribeRecord.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordRequest`
@@ -778,15 +778,15 @@
             model = models.DescribeRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordExistExceptDefaultNS(self, request):
         """判断是否有除系统默认的@-NS记录之外的记录存在
 
         :param request: Request instance for DescribeRecordExistExceptDefaultNS.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordExistExceptDefaultNSRequest`
@@ -801,15 +801,15 @@
             model = models.DescribeRecordExistExceptDefaultNSResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordGroupList(self, request):
         """查询解析记录分组列表
 
         :param request: Request instance for DescribeRecordGroupList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordGroupListRequest`
@@ -824,15 +824,15 @@
             model = models.DescribeRecordGroupListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordLineList(self, request):
         """获取等级允许的线路
 
         :param request: Request instance for DescribeRecordLineList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordLineListRequest`
@@ -847,15 +847,15 @@
             model = models.DescribeRecordLineListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordList(self, request):
         """获取某个域名下的解析记录列表
 
         :param request: Request instance for DescribeRecordList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordListRequest`
@@ -870,15 +870,15 @@
             model = models.DescribeRecordListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordSnapshotRollbackResult(self, request):
         """查询解析记录重新回滚的结果
 
         :param request: Request instance for DescribeRecordSnapshotRollbackResult.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordSnapshotRollbackResultRequest`
@@ -893,15 +893,15 @@
             model = models.DescribeRecordSnapshotRollbackResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRecordType(self, request):
         """获取等级允许的记录类型
 
         :param request: Request instance for DescribeRecordType.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeRecordTypeRequest`
@@ -916,15 +916,15 @@
             model = models.DescribeRecordTypeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotConfig(self, request):
         """查询解析快照配置
 
         :param request: Request instance for DescribeSnapshotConfig.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeSnapshotConfigRequest`
@@ -939,15 +939,15 @@
             model = models.DescribeSnapshotConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotList(self, request):
         """查询快照列表
 
         :param request: Request instance for DescribeSnapshotList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeSnapshotListRequest`
@@ -962,15 +962,15 @@
             model = models.DescribeSnapshotListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotRollbackResult(self, request):
         """查询快照回滚结果
 
         :param request: Request instance for DescribeSnapshotRollbackResult.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeSnapshotRollbackResultRequest`
@@ -985,15 +985,15 @@
             model = models.DescribeSnapshotRollbackResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotRollbackTask(self, request):
         """查询最近一次回滚
 
         :param request: Request instance for DescribeSnapshotRollbackTask.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeSnapshotRollbackTaskRequest`
@@ -1008,15 +1008,15 @@
             model = models.DescribeSnapshotRollbackTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSubdomainAnalytics(self, request):
         """统计子域名的解析量，帮助您了解流量情况、时间段分布。支持查看近 3 个月内的统计情况。仅付费套餐域名可用。
 
         :param request: Request instance for DescribeSubdomainAnalytics.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeSubdomainAnalyticsRequest`
@@ -1031,15 +1031,15 @@
             model = models.DescribeSubdomainAnalyticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUserDetail(self, request):
         """获取帐户信息
 
         :param request: Request instance for DescribeUserDetail.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeUserDetailRequest`
@@ -1054,15 +1054,15 @@
             model = models.DescribeUserDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVASStatistic(self, request):
         """获取域名增值服务用量
 
         :param request: Request instance for DescribeVASStatistic.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeVASStatisticRequest`
@@ -1077,15 +1077,15 @@
             model = models.DescribeVASStatisticResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadSnapshot(self, request):
         """下载快照
 
         :param request: Request instance for DownloadSnapshot.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DownloadSnapshotRequest`
@@ -1100,15 +1100,15 @@
             model = models.DownloadSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainLock(self, request):
         """锁定域名
 
         :param request: Request instance for ModifyDomainLock.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDomainLockRequest`
@@ -1123,15 +1123,15 @@
             model = models.ModifyDomainLockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainOwner(self, request):
         """域名过户
 
         :param request: Request instance for ModifyDomainOwner.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDomainOwnerRequest`
@@ -1146,15 +1146,15 @@
             model = models.ModifyDomainOwnerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainRemark(self, request):
         """设置域名备注
 
         :param request: Request instance for ModifyDomainRemark.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDomainRemarkRequest`
@@ -1169,15 +1169,15 @@
             model = models.ModifyDomainRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainStatus(self, request):
         """修改域名状态
 
         :param request: Request instance for ModifyDomainStatus.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDomainStatusRequest`
@@ -1192,15 +1192,15 @@
             model = models.ModifyDomainStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDomainUnlock(self, request):
         """域名锁定解锁
 
         :param request: Request instance for ModifyDomainUnlock.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDomainUnlockRequest`
@@ -1215,15 +1215,15 @@
             model = models.ModifyDomainUnlockResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDynamicDNS(self, request):
         """更新动态 DNS 记录
 
         :param request: Request instance for ModifyDynamicDNS.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyDynamicDNSRequest`
@@ -1238,15 +1238,15 @@
             model = models.ModifyDynamicDNSResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPackageAutoRenew(self, request):
         """DNS 解析套餐自动续费设置
 
         :param request: Request instance for ModifyPackageAutoRenew.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyPackageAutoRenewRequest`
@@ -1261,15 +1261,15 @@
             model = models.ModifyPackageAutoRenewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecord(self, request):
         """修改记录
 
         :param request: Request instance for ModifyRecord.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordRequest`
@@ -1284,15 +1284,15 @@
             model = models.ModifyRecordResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordBatch(self, request):
         """批量修改记录
 
         :param request: Request instance for ModifyRecordBatch.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordBatchRequest`
@@ -1307,15 +1307,15 @@
             model = models.ModifyRecordBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordFields(self, request):
         """修改记录可选字段
 
         :param request: Request instance for ModifyRecordFields.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordFieldsRequest`
@@ -1330,15 +1330,15 @@
             model = models.ModifyRecordFieldsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordGroup(self, request):
         """修改记录分组
 
         :param request: Request instance for ModifyRecordGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordGroupRequest`
@@ -1353,15 +1353,15 @@
             model = models.ModifyRecordGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordRemark(self, request):
         """设置记录备注
 
         :param request: Request instance for ModifyRecordRemark.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordRemarkRequest`
@@ -1376,15 +1376,15 @@
             model = models.ModifyRecordRemarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordStatus(self, request):
         """修改解析记录的状态
 
         :param request: Request instance for ModifyRecordStatus.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordStatusRequest`
@@ -1399,15 +1399,15 @@
             model = models.ModifyRecordStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyRecordToGroup(self, request):
         """将记录添加到分组
 
         :param request: Request instance for ModifyRecordToGroup.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyRecordToGroupRequest`
@@ -1422,15 +1422,15 @@
             model = models.ModifyRecordToGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySnapshotConfig(self, request):
         """修改快照配置
 
         :param request: Request instance for ModifySnapshotConfig.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifySnapshotConfigRequest`
@@ -1445,15 +1445,15 @@
             model = models.ModifySnapshotConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySubdomainStatus(self, request):
         """暂停子域名的解析记录
 
         :param request: Request instance for ModifySubdomainStatus.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifySubdomainStatusRequest`
@@ -1468,15 +1468,15 @@
             model = models.ModifySubdomainStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyVasAutoRenewStatus(self, request):
         """增值服务自动续费设置
 
         :param request: Request instance for ModifyVasAutoRenewStatus.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.ModifyVasAutoRenewStatusRequest`
@@ -1491,15 +1491,15 @@
             model = models.ModifyVasAutoRenewStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def PayOrderWithBalance(self, request):
         """DNSPod商品余额支付
 
         :param request: Request instance for PayOrderWithBalance.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.PayOrderWithBalanceRequest`
@@ -1514,15 +1514,15 @@
             model = models.PayOrderWithBalanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackRecordSnapshot(self, request):
         """重新回滚指定解析记录快照
 
         :param request: Request instance for RollbackRecordSnapshot.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.RollbackRecordSnapshotRequest`
@@ -1537,15 +1537,15 @@
             model = models.RollbackRecordSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RollbackSnapshot(self, request):
         """回滚快照
 
         :param request: Request instance for RollbackSnapshot.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.RollbackSnapshotRequest`
@@ -1560,8 +1560,8 @@
             model = models.RollbackSnapshotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.938/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.937/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.938/README.rst`

 * *Files identical despite different names*

