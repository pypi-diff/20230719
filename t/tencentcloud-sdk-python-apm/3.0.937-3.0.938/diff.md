# Comparing `tmp/tencentcloud-sdk-python-apm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-apm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.937.tar", last modified: Tue Jul 18 00:17:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.938.tar", last modified: Wed Jul 19 00:21:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apm-3.0.937.tar` & `tencentcloud-sdk-python-apm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8295 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/apm_client.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    70014 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8327 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/apm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    70014 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:21:11.000000 tencentcloud-sdk-python-apm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-apm-3.0.937/setup.py` & `tencentcloud-sdk-python-apm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/apm_client.py` & `tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/apm_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateApmInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApmAgent(self, request):
         """获取Apm Agent信息
 
         :param request: Request instance for DescribeApmAgent.
         :type request: :class:`tencentcloud.apm.v20210622.models.DescribeApmAgentRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeApmAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeApmInstances(self, request):
         """APM实例列表拉取
 
         :param request: Request instance for DescribeApmInstances.
         :type request: :class:`tencentcloud.apm.v20210622.models.DescribeApmInstancesRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeApmInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGeneralMetricData(self, request):
         """获取指标数据通用接口。用户根据需要上送请求参数，返回对应的指标数据。
         接口调用频率限制为：20次/秒，1200次/分钟。单请求的数据点数限制为1440个。
 
         :param request: Request instance for DescribeGeneralMetricData.
@@ -112,15 +112,15 @@
             model = models.DescribeGeneralMetricDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMetricRecords(self, request):
         """拉取通用指标列表
 
         :param request: Request instance for DescribeMetricRecords.
         :type request: :class:`tencentcloud.apm.v20210622.models.DescribeMetricRecordsRequest`
@@ -135,15 +135,15 @@
             model = models.DescribeMetricRecordsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServiceOverview(self, request):
         """服务概览数据拉取
 
         :param request: Request instance for DescribeServiceOverview.
         :type request: :class:`tencentcloud.apm.v20210622.models.DescribeServiceOverviewRequest`
@@ -158,15 +158,15 @@
             model = models.DescribeServiceOverviewResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyApmInstance(self, request):
         """修改Apm实例接口
 
         :param request: Request instance for ModifyApmInstance.
         :type request: :class:`tencentcloud.apm.v20210622.models.ModifyApmInstanceRequest`
@@ -181,15 +181,15 @@
             model = models.ModifyApmInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TerminateApmInstance(self, request):
         """apm销毁实例
 
         :param request: Request instance for TerminateApmInstance.
         :type request: :class:`tencentcloud.apm.v20210622.models.TerminateApmInstanceRequest`
@@ -204,8 +204,8 @@
             model = models.TerminateApmInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/errorcodes.py` & `tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/models.py` & `tencentcloud-sdk-python-apm-3.0.938/tencentcloud/apm/v20210622/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.938/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.938/tencentcloud_sdk_python_apm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.937/README.rst` & `tencentcloud-sdk-python-apm-3.0.938/README.rst`

 * *Files identical despite different names*

