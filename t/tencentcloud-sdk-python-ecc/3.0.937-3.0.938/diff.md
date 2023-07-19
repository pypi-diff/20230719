# Comparing `tmp/tencentcloud-sdk-python-ecc-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ecc-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecc-3.0.937.tar", last modified: Tue Jul 18 00:23:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecc-3.0.938.tar", last modified: Wed Jul 19 00:38:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecc-3.0.937.tar` & `tencentcloud-sdk-python-ecc-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4481 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/ecc_client.py
--rw-r--r--   0 root         (0) root         (0)    37203 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:14.000000 tencentcloud-sdk-python-ecc-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:13.000000 tencentcloud-sdk-python-ecc-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/ecc_client.py
+-rw-r--r--   0 root         (0) root         (0)    37203 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:38:27.000000 tencentcloud-sdk-python-ecc-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/setup.py` & `tencentcloud-sdk-python-ecc-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/errorcodes.py` & `tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/ecc_client.py` & `tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/ecc_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             model = models.CorrectMultiImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTask(self, request):
         """异步任务结果查询接口
 
         :param request: Request instance for DescribeTask.
         :type request: :class:`tencentcloud.ecc.v20181213.models.DescribeTaskRequest`
@@ -66,15 +66,15 @@
             model = models.DescribeTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ECC(self, request):
         """接口请求域名： ecc.tencentcloudapi.com
         纯文本英语作文批改
 
         :param request: Request instance for ECC.
@@ -90,15 +90,15 @@
             model = models.ECCResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EHOCR(self, request):
         """https://ecc.tencentcloudapi.com/?Action=EHOCR
         图像识别批改接口
 
         :param request: Request instance for EHOCR.
@@ -114,8 +114,8 @@
             model = models.EHOCRResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/ecc/v20181213/models.py` & `tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/ecc/v20181213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecc-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/tencentcloud_sdk_python_ecc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecc-3.0.938/tencentcloud_sdk_python_ecc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ecc-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecc
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ecc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecc-3.0.937/README.rst` & `tencentcloud-sdk-python-ecc-3.0.938/README.rst`

 * *Files identical despite different names*

