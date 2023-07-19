# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.937.tar", last modified: Tue Jul 18 00:23:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.938.tar", last modified: Wed Jul 19 00:38:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.937.tar` & `tencentcloud-sdk-python-emr-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30020 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    14329 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   455464 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:37.000000 tencentcloud-sdk-python-emr-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30148 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    14329 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455464 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:51.000000 tencentcloud-sdk-python-emr-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-emr-3.0.937/setup.py` & `tencentcloud-sdk-python-emr-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/emr_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.AddUsersForUserManagerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCluster(self, request):
         """创建EMR集群实例
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.emr.v20190103.models.CreateClusterRequest`
@@ -66,15 +66,15 @@
             model = models.CreateClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstance(self, request):
         """创建EMR集群实例
 
         :param request: Request instance for CreateInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.CreateInstanceRequest`
@@ -89,15 +89,15 @@
             model = models.CreateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteUserManagerUserList(self, request):
         """删除用户列表（用户管理）
 
         :param request: Request instance for DeleteUserManagerUserList.
         :type request: :class:`tencentcloud.emr.v20190103.models.DeleteUserManagerUserListRequest`
@@ -112,15 +112,15 @@
             model = models.DeleteUserManagerUserListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeClusterNodes(self, request):
         """查询集群节点信息
 
         :param request: Request instance for DescribeClusterNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeClusterNodesRequest`
@@ -135,15 +135,15 @@
             model = models.DescribeClusterNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCvmQuota(self, request):
         """获取账户的CVM配额
 
         :param request: Request instance for DescribeCvmQuota.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeCvmQuotaRequest`
@@ -158,15 +158,15 @@
             model = models.DescribeCvmQuotaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEmrApplicationStatics(self, request):
         """yarn application 统计接口查询
 
         :param request: Request instance for DescribeEmrApplicationStatics.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeEmrApplicationStaticsRequest`
@@ -181,15 +181,15 @@
             model = models.DescribeEmrApplicationStaticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHiveQueries(self, request):
         """获取hive查询信息
 
         :param request: Request instance for DescribeHiveQueries.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeHiveQueriesRequest`
@@ -204,15 +204,15 @@
             model = models.DescribeHiveQueriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImpalaQueries(self, request):
         """DescribeImpalaQueries
 
         :param request: Request instance for DescribeImpalaQueries.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeImpalaQueriesRequest`
@@ -227,15 +227,15 @@
             model = models.DescribeImpalaQueriesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceRenewNodes(self, request):
         """查询待续费节点信息
 
         :param request: Request instance for DescribeInstanceRenewNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeInstanceRenewNodesRequest`
@@ -250,15 +250,15 @@
             model = models.DescribeInstanceRenewNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """查询集群实例信息
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeInstancesRequest`
@@ -273,15 +273,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesList(self, request):
         """查询集群列表
 
         :param request: Request instance for DescribeInstancesList.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeInstancesListRequest`
@@ -296,15 +296,15 @@
             model = models.DescribeInstancesListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeJobFlow(self, request):
         """查询流程任务
 
         :param request: Request instance for DescribeJobFlow.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeJobFlowRequest`
@@ -319,15 +319,15 @@
             model = models.DescribeJobFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceSchedule(self, request):
         """查询YARN资源调度数据信息
 
         :param request: Request instance for DescribeResourceSchedule.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeResourceScheduleRequest`
@@ -342,15 +342,15 @@
             model = models.DescribeResourceScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsersForUserManager(self, request):
         """该接口支持安装了OpenLdap组件的集群。
         批量导出用户。对于kerberos集群，如果需要kertab文件下载地址，可以将NeedKeytabInfo设置为true；注意SupportDownLoadKeyTab为true，但是DownLoadKeyTabUrl为空字符串，表示keytab文件在后台没有准备好（正在生成）。
 
         :param request: Request instance for DescribeUsersForUserManager.
@@ -366,15 +366,15 @@
             model = models.DescribeUsersForUserManagerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeYarnApplications(self, request):
         """DescribeYarnApplications
 
         :param request: Request instance for DescribeYarnApplications.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeYarnApplicationsRequest`
@@ -389,15 +389,15 @@
             model = models.DescribeYarnApplicationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquirePriceRenewEmr(self, request):
         """集群续费询价。
 
         :param request: Request instance for InquirePriceRenewEmr.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquirePriceRenewEmrRequest`
