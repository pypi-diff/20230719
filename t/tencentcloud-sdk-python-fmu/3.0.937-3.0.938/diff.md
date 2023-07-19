# Comparing `tmp/tencentcloud-sdk-python-fmu-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-fmu-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.937.tar", last modified: Tue Jul 18 00:24:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.938.tar", last modified: Wed Jul 19 00:39:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-fmu-3.0.937.tar` & `tencentcloud-sdk-python-fmu-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)    10578 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/fmu_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45807 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:24:09.000000 tencentcloud-sdk-python-fmu-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)    10618 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/fmu_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    45807 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:39:24.000000 tencentcloud-sdk-python-fmu-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/setup.py` & `tencentcloud-sdk-python-fmu-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BeautifyPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BeautifyVideo(self, request):
         """视频美颜(此接口目前已下线)
 
         :param request: Request instance for BeautifyVideo.
         :type request: :class:`tencentcloud.fmu.v20191213.models.BeautifyVideoRequest`
@@ -65,15 +65,15 @@
             model = models.BeautifyVideoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CancelBeautifyVideoJob(self, request):
         """撤销视频美颜任务请求
 
         :param request: Request instance for CancelBeautifyVideoJob.
         :type request: :class:`tencentcloud.fmu.v20191213.models.CancelBeautifyVideoJobRequest`
@@ -88,15 +88,15 @@
             model = models.CancelBeautifyVideoJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateModel(self, request):
         """在使用LUT素材的modelid实现试唇色前，您需要先上传 LUT 格式的cube文件注册唇色ID。查看 [LUT文件的使用说明](https://cloud.tencent.com/document/product/1172/41701)。
 
         注：您也可以直接使用 [试唇色接口](https://cloud.tencent.com/document/product/1172/40706)，通过输入RGBA模型数值的方式指定唇色，更简单易用。
 
@@ -113,15 +113,15 @@
             model = models.CreateModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteModel(self, request):
         """删除已注册的唇色素材。
 
         :param request: Request instance for DeleteModel.
         :type request: :class:`tencentcloud.fmu.v20191213.models.DeleteModelRequest`
@@ -136,15 +136,15 @@
             model = models.DeleteModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetModelList(self, request):
         """查询已注册的唇色素材。
 
         :param request: Request instance for GetModelList.
         :type request: :class:`tencentcloud.fmu.v20191213.models.GetModelListRequest`
@@ -159,15 +159,15 @@
             model = models.GetModelListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryBeautifyVideoJob(self, request):
         """查询视频美颜处理进度
 
         :param request: Request instance for QueryBeautifyVideoJob.
         :type request: :class:`tencentcloud.fmu.v20191213.models.QueryBeautifyVideoJobRequest`
@@ -182,15 +182,15 @@
             model = models.QueryBeautifyVideoJobResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StyleImage(self, request):
         """上传一张照片，输出滤镜处理后的图片。
 
         :param request: Request instance for StyleImage.
         :type request: :class:`tencentcloud.fmu.v20191213.models.StyleImageRequest`
@@ -205,15 +205,15 @@
             model = models.StyleImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StyleImagePro(self, request):
         """上传一张照片，输出滤镜处理后的图片。
 
         :param request: Request instance for StyleImagePro.
         :type request: :class:`tencentcloud.fmu.v20191213.models.StyleImageProRequest`
@@ -228,15 +228,15 @@
             model = models.StyleImageProResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TryLipstickPic(self, request):
         """对图片中的人脸嘴唇进行着色，最多支持同时对一张图中的3张人脸进行试唇色。
 
         您可以通过事先注册在腾讯云的唇色素材（LUT文件）改变图片中的人脸唇色，也可以输入RGBA模型数值。
 
@@ -258,8 +258,8 @@
             model = models.TryLipstickPicResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-fmu-3.0.938/tencentcloud/fmu/v20191213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.938/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.937/README.rst` & `tencentcloud-sdk-python-fmu-3.0.938/README.rst`

 * *Files identical despite different names*

