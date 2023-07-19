# Comparing `tmp/tencentcloud-sdk-python-tcm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcm-3.0.937.tar", last modified: Tue Jul 18 00:31:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcm-3.0.938.tar", last modified: Wed Jul 19 00:49:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcm-3.0.937.tar` & `tencentcloud-sdk-python-tcm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/
--rw-r--r--   0 root         (0) root         (0)    11214 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/tcm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   129713 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:45.000000 tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/
+-rw-r--r--   0 root         (0) root         (0)    11262 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/tcm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   129713 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:49:11.000000 tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/setup.py` & `tencentcloud-sdk-python-tcm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/tcm_client.py` & `tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/tcm_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateMeshResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteMesh(self, request):
         """删除网格
 
         :param request: Request instance for DeleteMesh.
         :type request: :class:`tencentcloud.tcm.v20210413.models.DeleteMeshRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteMeshResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAccessLogConfig(self, request):
         """获取AccessLog配置
 
         :param request: Request instance for DescribeAccessLogConfig.
         :type request: :class:`tencentcloud.tcm.v20210413.models.DescribeAccessLogConfigRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeAccessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMesh(self, request):
         """查询网格详情
 
         :param request: Request instance for DescribeMesh.
         :type request: :class:`tencentcloud.tcm.v20210413.models.DescribeMeshRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeMeshResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMeshList(self, request):
         """查询网格列表
 
         :param request: Request instance for DescribeMeshList.
         :type request: :class:`tencentcloud.tcm.v20210413.models.DescribeMeshListRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeMeshListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LinkClusterList(self, request):
         """关联集群
 
         :param request: Request instance for LinkClusterList.
         :type request: :class:`tencentcloud.tcm.v20210413.models.LinkClusterListRequest`
@@ -157,15 +157,15 @@
             model = models.LinkClusterListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LinkPrometheus(self, request):
         """关联Prometheus
 
         :param request: Request instance for LinkPrometheus.
         :type request: :class:`tencentcloud.tcm.v20210413.models.LinkPrometheusRequest`
@@ -180,15 +180,15 @@
             model = models.LinkPrometheusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAccessLogConfig(self, request):
         """修改访问日志配置
 
         :param request: Request instance for ModifyAccessLogConfig.
         :type request: :class:`tencentcloud.tcm.v20210413.models.ModifyAccessLogConfigRequest`
@@ -203,15 +203,15 @@
             model = models.ModifyAccessLogConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyMesh(self, request):
         """修改网格
 
         :param request: Request instance for ModifyMesh.
         :type request: :class:`tencentcloud.tcm.v20210413.models.ModifyMeshRequest`
@@ -226,15 +226,15 @@
             model = models.ModifyMeshResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTracingConfig(self, request):
         """修改 Tracing 配置
 
         :param request: Request instance for ModifyTracingConfig.
         :type request: :class:`tencentcloud.tcm.v20210413.models.ModifyTracingConfigRequest`
@@ -249,15 +249,15 @@
             model = models.ModifyTracingConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlinkCluster(self, request):
         """解关联集群
 
         :param request: Request instance for UnlinkCluster.
         :type request: :class:`tencentcloud.tcm.v20210413.models.UnlinkClusterRequest`
@@ -272,15 +272,15 @@
             model = models.UnlinkClusterResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UnlinkPrometheus(self, request):
         """解除关联Prometheus
 
         :param request: Request instance for UnlinkPrometheus.
         :type request: :class:`tencentcloud.tcm.v20210413.models.UnlinkPrometheusRequest`
@@ -295,8 +295,8 @@
             model = models.UnlinkPrometheusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/errorcodes.py` & `tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/tencentcloud/tcm/v20210413/models.py` & `tencentcloud-sdk-python-tcm-3.0.938/tencentcloud/tcm/v20210413/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcm-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/README.rst` & `tencentcloud-sdk-python-tcm-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcm-3.0.937/tencentcloud_sdk_python_tcm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcm-3.0.938/tencentcloud_sdk_python_tcm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

