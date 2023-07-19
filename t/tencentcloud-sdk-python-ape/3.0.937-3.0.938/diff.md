# Comparing `tmp/tencentcloud-sdk-python-ape-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ape-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ape-3.0.937.tar", last modified: Tue Jul 18 00:16:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ape-3.0.938.tar", last modified: Wed Jul 19 00:20:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ape-3.0.937.tar` & `tencentcloud-sdk-python-ape-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8159 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/ape_client.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    42775 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:16:45.000000 tencentcloud-sdk-python-ape-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8191 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/ape_client.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    42775 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:20:57.000000 tencentcloud-sdk-python-ape-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ape-3.0.937/setup.py` & `tencentcloud-sdk-python-ape-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/ape_client.py` & `tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/ape_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchDescribeOrderCertificateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchDescribeOrderImage(self, request):
         """批量获取图片下载地址
 
         :param request: Request instance for BatchDescribeOrderImage.
         :type request: :class:`tencentcloud.ape.v20200513.models.BatchDescribeOrderImageRequest`
@@ -65,15 +65,15 @@
             model = models.BatchDescribeOrderImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrderAndDownloads(self, request):
         """核销图片，获取原图URL地址
 
         :param request: Request instance for CreateOrderAndDownloads.
         :type request: :class:`tencentcloud.ape.v20200513.models.CreateOrderAndDownloadsRequest`
@@ -88,15 +88,15 @@
             model = models.CreateOrderAndDownloadsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrderAndPay(self, request):
         """购买一张图片并且支付
 
         :param request: Request instance for CreateOrderAndPay.
         :type request: :class:`tencentcloud.ape.v20200513.models.CreateOrderAndPayRequest`
@@ -111,15 +111,15 @@
             model = models.CreateOrderAndPayResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAuthUsers(self, request):
         """分页查询授权人列表
 
         :param request: Request instance for DescribeAuthUsers.
         :type request: :class:`tencentcloud.ape.v20200513.models.DescribeAuthUsersRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeAuthUsersResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeDownloadInfos(self, request):
         """获取用户图片下载记录
 
         :param request: Request instance for DescribeDownloadInfos.
         :type request: :class:`tencentcloud.ape.v20200513.models.DescribeDownloadInfosRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeDownloadInfosResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImage(self, request):
         """根据ID查询一张图片的详细信息
 
         :param request: Request instance for DescribeImage.
         :type request: :class:`tencentcloud.ape.v20200513.models.DescribeImageRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeImageResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImages(self, request):
         """根据关键字搜索图片列表
 
         :param request: Request instance for DescribeImages.
         :type request: :class:`tencentcloud.ape.v20200513.models.DescribeImagesRequest`
@@ -203,8 +203,8 @@
             model = models.DescribeImagesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/errorcodes.py` & `tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.937/tencentcloud/ape/v20200513/models.py` & `tencentcloud-sdk-python-ape-3.0.938/tencentcloud/ape/v20200513/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ape-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ape-3.0.937/tencentcloud_sdk_python_ape.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ape-3.0.938/tencentcloud_sdk_python_ape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ape
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ape SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ape-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ape-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ape
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ape SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ape-3.0.937/README.rst` & `tencentcloud-sdk-python-ape-3.0.938/README.rst`

 * *Files identical despite different names*

