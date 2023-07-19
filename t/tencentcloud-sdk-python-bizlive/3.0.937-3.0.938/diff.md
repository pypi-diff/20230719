# Comparing `tmp/tencentcloud-sdk-python-bizlive-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-bizlive-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bizlive-3.0.937.tar", last modified: Tue Jul 18 00:17:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bizlive-3.0.938.tar", last modified: Wed Jul 19 00:21:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bizlive-3.0.937.tar` & `tencentcloud-sdk-python-bizlive-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/
--rw-r--r--   0 root         (0) root         (0)     6305 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/bizlive_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19225 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:52.000000 tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/bizlive_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19225 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:54.000000 tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/setup.py` & `tencentcloud-sdk-python-bizlive-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/bizlive_client.py` & `tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/bizlive_client.py`

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
 
 
     def DescribeStreamPlayInfoList(self, request):
         """查询播放数据，支持按流名称查询详细播放数据，也可按播放域名查询详细总数据。
 
         :param request: Request instance for DescribeStreamPlayInfoList.
         :type request: :class:`tencentcloud.bizlive.v20190313.models.DescribeStreamPlayInfoListRequest`
@@ -65,15 +65,15 @@
             model = models.DescribeStreamPlayInfoListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkers(self, request):
         """查询空闲机器数量
 
         :param request: Request instance for DescribeWorkers.
         :type request: :class:`tencentcloud.bizlive.v20190313.models.DescribeWorkersRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeWorkersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ForbidLiveStream(self, request):
         """禁止某条流的推送，可以预设某个时刻将流恢复。
 
         :param request: Request instance for ForbidLiveStream.
         :type request: :class:`tencentcloud.bizlive.v20190313.models.ForbidLiveStreamRequest`
@@ -111,15 +111,15 @@
             model = models.ForbidLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RegisterIM(self, request):
         """注册聊天室
 
         :param request: Request instance for RegisterIM.
         :type request: :class:`tencentcloud.bizlive.v20190313.models.RegisterIMRequest`
@@ -134,15 +134,15 @@
             model = models.RegisterIMResponse()
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
         :type request: :class:`tencentcloud.bizlive.v20190313.models.StopGameRequest`
@@ -157,8 +157,8 @@
             model = models.StopGameResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/errorcodes.py` & `tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud/bizlive/v20190313/models.py` & `tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud/bizlive/v20190313/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-bizlive-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bizlive
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bizlive SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/README.rst` & `tencentcloud-sdk-python-bizlive-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bizlive-3.0.937/tencentcloud_sdk_python_bizlive.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bizlive-3.0.938/tencentcloud_sdk_python_bizlive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bizlive
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Bizlive SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

