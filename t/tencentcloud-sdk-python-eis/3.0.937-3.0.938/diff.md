# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.937.tar", last modified: Tue Jul 18 00:23:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.938.tar", last modified: Wed Jul 19 00:38:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.937.tar` & `tencentcloud-sdk-python-eis-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5846 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39966 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:33.000000 tencentcloud-sdk-python-eis-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39966 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:47.000000 tencentcloud-sdk-python-eis-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.937/setup.py` & `tencentcloud-sdk-python-eis-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/eis_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.GetRuntimeMCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRuntimeResourceMonitorMetricMC(self, request):
         """获取运行时资源监控详情，cpu，memory，bandwidth
 
         :param request: Request instance for GetRuntimeResourceMonitorMetricMC.
         :type request: :class:`tencentcloud.eis.v20210601.models.GetRuntimeResourceMonitorMetricMCRequest`
@@ -65,15 +65,15 @@
             model = models.GetRuntimeResourceMonitorMetricMCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListDeployableRuntimesMC(self, request):
         """返回用户可用的运行时列表，发布应用时返回的运行时环境，仅shared和private运行时，无sandbox运行时，并且只有running/scaling状态的
 
         :param request: Request instance for ListDeployableRuntimesMC.
         :type request: :class:`tencentcloud.eis.v20210601.models.ListDeployableRuntimesMCRequest`
@@ -88,15 +88,15 @@
             model = models.ListDeployableRuntimesMCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListRuntimeDeployedInstancesMC(self, request):
         """获取运行时部署的应用实例列表
 
         :param request: Request instance for ListRuntimeDeployedInstancesMC.
         :type request: :class:`tencentcloud.eis.v20210601.models.ListRuntimeDeployedInstancesMCRequest`
@@ -111,15 +111,15 @@
             model = models.ListRuntimeDeployedInstancesMCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListRuntimesMC(self, request):
         """返回用户的运行时列表，运行时管理主页使用，包含沙箱、共享运行时及独立运行时环境，不包含已经删除的运行时
 
         :param request: Request instance for ListRuntimesMC.
         :type request: :class:`tencentcloud.eis.v20210601.models.ListRuntimesMCRequest`
@@ -134,8 +134,8 @@
             model = models.ListRuntimesMCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20210601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/eis_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeEisConnectorConfigResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEisConnectorOperations(self, request):
         """获取连接器操作列表
 
         :param request: Request instance for ListEisConnectorOperations.
         :type request: :class:`tencentcloud.eis.v20200715.models.ListEisConnectorOperationsRequest`
@@ -65,15 +65,15 @@
             model = models.ListEisConnectorOperationsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ListEisConnectors(self, request):
         """连接器列表
 
         :param request: Request instance for ListEisConnectors.
         :type request: :class:`tencentcloud.eis.v20200715.models.ListEisConnectorsRequest`
@@ -88,8 +88,8 @@
             model = models.ListEisConnectorsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eis-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.937/README.rst` & `tencentcloud-sdk-python-eis-3.0.938/README.rst`

 * *Files identical despite different names*

