# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.937.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.937.tar", last modified: Tue Jul 18 00:27:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.938.tar", last modified: Wed Jul 19 00:43:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.937.tar` & `tencentcloud-sdk-python-mps-3.0.938.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99031 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1229741 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99431 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1229741 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 00:43:01.000000 tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mps-3.0.937/setup.py` & `tencentcloud-sdk-python-mps-3.0.938/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.938/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/mps_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             model = models.BatchDeleteStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchStartStreamLinkFlow(self, request):
         """批量启动媒体传输流。
 
         :param request: Request instance for BatchStartStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.BatchStartStreamLinkFlowRequest`
@@ -65,15 +65,15 @@
             model = models.BatchStartStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def BatchStopStreamLinkFlow(self, request):
         """批量停止媒体传输流。
 
         :param request: Request instance for BatchStopStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.BatchStopStreamLinkFlowRequest`
@@ -88,15 +88,15 @@
             model = models.BatchStopStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAIAnalysisTemplate(self, request):
         """创建用户自定义内容分析模板，数量上限：50。
 
         :param request: Request instance for CreateAIAnalysisTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateAIAnalysisTemplateRequest`
@@ -111,15 +111,15 @@
             model = models.CreateAIAnalysisTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAIRecognitionTemplate(self, request):
         """创建用户自定义内容识别模板，数量上限：50。
 
         :param request: Request instance for CreateAIRecognitionTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateAIRecognitionTemplateRequest`
@@ -134,15 +134,15 @@
             model = models.CreateAIRecognitionTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAdaptiveDynamicStreamingTemplate(self, request):
         """创建转自适应码流模板，数量上限：100。
 
         :param request: Request instance for CreateAdaptiveDynamicStreamingTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateAdaptiveDynamicStreamingTemplateRequest`
@@ -157,15 +157,15 @@
             model = models.CreateAdaptiveDynamicStreamingTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAnimatedGraphicsTemplate(self, request):
         """创建用户自定义转动图模板，数量上限：16。
 
         :param request: Request instance for CreateAnimatedGraphicsTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateAnimatedGraphicsTemplateRequest`
@@ -180,15 +180,15 @@
             model = models.CreateAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateContentReviewTemplate(self, request):
         """创建用户自定义内容审核模板，数量上限：50。
 
         :param request: Request instance for CreateContentReviewTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateContentReviewTemplateRequest`
@@ -203,15 +203,15 @@
             model = models.CreateContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateImageSpriteTemplate(self, request):
         """创建用户自定义雪碧图模板，数量上限：16。
 
         :param request: Request instance for CreateImageSpriteTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateImageSpriteTemplateRequest`
@@ -226,15 +226,15 @@
             model = models.CreateImageSpriteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePersonSample(self, request):
         """该接口用于创建素材样本，用于通过五官定位等技术，进行内容识别、内容不适宜等视频处理。
 
         :param request: Request instance for CreatePersonSample.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreatePersonSampleRequest`
@@ -249,15 +249,15 @@
             model = models.CreatePersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSampleSnapshotTemplate(self, request):
         """创建用户自定义采样截图模板，数量上限：16。
 
         :param request: Request instance for CreateSampleSnapshotTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateSampleSnapshotTemplateRequest`
@@ -272,15 +272,15 @@
             model = models.CreateSampleSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSchedule(self, request):
         """对 COS 中指定 Bucket 的目录下上传的媒体文件，设置处理规则，包括：
         1. 视频转码（带水印）；
         2. 视频转动图；
         3. 对视频按指定时间点截图；
@@ -306,15 +306,15 @@
             model = models.CreateScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateSnapshotByTimeOffsetTemplate(self, request):
         """创建用户自定义指定时间点截图模板，数量上限：16。
 
         :param request: Request instance for CreateSnapshotByTimeOffsetTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateSnapshotByTimeOffsetTemplateRequest`
@@ -329,15 +329,15 @@
             model = models.CreateSnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStreamLinkEvent(self, request):
         """创建媒体传输的事件Event。
 
         :param request: Request instance for CreateStreamLinkEvent.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkEventRequest`
@@ -352,15 +352,15 @@
             model = models.CreateStreamLinkEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStreamLinkFlow(self, request):
         """创建媒体传输的传输流配置。
 
         :param request: Request instance for CreateStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkFlowRequest`
