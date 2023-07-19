# Comparing `tmp/tencentcloud-sdk-python-dbdc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-dbdc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbdc-3.0.937.tar", last modified: Tue Jul 18 00:22:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbdc-3.0.938.tar", last modified: Wed Jul 19 00:37:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbdc-3.0.937.tar` & `tencentcloud-sdk-python-dbdc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/dbdc_client.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    72272 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:14.000000 tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6439 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/dbdc_client.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72272 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:37:30.000000 tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/setup.py` & `tencentcloud-sdk-python-dbdc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/dbdc_client.py` & `tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/dbdc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeDBInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHostList(self, request):
         """本接口用于查询主机列表
 
         :param request: Request instance for DescribeHostList.
         :type request: :class:`tencentcloud.dbdc.v20201029.models.DescribeHostListRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeHostListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceDetail(self, request):
         """本接口用于查询独享集群详情
 
         :param request: Request instance for DescribeInstanceDetail.
         :type request: :class:`tencentcloud.dbdc.v20201029.models.DescribeInstanceDetailRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeInstanceDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstanceList(self, request):
         """本接口用于查询独享集群实例列表
 
         :param request: Request instance for DescribeInstanceList.
         :type request: :class:`tencentcloud.dbdc.v20201029.models.DescribeInstanceListRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeInstanceListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstances(self, request):
         """根据不同地域不同用户，获取集群列表信息
 
         :param request: Request instance for DescribeInstances.
         :type request: :class:`tencentcloud.dbdc.v20201029.models.DescribeInstancesRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeInstancesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyInstanceName(self, request):
         """本接口用于修改集群名称
 
         :param request: Request instance for ModifyInstanceName.
         :type request: :class:`tencentcloud.dbdc.v20201029.models.ModifyInstanceNameRequest`
@@ -157,8 +157,8 @@
             model = models.ModifyInstanceNameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/errorcodes.py` & `tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud/dbdc/v20201029/models.py` & `tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud/dbdc/v20201029/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-dbdc-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbdc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dbdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/README.rst` & `tencentcloud-sdk-python-dbdc-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.937/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbdc-3.0.938/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbdc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Dbdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

