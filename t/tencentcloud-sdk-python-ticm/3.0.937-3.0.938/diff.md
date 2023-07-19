# Comparing `tmp/tencentcloud-sdk-python-ticm-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ticm-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ticm-3.0.937.tar", last modified: Tue Jul 18 00:32:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ticm-3.0.938.tar", last modified: Wed Jul 19 00:50:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ticm-3.0.937.tar` & `tencentcloud-sdk-python-ticm-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/
--rw-r--r--   0 root         (0) root         (0)     4013 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/ticm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80377 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:56.000000 tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:32:55.000000 tencentcloud-sdk-python-ticm-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/ticm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80377 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-19 00:50:35.000000 tencentcloud-sdk-python-ticm-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/setup.py` & `tencentcloud-sdk-python-ticm-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/ticm_client.py` & `tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/ticm_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.DescribeVideoTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageModeration(self, request):
         """本接口提供多种维度的图像审核能力，支持色情和性感内容识别，政治人物和涉政敏感场景识别，以及暴恐人物、场景、旗帜标识等违禁内容的识别。
 
         :param request: Request instance for ImageModeration.
         :type request: :class:`tencentcloud.ticm.v20181127.models.ImageModerationRequest`
@@ -65,15 +65,15 @@
             model = models.ImageModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VideoModeration(self, request):
         """本接口提供多种维度的视频审核能力，支持色情和性感内容识别，政治人物和涉政敏感场景识别，以及暴恐人物、场景、旗帜标识等违禁内容的识别。
 
         :param request: Request instance for VideoModeration.
         :type request: :class:`tencentcloud.ticm.v20181127.models.VideoModerationRequest`
@@ -88,8 +88,8 @@
             model = models.VideoModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/errorcodes.py` & `tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/ticm/v20181127/models.py` & `tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/ticm/v20181127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ticm-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ticm-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ticm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ticm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ticm-3.0.938/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ticm
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ticm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.937/README.rst` & `tencentcloud-sdk-python-ticm-3.0.938/README.rst`

 * *Files identical despite different names*