@@ -375,15 +375,15 @@
             model = models.CreateStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStreamLinkInput(self, request):
         """创建媒体传输的输入配置。
 
         :param request: Request instance for CreateStreamLinkInput.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkInputRequest`
@@ -398,15 +398,15 @@
             model = models.CreateStreamLinkInputResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateStreamLinkOutputInfo(self, request):
         """创建媒体传输流的输出信息。
 
         :param request: Request instance for CreateStreamLinkOutputInfo.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkOutputInfoRequest`
@@ -421,15 +421,15 @@
             model = models.CreateStreamLinkOutputInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateTranscodeTemplate(self, request):
         """创建用户自定义转码模板，数量上限：1000。
 
         :param request: Request instance for CreateTranscodeTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateTranscodeTemplateRequest`
@@ -444,15 +444,15 @@
             model = models.CreateTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWatermarkTemplate(self, request):
         """创建用户自定义水印模板，数量上限：1000。
 
         :param request: Request instance for CreateWatermarkTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateWatermarkTemplateRequest`
@@ -467,15 +467,15 @@
             model = models.CreateWatermarkTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWordSamples(self, request):
         """该接口用于批量创建关键词样本，样本用于通过OCR、ASR技术，进行不适宜内容识别、内容识别等视频处理。
 
         :param request: Request instance for CreateWordSamples.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateWordSamplesRequest`
@@ -490,15 +490,15 @@
             model = models.CreateWordSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateWorkflow(self, request):
         """对 COS 中指定 Bucket 的目录下上传的媒体文件，设置处理规则，包括：
         1. 视频转码（带水印）；
         2. 视频转动图；
         3. 对视频按指定时间点截图；
@@ -524,15 +524,15 @@
             model = models.CreateWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAIAnalysisTemplate(self, request):
         """删除用户自定义内容分析模板。
 
         注意：模板 ID 为 10000 以下的为系统预置模板，不允许删除。
 
@@ -549,15 +549,15 @@
             model = models.DeleteAIAnalysisTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAIRecognitionTemplate(self, request):
         """删除用户自定义内容识别模板。
 
         :param request: Request instance for DeleteAIRecognitionTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteAIRecognitionTemplateRequest`
@@ -572,15 +572,15 @@
             model = models.DeleteAIRecognitionTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAdaptiveDynamicStreamingTemplate(self, request):
         """删除转自适应码流模板
 
         :param request: Request instance for DeleteAdaptiveDynamicStreamingTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteAdaptiveDynamicStreamingTemplateRequest`
@@ -595,15 +595,15 @@
             model = models.DeleteAdaptiveDynamicStreamingTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteAnimatedGraphicsTemplate(self, request):
         """删除用户自定义转动图模板。
 
         :param request: Request instance for DeleteAnimatedGraphicsTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteAnimatedGraphicsTemplateRequest`
@@ -618,15 +618,15 @@
             model = models.DeleteAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteContentReviewTemplate(self, request):
         """删除用户自定义内容审核模板。
 
         :param request: Request instance for DeleteContentReviewTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteContentReviewTemplateRequest`
@@ -641,15 +641,15 @@
             model = models.DeleteContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteImageSpriteTemplate(self, request):
         """删除雪碧图模板。
 
         :param request: Request instance for DeleteImageSpriteTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteImageSpriteTemplateRequest`
@@ -664,15 +664,15 @@
             model = models.DeleteImageSpriteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeletePersonSample(self, request):
         """该接口用于根据素材 ID，删除素材样本。
 
         :param request: Request instance for DeletePersonSample.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeletePersonSampleRequest`
@@ -687,15 +687,15 @@
             model = models.DeletePersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSampleSnapshotTemplate(self, request):
         """删除用户自定义采样截图模板。
 
         :param request: Request instance for DeleteSampleSnapshotTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteSampleSnapshotTemplateRequest`
