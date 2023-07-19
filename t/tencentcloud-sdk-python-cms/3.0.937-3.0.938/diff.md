# Comparing `tmp/tencentcloud-sdk-python-cms-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-cms-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.937.tar", last modified: Tue Jul 18 00:21:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.938.tar", last modified: Wed Jul 19 00:25:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cms-3.0.937.tar` & `tencentcloud-sdk-python-cms-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/
--rw-r--r--   0 root         (0) root         (0)     6573 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/cms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4152 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    97349 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:21:01.000000 tencentcloud-sdk-python-cms-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/cms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    97349 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:25:08.000000 tencentcloud-sdk-python-cms-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-cms-3.0.937/tencentcloud_sdk_python_cms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.938/tencentcloud_sdk_python_cms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.937/setup.py` & `tencentcloud-sdk-python-cms-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cms-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/cms_client.py` & `tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/cms_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateKeywordsSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteLibSamples(self, request):
         """删除关键词接口
 
         :param request: Request instance for DeleteLibSamples.
         :type request: :class:`tencentcloud.cms.v20190321.models.DeleteLibSamplesRequest`
@@ -65,15 +65,15 @@
             model = models.DeleteLibSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKeywordsLibs(self, request):
         """获取用户词库列表
 
         :param request: Request instance for DescribeKeywordsLibs.
         :type request: :class:`tencentcloud.cms.v20190321.models.DescribeKeywordsLibsRequest`
@@ -88,15 +88,15 @@
             model = models.DescribeKeywordsLibsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLibSamples(self, request):
         """获取关键词接口
 
         :param request: Request instance for DescribeLibSamples.
         :type request: :class:`tencentcloud.cms.v20190321.models.DescribeLibSamplesRequest`
@@ -111,15 +111,15 @@
             model = models.DescribeLibSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageModeration(self, request):
         """图片内容检测服务（Image Moderation, IM）能自动扫描图片，识别涉黄、涉恐、涉政、涉毒等有害内容，同时支持用户配置图片黑名单，打击自定义的违规图片。
 
         :param request: Request instance for ImageModeration.
         :type request: :class:`tencentcloud.cms.v20190321.models.ImageModerationRequest`
@@ -134,15 +134,15 @@
             model = models.ImageModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextModeration(self, request):
         """文本内容检测（Text Moderation）服务使用了深度学习技术，识别涉黄、涉政、涉恐等有害内容，同时支持用户配置词库，打击自定义的违规文本。
 
         :param request: Request instance for TextModeration.
         :type request: :class:`tencentcloud.cms.v20190321.models.TextModerationRequest`
@@ -157,8 +157,8 @@
             model = models.TextModerationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/errorcodes.py` & `tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.937/tencentcloud/cms/v20190321/models.py` & `tencentcloud-sdk-python-cms-3.0.938/tencentcloud/cms/v20190321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.938/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.937/README.rst` & `tencentcloud-sdk-python-cms-3.0.938/README.rst`

 * *Files identical despite different names*

