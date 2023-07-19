# Comparing `tmp/tencentcloud-sdk-python-tmt-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-tmt-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.937.tar", last modified: Tue Jul 18 00:33:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.938.tar", last modified: Wed Jul 19 00:51:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tmt-3.0.937.tar` & `tencentcloud-sdk-python-tmt-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9401 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)    46724 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:33:43.000000 tencentcloud-sdk-python-tmt-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9429 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    46724 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:51:21.000000 tencentcloud-sdk-python-tmt-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/setup.py` & `tencentcloud-sdk-python-tmt-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.938/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.FileTranslateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetFileTranslate(self, request):
         """在调用文档翻译请求接口后，有回调和轮询两种方式获取识别结果。
         •当采用回调方式时，翻译完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见文档翻译结果回调。
         • 当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见参数说明。
 
@@ -67,15 +67,15 @@
             model = models.GetFileTranslateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ImageTranslate(self, request):
         """提供13种语言的图片翻译服务，可自动识别图片中的文本内容并翻译成目标语言，识别后的文本按行翻译，后续会提供可按段落翻译的版本。<br />
         提示：对于一般开发者，我们建议优先使用SDK接入简化开发。SDK使用介绍请直接查看 5. 开发者资源 部分。
 
         :param request: Request instance for ImageTranslate.
@@ -91,15 +91,15 @@
             model = models.ImageTranslateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def LanguageDetect(self, request):
         """可自动识别文本内容的语言种类，轻量高效，无需额外实现判断方式，使面向客户的服务体验更佳。 <br />
         提示：对于一般开发者，我们建议优先使用SDK接入简化开发。SDK使用介绍请直接查看 5. 开发者资源 部分。
 
         :param request: Request instance for LanguageDetect.
@@ -115,15 +115,15 @@
             model = models.LanguageDetectResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SpeechTranslate(self, request):
         """本接口提供上传音频，将音频进行语音识别并翻译成文本的服务，目前开放中英互译的语音翻译服务。
         待识别和翻译的音频文件可以是 pcm、mp3和speex 格式，pcm采样率要求16kHz、位深16bit、单声道，音频内语音清晰。<br/>
         如果采用流式传输的方式，要求每个分片时长200ms~500ms；如果采用非流式的传输方式，要求音频时长不超过8s。注意最后一个分片的IsEnd参数设置为1。<br />
         提示：对于一般开发者，我们建议优先使用SDK接入简化开发。SDK使用介绍请直接查看 5. 开发者资源部分。
@@ -141,15 +141,15 @@
             model = models.SpeechTranslateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextTranslate(self, request):
         """提供中文到英文、英文到中文的等多种语言的文本内容翻译服务， 经过大数据语料库、多种解码算法、翻译引擎深度优化，在新闻文章、生活口语等不同语言场景中都有深厚积累，翻译结果专业评价处于行业领先水平。<br />
         提示：对于一般开发者，我们建议优先使用SDK接入简化开发。SDK使用介绍请直接查看 5. 开发者资源 部分。
 
         :param request: Request instance for TextTranslate.
@@ -165,15 +165,15 @@
             model = models.TextTranslateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def TextTranslateBatch(self, request):
         """文本翻译的批量接口
 
         :param request: Request instance for TextTranslateBatch.
         :type request: :class:`tencentcloud.tmt.v20180321.models.TextTranslateBatchRequest`
@@ -188,8 +188,8 @@
             model = models.TextTranslateBatchResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-tmt-3.0.938/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.938/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.937/README.rst` & `tencentcloud-sdk-python-tmt-3.0.938/README.rst`

 * *Files identical despite different names*

