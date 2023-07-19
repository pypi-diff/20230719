# Comparing `tmp/tencentcloud-sdk-python-tiems-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tiems-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiems-3.0.937.tar", last modified: Tue Jul 18 00:33:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiems-3.0.938.tar", last modified: Wed Jul 19 00:50:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiems-3.0.937.tar` & `tencentcloud-sdk-python-tiems-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28134 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/tiems_client.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   151851 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:33:06.000000 tencentcloud-sdk-python-tiems-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28234 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/tiems_client.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   151851 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:50:45.000000 tencentcloud-sdk-python-tiems-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/setup.py` & `tencentcloud-sdk-python-tiems-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/tencentcloud_sdk_python_tiems.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiems-3.0.938/tencentcloud_sdk_python_tiems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiems
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiems SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/tiems_client.py` & `tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/tiems_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             model = models.CreateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRsgAsGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         创建资源组的伸缩组。当前一个资源组仅允许创建一个伸缩组。
 
@@ -69,15 +69,15 @@
             model = models.CreateRsgAsGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRuntime(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         创建运行环境
 
@@ -94,15 +94,15 @@
             model = models.CreateRuntimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateService(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         创建服务
 
@@ -119,15 +119,15 @@
             model = models.CreateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateServiceConfig(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         创建服务配置
 
@@ -144,15 +144,15 @@
             model = models.CreateServiceConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteInstance(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除资源组中的节点。目前仅支持删除已经到期的预付费节点，和按量付费节点。
 
@@ -169,15 +169,15 @@
             model = models.DeleteInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteJob(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除任务
 
@@ -194,15 +194,15 @@
             model = models.DeleteJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteResourceGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除资源组
 
@@ -219,15 +219,15 @@
             model = models.DeleteResourceGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRsgAsGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         伸缩
 
@@ -244,15 +244,15 @@
             model = models.DeleteRsgAsGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteRuntime(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除运行环境
 
@@ -269,15 +269,15 @@
             model = models.DeleteRuntimeResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteService(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除服务
 
@@ -294,15 +294,15 @@
             model = models.DeleteServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteServiceConfig(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         删除服务配置
 
@@ -319,15 +319,15 @@
             model = models.DeleteServiceConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         获取节点列表
 
@@ -344,15 +344,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeResourceGroups(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         获取资源组列表
 
@@ -369,15 +369,15 @@
             model = models.DescribeResourceGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRsgAsGroupActivities(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         查询伸缩组活动
 
@@ -394,15 +394,15 @@
             model = models.DescribeRsgAsGroupActivitiesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRsgAsGroups(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         查询资源组的伸缩组信息
 
@@ -419,15 +419,15 @@
             model = models.DescribeRsgAsGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuntimes(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         描述服务运行环境
 
@@ -444,15 +444,15 @@
             model = models.DescribeRuntimesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceConfigs(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         描述服务配置
 
@@ -469,15 +469,15 @@
             model = models.DescribeServiceConfigsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServices(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         描述服务
 
@@ -494,15 +494,15 @@
             model = models.DescribeServicesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableRsgAsGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         停用资源组的伸缩组
 
@@ -519,15 +519,15 @@
             model = models.DisableRsgAsGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableRsgAsGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         启用资源组的伸缩组
 
@@ -544,15 +544,15 @@
             model = models.EnableRsgAsGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExposeService(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         暴露服务
 
@@ -569,15 +569,15 @@
             model = models.ExposeServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateJob(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         更新任务
 
@@ -594,15 +594,15 @@
             model = models.UpdateJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateRsgAsGroup(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         更新资源组的伸缩组
 
@@ -619,15 +619,15 @@
             model = models.UpdateRsgAsGroupResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateService(self, request):
         """因业务策略调整，腾讯云TI平台TI-EMS已经于2022年6月30日下线并停止提供服务。若您有新增的业务需求，可前往TI-ONE(https://cloud.tencent.com/document/product/851)使用。
 
         更新服务
 
@@ -644,8 +644,8 @@
             model = models.UpdateServiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/errorcodes.py` & `tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/tiems/v20190416/models.py` & `tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/tiems/v20190416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiems-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tiems-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiems
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tiems SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiems-3.0.937/README.rst` & `tencentcloud-sdk-python-tiems-3.0.938/README.rst`

 * *Files identical despite different names*

