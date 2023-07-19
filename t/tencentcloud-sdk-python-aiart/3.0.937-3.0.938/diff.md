# Comparing `tmp/tencentcloud-sdk-python-aiart-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-aiart-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.937.tar", last modified: Tue Jul 18 00:16:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.938.tar", last modified: Wed Jul 19 00:20:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aiart-3.0.937.tar` & `tencentcloud-sdk-python-aiart-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/
--rw-r--r--   0 root         (0) root         (0)     3668 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/aiart_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:16:08.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:07.000000 tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/
+-rw-r--r--   0 root         (0) root         (0)     3676 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/aiart_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:25.000000 tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/setup.py` & `tencentcloud-sdk-python-aiart-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/aiart_client.py` & `tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/aiart_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             model = models.ImageToImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextToImage(self, request):
         """智能文生图接口将根据输入的描述文本，智能生成与之相关的结果图。
         输入：512个字符以内的描述性文本，推荐使用中文。
         输出：对应风格及分辨率的 AI 生成图。
         可支持的风格详见 [智能文生图风格列表](https://cloud.tencent.com/document/product/1668/86249)，请将列表中的“风格编号”传入 Styles 数组，建议选择一种风格。
@@ -75,8 +75,8 @@
             model = models.TextToImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/errorcodes.py` & `tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/aiart/v20221229/models.py` & `tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/aiart/v20221229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aiart-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/README.rst` & `tencentcloud-sdk-python-aiart-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.937/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.938/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
