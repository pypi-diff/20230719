# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.937.tar", last modified: Tue Jul 18 00:35:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.938.tar", last modified: Wed Jul 19 00:53:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.937.tar` & `tencentcloud-sdk-python-vrs-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)     7434 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28696 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28696 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:48.000000 tencentcloud-sdk-python-vrs-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/setup.py` & `tencentcloud-sdk-python-vrs-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.938/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CancelVRSTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateVRSTask(self, request):
         """本接口服务对提交音频进行声音复刻任务创建接口，异步返回复刻结果。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
 
@@ -67,15 +67,15 @@
             model = models.CreateVRSTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeVRSTaskStatus(self, request):
         """在调用声音复刻创建任务请求接口后，有回调和轮询两种方式获取识别结果。
         • 当采用回调方式时，识别完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见 声音复刻结果回调 。
         • 当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见下文说明。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
@@ -94,15 +94,15 @@
             model = models.DescribeVRSTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DetectEnvAndSoundQuality(self, request):
         """本接口用于检测音频的环境和音频质量。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
 
@@ -119,15 +119,15 @@
             model = models.DetectEnvAndSoundQualityResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadVRSModel(self, request):
         """下载声音复刻离线模型
 
         :param request: Request instance for DownloadVRSModel.
         :type request: :class:`tencentcloud.vrs.v20200824.models.DownloadVRSModelRequest`
@@ -142,15 +142,15 @@
             model = models.DownloadVRSModelResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTrainingText(self, request):
         """本接口用于获取声音复刻训练文本信息。
          请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
 
@@ -167,8 +167,8 @@
             model = models.GetTrainingTextResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.938/tencentcloud/vrs/v20200824/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.937/README.rst` & `tencentcloud-sdk-python-vrs-3.0.938/README.rst`

 * *Files identical despite different names*

