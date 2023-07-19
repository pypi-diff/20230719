# Comparing `tmp/tencentcloud-sdk-python-tcbr-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tcbr-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcbr-3.0.937.tar", last modified: Tue Jul 18 00:31:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcbr-3.0.938.tar", last modified: Wed Jul 19 00:48:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcbr-3.0.937.tar` & `tencentcloud-sdk-python-tcbr-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/
--rw-r--r--   0 root         (0) root         (0)    10034 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/tcbr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88962 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:31:28.000000 tencentcloud-sdk-python-tcbr-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/tcbr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    88962 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:48:53.000000 tencentcloud-sdk-python-tcbr-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/setup.py` & `tencentcloud-sdk-python-tcbr-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/tcbr_client.py` & `tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/tcbr_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateCloudRunEnvResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCloudRunServer(self, request):
         """创建云托管服务接口
 
         :param request: Request instance for CreateCloudRunServer.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.CreateCloudRunServerRequest`
@@ -65,15 +65,15 @@
             model = models.CreateCloudRunServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudRunEnvs(self, request):
         """获取环境列表，含环境下的各个资源信息。尤其是各资源的唯一标识，是请求各资源的关键参数
 
         :param request: Request instance for DescribeCloudRunEnvs.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.DescribeCloudRunEnvsRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeCloudRunEnvsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudRunServerDetail(self, request):
         """查询云托管服务详情
 
         :param request: Request instance for DescribeCloudRunServerDetail.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.DescribeCloudRunServerDetailRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeCloudRunServerDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCloudRunServers(self, request):
         """查询云托管服务列表接口
 
         :param request: Request instance for DescribeCloudRunServers.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.DescribeCloudRunServersRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeCloudRunServersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEnvBaseInfo(self, request):
         """查询环境基础信息
 
         :param request: Request instance for DescribeEnvBaseInfo.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.DescribeEnvBaseInfoRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeEnvBaseInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeServerManageTask(self, request):
         """查询服务管理任务信息
 
         :param request: Request instance for DescribeServerManageTask.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.DescribeServerManageTaskRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeServerManageTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def OperateServerManage(self, request):
         """操作发布单
 
         :param request: Request instance for OperateServerManage.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.OperateServerManageRequest`
@@ -203,15 +203,15 @@
             model = models.OperateServerManageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseGray(self, request):
         """灰度发布
 
         :param request: Request instance for ReleaseGray.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.ReleaseGrayRequest`
@@ -226,15 +226,15 @@
             model = models.ReleaseGrayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateCloudRunServer(self, request):
         """更新云托管服务
 
         :param request: Request instance for UpdateCloudRunServer.
         :type request: :class:`tencentcloud.tcbr.v20220217.models.UpdateCloudRunServerRequest`
@@ -249,8 +249,8 @@
             model = models.UpdateCloudRunServerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/errorcodes.py` & `tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud/tcbr/v20220217/models.py` & `tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud/tcbr/v20220217/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/tencentcloud_sdk_python_tcbr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcbr-3.0.938/tencentcloud_sdk_python_tcbr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcbr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcbr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tcbr-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcbr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tcbr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcbr-3.0.937/README.rst` & `tencentcloud-sdk-python-tcbr-3.0.938/README.rst`

 * *Files identical despite different names*

