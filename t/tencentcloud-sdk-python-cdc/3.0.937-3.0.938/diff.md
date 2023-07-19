# Comparing `tmp/tencentcloud-sdk-python-cdc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cdc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdc-3.0.937.tar", last modified: Tue Jul 18 00:19:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdc-3.0.938.tar", last modified: Wed Jul 19 00:23:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdc-3.0.937.tar` & `tencentcloud-sdk-python-cdc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19359 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/cdc_client.py
--rw-r--r--   0 root         (0) root         (0)   138667 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:22.000000 tencentcloud-sdk-python-cdc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:19:21.000000 tencentcloud-sdk-python-cdc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19439 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/cdc_client.py
+-rw-r--r--   0 root         (0) root         (0)   138667 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:23:29.000000 tencentcloud-sdk-python-cdc-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/setup.py` & `tencentcloud-sdk-python-cdc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/errorcodes.py` & `tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/cdc_client.py` & `tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/cdc_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateDedicatedClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateDedicatedClusterOrder(self, request):
         """创建专用集群订单
 
         :param request: Request instance for CreateDedicatedClusterOrder.
         :type request: :class:`tencentcloud.cdc.v20201214.models.CreateDedicatedClusterOrderRequest`
@@ -65,15 +65,15 @@
             model = models.CreateDedicatedClusterOrderResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSite(self, request):
         """创建站点
 
         :param request: Request instance for CreateSite.
         :type request: :class:`tencentcloud.cdc.v20201214.models.CreateSiteRequest`
@@ -88,15 +88,15 @@
             model = models.CreateSiteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteDedicatedClusters(self, request):
         """删除专用集群
 
         :param request: Request instance for DeleteDedicatedClusters.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DeleteDedicatedClustersRequest`
@@ -111,15 +111,15 @@
             model = models.DeleteDedicatedClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSites(self, request):
         """删除站点
 
         :param request: Request instance for DeleteSites.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DeleteSitesRequest`
@@ -134,15 +134,15 @@
             model = models.DeleteSitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterCosCapacity(self, request):
         """查询专用集群内cos的容量信息
 
         :param request: Request instance for DescribeDedicatedClusterCosCapacity.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterCosCapacityRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeDedicatedClusterCosCapacityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterHostStatistics(self, request):
         """查询专用集群内宿主机的统计信息
 
         :param request: Request instance for DescribeDedicatedClusterHostStatistics.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterHostStatisticsRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeDedicatedClusterHostStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterHosts(self, request):
         """专用集群宿主机信息
 
         :param request: Request instance for DescribeDedicatedClusterHosts.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterHostsRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeDedicatedClusterHostsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterInstanceTypes(self, request):
         """查询专用集群支持的实例规格列表
 
         :param request: Request instance for DescribeDedicatedClusterInstanceTypes.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterInstanceTypesRequest`
@@ -226,15 +226,15 @@
             model = models.DescribeDedicatedClusterInstanceTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterOrders(self, request):
         """查询专用集群订单列表
 
         :param request: Request instance for DescribeDedicatedClusterOrders.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterOrdersRequest`
@@ -249,15 +249,15 @@
             model = models.DescribeDedicatedClusterOrdersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterOverview(self, request):
         """专用集群概览信息
 
         :param request: Request instance for DescribeDedicatedClusterOverview.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterOverviewRequest`
@@ -272,15 +272,15 @@
             model = models.DescribeDedicatedClusterOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusterTypes(self, request):
         """查询专有集群配置列表
 
         :param request: Request instance for DescribeDedicatedClusterTypes.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClusterTypesRequest`
@@ -295,15 +295,15 @@
             model = models.DescribeDedicatedClusterTypesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedClusters(self, request):
         """查询专用集群列表
 
         :param request: Request instance for DescribeDedicatedClusters.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedClustersRequest`
@@ -318,15 +318,15 @@
             model = models.DescribeDedicatedClustersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDedicatedSupportedZones(self, request):
         """查询专用集群支持的可用区列表
 
         :param request: Request instance for DescribeDedicatedSupportedZones.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeDedicatedSupportedZonesRequest`
@@ -341,15 +341,15 @@
             model = models.DescribeDedicatedSupportedZonesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSites(self, request):
         """查询站点列表
 
         :param request: Request instance for DescribeSites.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeSitesRequest`
@@ -364,15 +364,15 @@
             model = models.DescribeSitesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSitesDetail(self, request):
         """查询站点详情
 
         :param request: Request instance for DescribeSitesDetail.
         :type request: :class:`tencentcloud.cdc.v20201214.models.DescribeSitesDetailRequest`
@@ -387,15 +387,15 @@
             model = models.DescribeSitesDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyDedicatedClusterInfo(self, request):
         """修改本地专用集群信息
 
         :param request: Request instance for ModifyDedicatedClusterInfo.
         :type request: :class:`tencentcloud.cdc.v20201214.models.ModifyDedicatedClusterInfoRequest`
@@ -410,15 +410,15 @@
             model = models.ModifyDedicatedClusterInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyOrderStatus(self, request):
         """修改大订单、小订单的状态
 
         :param request: Request instance for ModifyOrderStatus.
         :type request: :class:`tencentcloud.cdc.v20201214.models.ModifyOrderStatusRequest`
@@ -433,15 +433,15 @@
             model = models.ModifyOrderStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySiteDeviceInfo(self, request):
         """修改机房设备信息
 
         :param request: Request instance for ModifySiteDeviceInfo.
         :type request: :class:`tencentcloud.cdc.v20201214.models.ModifySiteDeviceInfoRequest`
@@ -456,15 +456,15 @@
             model = models.ModifySiteDeviceInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySiteInfo(self, request):
         """修改机房信息
 
         :param request: Request instance for ModifySiteInfo.
         :type request: :class:`tencentcloud.cdc.v20201214.models.ModifySiteInfoRequest`
@@ -479,8 +479,8 @@
             model = models.ModifySiteInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/tencentcloud/cdc/v20201214/models.py` & `tencentcloud-sdk-python-cdc-3.0.938/tencentcloud/cdc/v20201214/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdc-3.0.938/tencentcloud_sdk_python_cdc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cdc-3.0.938/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdc-3.0.937/README.rst` & `tencentcloud-sdk-python-cdc-3.0.938/README.rst`

 * *Files identical despite different names*

