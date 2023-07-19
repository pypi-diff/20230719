# Comparing `tmp/tencentcloud-sdk-python-ims-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ims-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.937.tar", last modified: Tue Jul 18 00:25:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.938.tar", last modified: Wed Jul 19 00:40:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ims-3.0.937.tar` & `tencentcloud-sdk-python-ims-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/
--rw-r--r--   0 root         (0) root         (0)     3224 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/ims_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47064 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/
--rw-r--r--   0 root         (0) root         (0)     8549 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/ims_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65090 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:25:34.000000 tencentcloud-sdk-python-ims-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/
+-rw-r--r--   0 root         (0) root         (0)     3228 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    47064 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65090 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:40:57.000000 tencentcloud-sdk-python-ims-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ims-3.0.937/setup.py` & `tencentcloud-sdk-python-ims-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/ims_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,8 +58,8 @@
             model = models.ImageModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20200713/models.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/ims_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             model = models.CreateImageModerationAsyncTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageModeration(self, request):
         """本接口（Image Moderation, IM）用于提交图片文件进行同步智能审核任务。使用前请您使用腾讯云主账号登录控制台 [开通图片内容安全服务](https://console.cloud.tencent.com/cms/image/package) 并调整好对应的业务配置。
         ### 接口使用说明：
         - 前往“[内容安全控制台-图片内容安全](https://console.cloud.tencent.com/cms/image/package)”开启使用图片内容安全服务，首次开通服务的用户可免费领用试用套餐包，包含**1万张图片**识别额度，有效期为1个月。
         - 该接口为收费接口，计费方式敬请参见 [腾讯云图片内容安全定价](https://cloud.tencent.com/product/ims/pricing)。
@@ -122,8 +122,8 @@
             model = models.ImageModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/ims/v20201229/models.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/ims/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ims-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.937/tencentcloud_sdk_python_ims.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.938/tencentcloud_sdk_python_ims.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ims-3.0.937/README.rst` & `tencentcloud-sdk-python-ims-3.0.938/README.rst`

 * *Files identical despite different names*

