# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.937.tar", last modified: Tue Jul 18 00:17:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.938.tar", last modified: Wed Jul 19 00:21:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.937.tar` & `tencentcloud-sdk-python-asr-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29321 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   111858 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29417 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   111858 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:21:15.000000 tencentcloud-sdk-python-asr-3.0.938/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.937/setup.py` & `tencentcloud-sdk-python-asr-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.938/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.CloseAsyncRecognitionTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAsrVocab(self, request):
         """用户通过本接口进行热词表的创建。
         <br>•   默认最多可创建30个热词表。
         <br>•   每个热词表最多可添加128个词，每个词最长10个字，不能超出限制。
         <br>•   热词表可以通过数组或者本地文件形式上传。
@@ -70,15 +70,15 @@
             model = models.CreateAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAsyncRecognitionTask(self, request):
         """本接口用于对语音流进行准实时识别，通过异步回调来返回识别结果。适用于直播审核等场景。
         <br>• 支持rtmp、rtsp等流媒体协议，以及各类基于http协议的直播流(不支持hls)
         <br>• 音频流时长无限制，服务会自动拉取音频流数据，若连续10分钟拉不到流数据时，服务会终止识别任务
         <br>• 服务通过回调的方式来提供识别结果，用户需要提供CallbackUrl。回调时机为一小段话(最长15秒)回调一次。