@@ -412,15 +412,15 @@
             model = models.InquirePriceRenewEmrResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceCreateInstance(self, request):
         """创建实例询价
 
         :param request: Request instance for InquiryPriceCreateInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquiryPriceCreateInstanceRequest`
@@ -435,15 +435,15 @@
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
         """续费询价。
 
         :param request: Request instance for InquiryPriceRenewInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquiryPriceRenewInstanceRequest`
@@ -458,15 +458,15 @@
             model = models.InquiryPriceRenewInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceScaleOutInstance(self, request):
         """扩容询价. 当扩容时候，请通过该接口查询价格。
 
         :param request: Request instance for InquiryPriceScaleOutInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquiryPriceScaleOutInstanceRequest`
@@ -481,15 +481,15 @@
             model = models.InquiryPriceScaleOutInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def InquiryPriceUpdateInstance(self, request):
         """变配询价
 
         :param request: Request instance for InquiryPriceUpdateInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.InquiryPriceUpdateInstanceRequest`
@@ -504,15 +504,15 @@
             model = models.InquiryPriceUpdateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourcePools(self, request):
         """刷新YARN的动态资源池
 
         :param request: Request instance for ModifyResourcePools.
         :type request: :class:`tencentcloud.emr.v20190103.models.ModifyResourcePoolsRequest`
@@ -527,15 +527,15 @@
             model = models.ModifyResourcePoolsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourceScheduleConfig(self, request):
         """修改YARN资源调度的资源配置
 
         :param request: Request instance for ModifyResourceScheduleConfig.
         :type request: :class:`tencentcloud.emr.v20190103.models.ModifyResourceScheduleConfigRequest`
@@ -550,15 +550,15 @@
             model = models.ModifyResourceScheduleConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyResourceScheduler(self, request):
         """修改了yarn的资源调度器，点击部署生效
 
         :param request: Request instance for ModifyResourceScheduler.
         :type request: :class:`tencentcloud.emr.v20190103.models.ModifyResourceSchedulerRequest`
@@ -573,15 +573,15 @@
             model = models.ModifyResourceSchedulerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunJobFlow(self, request):
         """创建流程作业
 
         :param request: Request instance for RunJobFlow.
         :type request: :class:`tencentcloud.emr.v20190103.models.RunJobFlowRequest`
@@ -596,15 +596,15 @@
             model = models.RunJobFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleOutCluster(self, request):
         """扩容集群节点
 
         :param request: Request instance for ScaleOutCluster.
         :type request: :class:`tencentcloud.emr.v20190103.models.ScaleOutClusterRequest`
@@ -619,15 +619,15 @@
             model = models.ScaleOutClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScaleOutInstance(self, request):
         """扩容节点
 
         :param request: Request instance for ScaleOutInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.ScaleOutInstanceRequest`
@@ -642,15 +642,15 @@
             model = models.ScaleOutInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartStopServiceOrMonitor(self, request):
         """用于启停服务 重启服务等功能
 
         :param request: Request instance for StartStopServiceOrMonitor.
         :type request: :class:`tencentcloud.emr.v20190103.models.StartStopServiceOrMonitorRequest`
@@ -665,15 +665,15 @@
             model = models.StartStopServiceOrMonitorResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SyncPodState(self, request):
         """EMR同步TKE中POD状态
 
         :param request: Request instance for SyncPodState.
         :type request: :class:`tencentcloud.emr.v20190103.models.SyncPodStateRequest`
@@ -688,15 +688,15 @@
             model = models.SyncPodStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateClusterNodes(self, request):
         """销毁集群节点
 
         :param request: Request instance for TerminateClusterNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.TerminateClusterNodesRequest`
@@ -711,15 +711,15 @@
             model = models.TerminateClusterNodesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateInstance(self, request):
         """销毁EMR实例。此接口仅支持弹性MapReduce正式计费版本。
 
         :param request: Request instance for TerminateInstance.
         :type request: :class:`tencentcloud.emr.v20190103.models.TerminateInstanceRequest`
@@ -734,15 +734,15 @@
             model = models.TerminateInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateTasks(self, request):
         """缩容Task节点
 
         :param request: Request instance for TerminateTasks.
         :type request: :class:`tencentcloud.emr.v20190103.models.TerminateTasksRequest`
@@ -757,8 +757,8 @@
             model = models.TerminateTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.937/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.938/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.937/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.938/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.938/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.937/README.rst` & `tencentcloud-sdk-python-emr-3.0.938/README.rst`

 * *Files identical despite different names*

