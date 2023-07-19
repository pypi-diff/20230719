# Comparing `tmp/tencentcloud-sdk-python-facefusion-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-facefusion-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.937.tar", last modified: Tue Jul 18 00:23:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.938.tar", last modified: Wed Jul 19 00:39:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-facefusion-3.0.937.tar` & `tencentcloud-sdk-python-facefusion-3.0.938.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     5459 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20924 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5769 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35069 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-18 00:23:58.000000 tencentcloud-sdk-python-facefusion-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20924 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    35069 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-19 00:39:14.000000 tencentcloud-sdk-python-facefusion-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/setup.py` & `tencentcloud-sdk-python-facefusion-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeMaterialListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FuseFace(self, request):
         """本接口用于单脸、多脸、选脸融合，上传人脸图片，得到与素材模板融合后的人脸图片。支持为融合结果图添加标识。查看 <a href="https://cloud.tencent.com/document/product/670/38247" target="_blank">融合接入指引</a>。
 
         请求频率限制为20次/秒。
         >
@@ -69,8 +69,8 @@
             model = models.FuseFaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20220927/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeMaterialListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FaceFusion(self, request):
         """本接口用于人脸融合，用户上传人脸图片，获取与模板融合后的人脸图片。未发布的活动请求频率限制为1次/秒，已发布的活动请求频率限制50次/秒。如有需要提高活动的请求频率限制，请在控制台中申请。
         >
         - 公共参数中的签名方式必须指定为V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
 
@@ -67,15 +67,15 @@
             model = models.FaceFusionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FaceFusionLite(self, request):
         """人脸融合活动专用版，不推荐使用。人脸融合接口建议使用[人脸融合](https://cloud.tencent.com/document/product/670/31061)或[选脸融合](https://cloud.tencent.com/document/product/670/37736)接口
 
         :param request: Request instance for FaceFusionLite.
         :type request: :class:`tencentcloud.facefusion.v20181201.models.FaceFusionLiteRequest`
@@ -90,15 +90,15 @@
             model = models.FaceFusionLiteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def FuseFace(self, request):
         """本接口用于单脸、多脸融合，用户上传人脸图片，获取与模板融合后的人脸图片。查看 <a href="https://cloud.tencent.com/document/product/670/38247" target="_blank">选脸融合接入指引</a>。
 
         未发布的活动请求频率限制为1次/秒，已发布的活动请求频率限制50次/秒。如有需要提高活动的请求频率限制，请在控制台中申请。
         >
@@ -117,8 +117,8 @@
             model = models.FuseFaceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/facefusion/v20181201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-facefusion-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.937/README.rst` & `tencentcloud-sdk-python-facefusion-3.0.938/README.rst`

 * *Files identical despite different names*

