# Comparing `tmp/tencentcloud-sdk-python-tav-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tav-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tav-3.0.937.tar", last modified: Tue Jul 18 00:30:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tav-3.0.938.tar", last modified: Wed Jul 19 00:48:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tav-3.0.937.tar` & `tencentcloud-sdk-python-tav-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4379 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/tav_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    12546 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:30:58.000000 tencentcloud-sdk-python-tav-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4395 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/tav_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:23.000000 tencentcloud-sdk-python-tav-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tav-3.0.937/setup.py` & `tencentcloud-sdk-python-tav-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.937/tencentcloud_sdk_python_tav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tav-3.0.938/tencentcloud_sdk_python_tav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tav
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tav-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tav-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/tav_client.py` & `tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/tav_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.GetLocalEngineResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetScanResult(self, request):
         """tav文件上传扫描结果查询
 
         :param request: Request instance for GetScanResult.
         :type request: :class:`tencentcloud.tav.v20190118.models.GetScanResultRequest`
@@ -65,15 +65,15 @@
             model = models.GetScanResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanFile(self, request):
         """tav文件上传扫描
 
         :param request: Request instance for ScanFile.
         :type request: :class:`tencentcloud.tav.v20190118.models.ScanFileRequest`
@@ -88,15 +88,15 @@
             model = models.ScanFileResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ScanFileHash(self, request):
         """通过文件哈希值获取文件黑白属性
 
         :param request: Request instance for ScanFileHash.
         :type request: :class:`tencentcloud.tav.v20190118.models.ScanFileHashRequest`
@@ -111,8 +111,8 @@
             model = models.ScanFileHashResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/errorcodes.py` & `tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.937/tencentcloud/tav/v20190118/models.py` & `tencentcloud-sdk-python-tav-3.0.938/tencentcloud/tav/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tav-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tav
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tav-3.0.937/README.rst` & `tencentcloud-sdk-python-tav-3.0.938/README.rst`

 * *Files identical despite different names*