@@ -98,15 +98,15 @@
             model = models.CreateAsyncRecognitionTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateCustomization(self, request):
         """用户使用该接口可以创建自学习模型，以供识别调用。
 
         注意：调用该接口后，模型会自动训练。新建模型成功后，调用ModifyCustomizationState接口修改为上线状态，即可在识别请求中使用对应模型ID。
 
@@ -123,15 +123,15 @@
             model = models.CreateCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateRecTask(self, request):
         """本接口服务对时长5小时以内的录音文件进行识别，异步返回识别全部结果。
         • 支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、葡萄牙语、土耳其语、阿拉伯语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。
         • 支持wav、mp3、m4a、flv、mp4、wma、3gp、amr、aac、ogg-opus、flac格式。
         • 支持语音 URL 和本地语音文件两种请求方式。语音 URL 的音频时长不能长于5小时，文件大小不超过1GB。本地语音文件调用不能大于5MB。推荐使用 [ 腾讯云COS](https://cloud.tencent.com/document/product/436/38484) 来存储&生成URL提交任务，无外网&流量下行费用，节约成本、提升任务速度。(COS桶权限需要设置公有读私有写，或URL设置外部可访问)
@@ -154,15 +154,15 @@
             model = models.CreateRecTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAsrVocab(self, request):
         """用户通过本接口进行热词表的删除。
 
         :param request: Request instance for DeleteAsrVocab.
         :type request: :class:`tencentcloud.asr.v20190614.models.DeleteAsrVocabRequest`
@@ -177,15 +177,15 @@
             model = models.DeleteAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteCustomization(self, request):
         """用户通过该接口可以删除自学习模型
 
         :param request: Request instance for DeleteCustomization.
         :type request: :class:`tencentcloud.asr.v20190614.models.DeleteCustomizationRequest`
@@ -200,15 +200,15 @@
             model = models.DeleteCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAsyncRecognitionTasks(self, request):
         """本接口用于查询当前在运行的语音流异步识别任务列表。
         <br>•   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。
 
         :param request: Request instance for DescribeAsyncRecognitionTasks.
@@ -224,15 +224,15 @@
             model = models.DescribeAsyncRecognitionTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskStatus(self, request):
         """在调用录音文件识别请求接口后，有回调和轮询两种方式获取识别结果。
         <br>• 当采用回调方式时，识别完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见[ 录音识别结果回调 ](https://cloud.tencent.com/document/product/1093/52632)。
         <br>• 当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见下文说明。
         <br>•   请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
@@ -252,15 +252,15 @@
             model = models.DescribeTaskStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadAsrVocab(self, request):
         """用户通过本接口进行热词表的下载，获得词表权重文件形式的 base64 值，文件形式为通过 “|” 分割的词和权重，即 word|weight 的形式。
 
         :param request: Request instance for DownloadAsrVocab.
         :type request: :class:`tencentcloud.asr.v20190614.models.DownloadAsrVocabRequest`
@@ -275,15 +275,15 @@
             model = models.DownloadAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DownloadCustomization(self, request):
         """用户通过该接口可以下载自学习模型的语料
 
         :param request: Request instance for DownloadCustomization.
         :type request: :class:`tencentcloud.asr.v20190614.models.DownloadCustomizationRequest`
@@ -298,15 +298,15 @@
             model = models.DownloadCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAsrVocab(self, request):
         """用户根据词表的ID可以获取对应的热词表信息
 
         :param request: Request instance for GetAsrVocab.
         :type request: :class:`tencentcloud.asr.v20190614.models.GetAsrVocabRequest`
@@ -321,15 +321,15 @@
             model = models.GetAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetAsrVocabList(self, request):
         """用户通过该接口，可获得所有的热词表及其信息。
 
         :param request: Request instance for GetAsrVocabList.
         :type request: :class:`tencentcloud.asr.v20190614.models.GetAsrVocabListRequest`
@@ -344,15 +344,15 @@
             model = models.GetAsrVocabListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCustomizationList(self, request):
         """查询自学习模型列表
 
         :param request: Request instance for GetCustomizationList.
         :type request: :class:`tencentcloud.asr.v20190614.models.GetCustomizationListRequest`
@@ -367,15 +367,15 @@
             model = models.GetCustomizationListResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetModelInfo(self, request):
         """通过自学习模型id获取自学习模型详细信息
 
         :param request: Request instance for GetModelInfo.
         :type request: :class:`tencentcloud.asr.v20190614.models.GetModelInfoRequest`
@@ -390,15 +390,15 @@
             model = models.GetModelInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomization(self, request):
         """用户通过该接口可以更新自学习模型，如模型名称、模型类型、模型语料。
 
         :param request: Request instance for ModifyCustomization.
         :type request: :class:`tencentcloud.asr.v20190614.models.ModifyCustomizationRequest`
@@ -413,15 +413,15 @@
             model = models.ModifyCustomizationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyCustomizationState(self, request):
         """通过该接口，用户可以修改自学习模型状态，上下线自学习模型
 
         :param request: Request instance for ModifyCustomizationState.
         :type request: :class:`tencentcloud.asr.v20190614.models.ModifyCustomizationStateRequest`
@@ -436,15 +436,15 @@
             model = models.ModifyCustomizationStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SentenceRecognition(self, request):
         """本接口用于对60秒之内的短音频文件进行识别。<br>•   支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、泰语、葡萄牙语、土耳其语、阿拉伯语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。<br>•   支持本地语音文件上传和语音URL上传两种请求方式，音频时长不能超过60s，音频文件大小不能超过3MB。<br>•   音频格式支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac。<br>•   请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"<br>•   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。<br>•   默认接口请求频率限制：30次/秒，如您有提高请求频率限制的需求，请[前往购买](https://buy.cloud.tencent.com/asr)。
 
         :param request: Request instance for SentenceRecognition.
         :type request: :class:`tencentcloud.asr.v20190614.models.SentenceRecognitionRequest`
@@ -459,15 +459,15 @@
             model = models.SentenceRecognitionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def SetVocabState(self, request):
         """用户通过该接口可以设置热词表的默认状态。初始状态为0，用户可设置状态为1，即为默认状态。默认状态表示用户在请求识别时，如不设置热词表ID，则默认使用状态为1的热词表。
 
         :param request: Request instance for SetVocabState.
         :type request: :class:`tencentcloud.asr.v20190614.models.SetVocabStateRequest`
@@ -482,15 +482,15 @@
             model = models.SetVocabStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateAsrVocab(self, request):
         """用户通过本接口进行对应的词表信息更新。
 
         :param request: Request instance for UpdateAsrVocab.
         :type request: :class:`tencentcloud.asr.v20190614.models.UpdateAsrVocabRequest`
@@ -505,15 +505,15 @@
             model = models.UpdateAsrVocabResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VoicePrintDelete(self, request):
         """本接口用于以删除已经注册的说话人信息（删除之后，原有的说话人ID和说话人音频数据都会失效）
 
         :param request: Request instance for VoicePrintDelete.
         :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintDeleteRequest`
@@ -528,15 +528,15 @@
             model = models.VoicePrintDeleteResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VoicePrintEnroll(self, request):
         """说话人注册接口用于注册一个指定音频，生成一个唯一的说话人id，后续可通过说话人验证接口验证其它音频和已有的说话人ID匹配度，注册时可指定说话人昵称，方便标识说话人ID，  说话人昵称可重复配置。
         （注: 一个appid最多可以注册1000个说话人ID，一个说话人ID仅支持一条音频注册，后续可通过更新接口进行更新）
 
         使用须知
@@ -557,15 +557,15 @@
             model = models.VoicePrintEnrollResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VoicePrintUpdate(self, request):
         """本接口用于更新和覆盖已注册的音频数据和说话人昵称，更新后原有的音频数据将失效。
 
         :param request: Request instance for VoicePrintUpdate.
         :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintUpdateRequest`
@@ -580,15 +580,15 @@
             model = models.VoicePrintUpdateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VoicePrintVerify(self, request):
         """本接口用于校验传入音频与已注册音频的匹配程度，通过指定说话人ID（VoicePrintId）和一段音频进行音频和说话人的匹配度判断
 
         :param request: Request instance for VoicePrintVerify.
         :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintVerifyRequest`
@@ -603,8 +603,8 @@
             model = models.VoicePrintVerifyResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.938/tencentcloud/asr/v20190614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.938/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.937/README.rst` & `tencentcloud-sdk-python-asr-3.0.938/README.rst`

 * *Files identical despite different names*

