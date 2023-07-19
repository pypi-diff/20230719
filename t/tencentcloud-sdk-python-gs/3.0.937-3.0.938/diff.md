# Comparing `tmp/tencentcloud-sdk-python-gs-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-gs-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gs-3.0.937.tar", last modified: Tue Jul 18 00:24:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gs-3.0.938.tar", last modified: Wed Jul 19 00:39:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gs-3.0.937.tar` & `tencentcloud-sdk-python-gs-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/
--rw-r--r--   0 root         (0) root         (0)     7825 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/gs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25245 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:36.000000 tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/
+-rw-r--r--   0 root         (0) root         (0)     7857 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/gs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25245 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:55.000000 tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-gs-3.0.937/setup.py` & `tencentcloud-sdk-python-gs-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gs-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/gs_client.py` & `tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/gs_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateSessionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeInstancesCount(self, request):
         """获取并发总数和运行数
 
         :param request: Request instance for DescribeInstancesCount.
         :type request: :class:`tencentcloud.gs.v20191118.models.DescribeInstancesCountRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeInstancesCountResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SaveGameArchive(self, request):
         """保存游戏存档
 
         :param request: Request instance for SaveGameArchive.
         :type request: :class:`tencentcloud.gs.v20191118.models.SaveGameArchiveRequest`
@@ -88,15 +88,15 @@
             model = models.SaveGameArchiveResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartPublishStream(self, request):
         """开始云端推流
 
         :param request: Request instance for StartPublishStream.
         :type request: :class:`tencentcloud.gs.v20191118.models.StartPublishStreamRequest`
@@ -111,15 +111,15 @@
             model = models.StartPublishStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopGame(self, request):
         """强制退出游戏
 
         :param request: Request instance for StopGame.
         :type request: :class:`tencentcloud.gs.v20191118.models.StopGameRequest`
@@ -134,15 +134,15 @@
             model = models.StopGameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopPublishStream(self, request):
         """停止云端推流
 
         :param request: Request instance for StopPublishStream.
         :type request: :class:`tencentcloud.gs.v20191118.models.StopPublishStreamRequest`
@@ -157,15 +157,15 @@
             model = models.StopPublishStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwitchGameArchive(self, request):
         """切换游戏存档
 
         :param request: Request instance for SwitchGameArchive.
         :type request: :class:`tencentcloud.gs.v20191118.models.SwitchGameArchiveRequest`
@@ -180,15 +180,15 @@
             model = models.SwitchGameArchiveResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TrylockWorker(self, request):
         """尝试锁定机器
 
         :param request: Request instance for TrylockWorker.
         :type request: :class:`tencentcloud.gs.v20191118.models.TrylockWorkerRequest`
@@ -203,8 +203,8 @@
             model = models.TrylockWorkerResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/errorcodes.py` & `tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.937/tencentcloud/gs/v20191118/models.py` & `tencentcloud-sdk-python-gs-3.0.938/tencentcloud/gs/v20191118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-gs-3.0.938/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gs-3.0.937/README.rst` & `tencentcloud-sdk-python-gs-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.937/tencentcloud_sdk_python_gs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gs-3.0.938/tencentcloud_sdk_python_gs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Gs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

