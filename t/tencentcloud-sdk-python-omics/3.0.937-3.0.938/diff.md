# Comparing `tmp/tencentcloud-sdk-python-omics-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-omics-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.937.tar", last modified: Tue Jul 18 00:28:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.938.tar", last modified: Wed Jul 19 00:43:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-omics-3.0.937.tar` & `tencentcloud-sdk-python-omics-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)     4079 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89148 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:28:28.000000 tencentcloud-sdk-python-omics-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)     4079 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89148 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:43:47.000000 tencentcloud-sdk-python-omics-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-omics-3.0.937/tencentcloud_sdk_python_omics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.938/tencentcloud_sdk_python_omics.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.937/setup.py` & `tencentcloud-sdk-python-omics-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-omics-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/omics_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteEnvironment(self, request):
         """删除环境。
 
         :param request: Request instance for DeleteEnvironment.
         :type request: :class:`tencentcloud.omics.v20221128.models.DeleteEnvironmentRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteEnvironmentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvironments(self, request):
         """查询环境列表。
 
         :param request: Request instance for DescribeEnvironments.
         :type request: :class:`tencentcloud.omics.v20221128.models.DescribeEnvironmentsRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeEnvironmentsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRunGroups(self, request):
         """查询任务批次列表。
 
         :param request: Request instance for DescribeRunGroups.
         :type request: :class:`tencentcloud.omics.v20221128.models.DescribeRunGroupsRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeRunGroupsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRuns(self, request):
         """查询任务列表。
 
         :param request: Request instance for DescribeRuns.
         :type request: :class:`tencentcloud.omics.v20221128.models.DescribeRunsRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeRunsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTables(self, request):
         """查询表格。
 
         :param request: Request instance for DescribeTables.
         :type request: :class:`tencentcloud.omics.v20221128.models.DescribeTablesRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeTablesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTablesRows(self, request):
         """查询表格行数据。
 
         :param request: Request instance for DescribeTablesRows.
         :type request: :class:`tencentcloud.omics.v20221128.models.DescribeTablesRowsRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeTablesRowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRunCalls(self, request):
         """查询作业详情。
 
         :param request: Request instance for GetRunCalls.
         :type request: :class:`tencentcloud.omics.v20221128.models.GetRunCallsRequest`
@@ -203,15 +203,15 @@
             model = models.GetRunCallsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetRunStatus(self, request):
         """查询任务详情。
 
         :param request: Request instance for GetRunStatus.
         :type request: :class:`tencentcloud.omics.v20221128.models.GetRunStatusRequest`
@@ -226,15 +226,15 @@
             model = models.GetRunStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImportTableFile(self, request):
         """导入表格文件。
 
         :param request: Request instance for ImportTableFile.
         :type request: :class:`tencentcloud.omics.v20221128.models.ImportTableFileRequest`
@@ -249,15 +249,15 @@
             model = models.ImportTableFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RetryRuns(self, request):
         """重试任务。
 
         :param request: Request instance for RetryRuns.
         :type request: :class:`tencentcloud.omics.v20221128.models.RetryRunsRequest`
@@ -272,15 +272,15 @@
             model = models.RetryRunsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunApplication(self, request):
         """运行应用。
 
         :param request: Request instance for RunApplication.
         :type request: :class:`tencentcloud.omics.v20221128.models.RunApplicationRequest`
@@ -295,8 +295,8 @@
             model = models.RunApplicationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.937/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-omics-3.0.938/tencentcloud/omics/v20221128/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.938/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.937/README.rst` & `tencentcloud-sdk-python-omics-3.0.938/README.rst`

 * *Files identical despite different names*