@@ -710,15 +710,15 @@
             model = models.DeleteSampleSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSchedule(self, request):
         """删除编排
 
         :param request: Request instance for DeleteSchedule.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteScheduleRequest`
@@ -733,15 +733,15 @@
             model = models.DeleteScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteSnapshotByTimeOffsetTemplate(self, request):
         """删除用户自定义指定时间点截图模板。
 
         :param request: Request instance for DeleteSnapshotByTimeOffsetTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteSnapshotByTimeOffsetTemplateRequest`
@@ -756,15 +756,15 @@
             model = models.DeleteSnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStreamLinkEvent(self, request):
         """删除媒体传输的事件配置。
 
         :param request: Request instance for DeleteStreamLinkEvent.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkEventRequest`
@@ -779,15 +779,15 @@
             model = models.DeleteStreamLinkEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStreamLinkFlow(self, request):
         """删除媒体传输的传输流配置。
 
         :param request: Request instance for DeleteStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkFlowRequest`
@@ -802,15 +802,15 @@
             model = models.DeleteStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteStreamLinkOutput(self, request):
         """删除媒体传输流的输出配置。
 
         :param request: Request instance for DeleteStreamLinkOutput.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkOutputRequest`
@@ -825,15 +825,15 @@
             model = models.DeleteStreamLinkOutputResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteTranscodeTemplate(self, request):
         """删除用户自定义转码模板。
 
         :param request: Request instance for DeleteTranscodeTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteTranscodeTemplateRequest`
@@ -848,15 +848,15 @@
             model = models.DeleteTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWatermarkTemplate(self, request):
         """删除用户自定义水印模板。
 
         :param request: Request instance for DeleteWatermarkTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteWatermarkTemplateRequest`
@@ -871,15 +871,15 @@
             model = models.DeleteWatermarkTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWordSamples(self, request):
         """该接口用于批量删除关键词样本。
 
         :param request: Request instance for DeleteWordSamples.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteWordSamplesRequest`
@@ -894,15 +894,15 @@
             model = models.DeleteWordSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteWorkflow(self, request):
         """删除工作流。对于已启用的工作流，需要禁用后才能删除。
 
         :param request: Request instance for DeleteWorkflow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteWorkflowRequest`
@@ -917,15 +917,15 @@
             model = models.DeleteWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIAnalysisTemplates(self, request):
         """根据内容分析模板唯一标识，获取内容分析模板详情列表。返回结果包含符合条件的所有用户自定义内容分析模板及系统预置视频内容分析模板
 
         :param request: Request instance for DescribeAIAnalysisTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeAIAnalysisTemplatesRequest`
@@ -940,15 +940,15 @@
             model = models.DescribeAIAnalysisTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAIRecognitionTemplates(self, request):
         """根据内容识别模板唯一标识，获取内容识别模板详情列表。返回结果包含符合条件的所有用户自定义内容识别模板及系统预置视频内容识别模板
 
         :param request: Request instance for DescribeAIRecognitionTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeAIRecognitionTemplatesRequest`
@@ -963,15 +963,15 @@
             model = models.DescribeAIRecognitionTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAdaptiveDynamicStreamingTemplates(self, request):
         """查询转自适应码流模板，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeAdaptiveDynamicStreamingTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeAdaptiveDynamicStreamingTemplatesRequest`
@@ -986,15 +986,15 @@
             model = models.DescribeAdaptiveDynamicStreamingTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAnimatedGraphicsTemplates(self, request):
         """查询转动图模板列表，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeAnimatedGraphicsTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeAnimatedGraphicsTemplatesRequest`
@@ -1009,15 +1009,15 @@
             model = models.DescribeAnimatedGraphicsTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeContentReviewTemplates(self, request):
         """根据智能审核模板唯一标识，获取智能审核模板详情列表。返回结果包含符合条件的所有用户自定义模板及系统预置智能审核模板。
 
         :param request: Request instance for DescribeContentReviewTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeContentReviewTemplatesRequest`
@@ -1032,15 +1032,15 @@
             model = models.DescribeContentReviewTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeImageSpriteTemplates(self, request):
         """查询雪碧图模板，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeImageSpriteTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeImageSpriteTemplatesRequest`
