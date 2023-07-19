# Comparing `tmp/tencentcloud-sdk-python-ft-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ft-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ft-3.0.937.tar", last modified: Tue Jul 18 00:24:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ft-3.0.938.tar", last modified: Wed Jul 19 00:39:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ft-3.0.937.tar` & `tencentcloud-sdk-python-ft-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5534 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6803 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/ft_client.py
--rw-r--r--   0 root         (0) root         (0)    29493 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:24:14.000000 tencentcloud-sdk-python-ft-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/ft_client.py
+-rw-r--r--   0 root         (0) root         (0)    29493 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:39:31.000000 tencentcloud-sdk-python-ft-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ft-3.0.937/tencentcloud_sdk_python_ft.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ft-3.0.938/tencentcloud_sdk_python_ft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ft
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ft SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ft-3.0.937/setup.py` & `tencentcloud-sdk-python-ft-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/errorcodes.py` & `tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/ft_client.py` & `tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/ft_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelFaceMorphJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChangeAgePic(self, request):
         """用户上传一张人脸图片，基于人脸编辑与生成算法，输出一张人脸变老或变年轻的图片，支持实现人脸不同年龄的变化。
 
         :param request: Request instance for ChangeAgePic.
         :type request: :class:`tencentcloud.ft.v20200304.models.ChangeAgePicRequest`
@@ -65,15 +65,15 @@
             model = models.ChangeAgePicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FaceCartoonPic(self, request):
         """输入一张人脸照片，生成个性化的二次元动漫形象，可用于打造个性头像、趣味活动、特效类应用等场景，提升社交娱乐的体验。
 
         :param request: Request instance for FaceCartoonPic.
         :type request: :class:`tencentcloud.ft.v20200304.models.FaceCartoonPicRequest`
@@ -88,15 +88,15 @@
             model = models.FaceCartoonPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def MorphFace(self, request):
         """输入2-5张人脸照片，生成一段以人脸为焦点的渐变视频或GIF图，支持自定义图片播放速度、视频每秒传输帧数，可用于短视频、表情包、创意H5等应用场景，丰富静态图片的玩法。
 
         :param request: Request instance for MorphFace.
         :type request: :class:`tencentcloud.ft.v20200304.models.MorphFaceRequest`
@@ -111,15 +111,15 @@
             model = models.MorphFaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryFaceMorphJob(self, request):
         """查询人像渐变处理进度
 
         :param request: Request instance for QueryFaceMorphJob.
         :type request: :class:`tencentcloud.ft.v20200304.models.QueryFaceMorphJobRequest`
@@ -134,15 +134,15 @@
             model = models.QueryFaceMorphJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SwapGenderPic(self, request):
         """用户上传一张人脸图片，基于人脸编辑与生成算法，输出一张人脸性别转换的图片。男变女可实现美颜、淡妆、加刘海和长发的效果；女变男可实现加胡须、变短发的效果。
 
         :param request: Request instance for SwapGenderPic.
         :type request: :class:`tencentcloud.ft.v20200304.models.SwapGenderPicRequest`
@@ -157,8 +157,8 @@
             model = models.SwapGenderPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ft-3.0.937/tencentcloud/ft/v20200304/models.py` & `tencentcloud-sdk-python-ft-3.0.938/tencentcloud/ft/v20200304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ft-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ft-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ft-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ft-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ft
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ft SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ft-3.0.937/README.rst` & `tencentcloud-sdk-python-ft-3.0.938/README.rst`

 * *Files identical despite different names*

