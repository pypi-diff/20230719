# Comparing `tmp/tencentcloud-sdk-python-ie-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-ie-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ie-3.0.937.tar", last modified: Tue Jul 18 00:25:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ie-3.0.938.tar", last modified: Wed Jul 19 00:40:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ie-3.0.937.tar` & `tencentcloud-sdk-python-ie-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10985 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/ie_client.py
--rw-r--r--   0 root         (0) root         (0)   233379 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 00:25:20.000000 tencentcloud-sdk-python-ie-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/ie_client.py
+-rw-r--r--   0 root         (0) root         (0)   233379 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-19 00:40:40.000000 tencentcloud-sdk-python-ie-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-ie-3.0.937/tencentcloud_sdk_python_ie.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ie-3.0.938/tencentcloud_sdk_python_ie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ie
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ie SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ie-3.0.937/setup.py` & `tencentcloud-sdk-python-ie-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ie-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/errorcodes.py` & `tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/ie_client.py` & `tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/ie_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CreateEditingTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMediaProcessTask(self, request):
         """用于创建编辑处理任务，如媒体截取、媒体编辑、媒体拼接、媒体字幕。
 
         :param request: Request instance for CreateMediaProcessTask.
         :type request: :class:`tencentcloud.ie.v20200304.models.CreateMediaProcessTaskRequest`
@@ -65,15 +65,15 @@
             model = models.CreateMediaProcessTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateMediaQualityRestorationTask(self, request):
         """创建画质重生任务，对视频进行转码、去噪、去划痕、去毛刺、超分、细节增强和色彩增强。
 
         :param request: Request instance for CreateMediaQualityRestorationTask.
         :type request: :class:`tencentcloud.ie.v20200304.models.CreateMediaQualityRestorationTaskRequest`
@@ -88,15 +88,15 @@
             model = models.CreateMediaQualityRestorationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateQualityControlTask(self, request):
         """通过接口可以智能检测视频画面中抖动重影、模糊、低光照、过曝光、黑边、白边、黑屏、白屏、花屏、噪点、马赛克、二维码等在内的多个场景，还可以自动检测视频无音频异常、无声音片段。
 
         :param request: Request instance for CreateQualityControlTask.
         :type request: :class:`tencentcloud.ie.v20200304.models.CreateQualityControlTaskRequest`
@@ -111,15 +111,15 @@
             model = models.CreateQualityControlTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEditingTaskResult(self, request):
         """获取编辑理解任务结果。
 
         :param request: Request instance for DescribeEditingTaskResult.
         :type request: :class:`tencentcloud.ie.v20200304.models.DescribeEditingTaskResultRequest`
@@ -134,15 +134,15 @@
             model = models.DescribeEditingTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaProcessTaskResult(self, request):
         """用于获取编辑处理任务的结果。
 
         :param request: Request instance for DescribeMediaProcessTaskResult.
         :type request: :class:`tencentcloud.ie.v20200304.models.DescribeMediaProcessTaskResultRequest`
@@ -157,15 +157,15 @@
             model = models.DescribeMediaProcessTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaQualityRestorationTaskRusult(self, request):
         """获取画质重生任务结果，查看结束后的文件信息
 
         :param request: Request instance for DescribeMediaQualityRestorationTaskRusult.
         :type request: :class:`tencentcloud.ie.v20200304.models.DescribeMediaQualityRestorationTaskRusultRequest`
@@ -180,15 +180,15 @@
             model = models.DescribeMediaQualityRestorationTaskRusultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeQualityControlTaskResult(self, request):
         """获取媒体质检任务结果
 
         :param request: Request instance for DescribeQualityControlTaskResult.
         :type request: :class:`tencentcloud.ie.v20200304.models.DescribeQualityControlTaskResultRequest`
@@ -203,15 +203,15 @@
             model = models.DescribeQualityControlTaskResultResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMediaProcessTask(self, request):
         """用于停止正在进行中的编辑处理任务。
 
         :param request: Request instance for StopMediaProcessTask.
         :type request: :class:`tencentcloud.ie.v20200304.models.StopMediaProcessTaskRequest`
@@ -226,15 +226,15 @@
             model = models.StopMediaProcessTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopMediaQualityRestorationTask(self, request):
         """删除正在进行的画质重生任务
 
         :param request: Request instance for StopMediaQualityRestorationTask.
         :type request: :class:`tencentcloud.ie.v20200304.models.StopMediaQualityRestorationTaskRequest`
@@ -249,8 +249,8 @@
             model = models.StopMediaQualityRestorationTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-ie-3.0.937/tencentcloud/ie/v20200304/models.py` & `tencentcloud-sdk-python-ie-3.0.938/tencentcloud/ie/v20200304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ie-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-ie-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ie
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Ie SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ie-3.0.937/README.rst` & `tencentcloud-sdk-python-ie-3.0.938/README.rst`

 * *Files identical despite different names*