@@ -1055,15 +1055,15 @@
             model = models.DescribeImageSpriteTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeMediaMetaData(self, request):
         """获取媒体的元信息，包括视频画面宽、高、编码格式、时长、帧率等。
 
         :param request: Request instance for DescribeMediaMetaData.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeMediaMetaDataRequest`
@@ -1078,15 +1078,15 @@
             model = models.DescribeMediaMetaDataResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePersonSamples(self, request):
         """该接口用于查询素材样本信息，支持根据素材 ID、名称、标签，分页查询。
 
         :param request: Request instance for DescribePersonSamples.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribePersonSamplesRequest`
@@ -1101,15 +1101,15 @@
             model = models.DescribePersonSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSampleSnapshotTemplates(self, request):
         """查询采样截图模板，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeSampleSnapshotTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeSampleSnapshotTemplatesRequest`
@@ -1124,15 +1124,15 @@
             model = models.DescribeSampleSnapshotTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSchedules(self, request):
         """查询编排。
 
         :param request: Request instance for DescribeSchedules.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeSchedulesRequest`
@@ -1147,15 +1147,15 @@
             model = models.DescribeSchedulesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeSnapshotByTimeOffsetTemplates(self, request):
         """查询指定时间点截图模板，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeSnapshotByTimeOffsetTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeSnapshotByTimeOffsetTemplatesRequest`
@@ -1170,15 +1170,15 @@
             model = models.DescribeSnapshotByTimeOffsetTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkActivateState(self, request):
         """查询媒体传输开通状态。
 
         :param request: Request instance for DescribeStreamLinkActivateState.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkActivateStateRequest`
@@ -1193,15 +1193,15 @@
             model = models.DescribeStreamLinkActivateStateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkEvent(self, request):
         """查询媒体传输事件的配置信息。
 
         :param request: Request instance for DescribeStreamLinkEvent.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventRequest`
@@ -1216,15 +1216,15 @@
             model = models.DescribeStreamLinkEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkEventAttachedFlows(self, request):
         """查询媒体传输事件关联的所有媒体输入流的配置信息。
 
         :param request: Request instance for DescribeStreamLinkEventAttachedFlows.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventAttachedFlowsRequest`
@@ -1239,15 +1239,15 @@
             model = models.DescribeStreamLinkEventAttachedFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkEvents(self, request):
         """批量查询媒体传输事件的配置信息。
 
         :param request: Request instance for DescribeStreamLinkEvents.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventsRequest`
@@ -1262,15 +1262,15 @@
             model = models.DescribeStreamLinkEventsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlow(self, request):
         """查询媒体输入流的配置信息。
 
         :param request: Request instance for DescribeStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowRequest`
@@ -1285,15 +1285,15 @@
             model = models.DescribeStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlowLogs(self, request):
         """查询媒体传输流的日志信息。
 
         :param request: Request instance for DescribeStreamLinkFlowLogs.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowLogsRequest`
@@ -1308,15 +1308,15 @@
             model = models.DescribeStreamLinkFlowLogsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlowMediaStatistics(self, request):
         """查询媒体传输流的媒体质量数据。
 
         :param request: Request instance for DescribeStreamLinkFlowMediaStatistics.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowMediaStatisticsRequest`
@@ -1331,15 +1331,15 @@
             model = models.DescribeStreamLinkFlowMediaStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlowRealtimeStatus(self, request):
         """实时查询流的当前状态
 
         :param request: Request instance for DescribeStreamLinkFlowRealtimeStatus.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowRealtimeStatusRequest`
@@ -1354,15 +1354,15 @@
             model = models.DescribeStreamLinkFlowRealtimeStatusResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlowSRTStatistics(self, request):
         """查询媒体传输流的SRT质量数据。
 
         :param request: Request instance for DescribeStreamLinkFlowSRTStatistics.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowSRTStatisticsRequest`
@@ -1377,15 +1377,15 @@
             model = models.DescribeStreamLinkFlowSRTStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlowStatistics(self, request):
         """查询媒体传输流的媒体质量数据。
 
         :param request: Request instance for DescribeStreamLinkFlowStatistics.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowStatisticsRequest`
