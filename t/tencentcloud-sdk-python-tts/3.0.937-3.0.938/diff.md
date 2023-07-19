# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.937.tar", last modified: Tue Jul 18 00:34:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.938.tar", last modified: Wed Jul 19 00:53:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.937.tar` & `tencentcloud-sdk-python-tts-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23658 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:34.000000 tencentcloud-sdk-python-tts-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23658 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:53:17.000000 tencentcloud-sdk-python-tts-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tts-3.0.937/setup.py` & `tencentcloud-sdk-python-tts-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.937/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.938/tencentcloud/tts/v20190823/tts_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             model = models.CreateTtsTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTtsTaskStatus(self, request):
         """在调用长文本语音合成请求接口后，有回调和轮询两种方式获取识别结果。
 
         <li>当采用回调方式时，合成完毕后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见 长文本语音合成结果查询 。</li>
         <li>当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见下文说明。</li>
@@ -85,15 +85,15 @@
             model = models.DescribeTtsTaskStatusResponse()
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
         基础合成支持 SSML，语法详见 [SSML 标记语言](https://cloud.tencent.com/document/product/1073/49575)。
@@ -112,8 +112,8 @@
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

### Comparing `tencentcloud-sdk-python-tts-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.937/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.938/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.937/README.rst` & `tencentcloud-sdk-python-tts-3.0.938/README.rst`

 * *Files identical despite different names*

