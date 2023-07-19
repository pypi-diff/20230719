# Comparing `tmp/tencentcloud-sdk-python-mrs-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mrs-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mrs-3.0.937.tar", last modified: Tue Jul 18 00:27:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mrs-3.0.938.tar", last modified: Wed Jul 19 00:43:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mrs-3.0.937.tar` & `tencentcloud-sdk-python-mrs-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/
--rw-r--r--   0 root         (0) root         (0)     4657 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/mrs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   540004 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:27:46.000000 tencentcloud-sdk-python-mrs-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/
+-rw-r--r--   0 root         (0) root         (0)     4673 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/mrs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   540004 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:08.000000 tencentcloud-sdk-python-mrs-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/setup.py` & `tencentcloud-sdk-python-mrs-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/mrs_client.py` & `tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/mrs_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ImageToClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageToObject(self, request):
         """图片转结构化对象
 
         :param request: Request instance for ImageToObject.
         :type request: :class:`tencentcloud.mrs.v20200910.models.ImageToObjectRequest`
@@ -65,15 +65,15 @@
             model = models.ImageToObjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextToClass(self, request):
         """文本分类
 
         :param request: Request instance for TextToClass.
         :type request: :class:`tencentcloud.mrs.v20200910.models.TextToClassRequest`
@@ -88,15 +88,15 @@
             model = models.TextToClassResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextToObject(self, request):
         """文本转结构化对象。
 
         适用场景：经过腾讯医疗专用 OCR 从图片识别之后的文本，可以调用此接口。通过其它 OCR 识别的文本可能不适配。医院的 XML 格式文本也不适配，XML 文件需要经过特殊转换才能直接调用此接口。单次调用传入的文本不宜超过 2000 字。
 
@@ -113,8 +113,8 @@
             model = models.TextToObjectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/errorcodes.py` & `tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/tencentcloud/mrs/v20200910/models.py` & `tencentcloud-sdk-python-mrs-3.0.938/tencentcloud/mrs/v20200910/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mrs-3.0.938/tencentcloud_sdk_python_mrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mrs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mrs-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mrs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mrs-3.0.937/README.rst` & `tencentcloud-sdk-python-mrs-3.0.938/README.rst`

 * *Files identical despite different names*