@@ -1400,15 +1400,15 @@
             model = models.DescribeStreamLinkFlowStatisticsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkFlows(self, request):
         """批量查询媒体输入流的配置信息。
 
         :param request: Request instance for DescribeStreamLinkFlows.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowsRequest`
@@ -1423,15 +1423,15 @@
             model = models.DescribeStreamLinkFlowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamLinkRegions(self, request):
         """查询媒体传输所有地区。
 
         :param request: Request instance for DescribeStreamLinkRegions.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkRegionsRequest`
@@ -1446,15 +1446,15 @@
             model = models.DescribeStreamLinkRegionsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTaskDetail(self, request):
         """通过任务 ID 查询任务的执行状态和结果的详细信息（最多可以查询7天之内提交的任务）。
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeTaskDetailRequest`
@@ -1469,15 +1469,15 @@
             model = models.DescribeTaskDetailResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTasks(self, request):
         """* 该接口用于查询任务列表；
         * 当列表数据比较多时，单次接口调用无法拉取整个列表，可通过 ScrollToken 参数，分批拉取；
         * 只能查询到最近七天（168小时）内的任务。
 
@@ -1494,15 +1494,15 @@
             model = models.DescribeTasksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTranscodeTemplates(self, request):
         """根据转码模板唯一标识，获取转码模板详情列表。返回结果包含符合条件的所有用户自定义模板及[系统预置转码模板](https://cloud.tencent.com/document/product/266/33476#.E9.A2.84.E7.BD.AE.E8.BD.AC.E7.A0.81.E6.A8.A1.E6.9D.BF)。
 
         :param request: Request instance for DescribeTranscodeTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeTranscodeTemplatesRequest`
@@ -1517,15 +1517,15 @@
             model = models.DescribeTranscodeTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWatermarkTemplates(self, request):
         """查询用户自定义水印模板，支持根据条件，分页查询。
 
         :param request: Request instance for DescribeWatermarkTemplates.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeWatermarkTemplatesRequest`
@@ -1540,15 +1540,15 @@
             model = models.DescribeWatermarkTemplatesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWordSamples(self, request):
         """该接口用于根据应用场景、关键词、标签，分页查询关键词样本信息。
 
         :param request: Request instance for DescribeWordSamples.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeWordSamplesRequest`
@@ -1563,15 +1563,15 @@
             model = models.DescribeWordSamplesResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeWorkflows(self, request):
         """根据工作流 ID，获取工作流详情列表。
 
         :param request: Request instance for DescribeWorkflows.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeWorkflowsRequest`
@@ -1586,15 +1586,15 @@
             model = models.DescribeWorkflowsResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableSchedule(self, request):
         """禁用自动化触发编排任务。
 
         :param request: Request instance for DisableSchedule.
         :type request: :class:`tencentcloud.mps.v20190612.models.DisableScheduleRequest`
@@ -1609,15 +1609,15 @@
             model = models.DisableScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DisableWorkflow(self, request):
         """禁用工作流。
 
         :param request: Request instance for DisableWorkflow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DisableWorkflowRequest`
@@ -1632,15 +1632,15 @@
             model = models.DisableWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EditMedia(self, request):
         """对视频进行编辑（剪辑、拼接等），生成一个新的点播视频。编辑的功能包括：
 
         1. 对一个文件进行剪辑，生成一个新的视频；
         2. 对多个文件进行拼接，生成一个新的视频；
@@ -1659,15 +1659,15 @@
             model = models.EditMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableSchedule(self, request):
         """启用自动化触发编排任务。
 
         :param request: Request instance for EnableSchedule.
         :type request: :class:`tencentcloud.mps.v20190612.models.EnableScheduleRequest`
@@ -1682,15 +1682,15 @@
             model = models.EnableScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def EnableWorkflow(self, request):
         """启用工作流。
 
         :param request: Request instance for EnableWorkflow.
         :type request: :class:`tencentcloud.mps.v20190612.models.EnableWorkflowRequest`
@@ -1705,15 +1705,15 @@
             model = models.EnableWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ExecuteFunction(self, request):
         """本接口仅用于定制开发的特殊场景，除非云媒体处理客服人员主动告知您需要使用本接口，其它情况请勿调用。
 
         :param request: Request instance for ExecuteFunction.
         :type request: :class:`tencentcloud.mps.v20190612.models.ExecuteFunctionRequest`
@@ -1728,15 +1728,15 @@
             model = models.ExecuteFunctionResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ManageTask(self, request):
         """对已发起的任务进行管理。
 
         :param request: Request instance for ManageTask.
         :type request: :class:`tencentcloud.mps.v20190612.models.ManageTaskRequest`
@@ -1751,15 +1751,15 @@
             model = models.ManageTaskResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAIAnalysisTemplate(self, request):
         """修改用户自定义内容分析模板。
 
         注意：模板 ID 10000 以下的为系统预置模板，不允许修改。
 
@@ -1776,15 +1776,15 @@
             model = models.ModifyAIAnalysisTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAIRecognitionTemplate(self, request):
         """修改用户自定义内容识别模板。
 
         :param request: Request instance for ModifyAIRecognitionTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyAIRecognitionTemplateRequest`
@@ -1799,15 +1799,15 @@
             model = models.ModifyAIRecognitionTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAdaptiveDynamicStreamingTemplate(self, request):
         """修改转自适应码流模板
 
         :param request: Request instance for ModifyAdaptiveDynamicStreamingTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyAdaptiveDynamicStreamingTemplateRequest`
@@ -1822,15 +1822,15 @@
             model = models.ModifyAdaptiveDynamicStreamingTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyAnimatedGraphicsTemplate(self, request):
         """修改用户自定义转动图模板。
 
         :param request: Request instance for ModifyAnimatedGraphicsTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyAnimatedGraphicsTemplateRequest`
@@ -1845,15 +1845,15 @@
             model = models.ModifyAnimatedGraphicsTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyContentReviewTemplate(self, request):
         """修改用户自定义内容审核模板。
 
         :param request: Request instance for ModifyContentReviewTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyContentReviewTemplateRequest`
@@ -1868,15 +1868,15 @@
             model = models.ModifyContentReviewTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyImageSpriteTemplate(self, request):
         """修改用户自定义雪碧图模板。
 
         :param request: Request instance for ModifyImageSpriteTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyImageSpriteTemplateRequest`
@@ -1891,15 +1891,15 @@
             model = models.ModifyImageSpriteTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyPersonSample(self, request):
         """该接口用于根据素材 ID，修改素材样本信息，包括名称、描述的修改，以及五官、标签的添加、删除、重置操作。五官删除操作需保证至少剩余 1 张图片，否则，请使用重置操作。
 
         :param request: Request instance for ModifyPersonSample.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyPersonSampleRequest`
@@ -1914,15 +1914,15 @@
             model = models.ModifyPersonSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySampleSnapshotTemplate(self, request):
         """修改用户自定义采样截图模板。
 
         :param request: Request instance for ModifySampleSnapshotTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifySampleSnapshotTemplateRequest`
@@ -1937,15 +1937,15 @@
             model = models.ModifySampleSnapshotTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySchedule(self, request):
         """修改编排
 
         :param request: Request instance for ModifySchedule.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyScheduleRequest`
@@ -1960,15 +1960,15 @@
             model = models.ModifyScheduleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifySnapshotByTimeOffsetTemplate(self, request):
         """修改用户自定义指定时间点截图模板。
 
         :param request: Request instance for ModifySnapshotByTimeOffsetTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifySnapshotByTimeOffsetTemplateRequest`
@@ -1983,15 +1983,15 @@
             model = models.ModifySnapshotByTimeOffsetTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyStreamLinkEvent(self, request):
         """修改媒体传输的事件配置信息。
 
         :param request: Request instance for ModifyStreamLinkEvent.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkEventRequest`
@@ -2006,15 +2006,15 @@
             model = models.ModifyStreamLinkEventResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyStreamLinkFlow(self, request):
         """修改媒体传输的传输流配置信息。
 
         :param request: Request instance for ModifyStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkFlowRequest`
@@ -2029,15 +2029,15 @@
             model = models.ModifyStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyStreamLinkInput(self, request):
         """修改媒体传输流的输入信息。
 
         :param request: Request instance for ModifyStreamLinkInput.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkInputRequest`
@@ -2052,15 +2052,15 @@
             model = models.ModifyStreamLinkInputResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyStreamLinkOutputInfo(self, request):
         """修改媒体传输流的输出配置。
 
         :param request: Request instance for ModifyStreamLinkOutputInfo.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkOutputInfoRequest`
@@ -2075,15 +2075,15 @@
             model = models.ModifyStreamLinkOutputInfoResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyTranscodeTemplate(self, request):
         """修改用户自定义转码模板信息。
 
         :param request: Request instance for ModifyTranscodeTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyTranscodeTemplateRequest`
@@ -2098,15 +2098,15 @@
             model = models.ModifyTranscodeTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWatermarkTemplate(self, request):
         """修改用户自定义水印模板，水印类型不允许修改。
 
         :param request: Request instance for ModifyWatermarkTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyWatermarkTemplateRequest`
@@ -2121,15 +2121,15 @@
             model = models.ModifyWatermarkTemplateResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyWordSample(self, request):
         """该接口用于修改关键词的应用场景、标签，关键词本身不可修改，如需修改，可删除重建。
 
         :param request: Request instance for ModifyWordSample.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyWordSampleRequest`
@@ -2144,15 +2144,15 @@
             model = models.ModifyWordSampleResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseLiveStreamProcessNotification(self, request):
         """从 CMQ 获取到消息后，从消息的 msgBody 字段中解析出 MPS 直播流处理事件通知的内容。
         该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 中的解析实现事件通知的解析。
 
         :param request: Request instance for ParseLiveStreamProcessNotification.
@@ -2168,15 +2168,15 @@
             model = models.ParseLiveStreamProcessNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ParseNotification(self, request):
         """从 CMQ 获取到消息后，从消息的 msgBody 字段中解析出 MPS 事件通知的内容。
         该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 中的解析函数，实现事件通知的解析。
 
         :param request: Request instance for ParseNotification.
@@ -2192,15 +2192,15 @@
             model = models.ParseNotificationResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessLiveStream(self, request):
         """对直播流媒体发起处理任务，功能包括：
 
         * 智能内容审核（画面鉴黄、敏感信息检测、声音鉴黄）；
         * 智能内容识别（人脸、文本全文、文本关键词、语音全文、语音关键词、语音实时翻译）。
@@ -2220,15 +2220,15 @@
             model = models.ProcessLiveStreamResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ProcessMedia(self, request):
         """对 URL视频链接 或 COS 中的媒体文件发起处理任务，功能包括：
         1. 视频转码（普通转码、极速高清转码、音视频增强）；
         2. 视频转动图；
         3. 对视频按指定时间点截图；
@@ -2252,15 +2252,15 @@
             model = models.ProcessMediaResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RecognizeMediaForZhiXue(self, request):
         """智能媒体识别，包含表情和动作识别。仅用于智学，其他调用无效。
 
         :param request: Request instance for RecognizeMediaForZhiXue.
         :type request: :class:`tencentcloud.mps.v20190612.models.RecognizeMediaForZhiXueRequest`
@@ -2275,15 +2275,15 @@
             model = models.RecognizeMediaForZhiXueResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ResetWorkflow(self, request):
         """重新设置一个已经存在且处于禁用状态的工作流。
 
         :param request: Request instance for ResetWorkflow.
         :type request: :class:`tencentcloud.mps.v20190612.models.ResetWorkflowRequest`
@@ -2298,15 +2298,15 @@
             model = models.ResetWorkflowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StartStreamLinkFlow(self, request):
         """启动媒体传输流。
 
         :param request: Request instance for StartStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.StartStreamLinkFlowRequest`
@@ -2321,15 +2321,15 @@
             model = models.StartStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopStreamLinkFlow(self, request):
         """停止媒体传输流。
 
         :param request: Request instance for StopStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.StopStreamLinkFlowRequest`
@@ -2344,15 +2344,15 @@
             model = models.StopStreamLinkFlowResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def WithdrawsWatermark(self, request):
         """提取视频中的盲水印。
 
         :param request: Request instance for WithdrawsWatermark.
         :type request: :class:`tencentcloud.mps.v20190612.models.WithdrawsWatermarkRequest`
@@ -2367,8 +2367,8 @@
             model = models.WithdrawsWatermarkResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
-                raise TencentCloudSDKException(e.message, e.message)
+                raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.938/tencentcloud/mps/v20190612/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.937/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.937/README.rst` & `tencentcloud-sdk-python-mps-3.0.938/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.938/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.937
+Version: 3.0.938
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

