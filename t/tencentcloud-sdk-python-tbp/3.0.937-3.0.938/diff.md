# Comparing `tmp/tencentcloud-sdk-python-tbp-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tbp-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.937.tar", last modified: Tue Jul 18 00:31:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.938.tar", last modified: Wed Jul 19 00:48:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbp-3.0.937.tar` & `tencentcloud-sdk-python-tbp-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/
--rw-r--r--   0 root         (0) root         (0)     4420 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26651 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/
--rw-r--r--   0 root         (0) root         (0)     2682 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20731 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:31:13.000000 tencentcloud-sdk-python-tbp-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26651 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20731 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:48:38.000000 tencentcloud-sdk-python-tbp-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/setup.py` & `tencentcloud-sdk-python-tbp-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/tbp_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateBotResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def Reset(self, request):
         """对当前机器人的会话状态进行复位
 
         :param request: Request instance for Reset.
         :type request: :class:`tencentcloud.tbp.v20190311.models.ResetRequest`
@@ -65,15 +65,15 @@
             model = models.ResetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextProcess(self, request):
         """接收调用侧的文本输入，返回应答文本。已废弃，推荐使用最新版TextProcess接口。
 
         :param request: Request instance for TextProcess.
         :type request: :class:`tencentcloud.tbp.v20190311.models.TextProcessRequest`
@@ -88,15 +88,15 @@
             model = models.TextProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextReset(self, request):
         """会话重置接口。已废弃，推荐使用最新版TextReset接口。
 
         :param request: Request instance for TextReset.
         :type request: :class:`tencentcloud.tbp.v20190311.models.TextResetRequest`
@@ -111,8 +111,8 @@
             model = models.TextResetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190311/models.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190311/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/tbp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.TextProcessResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextReset(self, request):
         """会话重置接口。
 
         :param request: Request instance for TextReset.
         :type request: :class:`tencentcloud.tbp.v20190627.models.TextResetRequest`
@@ -65,8 +65,8 @@
             model = models.TextResetResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/tbp/v20190627/models.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/tbp/v20190627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.938/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.937/README.rst` & `tencentcloud-sdk-python-tbp-3.0.938/README.rst`

 * *Files identical despite different names*

