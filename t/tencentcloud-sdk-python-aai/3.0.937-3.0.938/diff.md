# Comparing `tmp/tencentcloud-sdk-python-aai-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-aai-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aai-3.0.937.tar", last modified: Tue Jul 18 00:15:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aai-3.0.938.tar", last modified: Wed Jul 19 00:19:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aai-3.0.937.tar` & `tencentcloud-sdk-python-aai-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/
--rw-r--r--   0 root         (0) root         (0)     5481 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/aai_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20548 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:15:37.000000 tencentcloud-sdk-python-aai-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/aai_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20548 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:19:56.000000 tencentcloud-sdk-python-aai-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-aai-3.0.937/setup.py` & `tencentcloud-sdk-python-aai-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/aai_client.py` & `tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/aai_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.ChatResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SentenceRecognition(self, request):
         """识别60s内的短语音，当音频放在请求body中传输时整个请求大小不能超过600KB，当音频以url方式传输时，音频时长不可超过60s。所有请求参数放在post的body中采用x-www-form-urlencoded（数据转换成一个字符串（name1=value1&name2=value2…）进行urlencode后）编码传输。现暂只支持中文普通话识别，支持识别8k(16k)的16bit的mp3或者wav音频。
 
         :param request: Request instance for SentenceRecognition.
         :type request: :class:`tencentcloud.aai.v20180522.models.SentenceRecognitionRequest`
@@ -65,15 +65,15 @@
             model = models.SentenceRecognitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SimultaneousInterpreting(self, request):
         """该接口是实时流式识别，可同时返回语音识别文本及翻译文本，当前仅支持中文和英文。该接口可配合同传windows客户端，提供会议现场同传服务。
 
         :param request: Request instance for SimultaneousInterpreting.
         :type request: :class:`tencentcloud.aai.v20180522.models.SimultaneousInterpretingRequest`
@@ -88,15 +88,15 @@
             model = models.SimultaneousInterpretingResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextToVoice(self, request):
         """腾讯云语音合成技术（TTS）可以将任意文本转化为语音，实现让机器和应用张口说话。
         腾讯TTS技术可以应用到很多场景，比如，移动APP语音播报新闻；智能设备语音提醒；依靠网上现有节目或少量录音，快速合成明星语音，降低邀约成本；支持车载导航语音合成的个性化语音播报。
         内测期间免费使用。
 
@@ -113,8 +113,8 @@
             model = models.TextToVoiceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/errorcodes.py` & `tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aai-3.0.937/tencentcloud/aai/v20180522/models.py` & `tencentcloud-sdk-python-aai-3.0.938/tencentcloud/aai/v20180522/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aai-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aai-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aai-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-aai-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aai
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aai-3.0.937/tencentcloud_sdk_python_aai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aai-3.0.938/tencentcloud_sdk_python_aai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aai
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Aai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aai-3.0.937/README.rst` & `tencentcloud-sdk-python-aai-3.0.938/README.rst`

 * *Files identical despite different names*

